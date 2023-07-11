# Comparing `tmp/atomcache-0.7.4.tar.gz` & `tmp/atomcache-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcache-0.7.4.tar", max compression
+gzip compressed data, was "atomcache-0.7.5.tar", max compression
```

## Comparing `atomcache-0.7.4.tar` & `atomcache-0.7.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.4/LICENSE
--rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.4/README.md
--rw-r--r--   0        0        0      160 2023-06-30 10:08:19.292207 atomcache-0.7.4/atomcache/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-30 10:06:30.127745 atomcache-0.7.4/atomcache/backend.py
--rw-r--r--   0        0        0     9790 2023-06-30 10:07:43.401727 atomcache-0.7.4/atomcache/base.py
--rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.4/atomcache/py.typed
--rw-r--r--   0        0        0     4962 2023-06-30 10:06:30.130746 atomcache-0.7.4/atomcache/redis.py
--rw-r--r--   0        0        0      951 2023-06-30 10:08:24.766280 atomcache-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.5/LICENSE
+-rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.5/README.md
+-rw-r--r--   0        0        0      160 2023-07-11 07:39:04.603650 atomcache-0.7.5/atomcache/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-30 10:06:30.127745 atomcache-0.7.5/atomcache/backend.py
+-rw-r--r--   0        0        0    10144 2023-07-11 07:38:24.711125 atomcache-0.7.5/atomcache/base.py
+-rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.5/atomcache/py.typed
+-rw-r--r--   0        0        0     4962 2023-06-30 10:06:30.130746 atomcache-0.7.5/atomcache/redis.py
+-rw-r--r--   0        0        0      951 2023-07-11 07:39:10.887890 atomcache-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.5/PKG-INFO
```

### Comparing `atomcache-0.7.4/LICENSE` & `atomcache-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.4/README.md` & `atomcache-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.4/atomcache/backend.py` & `atomcache-0.7.5/atomcache/backend.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.4/atomcache/base.py` & `atomcache-0.7.5/atomcache/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import asyncio
 import inspect
 import json
-from contextlib import suppress
 from functools import partial
 from hashlib import sha256
 from typing import Any, Awaitable, Callable, Coroutine, Dict, Optional, TypeVar, Union
 
 from fastapi import FastAPI, Request, Response, params
 from fastapi.encoders import jsonable_encoder
 from fastapi.routing import APIRoute
 from starlette.datastructures import CommaSeparatedStrings
 
 from redis.asyncio import Redis
 
 from .backend import DEFAULT_LOCK_TIMEOUT, EX, BaseCacheBackend
 from .redis import RedisCacheBackend
 
-MIN_AUTOREFRESH_RATE = 60
+MIN_AUTOREFRESH_RATE = 20
 _ResponseT = TypeVar("_ResponseT")
 
 
 class CachedResponse(Exception):  # noqa: N818
     def __init__(self, *args, content: str, ttl: int) -> None:
         self.content = content
         self.ttl = ttl
@@ -66,15 +65,14 @@
         assert exp is None or exp >= lock_timeout, f"ValueError: {lock_timeout=} must be less than {exp=}"
         self.auto_refresh = auto_refresh
         self._expire = exp
         self.namespace = namespace
         self._lock_timeout = lock_timeout
         self._allow_cache_control = cache_control
         self._autorefresh_callback: Union[Callable, Awaitable, None] = None
-        self._autorefresh_task: Optional[asyncio.Future] = None
         self._no_cache: bool = False
 
     async def __call__(self, request: Request):
         if self._allow_cache_control:
             self._no_cache = "no-cache" in CommaSeparatedStrings(request.headers.get("Cache-Control", ""))
         return self
 
@@ -161,30 +159,37 @@
             timeout=self._lock_timeout,
             with_lock=with_lock,
             lockspace=lockspace,
         )
         if cached_content is not None:
             raise CachedResponse(content=cached_content, ttl=ttl)
 
