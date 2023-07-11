# Comparing `tmp/sessypy-0.1.0.tar.gz` & `tmp/sessypy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessypy-0.1.0.tar", last modified: Sat Jul  1 15:05:02 2023, max compression
+gzip compressed data, was "sessypy-0.1.1.tar", last modified: Tue Jul 11 17:22:42 2023, max compression
```

## Comparing `sessypy-0.1.0.tar` & `sessypy-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-01 15:04:48.000000 sessypy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 15:05:02.806926 sessypy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 15:04:48.000000 sessypy-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-01 15:04:48.000000 sessypy-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-01 15:05:02.806926 sessypy-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/src/sessypy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/src/sessypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.420795 sessypy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-11 17:22:30.000000 sessypy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 17:22:42.420795 sessypy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 17:22:30.000000 sessypy-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-11 17:22:30.000000 sessypy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-11 17:22:42.420795 sessypy-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.416794 sessypy-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.420795 sessypy-0.1.1/src/sessypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.420795 sessypy-0.1.1/src/sessypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/top_level.txt
```

### Comparing `sessypy-0.1.0/LICENSE` & `sessypy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.0/PKG-INFO` & `sessypy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sessypy-0.1.0/src/sessypy/api.py` & `sessypy-0.1.1/src/sessypy/api.py`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.0/src/sessypy/const.py` & `sessypy-0.1.1/src/sessypy/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,18 @@
     WAITING_SAFE = "SYSTEM_STATE_WAITING_IN_SAFE_SITUATION"
     WAITING_PERIPHERALS = "SYSTEM_STATE_WAIT_FOR_PERIPHERALS"
     ERROR = "SYSTEM_STATE_ERROR"
     INITIALIZING = "SYSTEM_STATE_INIT", 
     OVERRIDE_OVER_FREQUENCY = "SYSTEM_STATE_OVERRIDE_OVERFREQUENCY", 
     OVERRIDE_UNDER_FREQUENCY = "SYSTEM_STATE_OVERRIDE_UNDERFREQUENCY", 
     DISCONNECT = "SYSTEM_STATE_DISCONNECT", 
-    RECONNECT = "SYSTEM_STATE_RECONNECT", 
-    BATTERY_EMPTY_OR_FULL = "SYSTEM_STATE_BATTERY_EMPTY_OR_FULL"
+    RECONNECT = "SYSTEM_STATE_RECONNECT",
+    BATTERY_EMPTY_OR_FULL = "SYSTEM_STATE_BATTERY_EMPTY_OR_FULL"  # unused as of version 1.5.0
+    BATTERY_FULL = "SYSTEM_STATE_BATTERY_FULL"
+    BATTERY_EMPTY = "SYSTEM_STATE_BATTERY_EMPTY"
 
 class SessyP1State(str, Enum):
     NOT_CONNECTED = "P1_NOT_CONNECTED"
     DATA_VALIDITY_ERROR = "P1_DATAVALIDITY_ERR"
     VERSION_ERROR = "P1_VERSION_ERR"
     PARSE_ERROR = "P1_PARSE_ERR"
     OK = "P1_OK"
```

### Comparing `sessypy-0.1.0/src/sessypy/devices.py` & `sessypy-0.1.1/src/sessypy/devices.py`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.0/src/sessypy.egg-info/PKG-INFO` & `sessypy-0.1.1/src/sessypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

