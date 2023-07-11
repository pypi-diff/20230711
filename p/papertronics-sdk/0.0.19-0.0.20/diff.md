# Comparing `tmp/papertronics-sdk-0.0.19.tar.gz` & `tmp/papertronics-sdk-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.19.tar", last modified: Tue Jul 11 08:59:12 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.20.tar", last modified: Tue Jul 11 09:13:33 2023, max compression
```

## Comparing `papertronics-sdk-0.0.19.tar` & `papertronics-sdk-0.0.20.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.247716 papertronics-sdk-0.0.19/papertronics_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/papertronics_sdk/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/base_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/papertronics_sdk/lab/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/exceptions/StatusException.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/cloud_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/station_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/user_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.247716 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:33.741623 papertronics-sdk-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 09:13:33.741623 papertronics-sdk-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:33.737623 papertronics-sdk-0.0.20/papertronics_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:33.741623 papertronics-sdk-0.0.20/papertronics_sdk/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/base_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:33.741623 papertronics-sdk-0.0.20/papertronics_sdk/lab/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/exceptions/StatusException.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:33.741623 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/cloud_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/models/station_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/papertronics_sdk/lab/user_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:13:33.737623 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 09:13:33.000000 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 09:13:33.000000 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:13:33.000000 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 09:13:33.000000 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 09:13:33.000000 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:13:33.000000 papertronics-sdk-0.0.20/papertronics_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 09:13:18.000000 papertronics-sdk-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 09:13:33.741623 papertronics-sdk-0.0.20/setup.cfg
```

### Comparing `papertronics-sdk-0.0.19/PKG-INFO` & `papertronics-sdk-0.0.20/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.19
+Version: 0.0.20
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/admin_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from typing import Optional, Union, List
 
 from .models.database import DeviceModel, DeviceLinkModel, DeviceStatisticModel, ProtocolModel, ProtocolLinkModel, \
     UserModel
 from .models.admin_cloud_models import DeviceRequest, UserRequest
-from base_client import BaseClient
+from .base_client import BaseClient
 
 
 class AdminLabClient(BaseClient):
 
     def __init__(self, url, token):
         super().__init__(url, token)
```

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/base_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import logging
-import time
-import uuid
-from typing import Optional, List, Union
 
 import httpx
 
-from .models.database import DeviceModel, UserModel, ProtocolModel, ExperimentModel, ExperimentStatus
-from .models.cloud_models import SaveProtocolRequest, ProtocolTestResponse, ExperimentStartRequest, \
-    ExperimentEditRequest
 from .exceptions import StatusException
 
 logger = logging.getLogger(__name__)
 
 
 class BaseClient:
```

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.20/papertronics_sdk/lab/user_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.20/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.19
+Version: 0.0.20
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.19/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.20/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.19/setup.cfg` & `papertronics-sdk-0.0.20/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.19
+version = 0.0.20
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

