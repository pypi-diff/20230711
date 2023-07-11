# Comparing `tmp/stlog-0.1.2.tar.gz` & `tmp/stlog-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.1.2.tar", max compression
+gzip compressed data, was "stlog-0.1.3.tar", max compression
```

## Comparing `stlog-0.1.2.tar` & `stlog-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-09 08:47:04.585869 stlog-0.1.2/LICENSE
--rw-r--r--   0        0        0     8415 2023-05-09 08:47:04.585869 stlog-0.1.2/README.md
--rw-r--r--   0        0        0     1089 2023-05-09 08:47:29.667365 stlog-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      593 2023-05-09 08:47:29.267341 stlog-0.1.2/stlog/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/adapter.py
--rw-r--r--   0        0        0     7783 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/base.py
--rw-r--r--   0        0        0     2638 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/context.py
--rw-r--r--   0        0        0    14032 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/formatter.py
--rw-r--r--   0        0        0     2499 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/handler.py
--rw-r--r--   0        0        0     5276 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/kvformatter.py
--rw-r--r--   0        0        0     5426 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/output.py
--rw-r--r--   0        0        0     7077 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/setup.py
--rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 13:56:44.519821 stlog-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8415 2023-07-11 13:56:44.519821 stlog-0.1.3/README.md
+-rw-r--r--   0        0        0     1089 2023-07-11 13:57:05.355695 stlog-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      614 2023-07-11 13:57:05.019694 stlog-0.1.3/stlog/__init__.py
+-rw-r--r--   0        0        0     2961 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/adapter.py
+-rw-r--r--   0        0        0     7908 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/context.py
+-rw-r--r--   0        0        0     1557 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/filter.py
+-rw-r--r--   0        0        0    14032 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/formatter.py
+-rw-r--r--   0        0        0      803 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/handler.py
+-rw-r--r--   0        0        0     5276 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/kvformatter.py
+-rw-r--r--   0        0        0     7375 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/output.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/py.typed
+-rw-r--r--   0        0        0     6976 2023-07-11 13:56:44.523821 stlog-0.1.3/stlog/setup.py
+-rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.3/PKG-INFO
```

### Comparing `stlog-0.1.2/LICENSE` & `stlog-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.1.2/README.md` & `stlog-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stlog-0.1.2/pyproject.toml` & `stlog-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stlog"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
```

### Comparing `stlog-0.1.2/stlog/__init__.py` & `stlog-0.1.3/stlog/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,12 +29,13 @@
     "fatal",
     "exception",
 ]
 __pdoc__ = {
     "base": False,
     "adapter": False,
     "handler": False,
+    "filter": False,
     "context": False,
     "warn": False,
     "fatal": False,
 }
-VERSION = "0.1.2"
+VERSION = "0.1.3"
```

### Comparing `stlog-0.1.2/stlog/adapter.py` & `stlog-0.1.3/stlog/adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,18 +43,25 @@
         kwargs["extra"] = extra
         return msg, kwargs
 
 
 class StLogLoggerAdapter(_KeywordArgumentAdapter):
     """stlog `LoggerAdapter` with `stlog.LogContext` support."""
 
+    def __init__(self, logger, extra, ignore_global_logging_context: bool = False):
+        self.ignore_global_logging_context = ignore_global_logging_context
+        super().__init__(logger, extra)
+
     def process(
         self, msg: typing.Any, kwargs: collections.abc.MutableMapping[str, typing.Any]
     ) -> tuple[typing.Any, collections.abc.MutableMapping[str, typing.Any]]:
-        new_kwargs = {**LogContext._get(), **kwargs}
+        if self.ignore_global_logging_context:
+            new_kwargs = dict(kwargs)
+        else:
+            new_kwargs = {**LogContext._get(), **kwargs}
         return super().process(msg, new_kwargs)
 
     def addFilter(self, filter):  # noqa: N802
         self.logger.addFilter(filter)
 
     def removeFilter(self, filter):  # noqa: N802
         self.logger.removeFilter(filter)
```

### Comparing `stlog-0.1.2/stlog/base.py` & `stlog-0.1.3/stlog/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 @dataclass
 class GlobalLoggingConfig:
     setup: bool = False
     program_name: str = field(
         default_factory=lambda: os.path.basename(inspect.stack()[-1][1])
     )
+    reinject_context_in_standard_logging: bool | None = None
+    read_extra_kwargs_from_standard_logging: bool | None = None
     _unit_tests_mode: bool = (
         os.environ.get("STLOG_UNIT_TESTS_MODE", "0").lower() in TRUE_VALUES
     )
 
 
 GLOBAL_LOGGING_CONFIG = GlobalLoggingConfig()
```

### Comparing `stlog-0.1.2/stlog/context.py` & `stlog-0.1.3/stlog/context.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.2/stlog/formatter.py` & `stlog-0.1.3/stlog/formatter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.2/stlog/kvformatter.py` & `stlog-0.1.3/stlog/kvformatter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.2/stlog/setup.py` & `stlog-0.1.3/stlog/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,19 @@
 import sys
 import traceback
 import types
 import typing
 import warnings
 
 from stlog.adapter import getLogger
