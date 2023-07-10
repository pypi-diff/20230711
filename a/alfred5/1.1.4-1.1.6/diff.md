# Comparing `tmp/alfred5-1.1.4.tar.gz` & `tmp/alfred5-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.1.4.tar", last modified: Sun May 14 20:05:56 2023, max compression
+gzip compressed data, was "alfred5-1.1.6.tar", last modified: Mon Jul 10 23:52:44 2023, max compression
```

## Comparing `alfred5-1.1.4.tar` & `alfred5-1.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.983430 alfred5-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-14 20:05:48.000000 alfred5-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 20:05:48.000000 alfred5-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-14 20:05:56.983430 alfred5-1.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-14 20:05:48.000000 alfred5-1.1.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:05:56.983430 alfred5-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-14 20:05:48.000000 alfred5-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.983430 alfred5-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:48.000000 alfred5-1.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 20:05:48.000000 alfred5-1.1.4/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:44.344384 alfred5-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-10 23:52:35.000000 alfred5-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:52:35.000000 alfred5-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-10 23:52:44.344384 alfred5-1.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:44.344384 alfred5-1.1.6/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 23:52:35.000000 alfred5-1.1.6/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-10 23:52:35.000000 alfred5-1.1.6/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-10 23:52:35.000000 alfred5-1.1.6/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:44.344384 alfred5-1.1.6/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-10 23:52:35.000000 alfred5-1.1.6/alfred5/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-07-10 23:52:35.000000 alfred5-1.1.6/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-10 23:52:35.000000 alfred5-1.1.6/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:44.344384 alfred5-1.1.6/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-10 23:52:44.000000 alfred5-1.1.6/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-10 23:52:44.000000 alfred5-1.1.6/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:52:44.000000 alfred5-1.1.6/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:52:44.000000 alfred5-1.1.6/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-10 23:52:44.000000 alfred5-1.1.6/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:52:44.000000 alfred5-1.1.6/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:44.344384 alfred5-1.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-10 23:52:35.000000 alfred5-1.1.6/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:52:44.344384 alfred5-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-10 23:52:35.000000 alfred5-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:44.344384 alfred5-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 23:52:35.000000 alfred5-1.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-10 23:52:35.000000 alfred5-1.1.6/tests/test_snippets.py
```

### Comparing `alfred5-1.1.4/LICENSE` & `alfred5-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.4/PKG-INFO` & `alfred5-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.4
+Version: 1.1.6
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
```

### Comparing `alfred5-1.1.4/alfred5/client.py` & `alfred5-1.1.6/alfred5/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
-from logging import Logger, StreamHandler
+
 import json
-import pkg_resources
-from .models import Result
-from traceback import format_exc
 import sys
 from asyncio import run
 from collections.abc import Callable, Coroutine
+from logging import Logger, StreamHandler
 from pathlib import Path
+from plistlib import load as plist_load
 from shutil import copy2, move
 from tempfile import TemporaryDirectory
-from zipfile import ZIP_DEFLATED, ZipFile
-from ruamel.yaml import load as yaml_load, dump as yaml_dump
-from plistlib import load as plist_load
-from .models import SNIPPET_INFO_TEMPLATE, Result, Snippet
+from traceback import format_exc
 from typing import NoReturn
+from zipfile import ZIP_DEFLATED, ZipFile
+
+import pkg_resources
+from yaml import safe_dump, safe_load
+
 from .errors import WorkflowError
-from ruamel.yaml import YAML
+from .models import SNIPPET_INFO_TEMPLATE, Result, Snippet
 
 
 class SnippetClient:
     snippets: list[Snippet]
 
     def __init__(self) -> None:
         self.snippets: list[Snippet] = []
@@ -99,16 +100,14 @@
         self.datadir = Path("db")
         self.datadir.mkdir(parents=True, exist_ok=True)
 
         self.log(f"datadir: {self.datadir.absolute()}")
         self.db_results = self.datadir / "results.yml"
         self.log(f"db_results: {self.db_results}")
 
-        self.yaml = YAML()
-
         self.results = []
 
     def log(self, msg: str):
         self.logger.debug(msg)
 
     def install_requirements(self) -> None:
         """Check if requirements are met"""
@@ -149,38 +148,38 @@
 
     def cache_response(self) -> None:
         """Cache response to workflow db_results"""
         if not self.db_results.exists():
             self.db_results.parent.mkdir(parents=True, exist_ok=True)
             self.db_results.touch()
         with self.db_results.open("r") as f:
-            data = yaml_load(f) or {}
+            data = safe_load(f) or {}
         data[self.bare_query] = [
             {
                 "title": result.title,
                 "subtitle": result.subtitle,
                 "icon_path": result.icon.path if result.icon else None,
                 "arg": result.arg,
             }
             for result in self.results
         ]
         with self.db_results.open("w") as f:
-            yaml_dump(data, f)
+            safe_dump(data, f)
             self.log(f"cached response to {self.db_results}")
 
     def load_cached_response(self) -> bool:
         """Load cached result from alfred"""
         if self.bare_query:
             self.log("skipped, bare_query is None")
             return False
 
         self.log(f"checking if `{self.bare_query}` exists in `{self.db_results}`")
         if self.db_results.exists():
             with self.db_results.open("r") as f:
-                data: dict[str, list[dict[str, str]]] = self.yaml.load(f)
+                data: dict[str, list[dict[str, str]]] = safe_load(f)
                 self.log(f"loaded data from {self.db_results} {len(data.keys())}")
                 if self.bare_query and self.bare_query in data:
                     self.results = [
                         Result(
                             title=result["title"],
                             subtitle=result["subtitle"],
                             icon=Result.Icon(result["icon_path"])
```

### Comparing `alfred5-1.1.4/alfred5/icons/download.png` & `alfred5-1.1.6/alfred5/icons/download.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.4/alfred5/icons/error.png` & `alfred5-1.1.6/alfred5/icons/error.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.4/alfred5/models.py` & `alfred5-1.1.6/alfred5/models.py`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.4/alfred5.egg-info/PKG-INFO` & `alfred5-1.1.6/alfred5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.4
+Version: 1.1.6
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
```

### Comparing `alfred5-1.1.4/docs/README.md` & `alfred5-1.1.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.4/setup.py` & `alfred5-1.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 
 References: 
     - https://github.com/openai/openai-python/blob/main/setup.cfg
 """
 
 from glob import glob
 from os.path import basename, splitext
-from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.1.4"
+from setuptools import find_packages, setup
+
+VERSION = "1.1.6"
 DESCRIPTION = "Simple python wrapper for alfred5 workflow / snippets"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
 KEYWORDS = [
     "alfred",
     "alfred5",
     "workflow",
     "snippets",
     "alfred-workflows",
     "alfred-snippets",
 ]
-INSTALL_REQUIRES = ["aiohttp==3.8.4", "ruamel.yaml==0.17.21"]
+INSTALL_REQUIRES = ["aiohttp==3.8.4", "PyYAML==6.0"]
 EXSTRAS_REQUIRE = {
     "dev": [
         "black==23.3.0",
         "autoflake==2.0.2",
         "pytest==7.3.0",
         "pytest-asyncio==0.21.0",
     ]
```

