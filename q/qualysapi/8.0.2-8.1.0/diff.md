# Comparing `tmp/qualysapi-8.0.2.tar.gz` & `tmp/qualysapi-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualysapi-8.0.2.tar", last modified: Tue Jul 19 16:00:40 2022, max compression
+gzip compressed data, was "qualysapi-8.1.0.tar", last modified: Tue Jul 11 13:39:09 2023, max compression
```

## Comparing `qualysapi-8.0.2.tar` & `qualysapi-8.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 16:00:40.307663 qualysapi-8.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-07-19 16:00:30.000000 qualysapi-8.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5344 2022-07-19 16:00:40.307663 qualysapi-8.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4551 2022-07-19 16:00:30.000000 qualysapi-8.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 16:00:40.307663 qualysapi-8.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-example.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-section-example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-simple-v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-simple-v2-creds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-simple-v2-report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-simple-v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-07-19 16:00:30.000000 qualysapi-8.0.2/examples/qualysapi-virtualhost.py
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-07-19 16:00:30.000000 qualysapi-8.0.2/license
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-19 16:00:30.000000 qualysapi-8.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 16:00:40.307663 qualysapi-8.0.2/qualysapi/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20036 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/api_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/api_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     6428 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/api_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    23747 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-19 16:00:30.000000 qualysapi-8.0.2/qualysapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 16:00:40.307663 qualysapi-8.0.2/qualysapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5344 2022-07-19 16:00:40.000000 qualysapi-8.0.2/qualysapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-07-19 16:00:40.000000 qualysapi-8.0.2/qualysapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 16:00:40.000000 qualysapi-8.0.2/qualysapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-19 16:00:40.000000 qualysapi-8.0.2/qualysapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-07-19 16:00:40.000000 qualysapi-8.0.2/qualysapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-07-19 16:00:40.307663 qualysapi-8.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-07-19 16:00:30.000000 qualysapi-8.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:39:09.022475 qualysapi-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 13:38:57.000000 qualysapi-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-11 13:39:09.022475 qualysapi-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-11 13:38:57.000000 qualysapi-8.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:39:09.022475 qualysapi-8.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-section-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-simple-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-simple-v2-creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-simple-v2-report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-simple-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 13:38:57.000000 qualysapi-8.1.0/examples/qualysapi-virtualhost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-11 13:38:57.000000 qualysapi-8.1.0/license
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 13:38:57.000000 qualysapi-8.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:39:09.022475 qualysapi-8.1.0/qualysapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20864 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/api_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/api_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/api_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-11 13:38:57.000000 qualysapi-8.1.0/qualysapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:39:09.022475 qualysapi-8.1.0/qualysapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-11 13:39:08.000000 qualysapi-8.1.0/qualysapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 13:39:08.000000 qualysapi-8.1.0/qualysapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:39:08.000000 qualysapi-8.1.0/qualysapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 13:39:08.000000 qualysapi-8.1.0/qualysapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 13:39:08.000000 qualysapi-8.1.0/qualysapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-11 13:39:09.026476 qualysapi-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-11 13:38:57.000000 qualysapi-8.1.0/setup.py
```

### Comparing `qualysapi-8.0.2/PKG-INFO` & `qualysapi-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: qualysapi
-Version: 8.0.2
+Version: 8.1.0
 Summary: Qualys API Helper
 Home-page: https://github.com/paragbaxi/qualysapi
 Author: Parag Baxi
 Author-email: parag.baxi@gmail.com
 License: BSD-new
 Project-URL: Bug Tracker, https://github.com/paragbaxi/qualysapi/issues
 Project-URL: Source Code, https://github.com/paragbaxi/qualysapi
 Keywords: Qualys,Qualys API
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -132,9 +131,7 @@
 Apache License, Version 2.0
 http://www.apache.org/licenses/LICENSE-2.0.html
 
 Acknowledgements
 ================
 
 Special thank you to Colin Bell for qualysconnect.