-from stlog.base import GLOBAL_LOGGING_CONFIG, check_env_false, check_env_true
-from stlog.handler import ContextReinjectHandlerWrapper
+from stlog.base import GLOBAL_LOGGING_CONFIG, check_env_false
 from stlog.output import Output, make_stream_or_rich_stream_output
 
 DEFAULT_LEVEL: str = os.environ.get("STLOG_LEVEL", "INFO")
 DEFAULT_CAPTURE_WARNINGS: bool = check_env_false("STLOG_CAPTURE_WARNINGS", True)
-DEFAULT_REINJECT_CONTEXT_IN_STANDARD_LOGGING: bool = check_env_false(
-    "STLOG_REINJECT_CONTEXT_IN_STANDARD_LOGGING", True
-)
-DEFAULT_READ_EXTRA_KWARG_FROM_STANDARD_LOGGING: bool = check_env_true(
-    "STLOG_READ_EXTRA_KWARGS_FROM_STANDARD_LOGGING", False
-)
 DEFAULT_PROGRAM_NAME: str | None = os.environ.get("STLOG_PROGRAM_NAME", None)
 
 
 def _make_default_outputs() -> list[Output]:
     return [make_stream_or_rich_stream_output(stream=sys.stderr)]
 
 
@@ -56,16 +49,16 @@
     capture_warnings: bool = DEFAULT_CAPTURE_WARNINGS,
     logging_excepthook: typing.Callable[
         [type[BaseException], BaseException, types.TracebackType | None],
         typing.Any,
     ]
     | None = _logging_excepthook,
     extra_levels: typing.Mapping[str, str | int] = {},
-    reinject_context_in_standard_logging: bool = DEFAULT_REINJECT_CONTEXT_IN_STANDARD_LOGGING,
-    read_extra_kwarg_from_standard_logging: bool = False,
+    reinject_context_in_standard_logging: bool | None = None,
+    read_extra_kwargs_from_standard_logging: bool | None = None,
 ) -> None:
     """Set up the Python logging with stlog (globally).
 
     This removes all existing handlers and
     sets up handlers/formatters/... for Python logging.
 
     Args:
@@ -77,42 +70,45 @@
             env var or auto-detected if not set.
         capture_warnings: capture warnings from the `warnings` module.
         logging_excepthook: if not None, override sys.excepthook with the given callable
             See https://docs.python.org/3/library/sys.html#sys.excepthook for details.
         extra_levels: dict "logger name => log level" for quick override of
             the root log level (for some loggers).
         reinject_context_in_standard_logging: if True, reinject the LogContext
-            in log record emitted with python standard loggers.
-        read_extra_kwarg_from_standard_logging: if try to reinject the extra kwargs from standard logging.
+            in log record emitted with python standard loggers (note: can be overriden per `stlog.output.Output`,
+            default to `STLOG_REINJECT_CONTEXT_IN_STANDARD_LOGGING` env var or True if not set).
+        read_extra_kwargs_from_standard_logging: if try to reinject the extra kwargs from standard logging
+            (note: can be overriden per `stlog.output.Output`, default to `STLOG_READ_EXTRA_KWARGS_FROM_STANDARD_LOGGING` env var
+            or False if not set).
+
     """
-    root_logger = logging.getLogger(None)
+    GLOBAL_LOGGING_CONFIG.reinject_context_in_standard_logging = (
+        reinject_context_in_standard_logging
+    )
+    GLOBAL_LOGGING_CONFIG.read_extra_kwargs_from_standard_logging = (
+        read_extra_kwargs_from_standard_logging
+    )
     if program_name is not None:
         GLOBAL_LOGGING_CONFIG.program_name = program_name
 
     if GLOBAL_LOGGING_CONFIG._unit_tests_mode:
         # remove all configured loggers
         for key in list(logging.Logger.manager.loggerDict.keys()):
             logging.Logger.manager.loggerDict.pop(key)
 
+    root_logger = logging.getLogger(None)
     # Remove all handlers
     for handler in list(root_logger.handlers):
         root_logger.removeHandler(handler)
 
     # Add configured handlers
     if outputs is None:
         outputs = _make_default_outputs()
     for out in outputs:
-        if reinject_context_in_standard_logging:
-            handler = ContextReinjectHandlerWrapper(
-                wrapped=out.get_handler(),
-                read_extra_kwarg_from_standard_logging=read_extra_kwarg_from_standard_logging,
-            )
-        else:
-            handler = out.get_handler()
-        root_logger.addHandler(handler)
+        root_logger.addHandler(out.get_handler())
 
     root_logger.setLevel(level)
 
     if logging_excepthook:
         sys.excepthook = logging_excepthook
 
     if capture_warnings:
```

### Comparing `stlog-0.1.2/PKG-INFO` & `stlog-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

