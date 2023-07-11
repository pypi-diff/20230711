# Comparing `tmp/redmage-0.2.0.tar.gz` & `tmp/redmage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.2.0.tar", max compression
+gzip compressed data, was "redmage-0.2.1.tar", max compression
```

## Comparing `redmage-0.2.0.tar` & `redmage-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.0/LICENSE
--rw-r--r--   0        0        0    14693 2023-05-15 02:00:21.924105 redmage-0.2.0/README.md
--rw-r--r--   0        0        0      660 2023-05-15 01:59:45.682116 redmage-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.0/redmage/__init__.py
--rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.2.0/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.0/redmage/convertors.py
--rw-r--r--   0        0        0     7389 2023-05-15 02:27:20.247267 redmage-0.2.0/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.2.0/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.0/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.0/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.0/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.0/redmage/triggers.py
--rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.2.0/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.0/redmage/utils.py
--rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.1/LICENSE
+-rw-r--r--   0        0        0    14693 2023-07-11 00:43:29.450794 redmage-0.2.1/README.md
+-rw-r--r--   0        0        0      660 2023-07-11 00:51:16.382615 redmage-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.1/redmage/__init__.py
+-rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.2.1/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.1/redmage/convertors.py
+-rw-r--r--   0        0        0     7766 2023-07-11 00:48:25.487066 redmage-0.2.1/redmage/core.py
+-rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.2.1/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.1/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.1/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.1/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.1/redmage/triggers.py
+-rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.2.1/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.1/redmage/utils.py
+-rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.2.1/PKG-INFO
```

### Comparing `redmage-0.2.0/LICENSE` & `redmage-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/README.md` & `redmage-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/pyproject.toml` & `redmage-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.2.0"
+version = "0.2.1"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.2.0/redmage/components.py` & `redmage-0.2.1/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/redmage/convertors.py` & `redmage-0.2.1/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/redmage/core.py` & `redmage-0.2.1/redmage/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from inspect import Parameter, getmembers, isfunction, signature
 from types import FunctionType
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, Union
 
 from starlette.applications import Starlette
 from starlette.convertors import CONVERTOR_TYPES as starlette_convertors
 from starlette.datastructures import FormData, QueryParams
+from starlette.middleware import Middleware
 from starlette.requests import Request
 from starlette.responses import HTMLResponse
 from starlette.routing import Route
 
 from redmage.exceptions import RedmageError
 
 from .components import Component
@@ -19,25 +20,34 @@
 logger = logging.getLogger("redmage")
 
 
 ComponentClass = Type[Component]
 
 
 class Redmage:
-    def __init__(self, debug: bool = False):
+    def __init__(
+        self, middleware: Optional[Sequence[Middleware]] = None, debug: bool = False
+    ):
         self.debug = debug
+        self.middleware = middleware
         self.routes: List[Route] = []
         self.components: List[Tuple[ComponentClass, Optional[Tuple[str]]]] = []
         # Could cause problems if multiple apps are created
         Component.set_app(self)
 
     @property
     def starlette(self) -> Starlette:
         if not hasattr(self, "_starlette"):
             self.create_routes()
+            if self.middleware:
+                self._starlette = Starlette(
+                    debug=self.debug,
+                    routes=self.routes,
+                    middleware=self.middleware,
+                )
             self._starlette = Starlette(debug=self.debug, routes=self.routes)
         return self._starlette
 
     def create_routes(self) -> None:
         for cls, routes in self.components:
             if routes:
                 self._register_routes(cls, routes)
```

### Comparing `redmage-0.2.0/redmage/elements.py` & `redmage-0.2.1/redmage/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 
 class Element:
     el: Type[hype.Element]
 
     def __init__(
         self,
         *content: Union[str, hype.Element],
+        # hx-* attributes
         swap: str = HTMXSwap.OUTER_HTML,
         target: Optional[Target] = None,
         trigger: Union[Trigger, Tuple[Trigger, ...]] = (),
         swap_oob: bool = False,
         confirm: Optional[str] = None,
         boost: bool = False,
         push_url: Optional[str] = None,
         indicator: bool = False,
+        on: Optional[str] = None,
+        # helper target+trigger combos
         click: Optional[Target] = None,
         submit: Optional[Target] = None,
         change: Optional[Target] = None,
         mouse_over: Optional[Target] = None,
         mouse_enter: Optional[Target] = None,
         load: Optional[Target] = None,
         intersect: Optional[Target] = None,
@@ -36,14 +39,15 @@
         self.target = target
         self.trigger = trigger
         self.swap_oob = swap_oob
         self.confirm = confirm
         self.boost = boost
         self.push_url = push_url
         self.indicator = indicator
+        self.on = on
         self.kwargs = kwargs
         self.click = click
         self.submit = submit
         self.change = change
         self.mouse_over = mouse_over
         self.mouse_enter = mouse_enter
         self.load = load
@@ -104,14 +108,17 @@
 
         if self.confirm:
             el.attrs(hx_confirm=self.confirm)
 
         if self.boost:
             el.attrs(hx_boost="true")
 
+        if self.on:
+            el.attrs(hx_on=self.on)
+
         return el
 
     def __str__(self) -> str:
         return str(self.render())
 
 
 class Doc:
```

### Comparing `redmage-0.2.0/redmage/targets.py` & `redmage-0.2.1/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/redmage/triggers.py` & `redmage-0.2.1/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/redmage/types.py` & `redmage-0.2.1/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/redmage/utils.py` & `redmage-0.2.1/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.0/PKG-INFO` & `redmage-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.2.0
+Version: 0.2.1
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

