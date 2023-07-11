# Comparing `tmp/taskiq-0.7.2.tar.gz` & `tmp/taskiq-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.7.2.tar", max compression
+gzip compressed data, was "taskiq-0.8.0.tar", max compression
```

## Comparing `taskiq-0.7.2.tar` & `taskiq-0.8.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0     1075 2023-06-17 16:32:30.737189 taskiq-0.7.2/LICENSE
--rw-r--r--   0        0        0     1875 2023-06-17 16:32:30.737189 taskiq-0.7.2/README.md
--rw-r--r--   0        0        0     2879 2023-06-17 16:32:30.741189 taskiq-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2161 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/__init__.py
--rw-r--r--   0        0        0     2093 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12576 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3002 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      496 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/acks.py
--rw-r--r--   0        0        0       34 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3998 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     6060 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7497 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6163 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0     1251 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/events.py
--rw-r--r--   0        0        0     1010 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    12601 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0     2084 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11302 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/task.py
--rw-r--r--   0        0        0      900 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/warnings.py
--rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 taskiq-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-10 21:35:39.047593 taskiq-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-07-10 21:35:39.047593 taskiq-0.8.0/README.md
+-rw-r--r--   0        0        0     2899 2023-07-10 21:35:39.055594 taskiq-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12957 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3562 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      496 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2831 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     4055 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     5805 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     8307 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6471 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     1567 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/compat.py
+-rw-r--r--   0        0        0     1251 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      928 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4535 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2799 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12601 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      237 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/result/__init__.py
+-rw-r--r--   0        0        0     2084 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/result/v1.py
+-rw-r--r--   0        0        0     1923 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/result/v2.py
+-rw-r--r--   0        0        0       35 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11916 2023-07-10 21:35:39.055594 taskiq-0.8.0/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-07-10 21:35:39.059594 taskiq-0.8.0/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-07-10 21:35:39.059594 taskiq-0.8.0/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-07-10 21:35:39.059594 taskiq-0.8.0/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-07-10 21:35:39.059594 taskiq-0.8.0/taskiq/warnings.py
+-rw-r--r--   0        0        0     3605 1970-01-01 00:00:00.000000 taskiq-0.8.0/PKG-INFO
```

### Comparing `taskiq-0.7.2/LICENSE` & `taskiq-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/README.md` & `taskiq-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/pyproject.toml` & `taskiq-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.7.2"
+version = "0.8.0"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
@@ -24,15 +24,15 @@
     "Development Status :: 3 - Alpha",
 ]
 keywords = ["taskiq", "tasks", "distributed", "async"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 typing-extensions = ">=3.10.0.0"
-pydantic = "^1.6.2"
+pydantic = ">=1.0,<=3.0"
 importlib-metadata = "*"
 pycron = "^3.0.0"
 taskiq_dependencies = "^1"
 anyio = "^3"
 # For prometheus metrics
 prometheus_client = { version = "^0", optional = true }
 # For ZMQBroker
@@ -54,14 +54,15 @@
 autoflake = "^1.4"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 wemake-python-styleguide = "^0.18.0"
+tox = "^4.6.4"
 
 [tool.poetry.extras]
 zmq = ["pyzmq"]
 uv = ["uvloop"]
 metrics = ["prometheus_client"]
 reload = ["watchdog", "gitignore-parser"]
```

### Comparing `taskiq-0.7.2/taskiq/__init__.py` & `taskiq-0.8.0/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/__main__.py` & `taskiq-0.8.0/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/abc/broker.py` & `taskiq-0.8.0/taskiq/abc/broker.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,18 +65,14 @@
 
     This abstract class must be implemented in order
     to get ability to send tasks to brokers
     in async mode.
     """
 
     available_tasks: Dict[str, AsyncTaskiqDecoratedTask[Any, Any]] = {}
-    # True only if broker runs in worker process.
-    is_worker_process: bool = False
-    # True only if broker runs in scheduler process.
-    is_scheduler_process: bool = False
 
     def __init__(
         self,
         result_backend: "Optional[AsyncResultBackend[_T]]" = None,
         task_id_generator: Optional[Callable[[], str]] = None,
     ) -> None:
         if result_backend is None:
@@ -107,14 +103,18 @@
         # And handler can be either sync or async.
         self.event_handlers: DefaultDict[
             TaskiqEvents,
             List[Callable[[TaskiqState], Optional[Awaitable[None]]]],
         ] = defaultdict(list)
         self.state = TaskiqState()
         self.custom_dependency_context: Dict[Any, Any] = {}
+        # True only if broker runs in worker process.
+        self.is_worker_process: bool = False
+        # True only if broker runs in scheduler process.
+        self.is_scheduler_process: bool = False
 
     def add_dependency_context(self, new_ctx: Dict[Any, Any]) -> None:
         """
         Add first-level dependencies.
 
         Provided dict will be used to inject new dependencies
         in all dependency graph contexts.
@@ -147,14 +147,18 @@
         event = TaskiqEvents.CLIENT_STARTUP
         if self.is_worker_process:
             event = TaskiqEvents.WORKER_STARTUP
 
         for handler in self.event_handlers[event]:
             await maybe_awaitable(handler(self.state))
 
+        for middleware in self.middlewares:
+            if middleware.__class__.startup != TaskiqMiddleware.startup:
+                await maybe_awaitable(middleware.startup)
+
         await self.result_backend.startup()
 
     async def shutdown(self) -> None:
         """
         Close the broker.
 
         This method is called,
@@ -164,14 +168,18 @@
         if self.is_worker_process:
             event = TaskiqEvents.WORKER_SHUTDOWN
 
         # Call all shutdown events.
         for handler in self.event_handlers[event]:
             await maybe_awaitable(handler(self.state))
 
+        for middleware in self.middlewares:
+            if middleware.__class__.shutdown != TaskiqMiddleware.shutdown:
+                await maybe_awaitable(middleware.shutdown)
+
         await self.result_backend.shutdown()
 
     @abstractmethod
     async def kick(
         self,
         message: BrokerMessage,
     ) -> None:
```

### Comparing `taskiq-0.7.2/taskiq/abc/formatter.py` & `taskiq-0.8.0/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/abc/middleware.py` & `taskiq-0.8.0/taskiq/abc/middleware.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,14 +16,34 @@
         """
         Sets broker to middleware.
 
         :param broker: broker to set.
         """
         self.broker = broker
 
+    def startup(self) -> "Union[None, Coroutine[Any, Any, None]]":
+        """
+        Startup method to perform various action during startup.
+
+        This function can be either sync or async.
+        Executed during broker's startup.
+
+        :returns nothing.
+        """
+
+    def shutdown(self) -> "Union[None, Coroutine[Any, Any, None]]":
+        """
+        Shutdown method to perform various action during shutdown.
+
+        This function can be either sync or async.
+        Executed during broker's shutdown.
+
+        :returns nothing.
+        """
+
     def pre_send(
         self,
         message: "TaskiqMessage",
     ) -> "Union[TaskiqMessage, Coroutine[Any, Any, TaskiqMessage]]":
         """
         Hook that executes before sending the task to worker.
```

### Comparing `taskiq-0.7.2/taskiq/abc/result_backend.py` & `taskiq-0.8.0/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/abc/schedule_source.py` & `taskiq-0.8.0/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/brokers/inmemory_broker.py` & `taskiq-0.8.0/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/brokers/shared_broker.py` & `taskiq-0.8.0/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/brokers/zmq_broker.py` & `taskiq-0.8.0/taskiq/brokers/zmq_broker.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.message import BrokerMessage
 
 try:
     import zmq  # noqa: WPS433
-    from zmq.asyncio import Context  # noqa: WPS433
+    from zmq.asyncio import Context, Socket  # noqa: WPS433
 except ImportError:
     zmq = None  # type: ignore
 
 _T = TypeVar("_T")  # noqa: WPS111
 
 logger = getLogger(__name__)
 
@@ -39,20 +39,31 @@
             raise RuntimeError(
                 "To use ZMQ broker please install pyzmq lib or taskiq[zmq].",
             )
         super().__init__(result_backend, task_id_generator)
         self.context = Context()
         self.pub_host = zmq_pub_host
         self.sub_host = zmq_sub_host
+        self.socket: Socket
+
+    async def startup(self) -> None:
+        """
+        Startup for zmq broker.
+
+        This function creates actual connections to
+        sockets. if current process is worker,
+        it subscribes, otherwise it becomes publisher.
+        """
         if self.is_worker_process:
             self.socket = self.context.socket(zmq.SUB)
             self.socket.setsockopt(zmq.SUBSCRIBE, b"")
         else:
             self.socket = self.context.socket(zmq.PUB)
             self.socket.bind(self.pub_host)
+        await super().startup()
 
     async def kick(self, message: BrokerMessage) -> None:
         """
         Kicking message.
 
         This method is used to publish message
         via socket.
```

### Comparing `taskiq-0.7.2/taskiq/cli/scheduler/args.py` & `taskiq-0.8.0/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/cli/scheduler/cmd.py` & `taskiq-0.8.0/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/cli/scheduler/run.py` & `taskiq-0.8.0/taskiq/cli/scheduler/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 from datetime import datetime, timedelta
 from logging import basicConfig, getLevelName, getLogger
 from typing import List
 
 from pycron import is_now
 
-from taskiq.abc.broker import AsyncBroker
 from taskiq.cli.scheduler.args import SchedulerArgs
 from taskiq.cli.utils import import_object, import_tasks
 from taskiq.kicker import AsyncKicker
 from taskiq.scheduler.scheduler import ScheduledTask, TaskiqScheduler
 
 logger = getLogger(__name__)
 
@@ -67,21 +66,24 @@
     Runs scheduler loop.
 
     This function imports taskiq scheduler
     and runs tasks when needed.
 
     :param args: parsed CLI args.
     """
-    AsyncBroker.is_scheduler_process = True
-    scheduler = import_object(args.scheduler)
-    if not isinstance(scheduler, TaskiqScheduler):
+    if isinstance(args.scheduler, str):
+        scheduler = import_object(args.scheduler)
+    else:
+        scheduler = args.scheduler
+    if not isinstance(args.scheduler, TaskiqScheduler):
         print(  # noqa: WPS421
             "Imported scheduler is not a subclass of TaskiqScheduler.",
         )
         exit(1)  # noqa: WPS421
+    scheduler.broker.is_scheduler_process = True
     import_tasks(args.modules, args.tasks_pattern, args.fs_discover)
     basicConfig(
         level=getLevelName(args.log_level),
         format=(
             "[%(asctime)s][%(levelname)-7s]"
             "[%(module)s:%(funcName)s:%(lineno)d]"
             " %(message)s"
```

### Comparing `taskiq-0.7.2/taskiq/cli/utils.py` & `taskiq-0.8.0/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/cli/watcher.py` & `taskiq-0.8.0/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/cli/worker/args.py` & `taskiq-0.8.0/taskiq/cli/worker/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,17 @@
 class WorkerArgs:
     """Taskiq worker CLI arguments."""
 
     broker: str
     modules: List[str]
     tasks_pattern: str = "tasks.py"
     fs_discover: bool = False
+    configure_logging: bool = True
     log_level: LogLevel = LogLevel.INFO
     workers: int = 2
-    log_collector_format: str = (
-        "[%(asctime)s][%(levelname)-7s][%(module)s:%(funcName)s:%(lineno)d] %(message)s"
-    )
     max_threadpool_threads: int = 10
     no_parse: bool = False
     shutdown_timeout: float = 5
     reload: bool = False
     no_gitignore: bool = False
     max_async_tasks: int = 100
     receiver: str = "taskiq.receiver:Receiver"
@@ -115,26 +113,14 @@
             "--workers",
             "-w",
             type=int,
             default=2,
             help="Number of worker child processes",
         )
         parser.add_argument(
-            "--log-collector-format",
-            "-lcf",
-            type=str,
-            default=(
-                "[%(asctime)s]"
-                "[%(levelname)-7s]"
-                "[%(module)s:%(funcName)s:%(lineno)d] "
-                "%(message)s"
-            ),
-            help="Format which is used when collecting logs from function execution",
-        )
-        parser.add_argument(
             "--no-parse",
             action="store_true",
             help=(
                 "If this parameter is on,"
                 " taskiq doesn't parse incoming parameters "
                 " with pydantic."
             ),
@@ -183,10 +169,16 @@
         parser.add_argument(
             "--max-prefetch",
             type=int,
             dest="max_prefetch",
             default=0,
             help="Maximum prefetched tasks per worker process. ",
         )
+        parser.add_argument(
+            "--no-configure-logging",
+            action="store_false",
+            dest="configure_logging",
+            help="Use this parameter if your application configures custom logging.",
+        )
 
         namespace = parser.parse_args(args)
         return WorkerArgs(**namespace.__dict__)
```

### Comparing `taskiq-0.7.2/taskiq/cli/worker/cmd.py` & `taskiq-0.8.0/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/cli/worker/log_collector.py` & `taskiq-0.8.0/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/cli/worker/process_manager.py` & `taskiq-0.8.0/taskiq/cli/worker/process_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import signal
+from contextlib import suppress
 from dataclasses import dataclass
-from multiprocessing import Process, Queue
+from multiprocessing import Event, Process, Queue, current_process
+from multiprocessing.synchronize import Event as EventType
 from time import sleep
 from typing import Any, Callable, List, Optional
 
 try:
     from watchdog.observers import Observer  # noqa: WPS433
 
     from taskiq.cli.watcher import FileWatcher  # noqa: WPS433
@@ -50,15 +52,15 @@
 
     worker_num: int
 
     def handle(
         self,
         workers: List[Process],
         args: WorkerArgs,
-        worker_func: Callable[[WorkerArgs], None],
+        worker_func: Callable[[WorkerArgs, EventType], None],
     ) -> None:
         """
         This action reloads a single process.
 
         :param workers: known children processes.
         :param args: args for new process.
         :param worker_func: function that is used to start worker processes.
@@ -69,30 +71,39 @@
         worker = workers[self.worker_num]
         try:
             worker.terminate()
         except ValueError:
             logger.debug(f"Process {worker.name} is already terminated.")
         # Waiting worker shutdown.
         worker.join()
+        event: EventType = Event()
         new_process = Process(
             target=worker_func,
-            kwargs={"args": args},
+            kwargs={"args": args, "event": event},
             name=f"worker-{self.worker_num}",
             daemon=True,
         )
         new_process.start()
         logger.info(f"Process {new_process.name} restarted with pid {new_process.pid}")
         workers[self.worker_num] = new_process
+        _wait_for_worker_startup(new_process, event)
 
 
 @dataclass
 class ShutdownAction(ProcessActionBase):
     """This action shuts down process manager loop."""
 
 
+def _wait_for_worker_startup(process: Process, event: EventType) -> None:
+    while process.is_alive():
+        with suppress(TimeoutError):
+            event.wait(0.1)
+            return
+
+
 def schedule_workers_reload(
     action_queue: "Queue[ProcessActionBase]",
 ) -> None:
     """
     Function to schedule workers to restart.
 
     It simply send FULL_RELOAD event, which is handled
@@ -114,14 +125,17 @@
     the action queue.
 
     :param action_queue: event queue.
     :returns: actual signal handler.
     """
 
     def _signal_handler(signum: int, _frame: Any) -> None:
+        if current_process().name.startswith("worker"):
+            raise KeyboardInterrupt
+
         logger.debug(f"Got signal {signum}.")
         action_queue.put(ShutdownAction())
         logger.warn("Workers are scheduled for shutdown.")
 
     return _signal_handler
 
 
@@ -133,16 +147,16 @@
     and maintains their states. If process
     is down, it tries to restart it.
     """
 
     def __init__(
         self,
         args: WorkerArgs,
-        worker_function: Callable[[WorkerArgs], None],
-        observer: Optional[Observer] = None,
+        worker_function: Callable[[WorkerArgs, EventType], None],
+        observer: Optional[Observer] = None,  # type: ignore[valid-type]
     ) -> None:
         self.worker_function = worker_function
         self.action_queue: "Queue[ProcessActionBase]" = Queue(-1)
         self.args = args
         if args.reload and observer is not None:
             observer.schedule(
                 FileWatcher(
@@ -158,28 +172,35 @@
         signal.signal(signal.SIGINT, signal_handler)
         signal.signal(signal.SIGTERM, signal_handler)
 
         self.workers: List[Process] = []
 
     def prepare_workers(self) -> None:
         """Spawn multiple processes."""
+        events: List[EventType] = []
         for process in range(self.args.workers):
+            event = Event()
             work_proc = Process(
                 target=self.worker_function,
-                kwargs={"args": self.args},
+                kwargs={"args": self.args, "event": event},
                 name=f"worker-{process}",
                 daemon=True,
             )
             work_proc.start()
             logger.info(
                 "Started process worker-%d with pid %s ",
                 process,
                 work_proc.pid,
             )
             self.workers.append(work_proc)
+            events.append(event)
+
+        # Wait for workers startup
+        for worker, event in zip(self.workers, events):
+            _wait_for_worker_startup(worker, event)
 
     def start(self) -> None:  # noqa: C901, WPS213
         """
         Start managing child processes.
 
         This function is an endless loop,
         which listens to new events from different sources.
```

### Comparing `taskiq-0.7.2/taskiq/cli/worker/run.py` & `taskiq-0.8.0/taskiq/cli/worker/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import logging
 import signal
 from concurrent.futures import ThreadPoolExecutor
+from multiprocessing.synchronize import Event
 from typing import Any, Type
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.cli.utils import import_object, import_tasks
 from taskiq.cli.worker.args import WorkerArgs
 from taskiq.cli.worker.process_manager import ProcessManager
 from taskiq.receiver import Receiver
@@ -61,44 +62,29 @@
     """
     receiver_type = import_object(args.receiver)
     if not (isinstance(receiver_type, type) and issubclass(receiver_type, Receiver)):
         raise ValueError("Unknown receiver type. Please use Receiver class.")
     return receiver_type
 
 
-def start_listen(args: WorkerArgs) -> None:  # noqa: WPS210, WPS213
+def start_listen(args: WorkerArgs, event: Event) -> None:  # noqa: WPS210, WPS213
     """
     This function starts actual listening process.
 
     It imports broker and all tasks.
     Since tasks registers themselves in a global set,
     it's easy to just import module where you have decorated
     function and they will be available in broker's `available_tasks`
     field.
 
     :param args: CLI arguments.
+    :param event: Event for notification.
     :raises ValueError: if broker is not an AsyncBroker instance.
     :raises ValueError: if receiver is not a Receiver type.
     """
-    if uvloop is not None:
-        logger.debug("UVLOOP found. Installing policy.")
-        uvloop.install()
-    # This option signals that current
-    # broker is running as a worker.
-    # We must set this field before importing tasks,
-    # so broker will remember all tasks it's related to.
-    AsyncBroker.is_worker_process = True
-    broker = import_object(args.broker)
-    import_tasks(args.modules, args.tasks_pattern, args.fs_discover)
-    if not isinstance(broker, AsyncBroker):
-        raise ValueError("Unknown broker type. Please use AsyncBroker instance.")
-
-    receiver_type = get_receiver_type(args)
-    receiver_args = dict(args.receiver_arg)
-
     # Here how we manage interruptions.
     # We have to remember shutting_down state,
     # because KeyboardInterrupt can be send multiple
     # times. And it may interrupt the broker's shutdown process.
     shutting_down = False
 
     def interrupt_handler(signum: int, _frame: Any) -> None:
@@ -118,14 +104,33 @@
             return
         shutting_down = True  # noqa: WPS442
         raise KeyboardInterrupt
 
     signal.signal(signal.SIGINT, interrupt_handler)
     signal.signal(signal.SIGTERM, interrupt_handler)
 
+    # Notify parent process, worker is ready
+    event.set()
+
+    if uvloop is not None:
+        logger.debug("UVLOOP found. Installing policy.")
+        uvloop.install()
+    # This option signals that current
+    # broker is running as a worker.
+    # We must set this field before importing tasks,
+    # so broker will remember all tasks it's related to.
+    broker = import_object(args.broker)
+    if not isinstance(broker, AsyncBroker):
+        raise ValueError("Unknown broker type. Please use AsyncBroker instance.")
+    broker.is_worker_process = True
+    import_tasks(args.modules, args.tasks_pattern, args.fs_discover)
+
+    receiver_type = get_receiver_type(args)
+    receiver_args = dict(args.receiver_arg)
+
     loop = asyncio.get_event_loop()
 
     try:
         logger.debug("Initialize receiver.")
         with ThreadPoolExecutor(args.max_threadpool_threads) as pool:
             receiver = receiver_type(
                 broker=broker,
@@ -149,18 +154,21 @@
     It just creates multiple child processes
     and joins them all.
 
     :param args: CLI arguments.
 
     :raises ValueError: if reload flag is used, but dependencies are not installed.
     """
-    logging.basicConfig(
-        level=logging.getLevelName(args.log_level),
-        format="[%(asctime)s][%(name)s][%(levelname)-7s][%(processName)s] %(message)s",
-    )
+    if args.configure_logging:
+        logging.basicConfig(
+            level=logging.getLevelName(args.log_level),
+            format="[%(asctime)s][%(name)s][%(levelname)-7s]"
+            + "[%(processName)s] %(message)s",
+        )
+    logging.getLogger("taskiq").setLevel(level=logging.getLevelName(args.log_level))
     logging.getLogger("watchdog.observers.inotify_buffer").setLevel(level=logging.INFO)
     logger.info("Starting %s worker processes.", args.workers)
 
     observer = None
 
     if args.reload and Observer is None:
         raise ValueError("To use '--reload' flag, please install 'taskiq[reload]'.")
```

### Comparing `taskiq-0.7.2/taskiq/context.py` & `taskiq-0.8.0/taskiq/context.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/decor.py` & `taskiq-0.8.0/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/exceptions.py` & `taskiq-0.8.0/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/formatters/json_formatter.py` & `taskiq-0.8.0/taskiq/formatters/json_formatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from taskiq.abc.formatter import TaskiqFormatter
+from taskiq.compat import model_dump_json, model_validate_json
 from taskiq.message import BrokerMessage, TaskiqMessage
 
 
 class JSONFormatter(TaskiqFormatter):
     """Default taskiq formatter."""
 
     def dumps(self, message: TaskiqMessage) -> BrokerMessage:
@@ -11,19 +12,19 @@
 
         :param message: message to send.
         :return: Dumped message.
         """
         return BrokerMessage(
             task_id=message.task_id,
             task_name=message.task_name,
-            message=message.json().encode(),
+            message=model_dump_json(message).encode(),
             labels=message.labels,
         )
 
     def loads(self, message: bytes) -> TaskiqMessage:
         """
         Loads json from message.
 
         :param message: broker's message.
         :return: parsed taskiq message.
         """
-        return TaskiqMessage.parse_raw(message)
+        return model_validate_json(TaskiqMessage, message)
```

### Comparing `taskiq-0.7.2/taskiq/funcs.py` & `taskiq-0.8.0/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/kicker.py` & `taskiq-0.8.0/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.8.0/taskiq/middlewares/prometheus_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from logging import getLogger
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Any, Optional
 
-from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.message import TaskiqMessage
 from taskiq.result import TaskiqResult
 
 logger = getLogger("taskiq.prometheus")
 
 
@@ -32,35 +31,28 @@
 
         self.found_errors = None
         self.received_tasks = None
         self.success_tasks = None
         self.saved_results = None
         self.execution_time = None
 
-        if not AsyncBroker.is_worker_process:
-            return
-
         metrics_path = metrics_path or Path(gettempdir()) / "taskiq_worker"
 
         if not metrics_path.exists():
             metrics_path.mkdir(parents=True)
 
         logger.debug(f"Setting up multiproc dir to {metrics_path}")
 
         os.environ["PROMETHEUS_MULTIPROC_DIR"] = str(metrics_path)
         os.environ["prometheus_multiproc_dir"] = str(metrics_path)
 
         logger.debug("Initializing metrics")
 
         try:
-            from prometheus_client import (  # noqa: WPS433
-                Counter,
-                Histogram,
-                start_http_server,
-            )
+            from prometheus_client import Counter, Histogram  # noqa: WPS433
         except ImportError as exc:
             raise ImportError(
                 "Cannot initialize metrics. Please install 'taskiq[metrics]'.",
             ) from exc
 
         self.found_errors = Counter(
             "found_errors",
@@ -83,18 +75,31 @@
             ["task_name"],
         )
         self.execution_time = Histogram(
             "execution_time",
             "Tome of function execution",
             ["task_name"],
         )
-        try:
-            start_http_server(port=server_port, addr=server_addr)
-        except OSError as exc:
-            logger.debug("Cannot start prometheus server: %s", exc)
+        self.server_port = server_port
+        self.server_addr = server_addr
+
+    def startup(self) -> None:
+        """
+        Prometheus startup.
+
+        This function starts prometheus server.
+        It starts it only in case if it's a worker process.
+        """
+        from prometheus_client import start_http_server  # noqa: WPS433
+
+        if self.broker.is_worker_process:
+            try:
+                start_http_server(port=self.server_port, addr=self.server_addr)
+            except OSError as exc:
+                logger.debug("Cannot start prometheus server: %s", exc)
 
     def pre_execute(
         self,
         message: "TaskiqMessage",
     ) -> "TaskiqMessage":
         """
         Function to track received tasks.
```

### Comparing `taskiq-0.7.2/taskiq/middlewares/retry_middleware.py` & `taskiq-0.8.0/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/receiver/params_parser.py` & `taskiq-0.8.0/taskiq/receiver/params_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 from logging import getLogger
 from typing import Any, Dict, Optional
 
-from pydantic import parse_obj_as
-
+from taskiq.compat import parse_obj_as
 from taskiq.message import TaskiqMessage
 
 logger = getLogger(__name__)
 
 
 def parse_params(  # noqa: C901
     signature: Optional[inspect.Signature],
```

### Comparing `taskiq-0.7.2/taskiq/receiver/receiver.py` & `taskiq-0.8.0/taskiq/receiver/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/result.py` & `taskiq-0.8.0/taskiq/result/v1.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/result_backends/dummy.py` & `taskiq-0.8.0/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/schedule_sources/label_based.py` & `taskiq-0.8.0/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/scheduler/merge_functions.py` & `taskiq-0.8.0/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/scheduler/scheduler.py` & `taskiq-0.8.0/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/serialization.py` & `taskiq-0.8.0/taskiq/serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Union,
 )
 
 import pydantic
 from typing_extensions import Protocol, TypeVar, runtime_checkable
 
 import taskiq.exceptions  # noqa: WPS301
+from taskiq.compat import IS_PYDANTIC2, validate_call
 
 DecodedType = TypeVar("DecodedType")
 EncodedType = TypeVar("EncodedType")
 
 UNWANTED_BASE_CLASSES = (Exception, BaseException, object)
 SEEN_EXCEPTIONS_CACHE: Set[int] = set()
 
@@ -241,26 +242,42 @@
     """
     if isinstance(exc, _UnpickleableExceptionWrapper):
         return exc.restore()
 
     return exc
 
 
-class ExceptionRepr(pydantic.BaseModel):
-    """Serialiable exception representation."""
+if IS_PYDANTIC2:
 
-    exc_type: str
-    exc_message: Tuple[Any, ...]
-    exc_module: Optional[str]
-    exc_cause: Optional[Union[BaseException, "ExceptionRepr"]] = None
-    exc_context: Optional[Union[BaseException, "ExceptionRepr"]] = None
-    exc_suppress_context: bool = False
+    class ExceptionRepr(pydantic.BaseModel):
+        """Serializable exception model for pydantic v2."""
 
-    class Config:
-        arbitrary_types_allowed = True
+        exc_type: str
+        exc_message: Tuple[Any, ...]
+        exc_module: Optional[str]
+        exc_cause: Optional[Union[BaseException, "ExceptionRepr"]] = None
+        exc_context: Optional[Union[BaseException, "ExceptionRepr"]] = None
+        exc_suppress_context: bool = False
+
+        model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
+
+else:
+
+    class ExceptionRepr(pydantic.BaseModel):  # type: ignore
+        """Serializable exception model for pydantic v1."""
+
+        exc_type: str
+        exc_message: Tuple[Any, ...]
+        exc_module: Optional[str]
+        exc_cause: Optional[Union[BaseException, "ExceptionRepr"]] = None
+        exc_context: Optional[Union[BaseException, "ExceptionRepr"]] = None
+        exc_suppress_context: bool = False
+
+        class Config:
+            arbitrary_types_allowed = True
 
 
 def _prepare_exception(
     exc: BaseException,
     coder: Coder[Any, Any],
 ) -> Optional[Union[BaseException, ExceptionRepr]]:
     # Prevent infinite loop
@@ -293,30 +310,30 @@
             exc_suppress_context=exc.__suppress_context__,
         )
 
     finally:
         SEEN_EXCEPTIONS_CACHE.discard(id(exc))
 
 
-@pydantic.validate_arguments(config={"arbitrary_types_allowed": True})
+@validate_call(config=pydantic.ConfigDict(arbitrary_types_allowed=True))
 def prepare_exception(
     exc: BaseException,
     coder: Coder[Any, Any],
 ) -> Union[BaseException, ExceptionRepr]:
     """Prepare exception for serialization.
 
     :param exc: exception to encode
     :param coder: serializer with `loads` and `dumps`
     :return: serializable exception
     """
     SEEN_EXCEPTIONS_CACHE.clear()
     return _prepare_exception(exc, coder)  # type: ignore
 
 
-@pydantic.validate_arguments(config={"arbitrary_types_allowed": True})
+@validate_call(config=pydantic.ConfigDict(arbitrary_types_allowed=True))
 def exception_to_python(  # noqa: C901, WPS210
     exc: Optional[Union[BaseException, ExceptionRepr]],
 ) -> Optional[BaseException]:
     """Convert serialized exception to Python exception.
 
     :param exc: encoded exception
     :raises SecurityError: exception isn't indead an exception
```

### Comparing `taskiq-0.7.2/taskiq/state.py` & `taskiq-0.8.0/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/task.py` & `taskiq-0.8.0/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/taskiq/utils.py` & `taskiq-0.8.0/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.2/PKG-INFO` & `taskiq-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.7.2
+Version: 0.8.0
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
@@ -28,15 +28,15 @@
 Provides-Extra: uv
 Provides-Extra: zmq
 Requires-Dist: anyio (>=3,<4)
 Requires-Dist: gitignore-parser (>=0,<1) ; extra == "reload"
 Requires-Dist: importlib-metadata
 Requires-Dist: prometheus_client (>=0,<1) ; extra == "metrics"
 Requires-Dist: pycron (>=3.0.0,<4.0.0)
-Requires-Dist: pydantic (>=1.6.2,<2.0.0)
+Requires-Dist: pydantic (>=1.0,<=3.0)
 Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2)
 Requires-Dist: typing-extensions (>=3.10.0.0)
 Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv"
 Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra == "reload"
 Project-URL: Documentation, https://taskiq-python.github.io/
 Project-URL: Repository, https://github.com/taskiq-python/taskiq
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.7.2 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.8.0 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -11,15 +11,15 @@
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Topic :: System
 :: Networking Classifier: Typing :: Typed Provides-Extra: metrics Provides-
 Extra: reload Provides-Extra: uv Provides-Extra: zmq Requires-Dist: anyio
 (>=3,<4) Requires-Dist: gitignore-parser (>=0,<1) ; extra == "reload" Requires-
 Dist: importlib-metadata Requires-Dist: prometheus_client (>=0,<1) ; extra ==
 "metrics" Requires-Dist: pycron (>=3.0.0,<4.0.0) Requires-Dist: pydantic
-(>=1.6.2,<2.0.0) Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
+(>=1.0,<=3.0) Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2) Requires-Dist: typing-extensions
 (>=3.10.0.0) Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv" Requires-Dist:
 watchdog (>=2.1.9,<3.0.0) ; extra == "reload" Project-URL: Documentation,
 https://taskiq-python.github.io/ Project-URL: Repository, https://github.com/
 taskiq-python/taskiq Description-Content-Type: text/markdown [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)]
 (https://pypi.org/project/taskiq/) [![PyPI](https://img.shields.io/pypi/v/
```

