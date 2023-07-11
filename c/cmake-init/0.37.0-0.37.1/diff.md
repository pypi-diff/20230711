# Comparing `tmp/cmake-init-0.37.0.tar.gz` & `tmp/cmake-init-0.37.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake-init-0.37.0.tar", last modified: Wed Jul  5 01:08:34 2023, max compression
+gzip compressed data, was "cmake-init-0.37.1.tar", last modified: Tue Jul 11 15:36:38 2023, max compression
```

## Comparing `cmake-init-0.37.0.tar` & `cmake-init-0.37.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:08:34.928245 cmake-init-0.37.0/
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-05 01:08:34.928245 cmake-init-0.37.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:08:34.928245 cmake-init-0.37.0/cmake_init.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:08:34.928245 cmake-init-0.37.0/cmake_init_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/cmake_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/template.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:08:34.928245 cmake-init-0.37.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-05 01:08:24.000000 cmake-init-0.37.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:36:38.814165 cmake-init-0.37.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-11 15:36:38.814165 cmake-init-0.37.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:36:38.810166 cmake-init-0.37.1/cmake_init.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:36:38.814165 cmake-init-0.37.1/cmake_init_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init_lib/cmake_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-11 15:36:38.000000 cmake-init-0.37.1/cmake_init_lib/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:36:38.814165 cmake-init-0.37.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-11 15:36:20.000000 cmake-init-0.37.1/setup.py
```

### Comparing `cmake-init-0.37.0/PKG-INFO` & `cmake-init-0.37.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-init
-Version: 0.37.0
+Version: 0.37.1
 Summary: The missing CMake project initializer
 Home-page: https://github.com/friendlyanon/cmake-init
 Author: friendlyanon
 Author-email: friendlyanon_@hotmail.com
 License: GPLv3+
 Description: # `cmake-init` - The missing CMake project initializer
```

### Comparing `cmake-init-0.37.0/cmake_init.egg-info/PKG-INFO` & `cmake-init-0.37.1/cmake_init.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-init
-Version: 0.37.0
+Version: 0.37.1
 Summary: The missing CMake project initializer
 Home-page: https://github.com/friendlyanon/cmake-init
 Author: friendlyanon
 Author-email: friendlyanon_@hotmail.com
 License: GPLv3+
 Description: # `cmake-init` - The missing CMake project initializer
```

### Comparing `cmake-init-0.37.0/cmake_init_lib/cmake_init.py` & `cmake-init-0.37.1/cmake_init_lib/cmake_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 import platform
 import re
 import subprocess
 import sys
 import zipfile
 
-__version__ = "0.37.0"
+__version__ = "0.37.1"
 
 is_windows = os.name == "nt"
 
 compile_template = None
 
 
 class Language:
```

### Comparing `cmake-init-0.37.0/cmake_init_lib/template.py` & `cmake-init-0.37.1/cmake_init_lib/template.py`

 * *Files identical despite different names*

### Comparing `cmake-init-0.37.0/setup.py` & `cmake-init-0.37.1/setup.py`

 * *Files identical despite different names*

