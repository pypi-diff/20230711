# Comparing `tmp/confluence_cli-0.8.0.tar.gz` & `tmp/confluence_cli-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluence_cli-0.8.0.tar", max compression
+gzip compressed data, was "confluence_cli-0.8.1.tar", max compression
```

## Comparing `confluence_cli-0.8.0.tar` & `confluence_cli-0.8.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1084 2022-12-03 16:21:12.562517 confluence_cli-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0      939 2022-12-12 18:03:51.829619 confluence_cli-0.8.0/README.md
--rw-r--r--   0        0        0      233 2022-12-03 16:21:12.318517 confluence_cli-0.8.0/confluence_cli/cli/__init__.py
--rw-r--r--   0        0        0     1860 2022-12-03 16:21:12.310517 confluence_cli-0.8.0/confluence_cli/cli/comala_api.py
--rw-r--r--   0        0        0     6880 2022-12-03 16:21:12.322517 confluence_cli-0.8.0/confluence_cli/cli/confluence_async.py
--rw-r--r--   0        0        0     1230 2022-12-12 17:53:44.181742 confluence_cli-0.8.0/confluence_cli/cli/confluence_limited.py
--rw-r--r--   0        0        0    13393 2022-12-12 21:17:59.128698 confluence_cli-0.8.0/confluence_cli/cli/confluence_wrapper.py
--rw-r--r--   0        0        0     7807 2022-12-12 21:46:12.711471 confluence_cli-0.8.0/confluence_cli/cli/paginators.py
--rw-r--r--   0        0        0     3339 2022-12-03 16:21:12.326516 confluence_cli-0.8.0/confluence_cli/cli/types.py
--rw-r--r--   0        0        0     3102 2022-12-03 16:21:12.246517 confluence_cli-0.8.0/confluence_cli/cli/utils.py
--rw-r--r--   0        0        0      817 2022-12-13 10:42:42.301674 confluence_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 confluence_cli-0.8.0/setup.py
--rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 confluence_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 16:21:12.562517 confluence_cli-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0      939 2022-12-12 18:03:51.829619 confluence_cli-0.8.1/README.md
+-rw-r--r--   0        0        0      233 2022-12-03 16:21:12.318517 confluence_cli-0.8.1/confluence_cli/cli/__init__.py
+-rw-r--r--   0        0        0     1860 2022-12-03 16:21:12.310517 confluence_cli-0.8.1/confluence_cli/cli/comala_api.py
+-rw-r--r--   0        0        0     7219 2023-01-30 19:37:24.723228 confluence_cli-0.8.1/confluence_cli/cli/confluence_async.py
+-rw-r--r--   0        0        0     1230 2022-12-12 17:53:44.181742 confluence_cli-0.8.1/confluence_cli/cli/confluence_limited.py
+-rw-r--r--   0        0        0    13393 2022-12-12 21:17:59.128698 confluence_cli-0.8.1/confluence_cli/cli/confluence_wrapper.py
+-rw-r--r--   0        0        0     8059 2023-01-30 14:53:18.184682 confluence_cli-0.8.1/confluence_cli/cli/paginators.py
+-rw-r--r--   0        0        0     3509 2023-01-30 13:48:54.049440 confluence_cli-0.8.1/confluence_cli/cli/types.py
+-rw-r--r--   0        0        0     2577 2023-07-08 20:52:47.543022 confluence_cli-0.8.1/confluence_cli/cli/utils.py
+-rw-r--r--   0        0        0      817 2023-07-11 14:29:55.502003 confluence_cli-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 confluence_cli-0.8.1/PKG-INFO
```

### Comparing `confluence_cli-0.8.0/LICENSE.txt` & `confluence_cli-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.0/README.md` & `confluence_cli-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.0/confluence_cli/cli/comala_api.py` & `confluence_cli-0.8.1/confluence_cli/cli/comala_api.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.0/confluence_cli/cli/confluence_async.py` & `confluence_cli-0.8.1/confluence_cli/cli/confluence_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,115 @@
 import asyncio
 from json import dumps
 from typing import List
 from urllib.parse import urlencode
 
 import aiohttp
