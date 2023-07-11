# Comparing `tmp/Perfole-0.0.4.tar.gz` & `tmp/Perfole-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Perfole-0.0.4.tar", last modified: Mon Jul 10 13:14:09 2023, max compression
+gzip compressed data, was "Perfole-0.0.5.tar", last modified: Tue Jul 11 21:11:11 2023, max compression
```

## Comparing `Perfole-0.0.4.tar` & `Perfole-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 13:14:09.005096 Perfole-0.0.4/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 13:14:09.004964 Perfole-0.0.4/PKG-INFO
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 13:14:09.003996 Perfole-0.0.4/Perfole/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12896 2023-07-10 13:13:47.000000 Perfole-0.0.4/Perfole/Perfole.py
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.4/Perfole/__init__.py
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 13:14:09.004736 Perfole-0.0.4/Perfole.egg-info/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/PKG-INFO
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/SOURCES.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/dependency_links.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/requires.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/top_level.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1183 2023-07-10 11:07:54.000000 Perfole-0.0.4/README.md
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.4/license.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 13:14:09.005138 Perfole-0.0.4/setup.cfg
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-10 13:14:03.000000 Perfole-0.0.4/setup.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-11 21:11:11.086309 Perfole-0.0.5/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1402 2023-07-11 21:11:11.086030 Perfole-0.0.5/PKG-INFO
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-11 21:11:11.084350 Perfole-0.0.5/Perfole/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12878 2023-07-11 21:05:52.000000 Perfole-0.0.5/Perfole/Perfole.py
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.5/Perfole/__init__.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-11 21:11:11.085526 Perfole-0.0.5/Perfole.egg-info/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1402 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/PKG-INFO
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/SOURCES.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/dependency_links.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/requires.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/top_level.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1211 2023-07-10 13:19:25.000000 Perfole-0.0.5/README.md
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.5/license.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-11 21:11:11.086367 Perfole-0.0.5/setup.cfg
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-11 21:09:13.000000 Perfole-0.0.5/setup.py
```

### Comparing `Perfole-0.0.4/PKG-INFO` & `Perfole-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.4
+Version: 0.0.5
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 
 Package for measuring software performance. Measuring is done by defining start and end point to measure. 
 Start and end point is called action. Action should have meaningful name. Multiple actions can exist.
 
-<!-- ## Import
-import Perfole; -->
+## Import
+```
+from Perfole.Perfole import PERFORMANCE_TEST
+```
 
 ## Set start/end points
 ```
     PERFORMANCE_TEST.StartAction(name...)
     ...
     PERFORMANCE_TEST.EndAction(name...)
 ```
```

### Comparing `Perfole-0.0.4/Perfole/Perfole.py` & `Perfole-0.0.5/Perfole/Perfole.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import requests
 import json
 import threading
-import asyncio
+import socket
 
 class PERFORMANCE_TEST:
     argumentsValue = {'shouldMeasure':False}
     actionsBeforeCalculation ={}
     calculatedActions ={}
     calculatedActionsPublish =[]
     execution_start_time=0
@@ -44,15 +44,15 @@
                         PERFORMANCE_TEST.argumentsValue['appVersion'] = "1.0"
 
                     if (machineName != ""):
                         PERFORMANCE_TEST.argumentsValue['machineName'] = machineName
                     else:
                         try:
                             import os
-                            PERFORMANCE_TEST.argumentsValue['machineName'] = os.uname()[1]#Environment.MachineName
+                            PERFORMANCE_TEST.argumentsValue['machineName'] = socket.gethostname()
                         except:
                             PERFORMANCE_TEST.argumentsValue['machineName'] = "Unknown"
                     pub = PERFORMANCE_TEST.publishResult(apiKey)
                     if (pub):
                         return PERFORMANCE_TEST.calculatedActions
                     else:
                         return []
```

### Comparing `Perfole-0.0.4/Perfole.egg-info/PKG-INFO` & `Perfole-0.0.5/Perfole.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.4
+Version: 0.0.5
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 
 Package for measuring software performance. Measuring is done by defining start and end point to measure. 
 Start and end point is called action. Action should have meaningful name. Multiple actions can exist.
 
-<!-- ## Import
-import Perfole; -->
+## Import
+```
+from Perfole.Perfole import PERFORMANCE_TEST
+```
 
 ## Set start/end points
 ```
     PERFORMANCE_TEST.StartAction(name...)
     ...
     PERFORMANCE_TEST.EndAction(name...)
 ```
```

### Comparing `Perfole-0.0.4/README.md` & `Perfole-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 Package for measuring software performance. Measuring is done by defining start and end point to measure. 
 Start and end point is called action. Action should have meaningful name. Multiple actions can exist.
 
-<!-- ## Import
-import Perfole; -->
+## Import
+```
+from Perfole.Perfole import PERFORMANCE_TEST
+```
 
 ## Set start/end points
 ```
     PERFORMANCE_TEST.StartAction(name...)
     ...
     PERFORMANCE_TEST.EndAction(name...)
 ```
```

### Comparing `Perfole-0.0.4/license.txt` & `Perfole-0.0.5/license.txt`

 * *Files identical despite different names*

