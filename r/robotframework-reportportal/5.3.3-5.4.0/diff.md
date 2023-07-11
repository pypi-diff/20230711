# Comparing `tmp/robotframework-reportportal-5.3.3.tar.gz` & `tmp/robotframework-reportportal-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-reportportal-5.3.3.tar", last modified: Tue Jun 13 12:14:13 2023, max compression
+gzip compressed data, was "robotframework-reportportal-5.4.0.tar", last modified: Tue Jul 11 15:45:43 2023, max compression
```

## Comparing `robotframework-reportportal-5.3.3.tar` & `robotframework-reportportal-5.4.0.tar`

### file list

```diff
@@ -1,35 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/robotframework_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/post_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/static.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/time_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/variables.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:45:43.099161 robotframework-reportportal-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-07-11 15:45:43.099161 robotframework-reportportal-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:45:43.099161 robotframework-reportportal-5.4.0/robotframework_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/post_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/result_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/result_visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/time_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/robotframework_reportportal/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:45:43.099161 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-07-11 15:45:43.000000 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-11 15:45:43.000000 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:45:43.000000 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 15:45:43.000000 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 15:45:43.000000 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 15:45:43.000000 robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 15:45:43.099161 robotframework-reportportal-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 15:45:38.000000 robotframework-reportportal-5.4.0/setup.py
```

### Comparing `robotframework-reportportal-5.3.3/CONTRIBUTING.rst` & `robotframework-reportportal-5.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/LICENSE.txt` & `robotframework-reportportal-5.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/PKG-INFO` & `robotframework-reportportal-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal
-Version: 5.3.3
+Version: 5.4.0
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.3.3
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.4.0
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ReportPortal RobotFramework agent
 
 [![PyPI](https://img.shields.io/pypi/v/robotframework-reportportal.svg?maxAge=259200)](https://pypi.python.org/pypi/robotframework-reportportal)
 [![Python versions](https://img.shields.io/pypi/pyversions/robotframework-reportportal.svg)](https://pypi.org/project/robotframework-reportportal)
```

### Comparing `robotframework-reportportal-5.3.3/README.md` & `robotframework-reportportal-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/__init__.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/exception.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/static.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""This module includes exceptions used across the agent modules.
+#  Copyright 2022 EPAM Systems
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#  https://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
 
-Copyright (c) 2021 https://reportportal.io .
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-https://www.apache.org/licenses/LICENSE-2.0
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+from typing import Text, Dict
 
-
-class RobotServiceException(Exception):
-    """General exception used by the agent."""
+LOG_LEVEL_MAPPING: Dict
+MAIN_SUITE_ID: Text
+PABOT_WIHOUT_LAUNCH_ID_MSG: Text
+STATUS_MAPPING: Dict
```

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/listener.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/listener.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,84 +14,100 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import os
 from functools import wraps
 from mimetypes import guess_type
+from typing import Optional, Dict, Union, Any
+from queue import LifoQueue
+from warnings import warn
 
 from reportportal_client.helpers import gen_attributes
 
-from .exception import RobotServiceException
 from .model import Keyword, Launch, Test, LogMessage, Suite
 from .service import RobotService
 from .static import MAIN_SUITE_ID, PABOT_WIHOUT_LAUNCH_ID_MSG
 from .variables import Variables
 
 logger = logging.getLogger(__name__)
 
 
+class _LifoQueue(LifoQueue):
+    def last(self):
+        with self.mutex:
+            if self._qsize():
+                return self.queue[-1]
+
+
 def check_rp_enabled(func):
     """Verify is RP is enabled in config."""
     @wraps(func)
     def wrap(*args, **kwargs):
         if args and isinstance(args[0], listener):
             if not args[0].service:
                 return
         func(*args, **kwargs)
     return wrap
 
 
-class listener(object):
+# noinspection PyPep8Naming
+class listener:
     """Robot Framework listener interface for reporting to Report Portal."""
 
+    _items: _LifoQueue = ...
+    _service: Optional[RobotService] = ...
+    _variables: Optional[Variables] = ...
     ROBOT_LISTENER_API_VERSION = 2
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize listener attributes."""
-        self._items = []
+        self._items = _LifoQueue()
         self._service = None
         self._variables = None
 
-    def _build_msg_struct(self, message):
+    def _build_msg_struct(self, message: Dict) -> LogMessage:
         """Check if the given message comes from our custom logger or not.
 
         :param message: Message passed by the Robot Framework
         """
         if isinstance(message['message'], LogMessage):
             msg = message['message']
         else:
             msg = LogMessage(message['message'])
             msg.level = message['level']
         if not msg.launch_log:
             msg.item_id = getattr(self.current_item, 'rp_item_id', None)
         return msg
 
-    def _finish_current_item(self):
-        """Remove the last item from the self._items list."""
-        return self._items.pop()
+    def _add_current_item(self, item: Union[Keyword, Launch, Suite, Test]) -> None:
+        """Add the last item from the self._items queue."""
+        self._items.put(item)
+
+    def _remove_current_item(self) -> Union[Keyword, Launch, Suite, Test]:
+        """Remove the last item from the self._items queue."""
+        return self._items.get()
 
     @property
-    def current_item(self):
-        """Get the last item from the self._items list."""
-        if self._items:
-            return self._items[-1]
+    def current_item(self) -> Optional[Union[Keyword, Launch, Suite, Test]]:
+        """Get the last item from the self._items queue."""
+        return self._items.last()
 
     @check_rp_enabled
-    def log_message(self, message):
+    def log_message(self, message: Dict) -> None:
         """Send log message to the Report Portal.
 
         :param message: Message passed by the Robot Framework
         """
         msg = self._build_msg_struct(message)
         logger.debug('ReportPortal - Log Message: {0}'.format(message))
         self.service.log(message=msg)
 
     @check_rp_enabled
-    def log_message_with_image(self, msg, image):
+    def log_message_with_image(self, msg: Dict, image: str):
         """Send log message to the Report Portal.
 
         :param msg:   Message passed by the Robot Framework
         :param image: Path to image
         """
         mes = self._build_msg_struct(msg)
         with open(image, 'rb') as fh:
@@ -101,69 +117,59 @@
                 'mime': guess_type(image)[0] or 'application/octet-stream'
             }
         logger.debug('ReportPortal - Log Message with Image: {0} {1}'
                      .format(mes, image))
         self.service.log(message=mes)
 
     @property
-    def parent_id(self):
+    def parent_id(self) -> Optional[str]:
         """Get rp_item_id attribute of the current item."""
         return getattr(self.current_item, 'rp_item_id', None)
 
     @property
-    def service(self):
+    def service(self) -> RobotService:
         """Initialize instance of the RobotService."""
-        if self.variables.enabled and self._service is None:
+        if self.variables.enabled and not self._service:
             self._service = RobotService()
-            self._service.init_service(
-                endpoint=self.variables.endpoint,
-                project=self.variables.project,
-                api_key=self.variables.api_key,
-                log_batch_size=self.variables.log_batch_size,
-                pool_size=self.variables.pool_size,
-                skipped_issue=self.variables.skipped_issue,
-                verify_ssl=self.variables.verify_ssl,
-                log_batch_payload_size=self.variables.log_batch_payload_size,
-                launch_id=self.variables.launch_id,
-            )
+            self._service.init_service(self.variables)
         return self._service
 
     @property
-    def variables(self):
+    def variables(self) -> Variables:
         """Get instance of the variables.Variables class."""
         if not self._variables:
             self._variables = Variables()
         return self._variables
 
     @check_rp_enabled
-    def start_launch(self, attributes, ts=None):
+    def start_launch(self, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new launch at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         launch = Launch(self.variables.launch_name, attributes)
         launch.attributes = gen_attributes(self.variables.launch_attributes)
         launch.doc = self.variables.launch_doc or launch.doc
         if not self.variables.launch_id:
             if self.variables.pabot_used:
-                raise RobotServiceException(PABOT_WIHOUT_LAUNCH_ID_MSG)
+                warn(PABOT_WIHOUT_LAUNCH_ID_MSG, stacklevel=2)
             logger.debug('ReportPortal - Start Launch: {0}'.format(
                 launch.attributes))
             self.service.start_launch(
                 launch=launch,
                 mode=self.variables.mode,
                 ts=ts,
                 rerun=self.variables.rerun,
                 rerun_of=self.variables.rerun_of)
         else:
             self.service.rp.launch_id = self.variables.launch_id
 
     @check_rp_enabled
-    def start_suite(self, name, attributes, ts=None):
+    def start_suite(self, name: str, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new test suite at the Report Portal.
 
         :param name:       Test suite name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if attributes['id'] == MAIN_SUITE_ID:
@@ -171,46 +177,46 @@
             if self.variables.pabot_used:
                 name += '.{0}'.format(self.variables.pabot_pool_id)
             logger.debug(
                 'ReportPortal - Create global Suite: {0}'
                 .format(attributes))
             suite = Suite(name, attributes)
             suite.rp_item_id = self.service.start_suite(suite=suite, ts=ts)
-            self._items.append(suite)
+            self._add_current_item(suite)
         else:
             logger.debug('ReportPortal - Start Suite: {0}'.format(attributes))
             suite = Suite(name, attributes)
             suite.rp_parent_item_id = self.parent_id
             suite.rp_item_id = self.service.start_suite(suite=suite, ts=ts)
-            self._items.append(suite)
+            self._add_current_item(suite)
 
     @check_rp_enabled
-    def end_suite(self, _, attributes, ts=None):
+    def end_suite(self, _: Optional[str], attributes: Dict, ts: Optional[Any] = None) -> None:
         """Finish started test suite at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if attributes['id'] == MAIN_SUITE_ID:
-            suite = self._finish_current_item().update(attributes)
+            suite = self._remove_current_item().update(attributes)
             logger.debug('ReportPortal - End Suite: {0}'
                          .format(suite.attributes))
             self.service.finish_suite(suite=suite, ts=ts)
             launch = Launch(self.variables.launch_name, attributes)
             logger.debug(
                 msg='ReportPortal - End Launch: {0}'.format(attributes))
             self.service.finish_launch(launch=launch, ts=ts)
         else:
-            suite = self._finish_current_item().update(attributes)
+            suite = self._remove_current_item().update(attributes)
             logger.debug(
                 'ReportPortal - End Suite: {0}'.format(suite.attributes))
             self.service.finish_suite(suite=suite, ts=ts)
 
     @check_rp_enabled
-    def start_test(self, name, attributes, ts=None):
+    def start_test(self, name: str, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new test case at the Report Portal.
 
         :param name:       Test case name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if 'source' not in attributes:
@@ -219,84 +225,84 @@
             attributes['source'] = getattr(self.current_item, 'source', None)
         test = Test(name=name, attributes=attributes)
         logger.debug('ReportPortal - Start Test: {0}'.format(attributes))
         test.attributes = gen_attributes(
             self.variables.test_attributes + test.tags)
         test.rp_parent_item_id = self.parent_id
         test.rp_item_id = self.service.start_test(test=test, ts=ts)
-        self._items.append(test)
+        self._add_current_item(test)
 
     @check_rp_enabled
-    def end_test(self, _, attributes, ts=None):
+    def end_test(self, _: Optional[str], attributes: Dict, ts: Optional[Any] = None) -> None:
         """Finish started test case at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         test = self.current_item.update(attributes)
         test.attributes = gen_attributes(
             self.variables.test_attributes + test.tags)
         if not test.critical and test.status == 'FAIL':
             test.status = 'SKIP'
         if test.message:
             self.log_message({'message': test.message, 'level': 'DEBUG'})
         logger.debug('ReportPortal - End Test: {0}'.format(test.attributes))
-        self._finish_current_item()
+        self._remove_current_item()
         self.service.finish_test(test=test, ts=ts)
 
     @check_rp_enabled
-    def start_keyword(self, name, attributes, ts=None):
+    def start_keyword(self, name: str, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new keyword(test step) at the Report Portal.
 
         :param name:       Keyword name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         kwd = Keyword(name=name, parent_type=self.current_item.type,
                       attributes=attributes)
         kwd.rp_parent_item_id = self.parent_id
         logger.debug('ReportPortal - Start Keyword: {0}'.format(attributes))
         kwd.rp_item_id = self.service.start_keyword(keyword=kwd, ts=ts)
-        self._items.append(kwd)
+        self._add_current_item(kwd)
 
     @check_rp_enabled
-    def end_keyword(self, _, attributes, ts=None):
+    def end_keyword(self, _: Optional[str], attributes: Dict, ts: Optional[Any] = None) -> None:
         """Finish started keyword at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
-        kwd = self._finish_current_item().update(attributes)
+        kwd = self._remove_current_item().update(attributes)
         logger.debug('ReportPortal - End Keyword: {0}'.format(kwd.attributes))
         self.service.finish_keyword(keyword=kwd, ts=ts)
 
-    def log_file(self, log_path):
+    def log_file(self, log_path: str) -> None:
         """Attach HTML log file created by Robot Framework to RP launch.
 
         :param log_path: Path to the log file
         """
         if self.variables.attach_log:
             message = {'message': 'Execution log', 'level': 'INFO'}
             self.log_message_with_image(message, log_path)
 
-    def report_file(self, report_path):
+    def report_file(self, report_path: str) -> None:
         """Attach HTML report created by Robot Framework to RP launch.
 
         :param report_path: Path to the report file
         """
         if self.variables.attach_report:
             message = {'message': 'Execution report', 'level': 'INFO'}
             self.log_message_with_image(message, report_path)
 
-    def xunit_file(self, xunit_path):
+    def xunit_file(self, xunit_path: str) -> None:
         """Attach XUnit file created by Robot Framework to RP launch.
 
         :param xunit_path: Path to the XUnit file
         """
         if self.variables.attach_xunit:
             message = {'message': 'XUnit result file', 'level': 'INFO'}
             self.log_message_with_image(message, xunit_path)
 
     @check_rp_enabled
-    def close(self):
+    def close(self) -> None:
         """Call service terminate when the whole test execution is done."""
         self.service.terminate_service()
```

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/logger.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/model.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/model.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/model.pyi` & `robotframework-reportportal-5.4.0/robotframework_reportportal/model.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/post_report.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/post_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/result_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.pyi` & `robotframework-reportportal-5.4.0/robotframework_reportportal/result_visitor.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/service.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module is a Robot service for reporting results to Report Portal."""
+from typing import Optional
 
 #  Copyright (c) 2023 EPAM Systems
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  https://www.apache.org/licenses/LICENSE-2.0
@@ -12,32 +13,32 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 from dateutil.parser import parse
 import logging
 
-from reportportal_client.logs.log_manager import MAX_LOG_BATCH_PAYLOAD_SIZE
 from reportportal_client.helpers import (
     dict_to_payload,
     get_launch_sys_attrs,
     get_package_version,
     timestamp
 )
 from reportportal_client.client import RPClient
 
-from .exception import RobotServiceException
+from .model import Launch, Suite, Test, Keyword, LogMessage
+from .variables import Variables
 from .static import LOG_LEVEL_MAPPING, STATUS_MAPPING
 
 logger = logging.getLogger(__name__)
 
 TOP_LEVEL_ITEMS = {'BEFORE_SUITE', 'AFTER_SUITE'}
 
 
-def to_epoch(date):
+def to_epoch(date: Optional[str]) -> Optional[str]:
     """Convert Robot Framework timestamp to UTC timestamp."""
     if not date:
         return None
     try:
         parsed_date = parse(date)
     except ValueError:
         return None
@@ -48,80 +49,67 @@
             float(parsed_date.strftime('%s')) + parsed_date.microsecond / 1e6
     return str(int(epoch_time * 1000))
 
 
 class RobotService(object):
     """Class represents service that sends Robot items to Report Portal."""
 
-    def __init__(self):
+    agent_name: str
+    agent_version: str
+    rp: Optional[RPClient]
+
+    def __init__(self) -> None:
         """Initialize service attributes."""
         self.agent_name = 'robotframework-reportportal'
         self.agent_version = get_package_version(self.agent_name)
         self.rp = None
 
-    def _get_launch_attributes(self, cmd_attrs):
+    def _get_launch_attributes(self, cmd_attrs: list) -> list:
         """Generate launch attributes including both system and user ones.
 
         :param list cmd_attrs: List for attributes from the command line
         """
         attributes = cmd_attrs or []
         system_attributes = get_launch_sys_attrs()
         system_attributes['agent'] = (
             '{}|{}'.format(self.agent_name, self.agent_version))
         return attributes + dict_to_payload(system_attributes)
 
-    def init_service(self, endpoint, project, api_key, log_batch_size,
-                     pool_size, skipped_issue=True, verify_ssl=True,
-                     log_batch_payload_size=MAX_LOG_BATCH_PAYLOAD_SIZE,
-                     launch_id=None):
+    def init_service(self, variables: Variables) -> None:
         """Initialize common Report Portal client.
 
-        :param endpoint:               Report Portal API endpoint
-        :param project:                Report Portal project
-        :param api_key:                API key
-        :param log_batch_size:         Number of logs to be sent within one
-                                       batch
-        :param pool_size:              HTTPAdapter max pool size
-        :param skipped_issue:          Mark skipped test items with
-                                       'To Investigate', default value 'True'
-        :param verify_ssl:             Disable SSL verification.
-        :param log_batch_payload_size: Maximum size of logs to be sent within
-                                       one batch
-        :param launch_id:              a launch id to use instead of starting
-                                       own one
+        :param variables: Report Portal variables
         """
         if self.rp is None:
-            logger.debug(
-                'ReportPortal - Init service: '
-                'endpoint={0}, project={1}, api_key={2}'
-                .format(endpoint, project, api_key))
+            logger.debug(f'ReportPortal - Init service: endpoint={variables.endpoint}, project={variables.project}, '
+                         f'api_key={variables.api_key}')
             self.rp = RPClient(
-                endpoint=endpoint,
-                project=project,
-                api_key=api_key,
-                is_skipped_an_issue=skipped_issue,
-                log_batch_size=log_batch_size,
+                endpoint=variables.endpoint,
+                project=variables.project,
+                api_key=variables.api_key,
+                is_skipped_an_issue=variables.skipped_issue,
+                log_batch_size=variables.log_batch_size,
                 retries=True,
-                verify_ssl=verify_ssl,
-                max_pool_size=pool_size,
-                log_batch_payload_size=log_batch_payload_size,
-                launch_id=launch_id
+                verify_ssl=variables.verify_ssl,
+                max_pool_size=variables.pool_size,
+                log_batch_payload_size=variables.log_batch_payload_size,
+                launch_id=variables.launch_id,
+                launch_uuid_print=variables.launch_uuid_print,
+                print_output=variables.launch_uuid_print_output
             )
             self.rp.start()
-        else:
-            raise RobotServiceException(
-                'RobotFrameworkService is already initialized.')
 
-    def terminate_service(self):
+    def terminate_service(self) -> None:
         """Terminate common reportportal client."""
-        if self.rp is not None:
+        if self.rp:
             self.rp.terminate()
 
-    def start_launch(self, launch, mode=None, rerun=False, rerun_of=None,
-                     ts=None):
+    def start_launch(self, launch: Launch, mode: Optional[str] = None, rerun: bool = False,
+                     rerun_of: Optional[str] = None,
+                     ts: Optional[str] = None) -> Optional[str]:
         """Call start_launch method of the common client.
 
         :param launch:         Instance of the Launch class
         :param mode:           Launch mode
         :param rerun:          Rerun mode. Allowable values 'True' of 'False'
         :param rerun_of:       Rerun mode. Specifies launch to be re-runned.
                                Should be used with the 'rerun' option.
@@ -137,29 +125,29 @@
             'rerun_of': rerun_of,
             'start_time': ts or to_epoch(launch.start_time) or timestamp()
         }
         logger.debug(
             'ReportPortal - Start launch: request_body={0}'.format(sl_pt))
         return self.rp.start_launch(**sl_pt)
 
-    def finish_launch(self, launch, ts=None):
+    def finish_launch(self, launch: Launch, ts: Optional[str] = None) -> None:
         """Finish started launch.
 
         :param launch: Launch name
         :param ts:     End time
         """
         fl_rq = {
             'end_time': ts or to_epoch(launch.end_time) or timestamp(),
             'status': STATUS_MAPPING[launch.status]
         }
         logger.debug(
             'ReportPortal - Finish launch: request_body={0}'.format(fl_rq))
         self.rp.finish_launch(**fl_rq)
 
-    def start_suite(self, suite, ts=None):
+    def start_suite(self, suite: Suite, ts: Optional[str] = None) -> Optional[str]:
         """Call start_test method of the common client.
 
         :param suite: model.Suite object
         :param ts:    Start time
         :return:      Suite UUID
         """
         start_rq = {
@@ -170,15 +158,16 @@
             'parent_item_id': suite.rp_parent_item_id,
             'start_time': ts or to_epoch(suite.start_time) or timestamp()
         }
         logger.debug(
             'ReportPortal - Start suite: request_body={0}'.format(start_rq))
         return self.rp.start_test_item(**start_rq)
 
-    def finish_suite(self, suite, issue=None, ts=None):
+    def finish_suite(self, suite: Suite, issue: Optional[str] = None,
+                     ts: Optional[str] = None) -> None:
         """Finish started suite.
 
         :param suite: Instance of the started suite item
         :param issue: Corresponding issue if it exists
         :param ts:    End time
         """
         fta_rq = {
@@ -187,15 +176,15 @@
             'item_id': suite.rp_item_id,
             'status': STATUS_MAPPING[suite.status]
         }
         logger.debug(
             'ReportPortal - Finish suite: request_body={0}'.format(fta_rq))
         self.rp.finish_test_item(**fta_rq)
 
-    def start_test(self, test, ts=None):
+    def start_test(self, test: Test, ts: Optional[str] = None):
         """Call start_test method of the common client.
 
         :param test: model.Test object
         :param ts:   Start time
         """
         # Item type should be sent as "STEP" until we upgrade to RPv6.
         # Details at:
@@ -210,15 +199,15 @@
             'start_time': ts or to_epoch(test.start_time) or timestamp(),
             'test_case_id': test.test_case_id
         }
         logger.debug(
             'ReportPortal - Start test: request_body={0}'.format(start_rq))
         return self.rp.start_test_item(**start_rq)
 
-    def finish_test(self, test, issue=None, ts=None):
+    def finish_test(self, test: Test, issue: Optional[str] = None, ts: Optional[str] = None):
         """Finish started test case.
 
         :param test:  Instance of started test item
         :param issue: Corresponding issue if it exists
         :param ts:    End time
         """
         fta_rq = {
@@ -228,15 +217,15 @@
             'item_id': test.rp_item_id,
             'status': STATUS_MAPPING[test.status]
         }
         logger.debug(
             'ReportPortal - Finish test: request_body={0}'.format(fta_rq))
         self.rp.finish_test_item(**fta_rq)
 
-    def start_keyword(self, keyword, ts=None):
+    def start_keyword(self, keyword: Keyword, ts: Optional[str] = None):
         """Call start_test method of the common client.
 
         :param keyword: model.Keyword object
         :param ts:      Start time
         """
         start_rq = {
             'description': keyword.doc,
@@ -246,15 +235,15 @@
             'parent_item_id': keyword.rp_parent_item_id,
             'start_time': ts or to_epoch(keyword.start_time) or timestamp()
         }
         logger.debug(
             'ReportPortal - Start keyword: request_body={0}'.format(start_rq))
         return self.rp.start_test_item(**start_rq)
 
-    def finish_keyword(self, keyword, issue=None, ts=None):
+    def finish_keyword(self, keyword: Keyword, issue: Optional[str] = None, ts: Optional[str] = None):
         """Finish started keyword item.
 
         :param keyword: Instance of started keyword item
         :param issue:   Corresponding issue if it exists
         :param ts:      End time
         """
         fta_rq = {
@@ -263,15 +252,15 @@
             'item_id': keyword.rp_item_id,
             'status': STATUS_MAPPING[keyword.status]
         }
         logger.debug(
             'ReportPortal - Finish keyword: request_body={0}'.format(fta_rq))
         self.rp.finish_test_item(**fta_rq)
 
-    def log(self, message, ts=None):
+    def log(self, message: LogMessage, ts: Optional[str] = None):
         """Send log message to Report Portal.
 
         :param message: model.LogMessage object
         :param ts:      Timestamp
         """
         sl_rq = {
             'attachment': message.attachment,
```

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/static.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/static.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/time_visitor.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/time_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal/variables.py` & `robotframework-reportportal-5.4.0/robotframework_reportportal/variables.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,42 +9,74 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
+import sys
+
 from distutils.util import strtobool
 from os import path
+from typing import Optional, Union, Dict, Any, TextIO
 from warnings import warn
 
 from reportportal_client.logs.log_manager import MAX_LOG_BATCH_PAYLOAD_SIZE
 from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
 
 # This is a storage for the result visitor
-_variables = {}
+_variables: Dict[str, Any] = {}
+
+OUTPUT_TYPES: Dict[str, TextIO] = {
+    'stdout': sys.stdout,
+    'stderr': sys.stderr
+}
 
 
-def get_variable(name, default=None):
+def get_variable(name: str, default: Optional[str] = None) -> Optional[str]:
     """Get Robot Framework variable.
 
     :param name:    Name of the variable
     :param default: Default value
     :return:        The value of the variable, otherwise default value
     """
     try:
         return BuiltIn().get_variable_value("${" + name + "}", default=default)
     except RobotNotRunningError:
         return _variables.get(name, default)
 
 
-class Variables(object):
+class Variables:
     """This class stores Robot Framework variables related to Report Portal."""
 
-    def __init__(self):
+    enabled: bool = ...
+    endpoint: Optional[str] = ...
+    launch_name: Optional[str] = ...
+    _pabot_pool_id: Optional[int] = ...
+    _pabot_used: Optional[str] = ...
+    project: Optional[str] = ...
+    api_key: Optional[str] = ...
+    attach_log: bool = ...
+    attach_report: bool = ...
+    attach_xunit: bool = ...
+    launch_attributes: list = ...
+    launch_id: Optional[str] = ...
+    launch_doc: Optional[str] = ...
+    log_batch_size: Optional[int] = ...
+    mode: Optional[str] = ...
+    pool_size: Optional[int] = ...
+    rerun: bool = ...
+    rerun_of: Optional[str] = ...
+    test_attributes: Optional[list] = ...
+    skipped_issue: bool = ...
+    log_batch_payload_size: int = ...
+    launch_uuid_print: bool
+    launch_uuid_print_output: TextIO
+
+    def __init__(self) -> None:
         """Initialize instance attributes."""
         self.endpoint = get_variable('RP_ENDPOINT')
         self.launch_name = get_variable('RP_LAUNCH')
         self.project = get_variable('RP_PROJECT')
 
         self._pabot_pool_id = None
         self._pabot_used = None
@@ -66,16 +98,19 @@
             'RP_RERUN', default='False')))
         self.rerun_of = get_variable('RP_RERUN_OF', default=None)
         self.skipped_issue = bool(strtobool(get_variable(
             'RP_SKIPPED_ISSUE', default='True')))
         self.test_attributes = get_variable(
             'RP_TEST_ATTRIBUTES', default='').split()
         self.log_batch_payload_size = int(get_variable(
-            "RP_LOG_BATCH_PAYLOAD_SIZE",
+            'RP_LOG_BATCH_PAYLOAD_SIZE',
             default=str(MAX_LOG_BATCH_PAYLOAD_SIZE)))
+        self.launch_uuid_print = bool(strtobool(get_variable('RP_LAUNCH_UUID_PRINT', default='False')))
+        self.launch_uuid_print_output = OUTPUT_TYPES.get(
+            get_variable('RP_LAUNCH_UUID_PRINT_OUTPUT', default='stdout').lower(), OUTPUT_TYPES['stdout'])
 
         self.api_key = get_variable('RP_API_KEY')
         if not self.api_key:
             token = get_variable('RP_UUID')
             if token:
                 warn(
                     message="Argument `token` is deprecated since 2.0.4 and "
@@ -102,33 +137,33 @@
                 'One or required parameter is missing, Report Portal listener '
                 'will be disabled. Please check agent documentation.',
                 RuntimeWarning,
                 2
             )
 
     @property
-    def pabot_pool_id(self):
+    def pabot_pool_id(self) -> int:
         """Get pool id for the current Robot Framework executor.
 
         :return: Pool id for the current Robot Framework executor
         """
         if not self._pabot_pool_id:
             self._pabot_pool_id = get_variable(name='PABOTEXECUTIONPOOLID')
         return self._pabot_pool_id
 
     @property
-    def pabot_used(self):
+    def pabot_used(self) -> Optional[str]:
         """Get status of using pabot in test execution.
 
         :return: Cached value of the Pabotlib URI
         """
         if not self._pabot_used:
             self._pabot_used = get_variable(name='PABOTLIBURI')
         return self._pabot_used
 
     @property
-    def verify_ssl(self):
+    def verify_ssl(self) -> Union[bool, str]:
         """Get value of the verify_ssl parameter for the client."""
         verify_ssl = get_variable('RP_VERIFY_SSL', default='True')
         if path.exists(verify_ssl):
             return verify_ssl
         return bool(strtobool(verify_ssl))
```

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/PKG-INFO` & `robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal
-Version: 5.3.3
+Version: 5.4.0
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.3.3
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.4.0
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ReportPortal RobotFramework agent
 
 [![PyPI](https://img.shields.io/pypi/v/robotframework-reportportal.svg?maxAge=259200)](https://pypi.python.org/pypi/robotframework-reportportal)
 [![Python versions](https://img.shields.io/pypi/pyversions/robotframework-reportportal.svg)](https://pypi.org/project/robotframework-reportportal)
```

### Comparing `robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/SOURCES.txt` & `robotframework-reportportal-5.4.0/robotframework_reportportal.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,25 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 robotframework_reportportal/__init__.py
-robotframework_reportportal/exception.py
 robotframework_reportportal/listener.py
-robotframework_reportportal/listener.pyi
 robotframework_reportportal/logger.py
 robotframework_reportportal/model.py
 robotframework_reportportal/model.pyi
 robotframework_reportportal/post_report.py
 robotframework_reportportal/result_visitor.py
 robotframework_reportportal/result_visitor.pyi
 robotframework_reportportal/service.py
-robotframework_reportportal/service.pyi
 robotframework_reportportal/static.py
 robotframework_reportportal/static.pyi
 robotframework_reportportal/time_visitor.py
 robotframework_reportportal/variables.py
-robotframework_reportportal/variables.pyi
 robotframework_reportportal.egg-info/PKG-INFO
 robotframework_reportportal.egg-info/SOURCES.txt
 robotframework_reportportal.egg-info/dependency_links.txt
 robotframework_reportportal.egg-info/entry_points.txt
 robotframework_reportportal.egg-info/requires.txt
 robotframework_reportportal.egg-info/top_level.txt
```

### Comparing `robotframework-reportportal-5.3.3/setup.py` & `robotframework-reportportal-5.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup instructions for the package."""
 
 import os
 from setuptools import setup
 
 
-__version__ = '5.3.3'
+__version__ = '5.4.0'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
@@ -32,20 +32,19 @@
     download_url=(
         'https://github.com/reportportal/agent-Python-RobotFramework/'
         'tarball/{version}'.format(version=__version__)),
     keywords=['testing', 'reporting', 'robot framework', 'reportportal',
               'agent'],
     classifiers=[
         'Framework :: Robot Framework',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         ],
     install_requires=read_file('requirements.txt').splitlines(),
     entry_points={
         'console_scripts': [
             'post_report=robotframework_reportportal.post_report:main'
         ]
     },
```

