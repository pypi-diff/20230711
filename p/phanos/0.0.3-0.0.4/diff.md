# Comparing `tmp/phanos-0.0.3.tar.gz` & `tmp/phanos-0.0.4.tar.gz`

## Comparing `phanos-0.0.3.tar` & `phanos-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.3/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.3/Pipfile.lock
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 phanos-0.0.3/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/__init__.py
--rw-r--r--   0        0        0    14820 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/metrics.py
--rw-r--r--   0        0        0    15292 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/publisher.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/tree.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.3/test/__init__.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.3/test/dummy_api.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 phanos-0.0.3/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.3/test/run_tests.py
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 phanos-0.0.3/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.3/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.3/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.3/LICENSE
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 phanos-0.0.3/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 phanos-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 phanos-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.4/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.4/Pipfile.lock
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/log.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/metrics.py
+-rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/publisher.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/tree.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.4/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.4/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.4/test/run_tests.py
+-rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.4/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.4/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.4/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 phanos-0.0.4/PKG-INFO
```

### Comparing `phanos-0.0.3/Pipfile.lock` & `phanos-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/deactivate/bin/Activate.ps1` & `phanos-0.0.4/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/deactivate/bin/activate` & `phanos-0.0.4/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/deactivate/bin/activate.csh` & `phanos-0.0.4/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/deactivate/bin/activate.fish` & `phanos-0.0.4/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/src/phanos/metrics.py` & `phanos-0.0.4/src/phanos/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 import logging
 import sys
 import typing
 from datetime import datetime as dt
 
 from flask import current_app as app
 from imp_prof import Record
+from . import log
 
 
-class MetricWrapper:
+class MetricWrapper(log.InstanceLoggerMixin):
     """Wrapper around all Prometheus metric types"""
 
     name: str
     item: typing.List[str]
     method: typing.List[str]
     job: str
     metric: str
     _values: typing.List[tuple[str, typing.Union[float, str, dict[str, typing.Any]]]]
     label_names: typing.List[str]
     _label_values: typing.List[typing.Dict[str, str]]
     operations: typing.Dict[str, typing.Callable]
     default_operation: str
 
-    _logger: logging.Logger
-
     def __init__(
         self,
         name: str,
         units: str,
         labels: typing.Optional[typing.List[str]] = None,
         logger: typing.Optional[logging.Logger] = None,
     ) -> None:
@@ -46,15 +45,15 @@
         self._values = []
         self.method = []
         self.job = ""
         self.label_names = list(set(labels)) if labels else []
         self._label_values = []
         self.operations = {}
         self.default_operation = ""
-        self._logger = logger or logging.getLogger(__name__)
+        super().__init__(logged_name="phanos", logger=logger or logging.getLogger(__name__))
 
     def to_records(self) -> typing.List[Record]:
         """Convert measured values into Type Record
 
         :returns: List of records"""
         records = []
         for i in range(len(self._values)):
@@ -126,32 +125,30 @@
             if labels_ok and label_values is not None:
                 self._label_values.append(label_values)
             else:
                 raise ValueError("Unknown or missing label")
             if operation is None:
                 operation = self.default_operation
             self.method.append(method)
-            self._logger.debug(
-                f"Phanos - metric {self.name} stored operation {operation}, value {value}",
-            )
+            self.debug("metric %s stored operation %s, value %s", self.name, operation, value)
             self.operations[operation](value, args, kwargs)
         except KeyError as exc:
             raise ValueError("Unknown operation") from exc
 
     def cleanup(self) -> None:
         """Cleanup after metrics was sent"""
         if self._values is not None:
             self._values.clear()
         if self._label_values is not None:
             self._label_values.clear()
         if self.method is not None:
             self.method.clear()
         if self.item is not None:
             self.item.clear()
-        self._logger.debug(f"Phanos - metric {self.name} cleared")
+        self.debug("metric %s cleared", self.name)
 
 
 class Histogram(MetricWrapper):
     """class representing histogram metric of Prometheus"""
 
     metric: str
```

### Comparing `phanos-0.0.3/src/phanos/publisher.py` & `phanos-0.0.4/src/phanos/publisher.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from logging import Logger
 
 import imp_prof.messaging.publisher
 
 from imp_prof.messaging.publisher import BlockingPublisher
 
 from .metrics import MetricWrapper, TimeProfiler, ResponseSize
