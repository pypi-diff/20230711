# Comparing `tmp/papertronics-sdk-0.0.26.tar.gz` & `tmp/papertronics-sdk-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.26.tar", last modified: Tue Jul 11 10:37:43 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.27.tar", last modified: Tue Jul 11 10:40:49 2023, max compression
```

## Comparing `papertronics-sdk-0.0.26.tar` & `papertronics-sdk-0.0.27.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.26/LICENSE
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      496 2023-07-11 08:58:02.000000 papertronics-sdk-0.0.26/README.md
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.26/papertronics_sdk/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/lab/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5836 2023-07-11 10:37:30.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/admin_client.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1571 2023-07-11 10:35:19.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/base_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/lab/exceptions/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/exceptions/StatusException.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/exceptions/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/config.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/database.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/generic.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/station_protocol.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9144 2023-07-11 10:37:30.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/user_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/requires.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/top_level.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/zip-safe
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.26/pyproject.toml
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/setup.cfg
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:40:49.967653 papertronics-sdk-0.0.27/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.27/LICENSE
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:40:49.967653 papertronics-sdk-0.0.27/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      496 2023-07-11 08:58:02.000000 papertronics-sdk-0.0.27/README.md
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:40:49.963653 papertronics-sdk-0.0.27/papertronics_sdk/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.27/papertronics_sdk/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:40:49.963653 papertronics-sdk-0.0.27/papertronics_sdk/lab/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5836 2023-07-11 10:37:30.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/admin_client.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1588 2023-07-11 10:40:39.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/base_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:40:49.963653 papertronics-sdk-0.0.27/papertronics_sdk/lab/exceptions/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/exceptions/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/exceptions/status_exception.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:40:49.967653 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/config.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/database.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/generic.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/models/station_protocol.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9144 2023-07-11 10:37:30.000000 papertronics-sdk-0.0.27/papertronics_sdk/lab/user_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:40:49.963653 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:40:49.000000 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      842 2023-07-11 10:40:49.000000 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:40:49.000000 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-11 10:40:49.000000 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/requires.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-11 10:40:49.000000 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:40:49.000000 papertronics-sdk-0.0.27/papertronics_sdk.egg-info/zip-safe
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.27/pyproject.toml
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-11 10:40:49.967653 papertronics-sdk-0.0.27/setup.cfg
```

### Comparing `papertronics-sdk-0.0.26/PKG-INFO` & `papertronics-sdk-0.0.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.26
+Version: 0.0.27
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/admin_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/base_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import httpx
 
-from .exceptions import StatusException
+from .exceptions.status_exception import StatusException
 
 logger = logging.getLogger(__name__)
 
 
 def http_request(func):
     def wrap(self, url, include_token=True, **kwargs):
         print(url)
```

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.27/papertronics_sdk/lab/user_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.27/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.26
+Version: 0.0.27
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.26/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.27/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 papertronics_sdk.egg-info/requires.txt
 papertronics_sdk.egg-info/top_level.txt
 papertronics_sdk.egg-info/zip-safe
 papertronics_sdk/lab/__init__.py
 papertronics_sdk/lab/admin_client.py
 papertronics_sdk/lab/base_client.py
 papertronics_sdk/lab/user_client.py
-papertronics_sdk/lab/exceptions/StatusException.py
 papertronics_sdk/lab/exceptions/__init__.py
+papertronics_sdk/lab/exceptions/status_exception.py
 papertronics_sdk/lab/models/__init__.py
 papertronics_sdk/lab/models/admin_cloud_models.py
 papertronics_sdk/lab/models/cloud_models.py
 papertronics_sdk/lab/models/config.py
 papertronics_sdk/lab/models/database.py
 papertronics_sdk/lab/models/generic.py
 papertronics_sdk/lab/models/station_protocol.py
```

### Comparing `papertronics-sdk-0.0.26/setup.cfg` & `papertronics-sdk-0.0.27/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.26
+version = 0.0.27
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

