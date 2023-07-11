# Comparing `tmp/dice_lib-0.5.0.tar.gz` & `tmp/dice_lib-2023.7.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dice_lib-0.5.0.tar", last modified: Fri Jan 20 16:55:04 2023, max compression
+gzip compressed data, was "dice_lib-2023.7.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dice_lib-0.5.0.tar` & `dice_lib-2023.7.11.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1523 2023-01-20 16:54:55.883466 dice_lib-0.5.0/LICENSE
--rw-r--r--   0        0        0     1029 2023-01-20 16:54:55.883466 dice_lib-0.5.0/README.md
--rw-r--r--   0        0        0     2192 2023-01-20 16:54:55.883466 dice_lib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      157 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/__init__.py
--rw-r--r--   0        0        0     1824 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/_config.py
--rw-r--r--   0        0        0      267 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/date.py
--rw-r--r--   0        0        0      267 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/distributed/__init__.py
--rw-r--r--   0        0        0     3002 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/__init__.py
--rw-r--r--   0        0        0     2209 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_base.py
--rw-r--r--   0        0        0       75 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_davix.py
--rw-r--r--   0        0        0       77 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_gridftp.py
--rw-r--r--   0        0        0     2745 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_hdfs.py
--rw-r--r--   0        0        0     3503 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_posix.py
--rw-r--r--   0        0        0       72 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_s3.py
--rw-r--r--   0        0        0       76 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/fs/_xrootd.py
--rw-r--r--   0        0        0      606 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/glossary.py
--rw-r--r--   0        0        0     2163 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/hdfs.py
--rw-r--r--   0        0        0     5144 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/host.py
--rw-r--r--   0        0        0        0 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/network/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/py.typed
--rw-r--r--   0        0        0      581 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/ranges.py
--rw-r--r--   0        0        0      743 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/units.py
--rw-r--r--   0        0        0      710 2023-01-20 16:54:55.883466 dice_lib-0.5.0/src/dice_lib/user.py
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 dice_lib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/LICENSE
+-rw-r--r--   0        0        0     1029 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/README.md
+-rw-r--r--   0        0        0     2249 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/_config.py
+-rw-r--r--   0        0        0      267 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/date.py
+-rw-r--r--   0        0        0      267 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/distributed/__init__.py
+-rw-r--r--   0        0        0     3241 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/__init__.py
+-rw-r--r--   0        0        0     2209 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_base.py
+-rw-r--r--   0        0        0       75 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_davix.py
+-rw-r--r--   0        0        0       77 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_gridftp.py
+-rw-r--r--   0        0        0     2745 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_hdfs.py
+-rw-r--r--   0        0        0     3164 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_posix.py
+-rw-r--r--   0        0        0       72 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_s3.py
+-rw-r--r--   0        0        0       76 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/fs/_xrootd.py
+-rw-r--r--   0        0        0      606 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/glossary.py
+-rw-r--r--   0        0        0     2163 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/hdfs.py
+-rw-r--r--   0        0        0      146 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/health/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/health/apel_accounting.py
+-rw-r--r--   0        0        0     5144 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/host.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/network/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/py.typed
+-rw-r--r--   0        0        0      581 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/ranges.py
+-rw-r--r--   0        0        0      743 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/units.py
+-rw-r--r--   0        0        0      710 2023-07-11 14:20:16.857333 dice_lib-2023.7.11/src/dice_lib/user.py
+-rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 dice_lib-2023.7.11/PKG-INFO
```

### Comparing `dice_lib-0.5.0/LICENSE` & `dice_lib-2023.7.11/LICENSE`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/README.md` & `dice_lib-2023.7.11/README.md`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/pyproject.toml` & `dice_lib-2023.7.11/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "Programming Language :: Python :: 3.10",
     "Development Status :: 1 - Planning",
 ]
 
 
 dynamic = ["version"]
 dependencies = [
+    "beautifulsoup4 < 5",
     "dnspython>=2.2.0",
     "htcondor<10.0.0",
     "omegaconf>=2.1.2",
     "pandas<1.5.0",
     "paramiko",
     "plumbum",
     "pyarrow>=5.0.0",
@@ -93,10 +94,12 @@
 disallow_untyped_decorators = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 no_implicit_reexport = true
 strict_equality = true
+ignore_missing_imports = true
+
 
 [tool.isort]
 profile = "black"
```

### Comparing `dice_lib-0.5.0/src/dice_lib/_config.py` & `dice_lib-2023.7.11/src/dice_lib/_config.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/fs/__init__.py` & `dice_lib-2023.7.11/src/dice_lib/fs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, List, Tuple, Type
 
+from .._config import DEFAULT_DICE_CONFIG_PATH, load_config
 from ._base import FileSystem
 from ._davix import DavixFileSystem
 from ._gridftp import GridFTPFileSystem
 from ._hdfs import HDFS
 from ._posix import PosixFileSystem
 from ._s3 import S3FileSystem
 from ._xrootd import XrootDFileSystem
@@ -27,15 +28,15 @@
     "GridFTPFileSystem",
     "PosixFileSystem",
     "S3FileSystem",
     "XRootDFileSystem",
 ]
 
 