-from .tree import MethodTree
-
+from .tree import MethodTreeNode
+from . import log
 
 TIME_PROFILER = "time_profiler"
 RESPONSE_SIZE = "response_size"
 
 
 class OutputFormatter:
     """class for converting Record type into profiling string"""
@@ -43,15 +43,15 @@
             f"method: {record.get('method')}, "
             f"value: {value} {record.get('units')}, "
             f"labels: {labels}"
         )
 
 
 class BaseHandler:
-    """base class for record handling"""
+    """ " base class for record handling"""
 
     handler_name: str
 
     def __init__(self, handler_name: str) -> None:
         """
         :param handler_name: name of handler. used for managing handlers"""
         self.handler_name = handler_name
@@ -65,15 +65,15 @@
 
         :param profiler_name: name of profiler
         :param records: list of records to handle
         """
         raise NotImplementedError
 
 
-class RabbitMQHandler(BaseHandler):
+class ImpProfHandler(BaseHandler):
     """RabbitMQ record handler"""
 
     _publisher: BlockingPublisher
     _logger: logging.Logger
 
     def __init__(
         self,
@@ -91,24 +91,32 @@
         logger: typing.Optional[Logger] = None,
         **kwargs,
     ) -> None:
         """Creates BlockingPublisher instance (connection not established yet),
          sets logger and create time profiler and response size profiler
 
         :param handler_name: name of handler. used for managing handlers
-        :param host: RabbitMQ server host
-        :param port: RabbitMQ server port
-        :param user: RabbitMQ username
-        :param password: RabbitMQ user password
-        :param heartbeat:
-        :param timeout:
-        :param retry_delay:
-        :param retry:
-        :param exchange_name:
-        :param exchange_type:
+        :param host: rabbitMQ server host
+        :param port: rabbitMQ server port
+        :param user: rabbitMQ login username
+        :param password: rabbitMQ user password
+        :param exchange_name: exchange name to bind queue with
+        :param exchange_type: exchange type to bind queue with
+        :param logger: loging object to use
+        :param retry: how many times to retry publish event
+        :param int|float retry_delay: Time to wait in seconds, before the next
+        :param timeout: If not None,
+            the value is a non-negative timeout, in seconds, for the
+            connection to remain blocked (triggered by Connection.Blocked from
+            broker); if the timeout expires before connection becomes unblocked,
+            the connection will be torn down, triggering the adapter-specific
+            mechanism for informing client app about the closed connection (
+            e.g., on_close_callback or ConnectionClosed exception) with
+            `reason_code` of `InternalCloseReasons.BLOCKED_CONNECTION_TIMEOUT`.
+        :param kwargs: other connection params, like `timeout goes here`
         :param logger: logger
         """
         super().__init__(handler_name)
 
         self._logger = logger or logging.getLogger(__name__)
         self._publisher = BlockingPublisher(
             host=host,
@@ -124,18 +132,19 @@
             logger=logger,
             **kwargs,
         )
         try:
             self._publisher.connect()
         except imp_prof.messaging.publisher.NETWORK_ERRORS as err:
             self._logger.error(
-                f"RabbitMQHandler cannot connect to RabbitMQ because of {err}"
+                f"ImpProfHandler cannot connect to RabbitMQ because of {err}"
             )
             raise RuntimeError("Cannot connect to RabbitMQ") from err
-        self._logger.info("RabbitMQHandler created successfully")
+
+        self._logger.info("ImpProfHandler created successfully")
         self._publisher.close()
 
     def handle(
         self,
         records: typing.List[imp_prof.Record],
         profiler_name: str = "profiler",
     ) -> None:
@@ -226,22 +235,21 @@
                 print(
                     self._formatter.record_to_str(profiler_name, record),
                     file=self.output,
                     flush=True,
                 )
 
 
-class PhanosProfiler:
+class PhanosProfiler(log.InstanceLoggerMixin):
     """Class responsible for sending records to IMP_prof RabbitMQ publish queue"""
 
-    _logger: Logger
     _metrics: typing.Dict[str, MetricWrapper]
 
-    _root: MethodTree
-    current_node: MethodTree
+    _root: MethodTreeNode
+    current_node: MethodTreeNode
 
     time_profile: typing.Optional[TimeProfiler]
     resp_size_profile: typing.Optional[ResponseSize]
 
     before_func: typing.Optional[typing.Callable]
     after_func: typing.Optional[typing.Callable]
     before_root_func: typing.Optional[typing.Callable]
@@ -263,60 +271,61 @@
         self.request_size_profile = None
         self.time_profile = None
 
         self.before_func = None
         self.after_func = None
         self.before_root_func = None
         self.after_root_func = None
+        super().__init__(logged_name="phanos")
 
     def config(
         self,
         logger=None,
         time_profile: bool = True,
         request_size_profile: bool = True,
         handle_records: bool = True,
     ) -> None:
         """configure PhanosProfiler
         :param logger: logger instance
         :param time_profile: should create instance time profiler
         :param request_size_profile: should create instance of request size profiler
         :param handle_records: should handle recorded records
         """
-        self._logger = logger or logging.getLogger(__name__)
+        self.logger = logger or logging.getLogger(__name__)
         if time_profile:
             self.create_time_profiler()
         if request_size_profile:
             self.create_response_size_profiler()
         self.handle_records = handle_records
 
-        self._root = MethodTree(None, self._logger)
+        self._root = MethodTreeNode(None, self.logger)
         self.current_node = self._root
 
     def create_time_profiler(self) -> None:
         """Create time profiling metric"""
-        self.time_profile = TimeProfiler(TIME_PROFILER, logger=self._logger)
+        self.time_profile = TimeProfiler(TIME_PROFILER, logger=self.logger)
         self.add_metric(self.time_profile)
-        self._logger.debug("Phanos - time profiler created")
+        self.debug("Phanos - time profiler created")
 
     def create_response_size_profiler(self) -> None:
         """create response size profiling metric"""
-        self.resp_size_profile = ResponseSize(RESPONSE_SIZE, logger=self._logger)
+        self.resp_size_profile = ResponseSize(RESPONSE_SIZE, logger=self.logger)
         self.add_metric(self.resp_size_profile)
-        self._logger.debug("Phanos - response size profiler created")
+        self.debug("response size profiler created")
 
     def delete_metric(self, item: str) -> None:
         """deletes one metric instance
         :param item: name of the metric instance
         """
         _ = self._metrics.pop(item, None)
         if item == "time_profiler":
             self.time_profile = None
         if item == "response_size":
             self.resp_size_profile = None
-        self._logger.debug(f"Phanos - metric {item} deleted")
+        self.debug(f"metric {item} deleted")
 
     def delete_metrics(
         self, rm_time_profile: bool = False, rm_resp_size_profile: bool = False
     ) -> None:
         """deletes all custom metric instances
 
         :param rm_time_profile: should pre created time_profiler be deleted
