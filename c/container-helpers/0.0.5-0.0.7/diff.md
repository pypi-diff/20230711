# Comparing `tmp/container_helpers-0.0.5.tar.gz` & `tmp/container_helpers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container_helpers-0.0.5.tar", max compression
+gzip compressed data, was "container_helpers-0.0.7.tar", max compression
```

## Comparing `container_helpers-0.0.5.tar` & `container_helpers-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-07-01 06:46:17.196872 container_helpers-0.0.5/LICENSE
--rw-r--r--   0        0        0      438 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/__init__.py
--rw-r--r--   0        0        0     1237 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/data_types.py
--rw-r--r--   0        0        0        0 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/__init__.py
--rw-r--r--   0        0        0      190 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/base.py
--rw-r--r--   0        0        0      773 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/helpers.py
--rw-r--r--   0        0        0     5119 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/podman.py
--rw-r--r--   0        0        0      388 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/services/__init__.py
--rw-r--r--   0        0        0     2720 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/services/base.py
--rw-r--r--   0        0        0     4470 2023-07-01 06:46:17.200872 container_helpers-0.0.5/containers/services/windows.py
--rw-r--r--   0        0        0      568 2023-07-01 06:46:17.200872 container_helpers-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-11 07:04:41.390212 container_helpers-0.0.7/LICENSE
+-rw-r--r--   0        0        0      438 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/data_types.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/base.py
+-rw-r--r--   0        0        0      773 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/helpers.py
+-rw-r--r--   0        0        0     5119 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/podman.py
+-rw-r--r--   0        0        0      388 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/services/__init__.py
+-rw-r--r--   0        0        0     2720 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/services/base.py
+-rw-r--r--   0        0        0     4470 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/services/windows.py
+-rw-r--r--   0        0        0      568 2023-07-11 07:04:41.390212 container_helpers-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.7/PKG-INFO
```

### Comparing `container_helpers-0.0.5/LICENSE` & `container_helpers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.5/containers/data_types.py` & `container_helpers-0.0.7/containers/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     target: PathType
 
 
 @dataclasses.dataclass
 class BindMount(Mount):
     source: PathType
     readonly: bool
-    chown: bool = True
+    chown: bool = False
     relabel: typing.Optional[str] = None
     bind_propagation: typing.Optional[str] = None
 
 
 @dataclasses.dataclass
 class VolumeMount(Mount):
     readonly: bool
-    chown: bool = True
+    chown: bool = False
 
 
 @dataclasses.dataclass
 class ImageMount(Mount):
     source: str
     read_write: bool = False
```

### Comparing `container_helpers-0.0.5/containers/providers/helpers.py` & `container_helpers-0.0.7/containers/providers/helpers.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.5/containers/providers/podman.py` & `container_helpers-0.0.7/containers/providers/podman.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.5/containers/services/base.py` & `container_helpers-0.0.7/containers/services/base.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.5/containers/services/windows.py` & `container_helpers-0.0.7/containers/services/windows.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.5/pyproject.toml` & `container_helpers-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "container-helpers"
-version = "0.0.5"
+version = "0.0.7"
 description = "Helpers for running docker or podman containers easily in Python"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/container-helpers"
 packages = [{include = "containers"}]
 
 [tool.poetry.dependencies]
```

### Comparing `container_helpers-0.0.5/PKG-INFO` & `container_helpers-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-helpers
-Version: 0.0.5
+Version: 0.0.7
 Summary: Helpers for running docker or podman containers easily in Python
 Home-page: https://github.com/LaunchPlatform/container-helpers
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