-def __deduce_fs_from_path(path: str) -> FileSystem:
+def _deduce_fs_from_path(path: str) -> FileSystem:
     for prefix, factory in FACTORIES.items():
         if path.startswith(prefix):
             return factory()
     return FACTORIES["Default"]()
 
 
 def get_mount_settings_from_config(config: Dict[str, Any]) -> MountSettings:
@@ -77,19 +78,21 @@
                 )
                 if remove_mount_for_native_access:
                     path = path[len(mount) :]
                 processed_paths[processed_paths.index(original_path)] = protocol + path
     return processed_paths
 
 
-def get_owner(pathstr: str, mount_settings: MountSettings) -> str:
-    pathstr = prepare_paths([pathstr], mount_settings)[0]
-    fs = __deduce_fs_from_path(pathstr)
-    return fs.get_owner(pathstr)
-
-
-def size_of_paths(
-    paths: List[str], mount_settings: MountSettings
-) -> List[Tuple[str, int, float, str]]:
-    paths = prepare_paths(paths, mount_settings)
-    fs = __deduce_fs_from_path(paths[0])
-    return fs.size_of_paths(paths)
+class FSClient:
+    def __init__(self, config_path: str = DEFAULT_DICE_CONFIG_PATH):
+        config = load_config(config_path)
+        self.mount_settings = get_mount_settings_from_config(config)
+
+    def get_owner(self, pathstr: str) -> str:
+        pathstr = prepare_paths([pathstr], self.mount_settings)[0]
+        fs = _deduce_fs_from_path(pathstr)
+        return fs.get_owner(pathstr)
+
+    def size_of_paths(self, paths: List[str]) -> List[Tuple[str, int, float, str]]:
+        paths = prepare_paths(paths, self.mount_settings)
+        fs = _deduce_fs_from_path(paths[0])
+        return fs.size_of_paths(paths)
```

### Comparing `dice_lib-0.5.0/src/dice_lib/fs/_base.py` & `dice_lib-2023.7.11/src/dice_lib/fs/_base.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/fs/_hdfs.py` & `dice_lib-2023.7.11/src/dice_lib/fs/_hdfs.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/fs/_posix.py` & `dice_lib-2023.7.11/src/dice_lib/fs/_posix.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,28 +31,16 @@
 
     def size_of_path(self, path: str) -> Tuple[str, int, float, str]:
         total, _ = self._size_cmd(path).split()
         total = int(total)
         total_scaled, unit = convert_to_largest_unit(total, "B", scale=1024)
         return str(path), total, total_scaled, unit
 
-    def __size_of_path(
-        self, path: str, size_cmd: BoundCommand
-    ) -> Tuple[str, int, float, str]:
-        tmp = self._size_cmd
-        self._size_cmd = size_cmd
-        result = self.size_of_path(path)
-        self._size_cmd = tmp
-        return result
-
     def size_of_paths(self, paths: List[str]) -> List[Tuple[str, int, float, str]]:
-        return [
-            self.__size_of_path(path, lambda path: self._size_cmd[path]())
-            for path in paths
-        ]
+        return [self.size_of_path(path) for path in paths]
 
     def copy(self, src: str, dest: str) -> None:
         self._copy_cmd(src, dest)
 
     def copy_recursive(self, src: str, dest: str) -> None:
         self._copy_recursive_cmd(src, dest)
```

### Comparing `dice_lib-0.5.0/src/dice_lib/glossary.py` & `dice_lib-2023.7.11/src/dice_lib/glossary.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/hdfs.py` & `dice_lib-2023.7.11/src/dice_lib/hdfs.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/host.py` & `dice_lib-2023.7.11/src/dice_lib/host.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/ranges.py` & `dice_lib-2023.7.11/src/dice_lib/ranges.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/units.py` & `dice_lib-2023.7.11/src/dice_lib/units.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/src/dice_lib/user.py` & `dice_lib-2023.7.11/src/dice_lib/user.py`

 * *Files identical despite different names*

### Comparing `dice_lib-0.5.0/PKG-INFO` & `dice_lib-2023.7.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dice_lib
-Version: 0.5.0
+Version: 2023.7.11
 Summary: Python Library for DICE
 Author-email: UoB DICE team <lcg-admin@bristol.ac.uk>
 Maintainer-email: The UoB DICE Team <lcg-admin@bristol.ac.uk>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 1 - Planning
+Requires-Dist: beautifulsoup4 < 5
 Requires-Dist: dnspython>=2.2.0
 Requires-Dist: htcondor<10.0.0
 Requires-Dist: omegaconf>=2.1.2
 Requires-Dist: pandas<1.5.0
 Requires-Dist: paramiko
 Requires-Dist: plumbum
 Requires-Dist: pyarrow>=5.0.0
```