@@ -339,67 +348,67 @@
 
     def add_metric(self, metric: MetricWrapper) -> None:
         """adds new metric to profiling
 
         :param metric: metric instance
         """
         self._metrics[metric.name] = metric
-        self._logger.debug(f"Phanos - metric {metric.name} added")
+        self.debug(f"metric {metric.name} added")
 
     def add_handler(self, handler: BaseHandler) -> None:
         """Add handler to profiler
 
         :param handler: handler instance
         """
         self._handlers[handler.handler_name] = handler
-        self._logger.debug(f"Handler {handler.handler_name} added to phanos profiler")
+        self.debug("handler {handler.handler_name} added to phanos profiler")
 
     def delete_handler(self, handler_name: str) -> None:
         """Delete handler from profiler
 
         :param handler_name: name of handler:
         """
         _ = self._handlers.pop(handler_name, None)
-        self._logger.debug(f"Phanos - handler {handler_name} deleted")
+        self.debug("handler {handler_name} deleted")
 
     def delete_handlers(self) -> None:
         """delete all handlers"""
         self._handlers.clear()
-        self._logger.debug(f"Phanos - All handlers deleted")
+        self.debug(f"all handlers deleted")
 
     def profile(self, func: typing.Callable) -> typing.Callable:
         """
         Decorator specifying which methods should be profiled.
         Default profiler is time profiler which measures execution time of decorated methods
 
         Usage: decorate methods which you want to be profiled
 
         :param func: method or function which should be profiled
         """
 
         def inner(*args, **kwargs) -> typing.Any:
             if self._handlers and self.handle_records:
                 self.current_node = self.current_node.add_child(
-                    MethodTree(func, self._logger)
+                    MethodTreeNode(func, self.logger)
                 )
 
                 if self.current_node.parent == self._root:
-                    self._logger.debug(f"Phanos - before root execution")
+                    self.debug("before root execution")
                     self._before_root_func(*args, **kwargs)
