# Comparing `tmp/ms_python_client-1.0.2.tar.gz` & `tmp/ms_python_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-1.0.2.tar", max compression
+gzip compressed data, was "ms_python_client-1.0.3.tar", max compression
```

## Comparing `ms_python_client-1.0.2.tar` & `ms_python_client-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1100 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/LICENSE
--rw-r--r--   0        0        0     5657 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5551 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/api_client.py
--rw-r--r--   0        0        0     1380 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/cern_ms_api_client.py
--rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     3856 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/cern_events_component.py
--rw-r--r--   0        0        0     3100 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/events_component.py
--rw-r--r--   0        0        0      874 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/users_component.py
--rw-r--r--   0        0        0     5696 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1312 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0      383 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/error.py
--rw-r--r--   0        0        0     5047 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/event_generator.py
--rw-r--r--   0        0        0       97 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1003 2023-07-10 15:21:45.848628 ms_python_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6409 1970-01-01 00:00:00.000000 ms_python_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5593 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/api_client.py
+-rw-r--r--   0        0        0     1380 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/cern_ms_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     4145 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/events/cern_events_component.py
+-rw-r--r--   0        0        0     3100 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/users/__init__.py
+-rw-r--r--   0        0        0      874 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/users/users_component.py
+-rw-r--r--   0        0        0     5695 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1312 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/error.py
+-rw-r--r--   0        0        0     4967 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/event_generator.py
+-rw-r--r--   0        0        0       97 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1000 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 ms_python_client-1.0.3/PKG-INFO
```

### Comparing `ms_python_client-1.0.2/LICENSE` & `ms_python_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/README.md` & `ms_python_client-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Microsoft Python client
 