-from aiohttp import BasicAuth, ClientResponse
+from aiohttp import BasicAuth
 from aiologger import Logger
 from aiologger.formatters.base import Formatter
 from aiologger.levels import LogLevel
 from atlassian.errors import ApiValueError, ApiNotFoundError
 
 from confluence_cli.cli import ConfluenceWrapper
 from confluence_cli.cli.types import Page
 from confluence_cli.cli.utils import type_wrap
 
-aiologger = Logger.with_default_handlers(name="aio_confluence_log",
-                                         formatter=Formatter(
-                                             fmt='%(asctime)s,%(msecs)03d - %(levelname)s - %(filename)s - %(message)s'),
-                                         level=LogLevel.INFO)
+aiologger = Logger.with_default_handlers(
+    name="aio_confluence_log",
+    formatter=Formatter(
+        fmt="%(asctime)s,%(msecs)03d - %(levelname)s - %(filename)s - %(message)s"
+    ),
+    level=LogLevel.INFO,
+)
 
 
 class ConfluenceAsyncWrapper(object):
     """
     Use:
     async with ConfluenceAsyncWrapper(confluence) as aconflu:
         pages: Pages = await aconflu.async_update_pages(pages=all_pages)
     """
 
     def __init__(self, confluence_wrapper: ConfluenceWrapper):
         self.confluence_api = confluence_wrapper
 
-
     async def __aenter__(self):  # setting up a connection
-        self._aio_session = aiohttp.ClientSession(auth=BasicAuth(login=self.confluence_api.username,
-                                                                 password=self.confluence_api.password),
-                                                  headers=self.confluence_api._session.headers)
+        if self.confluence_api.username and self.confluence_api.password:
+            self._aio_session = aiohttp.ClientSession(
+                auth=BasicAuth(
+                    login=self.confluence_api.username,
+                    password=self.confluence_api.password,
+                ),
+                headers=self.confluence_api._session.headers,
+            )
+        else:
+            self._aio_session = aiohttp.ClientSession(
+                headers=self.confluence_api._session.headers
+            )
         return self
 
     async def __aexit__(self, *err):  # closing the connection
         await self._aio_session.close()
         self._aio_session = None
 
     async def async_update_pages(self, pages: List[Page]):
         """Needs to be executed inside confluence async context:
 
         with async confluence as api:
             await api.async_update_pages ..."""
         tasks = []
         for page in pages:
-            tasks.append(asyncio.create_task(self.async_update_page(page.id, page.title,
-                                                                    page.version.number,
-                                                                    body=page.body_storage,
-                                                                    always_update=True)))
+            tasks.append(
+                asyncio.create_task(
+                    self.async_update_page(
+                        page.id,
+                        page.title,
+                        page.version.number,
+                        page=page,
+                        body=page.body_storage,
+                        always_update=True,
+                    )
+                )
+            )
 
         return await asyncio.gather(*tasks)
 
-    async def async_update_page(self, page_id, title, preupdate_version: int,
-                                body=None,
-                                parent_id=None,
-                                type="page",
-                                representation="storage",
-                                minor_edit=False, version_comment=None, always_update=False):
+    async def async_update_page(
+        self,
+        page_id,
+        title,
+        preupdate_version: int,
+        page: Page = None,
+        body=None,
+        parent_id=None,
+        type="page",
+        representation="storage",
+        minor_edit=False,
+        version_comment=None,
+        always_update=False,
+    ):
 
         aiologger.info('Updating {type} "{title}"'.format(title=title, type=type))
 
-        if not always_update and body is not None \
-                and self.confluence_api.is_page_content_is_already_updated(page_id, body, title):
+        if (
+            not always_update
+            and body is not None
+            and self.confluence_api.is_page_content_is_already_updated(
+                page_id, body, title
+            )
+        ):
             return self.confluence_api.get_page_by_id(page_id)
 
         try:
             version = preupdate_version + 1
         except (IndexError, TypeError) as e:
-            aiologger.error("Can't find '{title}' {type}!".format(title=title, type=type))
+            aiologger.error(
+                "Can't find '{title}' {type}!".format(title=title, type=type)
+            )
             aiologger.debug(e)
             return None
 
         data = {
             "id": page_id,
             "type": type,
             "title": title,
@@ -85,41 +119,50 @@
             data["body"] = self.confluence_api._create_body(body, representation)
 
         if parent_id:
             data["ancestors"] = [{"type": "page", "id": parent_id}]
         if version_comment:
             data["version"]["message"] = version_comment
 
+        # * Set labels from page object
+        if page:
+            labels_lst = [{"name": label} for label in page.labels]
+            data["metadata"] = {"labels": {"results": labels_lst}}
+
         try:
-            response = await self.async_put("rest/api/content/{0}".format(page_id), data=data)
+            response = await self.async_put(
+                "rest/api/content/{0}".format(page_id), data=data
+            )
         except aiohttp.ClientResponseError as e:
             if e.status == 400:
                 raise ApiValueError(
                     "No space or no content type, or setup a wrong version "
                     "type set to content, or status param is not draft and "
                     "status content is current",
                     reason=e,
                 )
             if e.status == 404:
-                raise ApiNotFoundError("Can not find draft with current content", reason=e)
+                raise ApiNotFoundError(
+                    "Can not find draft with current content", reason=e
+                )
 
             raise
 
         return type_wrap(response)
 
     async def async_put(
-            self,
-            path,
-            data=None,
-            headers=None,
-            files=None,
-            trailing=None,
-            params=None,
-            absolute=False,
-            advanced_mode=False,
+        self,
+        path,
+        data=None,
+        headers=None,
+        files=None,
+        trailing=None,
+        params=None,
+        absolute=False,
+        advanced_mode=False,
     ):
         response = await self.async_request(
             "PUT",
             path=path,
             data=data,
             headers=headers,
             files=files,
@@ -127,51 +170,63 @@
             trailing=trailing,
             absolute=absolute,
         )
 
         return response
 
     async def async_request(
-            self,
-            method="GET",
-            path="/",
-            data=None,
-            json=None,
-            flags=None,
-            params=None,
-            headers=None,
-            files=None,
-            trailing=None,
-            absolute=False,
+        self,
+        method="GET",
+        path="/",
+        data=None,
+        json=None,
+        flags=None,
+        params=None,
+        headers=None,
+        files=None,
+        trailing=None,
+        absolute=False,
     ) -> dict:
 
-        url = self.confluence_api.url_joiner(None if absolute else self.confluence_api.url, path, trailing)
+        url = self.confluence_api.url_joiner(
+            None if absolute else self.confluence_api.url, path, trailing
+        )
         params_already_in_url = True if "?" in url else False
         if params or flags:
             if params_already_in_url:
                 url += "&"
             else:
                 url += "?"
         if params:
             url += urlencode(params or {})
         if flags:
-            url += ("&" if params or params_already_in_url else "") + "&".join(flags or [])
+            url += ("&" if params or params_already_in_url else "") + "&".join(
+                flags or []
+            )
         json_dump = None
         if files is None:
             data = None if not data else dumps(data)
             json_dump = None if not json else dumps(json)
-        self.confluence_api.log_curl_debug(method=method, url=url, headers=headers, data=data if data else json_dump)
+        self.confluence_api.log_curl_debug(
+            method=method, url=url, headers=headers, data=data if data else json_dump
+        )
         headers = headers or self.confluence_api.default_headers
         # * For multi part class aiohttp.FormData(fields, quote_fields=True, charset=None)
-        async with self._aio_session.request(method=method,
-                                             url=url,
-                                             headers=headers,
-                                             data=data,
-                                             json=json,
-                                             proxy=self.confluence_api.proxies["https"],
-                                             verify_ssl=self.confluence_api.verify_ssl) as response:
+        async with self._aio_session.request(
+            method=method,
+            url=url,
+            headers=headers,
+            data=data,
+            json=json,
+            proxy=self.confluence_api.proxies["https"],
+            verify_ssl=self.confluence_api.verify_ssl,
+        ) as response:
             # response.encoding = "utf-8"
-            aiologger.debug("HTTP: {} {} -> {} {}".format(method, path, response.status, response.reason))
+            aiologger.debug(
+                "HTTP: {} {} -> {} {}".format(
+                    method, path, response.status, response.reason
+                )
+            )
             aiologger.debug("HTTP: Response text -> {}".format(response.text))
 
             response.raise_for_status()
             return await response.json()
```

### Comparing `confluence_cli-0.8.0/confluence_cli/cli/confluence_limited.py` & `confluence_cli-0.8.1/confluence_cli/cli/confluence_limited.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.0/confluence_cli/cli/confluence_wrapper.py` & `confluence_cli-0.8.1/confluence_cli/cli/confluence_wrapper.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.0/confluence_cli/cli/paginators.py` & `confluence_cli-0.8.1/confluence_cli/cli/paginators.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,20 +142,26 @@
     def _get_results(self):
         start = 0
         total_size = 1
         while start < total_size:
             contents = self.confluence.cql(cql=self.cql, start=start, expand=self.expand, limit=self.page_size)
             if contents:
                 # confluence wrapper sets totalSize key inside content (see confluence wrapper cql method)
-                total_size = int(contents.get("totalSize"))
+                if isinstance(contents, dict):
+                    total_size = int(contents.get("totalSize"))
+                    content_lst = contents.get("results")
+                else:
+                    total_size = int(contents[0].get("totalSize"))
+                    content_lst = contents
             else:
                 logger.info("Total Size cql: 0")
                 self.total_size = 0
+                return
 
-            for content in contents.get("results"):
+            for content in content_lst:
                 yield content
             start = start + self.page_size
 
 
 class CQLPaginator(object):
     """Use like:
```

### Comparing `confluence_cli-0.8.0/confluence_cli/cli/types.py` & `confluence_cli-0.8.1/confluence_cli/cli/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,19 @@
     def body_storage(self):
         return self.body.storage.value
 
     @property
     def labels(self):
         return [label.name for label in self.metadata.labels.results]
 
+    @labels.setter
+    def labels(self, labels: List[str]):
+        label_regs = [{"name": label} for label in labels]
+        self.metadata.labels.results = label_regs
+
     @property
     def ancestor_ids(self):
         return [ancestor.id for ancestor in self.ancestors]
 
     @property
     def body_view(self):
         return self.body.export_view.value
```

### Comparing `confluence_cli-0.8.0/pyproject.toml` & `confluence_cli-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "confluence-cli"
-version = "0.8.0"
+version = "0.8.1"
 description = "Just another Atlassian Confluence API cli extension"
 authors = ["J. Andres Guerrero <juguerre@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "confluence_cli/cli"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0 <3.9"
-requests = "^2.28.1"
+requests = "~2.28.1"
 atlassian-python-api = "3.23.0"
 click = "^8.1.3"
 click-completion = "^0.5.2"
 tqdm = "^4.64.1"
 coloredlogs = "^15.0.1"
 urllib3 = "^1.26.13"
 python-decouple = "^3.6"
```

### Comparing `confluence_cli-0.8.0/PKG-INFO` & `confluence_cli-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluence-cli
-Version: 0.8.0
+Version: 0.8.1
 Summary: Just another Atlassian Confluence API cli extension
 License: MIT
 Author: J. Andres Guerrero
 Author-email: juguerre@gmail.com
 Requires-Python: >=3.8.0,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-completion (>=0.5.2,<0.6.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: python-box (>=6.1.0,<7.0.0)
 Requires-Dist: python-decouple (>=3.6,<4.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2.28.1,<2.29.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.13,<2.0.0)
 Description-Content-Type: text/markdown
 
 # confluence-cli
 
 confluence-cli is a convenient wrapper module for python atlassian confluence original package.
```