-                self._logger.debug(f"Phanos - before func execution")
+                self.debug("before func execution")
                 self._before_func(*args, **kwargs)
 
             result = func(*args, **kwargs)
 
             if self._handlers and self.handle_records:
-                self._logger.debug(f"Phanos - after func execution")
+                self.debug("after func execution")
                 self._after_func(*args, **kwargs)
 
                 if self.current_node.parent == self._root:
-                    self._logger.debug(f"Phanos - after root execution")
+                    self.debug("after root execution")
                     self._after_root_func(*args, **kwargs)
                     self.handle_records_clear()
 
                 self.current_node = self.current_node.parent
                 self.current_node.delete_child()
             return result
 
@@ -443,23 +452,23 @@
 
     def _after_func(self, fn_result: typing.Any, *args, **kwargs) -> None:
         # mine
         if self.time_profile:
             self.time_profile.store_operation(
                 operation="stop", method=self.current_node.context, label_values={}
             )
-            self._logger.debug(f"Phanos - {self.time_profile.name} recorded operation ")
+            self.debug(f"{self.time_profile.name} recorded operation ")
         # custom
         if callable(self.after_func):
             self.after_func(fn_result=fn_result, *args, **kwargs)
 
     def handle_records_clear(self) -> None:
         """Pass records to each registered Handler and clear stored records"""
         # send records and log em
         for metric in self._metrics.values():
             records = metric.to_records()
             for handler in self._handlers.values():