-    def schedule_autorefresh(self):
-        if self.auto_refresh:
-            self._autorefresh_task = asyncio.ensure_future(self._autorefresh())
+    def schedule_autorefresh(self, __task: Optional[asyncio.Task[None]] = None) -> None:  # noqa: WPS112
+        if __task is None:
+            autorefresh_task = asyncio.create_task(self._autorefresh())
+            autorefresh_task.add_done_callback(self.schedule_autorefresh)
+            return
+        if __task.cancelled():
+            return
+        loop = asyncio.get_running_loop()
+        loop.call_later(MIN_AUTOREFRESH_RATE, self.schedule_autorefresh, None)
 
     @classmethod
     async def init(cls, app: FastAPI, cache_client: Redis, autorefresh: bool = True):
         cls.app = app
         if isinstance(cache_client, Redis):
             cls.backend = await RedisCacheBackend(cache_client)
         else:
             raise TypeError(f"Unsupported {type(cache_client)} cache client type.")
         app.add_exception_handler(CachedResponse, cached_response_handler)
         cls._config_caches(app)
-        if autorefresh:
-            for cache in cls.autorefresh.values():
-                cache.schedule_autorefresh()
+        if not autorefresh:
+            return
+        for cache in cls.autorefresh.values():
+            cache.schedule_autorefresh()
 
     @classmethod
     def _config_caches(cls, app: FastAPI) -> None:  # noqa: WPS231
         """
         Should be called only after all routes have been added.
         """
         for route in app.routes:
@@ -197,19 +202,22 @@
                     continue
                 cache = default.dependency
                 if cache.namespace is None:
                     cache.set_namespace(route.path)
                 if cache.auto_refresh:
                     cache.set_autorefresh_callback(route.endpoint)
 
-    async def _autorefresh(self):
+    async def _autorefresh(self) -> None:
         while True:  # noqa: WPS457
-            with suppress(CachedResponse):
+            try:
                 await self._autorefresh_callback()
-            await asyncio.sleep(self._expire - self._lock_timeout)
+            except CachedResponse as cached_response:
+                await asyncio.sleep(cached_response.ttl or 1)
+            else:
+                await asyncio.sleep(self._lock_timeout)
 
 
 def cached_response_handler(request: Request, exc: CachedResponse) -> Response:
     if_none_match = request.headers.get("if-none-match")
     etag = f"W/{hashsum(exc.content)}"
     if if_none_match == etag:
         response = Response(status_code=304, headers={"Cache-Control": f"max-age={exc.ttl}"})  # noqa:WPS432
```

### Comparing `atomcache-0.7.4/atomcache/redis.py` & `atomcache-0.7.5/atomcache/redis.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.4/pyproject.toml` & `atomcache-0.7.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atomcache"
-version = "0.7.4"
+version = "0.7.5"
 description = "Asynchronous cache manager designed for horizontally scaled web applications."
 authors = ["Serghei Ungurean <srg@intelbit.io>", "Nichita Morcotilo <nmorkotilo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pysergio/atomcache"
 repository = "https://github.com/pysergio/atomcache"
```

### Comparing `atomcache-0.7.4/PKG-INFO` & `atomcache-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomcache
-Version: 0.7.4
+Version: 0.7.5
 Summary: Asynchronous cache manager designed for horizontally scaled web applications.
 Home-page: https://github.com/pysergio/atomcache
 License: MIT
 Author: Serghei Ungurean
 Author-email: srg@intelbit.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: atomcache Version: 0.7.4 Summary: Asynchronous
+Metadata-Version: 2.1 Name: atomcache Version: 0.7.5 Summary: Asynchronous
 cache manager designed for horizontally scaled web applications. Home-page:
 https://github.com/pysergio/atomcache License: MIT Author: Serghei Ungurean
 Author-email: srg@intelbit.io Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fastapi
```