-[![Python tests](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/python-tests.yml)
-[![pre-commit](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/pre-commit.yaml)
-[![CodeQL](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/codeql-analysis.yml)
-[![codecov](https://codecov.io/gh/SamuelGuillemet/MS-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/SamuelGuillemet/MS-python-client)
+[![Python tests](https://github.com/cern-vc/ms-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/ms-python-client/actions/workflows/python-tests.yml)
+[![pre-commit](https://github.com/cern-vc/ms-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/ms-python-client/actions/workflows/pre-commit.yaml)
+[![CodeQL](https://github.com/cern-vc/ms-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/ms-python-client/actions/workflows/codeql-analysis.yml)
+[![codecov](https://codecov.io/gh/cern-vc/MS-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/MS-python-client)
 
 Microsoft graph API Python client with support for [Server to Server Oauth tokens](https://learn.microsoft.com/en-us/graph/auth/auth-concepts?view=graph-rest-1.0) with App Only access.
 
 ## Install
 
 This package is [available on Pypi](https://pypi.org/project/ms-python-client/)
```

### Comparing `ms_python_client-1.0.2/ms_python_client/api_client.py` & `ms_python_client-1.0.3/ms_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/ms_python_client/cern_ms_api_client.py` & `ms_python_client-1.0.3/ms_python_client/cern_ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/ms_python_client/components/events/cern_events_component.py` & `ms_python_client-1.0.3/ms_python_client/components/events/cern_events_component.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from typing import Mapping, Optional
 
 from ms_python_client.components.events.events_component import EventsComponent
 from ms_python_client.ms_client_interface import MSClientInterface
 from ms_python_client.utils.event_generator import (
+    ZOOM_ID_EXTENDED_PROPERTY_ID,
     EventParameters,
     PartialEventParameters,
     create_event_body,
     create_partial_event_body,
 )
 
 logger = logging.getLogger("ms_python_client")
@@ -54,15 +55,21 @@
 
         Args:
             zoom_id (str): The event id
 
         Returns:
             dict: The response of the request
         """
-        parameters = {"$count": "true", "$filter": f"contains(subject,'{zoom_id}')"}
+        parameters = {
+            "$count": "true",
+            "$filter": f"singleValueExtendedProperties/Any(ep: ep/id eq \
+                '{ZOOM_ID_EXTENDED_PROPERTY_ID}' and ep/value eq '{zoom_id}')",
+            "$expand": f"singleValueExtendedProperties($filter=id eq \
+                '{ZOOM_ID_EXTENDED_PROPERTY_ID}')",
+        }
         response = self.events_component.list_events(user_id, parameters, extra_headers)
 
         count = response.get("@odata.count", 0)
         if count == 0:
             raise NotFoundError(f"Event with zoom id {zoom_id} not found")
 
         if count > 1:
```

### Comparing `ms_python_client-1.0.2/ms_python_client/components/events/events_component.py` & `ms_python_client-1.0.3/ms_python_client/components/events/events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/ms_python_client/components/events/users_component.py` & `ms_python_client-1.0.3/ms_python_client/components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/ms_python_client/ms_api_client.py` & `ms_python_client-1.0.3/ms_python_client/ms_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Mapping, Optional
 
 import requests
 from msal import ConfidentialClientApplication, SerializableTokenCache
 
 from ms_python_client.api_client import ApiClient
 from ms_python_client.components.events.events_component import EventsComponent
-from ms_python_client.components.events.users_component import UsersComponent
+from ms_python_client.components.users.users_component import UsersComponent
 from ms_python_client.ms_client_interface import MSClientInterface
 from ms_python_client.utils import init_from_env
 
 logging.getLogger("ms_python_client").addHandler(logging.NullHandler())
 logger = logging.getLogger("ms_python_client")
 
 _Data = Mapping[str, Any]
```

### Comparing `ms_python_client-1.0.2/ms_python_client/ms_client_interface.py` & `ms_python_client-1.0.3/ms_python_client/ms_client_interface.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/ms_python_client/utils/event_generator.py` & `ms_python_client-1.0.3/ms_python_client/utils/event_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 
     zoom_url: str
     subject: str
     start_time: str
     end_time: str
 
 
+ZOOM_ID_EXTENDED_PROPERTY_ID = (
+    "String {d3123b00-8eb5-4f10-ae88-1269fe4cbaf0} Name ZoomId"
+)
+
+
 def create_event_body(event_parameters: EventParameters) -> dict:
     """Creates an event from the given parameters
 
     Args:
         event_parameters (EventParameters): The parameters of the event
 
     Returns:
@@ -69,19 +74,15 @@
     zoom_id_from_url = event_parameters["zoom_url"].split("/")[-1].split("?")[0]
     if zoom_id_from_url != event_parameters["zoom_id"]:
         raise ValueError(
             "The zoom_id from the url does not match the zoom_id from the event parameters"
         )
 
     return {
-        "subject": f"[{event_parameters['zoom_id']}] {event_parameters['subject']}",
-        "body": {
-            "contentType": "text",
-            "content": f"Zoom URL: {event_parameters['zoom_url']}",
-        },
+        "subject": event_parameters["subject"],
         "start": {
             "dateTime": datetime.datetime.fromisoformat(
                 event_parameters["start_time"]
             ).isoformat(),
             "timeZone": timezone,
         },
         "end": {
@@ -97,14 +98,20 @@
             "uniqueId": event_parameters["zoom_url"],
         },
         "attendees": [],
         "allowNewTimeProposals": False,
         "isOnlineMeeting": True,
         "onlineMeetingProvider": "unknown",
         "onlineMeetingUrl": event_parameters["zoom_url"],
+        "singleValueExtendedProperties": [
+            {
+                "id": ZOOM_ID_EXTENDED_PROPERTY_ID,
+                "value": event_parameters["zoom_id"],
+            }
+        ],
     }
 
 
 def create_partial_event_body(event_parameters: PartialEventParameters) -> dict:
     """Updates an event from the given parameters
 
     Args:
@@ -121,32 +128,28 @@
         zoom_id_from_url = event_parameters["zoom_url"].split("/")[-1].split("?")[0]
         if zoom_id_from_url != event_parameters["zoom_id"]:
             raise ValueError(
                 "The zoom_id from the url does not match the zoom_id from the event parameters"
             )
         event.update(
             {
-                "body": {
-                    "contentType": "text",
-                    "content": f"Zoom URL: {event_parameters['zoom_url']}",
-                },
                 "location": {
                     "displayName": event_parameters["zoom_url"],
                     "locationType": "default",
                     "uniqueIdType": "private",
                     "uniqueId": event_parameters["zoom_url"],
                 },
                 "onlineMeetingUrl": event_parameters["zoom_url"],
             }
         )
 
     if "subject" in event_parameters:
         event.update(
             {
-                "subject": f"[{event_parameters['zoom_id']}] {event_parameters['subject']}"
+                "subject": event_parameters["subject"],
             }
         )
 
     if "start_time" in event_parameters:
         event.update(
             {
                 "start": {
```

### Comparing `ms_python_client-1.0.2/ms_python_client/utils/init_from_env.py` & `ms_python_client-1.0.3/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/ms_python_client/utils/logger.py` & `ms_python_client-1.0.3/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.2/pyproject.toml` & `ms_python_client-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "1.0.2"
+version = "1.0.3"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 msal = "^1.22.0"
 requests = "^2.31.0"
 
-[tool.poetry.dev-dependencies]
-black = "23.3.0"
+[tool.poetry.group.dev.dependencies]
+black = "23.7.0"
 flake8 = "6.0.0"
 isort = "5.12.0"
-pre-commit = "2.15.0"
+pre-commit = "3.3.3"
 mypy = "1.4.1"
 mypy-extensions = "1.0.0"
 pylint = "2.17.4"
 pytest = "7.4.0"
 pytest-cov = "4.1.0"
 responses = "0.23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/SamuelGuillemet/ms-python-client/issues"
+"Bug Tracker" = "https://github.com/cern-vc/ms-python-client/issues"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 no_strict_optional = true
 ignore_missing_imports = true
```

### Comparing `ms_python_client-1.0.2/PKG-INFO` & `ms_python_client-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msal (>=1.22.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Bug Tracker, https://github.com/SamuelGuillemet/ms-python-client/issues
+Project-URL: Bug Tracker, https://github.com/cern-vc/ms-python-client/issues
 Description-Content-Type: text/markdown
 
 # Microsoft Python client
 
-[![Python tests](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/python-tests.yml)
-[![pre-commit](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/pre-commit.yaml)
-[![CodeQL](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/codeql-analysis.yml)
-[![codecov](https://codecov.io/gh/SamuelGuillemet/MS-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/SamuelGuillemet/MS-python-client)
+[![Python tests](https://github.com/cern-vc/ms-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/ms-python-client/actions/workflows/python-tests.yml)
+[![pre-commit](https://github.com/cern-vc/ms-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/ms-python-client/actions/workflows/pre-commit.yaml)
+[![CodeQL](https://github.com/cern-vc/ms-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/ms-python-client/actions/workflows/codeql-analysis.yml)
+[![codecov](https://codecov.io/gh/cern-vc/MS-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/MS-python-client)
 
 Microsoft graph API Python client with support for [Server to Server Oauth tokens](https://learn.microsoft.com/en-us/graph/auth/auth-concepts?view=graph-rest-1.0) with App Only access.
 
 ## Install
 
 This package is [available on Pypi](https://pypi.org/project/ms-python-client/)
```