-                self._logger.debug(
-                    f"Phanos - handler {handler.handler_name} handling metric {metric.name}"
+                self.debug(
+                    f"handler %s handling metric %s", handler.handler_name, metric.name
                 )
                 handler.handle(records, metric.name)
             metric.cleanup()
```

### Comparing `phanos-0.0.3/src/phanos/tree.py` & `phanos-0.0.4/src/phanos/tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 from __future__ import annotations
 
 import inspect
 import logging
 import typing
+from . import log
 
 
-class MethodTree:
+class MethodTreeNode(log.InstanceLoggerMixin):
     """
     Tree for storing method calls context
     """
 
-    parent: typing.Optional[MethodTree]
-    children: typing.List[MethodTree]
+    parent: typing.Optional[MethodTreeNode]
+    children: typing.List[MethodTreeNode]
     method: typing.Optional[typing.Callable]
     context: str
 
-    _logger: logging.Logger
-
     def __init__(
         self,
         method: typing.Optional[typing.Callable] = None,
         logger: typing.Optional[logging.Logger] = None,
     ) -> None:
         """Set method and nodes context
 
         :param method: method, which was decorated with @profile if None then root node
         """
+        super().__init__(logged_name="phanos", logger=logger)
         self.children = []
         self.parent = None
         self.method = None
 
         self.context = ""
         if method is not None:
             self.method = method
             self.context = method.__name__
 
-        self._logger = logger or logging.getLogger(__name__)
-
-    def add_child(self, child: MethodTree) -> MethodTree:
+    def add_child(self, child: MethodTreeNode) -> MethodTreeNode:
         """Add child to method tree node
 
         Adds child to tree node. Sets Context string of child node
 
         :param child: child to be inserted
         """
         child.parent = self
         if self.method is None:  # equivalent of 'self.context != ""' -> i am root
             child.context = (
                 self.get_method_class(child.method) + ":" + child.context
             )  # child.method cannot be None
         else:
             child.context = self.context + "." + child.context
         self.children.append(child)
-        self._logger.debug(f"Phanos - node {self.context} added child: {child.context}")
+        self.debug(f"node {self.context} added child: {child.context}")
         return child
 
     def delete_child(self) -> None:
         """Delete first child of node"""
         child = self.children.pop(0)
         child.parent = None
-        self._logger.debug(
-            f"Phanos - node {self.context} deleted child: {child.context}"
-        )
+        self.debug(f"node {self.context} deleted child: {child.context}")
 
     def clear_tree(self) -> None:
         """Clears tree of all nodes from self"""
         for child in self.children:
             child.clear_tree()
         self._clear_children()
 
     def _clear_children(self):
         self.parent = None
         children = []
         for child in self.children:
             children.append(child.context)
         self.children.clear()
-        self._logger.debug(f"Phanos - node {self.context} deleted children: {children}")
+        self.debug(f"node {self.context} deleted children: {children}")
 
     @staticmethod
     def get_method_class(meth: typing.Callable) -> str:
         """
         Gets class/module name where specified method/function was defined.
 
         Cannot do: partial, lambda !!!!!
```

### Comparing `phanos-0.0.3/test/dummy_api.py` & `phanos-0.0.4/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/test/run_tests.py` & `phanos-0.0.4/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/test/test_metric.py` & `phanos-0.0.4/test/test_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from flask import Flask
 from flask.ctx import AppContext
 from flask.testing import FlaskClient
 
 from src.phanos import phanos_profiler, publisher
 from src.phanos.publisher import (
     StreamHandler,
-    RabbitMQHandler,
+    ImpProfHandler,
     LoggerHandler,
     BaseHandler,
 )
-from src.phanos.tree import MethodTree
+from src.phanos.tree import MethodTreeNode
 from test import testing_data, dummy_api
 from test.dummy_api import app, dummy_method, DummyDbAccess
 from src.phanos.metrics import (
     Histogram,
     Summary,
     Counter,
     Info,
@@ -35,59 +35,59 @@
     def setUpClass(cls) -> None:
         phanos_profiler.config()
 
     def tearDown(self) -> None:
         pass
 
     def test_tree(self):
-        root = MethodTree()
+        root = MethodTreeNode()
         # classmethod
-        first = MethodTree(dummy_api.DummyDbAccess.test_class)
+        first = MethodTreeNode(dummy_api.DummyDbAccess.test_class)
         root.add_child(first)
         self.assertEqual(first.parent, root)
         self.assertEqual(root.children, [first])
         self.assertEqual(first.context, "DummyDbAccess:test_class")
         root.delete_child()
         self.assertEqual(root.children, [])
         self.assertEqual(first.parent, None)
         # method
-        first = MethodTree(dummy_api.DummyDbAccess.test_method)
+        first = MethodTreeNode(dummy_api.DummyDbAccess.test_method)
         root.add_child(first)
         self.assertEqual(first.context, "DummyDbAccess:test_method")
         root.delete_child()
         # function
-        first = MethodTree(dummy_method)
+        first = MethodTreeNode(dummy_method)
         root.add_child(first)
         self.assertEqual(first.context, "dummy_api:dummy_method")
         root.delete_child()
         # descriptor
         access = DummyDbAccess()
-        first = MethodTree(access.__getattribute__)
+        first = MethodTreeNode(access.__getattribute__)
         root.add_child(first)
         self.assertEqual(first.context, "object:__getattribute__")
         root.delete_child()
         # staticmethod
-        first = MethodTree(access.test_static)
+        first = MethodTreeNode(access.test_static)
         root.add_child(first)
         self.assertEqual(first.context, "DummyDbAccess:test_static")
         root.delete_child()
 
-        first = MethodTree(self.tearDown)
+        first = MethodTreeNode(self.tearDown)
         root.add_child(first)
         self.assertEqual(first.context, "TestTree:tearDown")
 
     def test_clear_tree(self):
         root = phanos_profiler._root
-        _1 = MethodTree(self.tearDown)
+        _1 = MethodTreeNode(self.tearDown)
         root.add_child(_1)
         self.assertEqual(_1.context, "TestTree:tearDown")
-        _1.add_child(MethodTree(self.tearDown))
-        _1.add_child(MethodTree(self.tearDown))
-        _1.add_child(MethodTree(self.tearDown))
-        with patch.object(MethodTree, "_clear_children") as mock:
+        _1.add_child(MethodTreeNode(self.tearDown))
+        _1.add_child(MethodTreeNode(self.tearDown))
+        _1.add_child(MethodTreeNode(self.tearDown))
+        with patch.object(MethodTreeNode, "_clear_children") as mock:
             phanos_profiler.clear()
 
         mock.assert_any_call()
         self.assertEqual(mock.call_count, 5)
 
 
 class TestHandlers(unittest.TestCase):
@@ -143,20 +143,20 @@
         self.assertEqual(len(phanos_profiler._handlers), length + 2)
         phanos_profiler.delete_handler("log_handler1")
         self.assertEqual(phanos_profiler._handlers.get("log_handler1"), None)
         phanos_profiler.delete_handlers()
         self.assertEqual(phanos_profiler._handlers, {})
 
     def test_rabbit_handler_connection(self):
-        self.assertRaises(RuntimeError, RabbitMQHandler, "handle")
+        self.assertRaises(RuntimeError, ImpProfHandler, "handle")
 
     def test_rabbit_handler_publish(self):
         handler = None
         with patch("src.phanos.publisher.BlockingPublisher") as test_publisher:
-            handler = RabbitMQHandler("rabbit")
+            handler = ImpProfHandler("rabbit")
             test_publisher.assert_called()
 
             test_publish = handler._publisher.publish = MagicMock(return_value=3)
 
             #  self.assert
             handler.handle(profiler_name="name", records=testing_data.test_handler_in)
             test_publish.assert_called()
```

### Comparing `phanos-0.0.3/test/testing_data.py` & `phanos-0.0.4/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/.gitignore` & `phanos-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/LICENSE` & `phanos-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.3/README.md` & `phanos-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
    def some_method():
       # some code
    ```
 
 2. Instantiate handlers you need for measured records at app construction.
    ```python      
    from phanos import phanos_profiler
-   from phanos.publisher import LoggerHandler, RabbitMQHandler
+   from phanos.publisher import LoggerHandler, ImpProfHandler
    # some code
    class SomeApp(Flask):
       """some code""" 
    log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
    phanos_profiler.addHandler(log_handler)    
       # some code
    ```
@@ -41,15 +41,15 @@
 Each handler have handler_name parameter. This string can be used to delete handlers later
 with `phanos_profiler.deleteHandler(handler_name)`.
 
 Records can be handled by these handlers:
  - `StreamHandler(handler_name, output)` - write records to given output (default is sys.stdout)
  - `LoggerHandler(handler_name, logger, level)` - logs string representation of records with given logger and with given level
 (default level is `logging.DEBUG`) 
- - `RabbitMQHandler(handler_name, **rabbit_connection_params, logger)` - sending records to RabbitMQ queue of IMP_prof
+ - `ImpProfHandler(handler_name, **rabbit_connection_params, logger)` - sending records to RabbitMQ queue of IMP_prof
 
 ## Phanos metrics:
 
 ### Basic Prometheus metrics:
 
  - Histogram
  - Summary
```

### Comparing `phanos-0.0.3/pyproject.toml` & `phanos-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
-dependencies = [
-    "Flask>=2.2.3",
-    "imp_prof>=0.1.0",
-]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+
 [project.urls]
 "Homepage" = "https://github.com/kajotgames/phanos"
-"Bug Tracker" = "https://github.com/kajotgames/phanos/issues"
-
-[coverage.run]
-branch = true
-source = [
-    "src/phanos",
-    "test",
-]
-
-[coverage.paths]
-source = "phanos"
+"Bug Tracker" = "https://github.com/kajotgames/phanos/issues"
```

### Comparing `phanos-0.0.3/PKG-INFO` & `phanos-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.6
-Requires-Dist: flask>=2.2.3
-Requires-Dist: imp-prof>=0.1.0
 Description-Content-Type: text/markdown
 
 # PHANOS
 Python client to gather data for Prometheus logging in server with multiple instances and workers.
 
 ## Profiling
 
@@ -37,15 +35,15 @@
    def some_method():
       # some code
    ```
 
 2. Instantiate handlers you need for measured records at app construction.
    ```python      
    from phanos import phanos_profiler
-   from phanos.publisher import LoggerHandler, RabbitMQHandler
+   from phanos.publisher import LoggerHandler, ImpProfHandler
    # some code
    class SomeApp(Flask):
       """some code""" 
    log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
    phanos_profiler.addHandler(log_handler)    
       # some code
    ```
@@ -57,15 +55,15 @@
 Each handler have handler_name parameter. This string can be used to delete handlers later
 with `phanos_profiler.deleteHandler(handler_name)`.
 
 Records can be handled by these handlers:
  - `StreamHandler(handler_name, output)` - write records to given output (default is sys.stdout)
  - `LoggerHandler(handler_name, logger, level)` - logs string representation of records with given logger and with given level
 (default level is `logging.DEBUG`) 
- - `RabbitMQHandler(handler_name, **rabbit_connection_params, logger)` - sending records to RabbitMQ queue of IMP_prof
+ - `ImpProfHandler(handler_name, **rabbit_connection_params, logger)` - sending records to RabbitMQ queue of IMP_prof
 
 ## Phanos metrics:
 
 ### Basic Prometheus metrics:
 
  - Histogram
  - Summary
```