-
-
```

### Comparing `qualysapi-8.0.2/README.md` & `qualysapi-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-example.py` & `qualysapi-8.1.0/examples/qualysapi-example.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-section-example.py` & `qualysapi-8.1.0/examples/qualysapi-section-example.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-simple-v1.py` & `qualysapi-8.1.0/examples/qualysapi-simple-v1.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-simple-v2-creds.py` & `qualysapi-8.1.0/examples/qualysapi-simple-v2-creds.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-simple-v2-report.py` & `qualysapi-8.1.0/examples/qualysapi-simple-v2-report.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-simple-v2.py` & `qualysapi-8.1.0/examples/qualysapi-simple-v2.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/examples/qualysapi-virtualhost.py` & `qualysapi-8.1.0/examples/qualysapi-virtualhost.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/license` & `qualysapi-8.1.0/license`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/qualysapi/api_actions.py` & `qualysapi-8.1.0/qualysapi/api_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -556,7 +556,31 @@
 
         if max_retries <= 0:
             logging.info("%s %s", code, res.TEXT)
             return None
 
         logging.debug("%s %s %s", res.DATETIME, code, res.TEXT)
         return code, res
+
+    def listAppliances(self):
+        call = "/api/2.0/fo/appliance/"
+        parameters = {
+            "action": "list"
+        }
+
+        scanner_data = objectify.fromstring(self.request(call, parameters).encode("utf-8"))
+        scanner_array = []
+        for scanner in scanner_data.RESPONSE.APPLIANCE_LIST.APPLIANCE:
+            scanner_array.append(
+                Scanner(
+                    scanner.find("ID"),
+                    scanner.find("UUID"),
+                    scanner.find("NAME"),
+                    scanner.find("NETWORK_ID"),
+                    scanner.find("SOFTWARE_VERSION"),
+                    scanner.find("RUNNING_SLICES_COUNT"),
+                    scanner.find("RUNNING_SCAN_COUNT"),
+                    scanner.find("STATUS")
+                )
+            )
+
+        return scanner_array
```

### Comparing `qualysapi-8.0.2/qualysapi/api_methods.py` & `qualysapi-8.1.0/qualysapi/api_methods.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/qualysapi/api_objects.py` & `qualysapi-8.1.0/qualysapi/api_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,7 +186,20 @@
             parameters = {"action": "resume", "scan_ref": self.ref}
             conn.request(call, parameters)
 
             parameters = {"action": "list", "scan_ref": self.ref, "show_status": 1}
             self.status = objectify.fromstring(
                 conn.request(call, parameters).encode("utf-8")
             ).RESPONSE.SCAN_LIST.SCAN.STATUS.STATE
+
+
+class Scanner:
+    def __init__(self, id: int, uuid: str, name: str, network_id: int, software_version:str,
+                 running_slices_count: int, running_scan_count: int, status: str):
+        self.id = id
+        self.uuid = uuid
+        self.name = name
+        self.network_id = network_id
+        self.software_version = software_version
+        self.running_slices_count = running_slices_count
+        self.running_scan_count = running_scan_count
+        self.status = status
```

### Comparing `qualysapi-8.0.2/qualysapi/config.py` & `qualysapi-8.1.0/qualysapi/config.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/qualysapi/connector.py` & `qualysapi-8.1.0/qualysapi/connector.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/qualysapi/util.py` & `qualysapi-8.1.0/qualysapi/util.py`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/qualysapi.egg-info/PKG-INFO` & `qualysapi-8.1.0/qualysapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: qualysapi
-Version: 8.0.2
+Version: 8.1.0
 Summary: Qualys API Helper
 Home-page: https://github.com/paragbaxi/qualysapi
 Author: Parag Baxi
 Author-email: parag.baxi@gmail.com
 License: BSD-new
 Project-URL: Bug Tracker, https://github.com/paragbaxi/qualysapi/issues
 Project-URL: Source Code, https://github.com/paragbaxi/qualysapi
 Keywords: Qualys,Qualys API
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -132,9 +131,7 @@
 Apache License, Version 2.0
 http://www.apache.org/licenses/LICENSE-2.0.html
 
 Acknowledgements
 ================
 
 Special thank you to Colin Bell for qualysconnect.
-
-
```

### Comparing `qualysapi-8.0.2/qualysapi.egg-info/SOURCES.txt` & `qualysapi-8.1.0/qualysapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/setup.cfg` & `qualysapi-8.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qualysapi-8.0.2/setup.py` & `qualysapi-8.1.0/setup.py`

 * *Files identical despite different names*

