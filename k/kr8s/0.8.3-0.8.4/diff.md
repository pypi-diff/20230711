# Comparing `tmp/kr8s-0.8.3.tar.gz` & `tmp/kr8s-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.8.3.tar", max compression
+gzip compressed data, was "kr8s-0.8.4.tar", max compression
```

## Comparing `kr8s-0.8.3.tar` & `kr8s-0.8.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-07 12:03:40.607465 kr8s-0.8.3/LICENSE
--rw-r--r--   0        0        0     2587 2023-07-07 12:03:40.607465 kr8s-0.8.3/README.md
--rw-r--r--   0        0        0     1143 2023-07-07 12:04:11.973384 kr8s-0.8.3/kr8s/__init__.py
--rw-r--r--   0        0        0    14674 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4336 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_io.py
--rw-r--r--   0        0        0    33118 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_objects.py
--rw-r--r--   0        0        0     8074 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/_testutils.py
--rw-r--r--   0        0        0      248 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1681 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-07 12:03:40.631466 kr8s-0.8.3/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     5909 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3394 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    17697 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-07 12:03:40.635467 kr8s-0.8.3/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2556 2023-07-07 12:04:11.973384 kr8s-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 kr8s-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-11 16:29:57.052792 kr8s-0.8.4/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-11 16:29:57.052792 kr8s-0.8.4/README.md
+-rw-r--r--   0        0        0     1143 2023-07-11 16:30:26.706629 kr8s-0.8.4/kr8s/__init__.py
+-rw-r--r--   0        0        0    14674 2023-07-11 16:29:57.072793 kr8s-0.8.4/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-07-11 16:29:57.072793 kr8s-0.8.4/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_io.py
+-rw-r--r--   0        0        0    33161 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     5909 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    17737 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2578 2023-07-11 16:30:26.706629 kr8s-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.4/PKG-INFO
```

### Comparing `kr8s-0.8.3/LICENSE` & `kr8s-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/README.md` & `kr8s-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/__init__.py` & `kr8s-0.8.4/kr8s/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .asyncio import (
     version as _version,
 )
 from .asyncio import (
     watch as _watch,
 )
 
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.8.3/kr8s/_api.py` & `kr8s-0.8.4/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/_auth.py` & `kr8s-0.8.4/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/_data_utils.py` & `kr8s-0.8.4/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/_io.py` & `kr8s-0.8.4/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/_objects.py` & `kr8s-0.8.4/kr8s/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 
 import anyio
 import httpx
 import jsonpath
 import yaml
+from box import Box
 
 import kr8s
 import kr8s.asyncio
 from kr8s._api import Api
 from kr8s._data_utils import dict_to_selector, dot_to_nested_dict, list_dict_unpack
 from kr8s._exceptions import NotFoundError
 from kr8s.asyncio.portforward import PortForward as AsyncPortForward
@@ -93,43 +94,43 @@
     def namespace(self) -> str:
         """Namespace of the Kubernetes resource."""
         if self.namespaced:
             return self.raw.get("metadata", {}).get("namespace", self.api.namespace)
         return None
 
     @property
-    def metadata(self) -> dict:
+    def metadata(self) -> Box:
         """Metadata of the Kubernetes resource."""
-        return self.raw["metadata"]
+        return Box(self.raw["metadata"])
 
     @property
-    def spec(self) -> dict:
+    def spec(self) -> Box:
         """Spec of the Kubernetes resource."""
-        return self.raw["spec"]
+        return Box(self.raw["spec"])
 
     @property
-    def status(self) -> dict:
+    def status(self) -> Box:
         """Status of the Kubernetes resource."""
-        return self.raw["status"]
+        return Box(self.raw["status"])
 
     @property
-    def labels(self) -> dict:
+    def labels(self) -> Box:
         """Labels of the Kubernetes resource."""
         try:
-            return self.raw["metadata"]["labels"]
+            return Box(self.raw["metadata"]["labels"])
         except KeyError:
-            return {}
+            return Box({})
 
     @property
-    def annotations(self) -> dict:
+    def annotations(self) -> Box:
         """Annotations of the Kubernetes resource."""
         try:
-            return self.raw["metadata"]["annotations"]
+            return Box(self.raw["metadata"]["annotations"])
         except KeyError:
-            return {}
+            return Box({})
 
     @property
     def replicas(self) -> int:
         """Replicas of the Kubernetes resource."""
         if self.scalable:
             keys = self.scalable_spec.split(".")
             spec = self.raw["spec"]
@@ -251,15 +252,15 @@
         except httpx.HTTPStatusError as e:
             if e.response.status_code == 404:
                 raise NotFoundError(f"Object {self.name} does not exist") from e
             raise e
 
     async def patch(self, patch, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
-        return await self._patch(patch, subresource=subresource)
+        await self._patch(patch, subresource=subresource)
 
     async def _patch(self, patch: Dict, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
         url = f"{self.endpoint}/{self.name}"
         if subresource:
             url = f"{url}/{subresource}"
         async with self.api.call_api(
```

### Comparing `kr8s-0.8.3/kr8s/_portforward.py` & `kr8s-0.8.4/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/_testutils.py` & `kr8s-0.8.4/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/asyncio/_api.py` & `kr8s-0.8.4/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/asyncio/_helpers.py` & `kr8s-0.8.4/kr8s/asyncio/_helpers.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/asyncio/objects.py` & `kr8s-0.8.4/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/conftest.py` & `kr8s-0.8.4/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/objects.py` & `kr8s-0.8.4/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.4/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/tests/test_api.py` & `kr8s-0.8.4/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/tests/test_auth.py` & `kr8s-0.8.4/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/tests/test_data_utils.py` & `kr8s-0.8.4/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/tests/test_io.py` & `kr8s-0.8.4/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/kr8s/tests/test_objects.py` & `kr8s-0.8.4/kr8s/tests/test_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,24 +531,25 @@
     objects = await objects_from_files(
         CURRENT_DIR / "resources" / "simple" / "nginx_pod.yaml", api=api
     )
     assert len(objects) == 1
     assert isinstance(objects[0], Pod)
     assert objects[0].kind == "Pod"
     assert objects[0].name == "nginx"
-    assert len(objects[0].spec["containers"]) == 1
+    assert len(objects[0].spec.containers) == 1
 
 
 async def test_objects_from_file():
     objects = await objects_from_files(
         CURRENT_DIR / "resources" / "simple" / "nginx_pod_service.yaml"
     )
     assert len(objects) == 2
     assert isinstance(objects[0], Pod)
     assert isinstance(objects[1], Service)
+    assert len(objects[1].spec.ports) == 1
 
 
 async def test_objects_from_files():
     simple_dir = CURRENT_DIR / "resources" / "simple"
     objects = await objects_from_files(simple_dir)
     assert len(objects) > 1
```

### Comparing `kr8s-0.8.3/kr8s/tests/test_testutils.py` & `kr8s-0.8.4/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.3/pyproject.toml` & `kr8s-0.8.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.8.3"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.4"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
@@ -35,14 +35,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.4"
 pyyaml = "^6.0"
 python-jsonpath = "^0.7.1"
 anyio = "^3.7.0"
 httpx = "^0.24.1"
+python-box = "^7.0.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
```

### Comparing `kr8s-0.8.3/PKG-INFO` & `kr8s-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.8.3
+Version: 0.8.4
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: python-box (>=7.0.1,<8.0.0)
 Requires-Dist: python-jsonpath (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
 
 [![Test](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml/badge.svg)](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml)
```

