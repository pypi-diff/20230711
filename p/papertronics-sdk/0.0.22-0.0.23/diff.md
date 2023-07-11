# Comparing `tmp/papertronics-sdk-0.0.22.tar.gz` & `tmp/papertronics-sdk-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.22.tar", last modified: Tue Jul 11 10:17:44 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.23.tar", last modified: Tue Jul 11 10:20:12 2023, max compression
```

## Comparing `papertronics-sdk-0.0.22.tar` & `papertronics-sdk-0.0.23.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:17:44.706000 papertronics-sdk-0.0.22/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.22/LICENSE
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:17:44.706000 papertronics-sdk-0.0.22/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      496 2023-07-11 08:58:02.000000 papertronics-sdk-0.0.22/README.md
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:17:44.702000 papertronics-sdk-0.0.22/papertronics_sdk/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.22/papertronics_sdk/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:17:44.702000 papertronics-sdk-0.0.22/papertronics_sdk/lab/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5230 2023-07-11 09:12:17.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/admin_client.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1405 2023-07-11 10:17:16.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/base_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:17:44.702000 papertronics-sdk-0.0.22/papertronics_sdk/lab/exceptions/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/exceptions/StatusException.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/exceptions/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:17:44.706000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/config.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/database.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/generic.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/models/station_protocol.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9109 2023-07-11 07:55:49.000000 papertronics-sdk-0.0.22/papertronics_sdk/lab/user_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:17:44.702000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:17:44.000000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-11 10:17:44.000000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:17:44.000000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-11 10:17:44.000000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/requires.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-11 10:17:44.000000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/top_level.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:17:44.000000 papertronics-sdk-0.0.22/papertronics_sdk.egg-info/zip-safe
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.22/pyproject.toml
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-11 10:17:44.706000 papertronics-sdk-0.0.22/setup.cfg
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.23/LICENSE
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      496 2023-07-11 08:58:02.000000 papertronics-sdk-0.0.23/README.md
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/papertronics_sdk/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.23/papertronics_sdk/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/papertronics_sdk/lab/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5230 2023-07-11 09:12:17.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/admin_client.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1433 2023-07-11 10:20:06.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/base_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/papertronics_sdk/lab/exceptions/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/exceptions/StatusException.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/exceptions/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/config.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/database.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/generic.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/models/station_protocol.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9109 2023-07-11 07:55:49.000000 papertronics-sdk-0.0.23/papertronics_sdk/lab/user_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:20:12.000000 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-11 10:20:12.000000 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:20:12.000000 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-11 10:20:12.000000 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/requires.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-11 10:20:12.000000 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:20:12.000000 papertronics-sdk-0.0.23/papertronics_sdk.egg-info/zip-safe
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.23/pyproject.toml
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-11 10:20:12.475975 papertronics-sdk-0.0.23/setup.cfg
```

### Comparing `papertronics-sdk-0.0.22/PKG-INFO` & `papertronics-sdk-0.0.23/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.22
+Version: 0.0.23
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/admin_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 from .exceptions import StatusException
 
 logger = logging.getLogger(__name__)
 
 
 def http_request(func):
     def wrap(self, url, **kwargs):
-        if self.token is None:
-            raise Exception("Client is not Authenticated")
-
         print(self)
         print(url)
 
         url = f"{self.url}{url}"
         if kwargs.get("include_token", True):
+            if self.token is None:
+                raise Exception("Client is not Authenticated")
             kwargs["headers"] = kwargs.get("headers", {})
             kwargs["headers"]["Authorization"] = f"Bearer {self.token}"
         response = func(self, url, **kwargs)
         logger.debug(f"{func.__name__} {url} {response.status_code}")
         if response.status_code != 200:
             raise StatusException.from_response(response)
         return response
@@ -29,15 +28,15 @@
 
 class BaseClient:
 
     def __init__(self, url, token=None):
         self.url = url
         self.token = token
         try:
-            response = self.get(f"")
+            response = self.get(f"", include_token=False)
             if response.status_code != 200:
                 raise Exception(response.status_code)
         except Exception as e:
             raise Exception(f"could not connect to {url}: {e}")
 
     @http_request
     def get(self, url, **kwargs):
```

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.23/papertronics_sdk/lab/user_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.23/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.22
+Version: 0.0.23
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.22/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.23/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.22/setup.cfg` & `papertronics-sdk-0.0.23/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.22
+version = 0.0.23
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

