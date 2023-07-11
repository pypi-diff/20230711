# Comparing `tmp/pyno_logger-0.0.8.tar.gz` & `tmp/pyno_logger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyno_logger-0.0.8.tar", last modified: Mon Jul 10 06:02:17 2023, max compression
+gzip compressed data, was "pyno_logger-0.0.9.tar", last modified: Mon Jul 10 06:16:47 2023, max compression
```

## Comparing `pyno_logger-0.0.8.tar` & `pyno_logger-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:02:17.993774 pyno_logger-0.0.8/
--rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.8/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     5981 2023-07-10 06:02:17.993656 pyno_logger-0.0.8/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     5463 2023-07-10 05:59:28.000000 pyno_logger-0.0.8/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:02:17.993000 pyno_logger-0.0.8/pyno_logger/
--rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.8/pyno_logger/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     5999 2023-07-10 05:47:16.000000 pyno_logger-0.0.8/pyno_logger/pyno_logger.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:02:17.993474 pyno_logger-0.0.8/pyno_logger.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     5981 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-10 06:00:22.000000 pyno_logger-0.0.8/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-10 06:02:17.993815 pyno_logger-0.0.8/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:16:47.582744 pyno_logger-0.0.9/
+-rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.9/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     6230 2023-07-10 06:16:47.582629 pyno_logger-0.0.9/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     5712 2023-07-10 06:16:35.000000 pyno_logger-0.0.9/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:16:47.581987 pyno_logger-0.0.9/pyno_logger/
+-rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.9/pyno_logger/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     6311 2023-07-10 06:09:24.000000 pyno_logger-0.0.9/pyno_logger/pyno_logger.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:16:47.582471 pyno_logger-0.0.9/pyno_logger.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     6230 2023-07-10 06:16:47.000000 pyno_logger-0.0.9/pyno_logger.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-10 06:16:47.000000 pyno_logger-0.0.9/pyno_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-10 06:16:47.000000 pyno_logger-0.0.9/pyno_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-10 06:16:47.000000 pyno_logger-0.0.9/pyno_logger.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-10 06:15:24.000000 pyno_logger-0.0.9/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-10 06:16:47.582786 pyno_logger-0.0.9/setup.cfg
```

### Comparing `pyno_logger-0.0.8/LICENSE` & `pyno_logger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.8/PKG-INFO` & `pyno_logger-0.0.9/pyno_logger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyno_logger
-Version: 0.0.8
+Name: pyno-logger
+Version: 0.0.9
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,29 +32,33 @@
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
-- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
+- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". If set, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict. Defaults to `INFO`.
 
-- `base` (optional): Dictionary with any base configuration that is applied to all logs.
+- `base` (optional): Dictionary with any base configuration that is applied to all logs. Defaults to `{}`.
 
-- `enabled` (optional): Boolean value that sets the enabled state of the logger.
+- `enabled` (optional): Boolean value that sets the enabled state of the logger. Defaults to `True`.
+
+- `log_none` (optional): Boolean value that determines if `None` values are logged in JSON output. Defaults to `False`.
 
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
 
-- `redact_value` (optional): Custom value for any keys that are redacted during a log.
+- `redact_value` (optional): Custom value for any keys that are redacted during a log. Defaults to `[REDACTED]`.
+
+- `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string. Defaults to `[]`.
+
+- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission. Defaults to `[]`.
 
-- `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
-- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission.
-- `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
+- `newlines` (optional): Boolean value that specifies whether to append a newline character to the end of each log message. Defaults to `False`.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
 ### Logging Methods
```

### Comparing `pyno_logger-0.0.8/README.md` & `pyno_logger-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
-- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
+- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". If set, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict. Defaults to `INFO`.
 
-- `base` (optional): Dictionary with any base configuration that is applied to all logs.
+- `base` (optional): Dictionary with any base configuration that is applied to all logs. Defaults to `{}`.
 
-- `enabled` (optional): Boolean value that sets the enabled state of the logger.
+- `enabled` (optional): Boolean value that sets the enabled state of the logger. Defaults to `True`.
+
+- `log_none` (optional): Boolean value that determines if `None` values are logged in JSON output. Defaults to `False`.
 
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
 
-- `redact_value` (optional): Custom value for any keys that are redacted during a log.
+- `redact_value` (optional): Custom value for any keys that are redacted during a log. Defaults to `[REDACTED]`.
+
+- `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string. Defaults to `[]`.
+
+- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission. Defaults to `[]`.
 
-- `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
-- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission.
-- `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
+- `newlines` (optional): Boolean value that specifies whether to append a newline character to the end of each log message. Defaults to `False`.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
 ### Logging Methods
```

### Comparing `pyno_logger-0.0.8/pyno_logger/pyno_logger.py` & `pyno_logger-0.0.9/pyno_logger/pyno_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     }
     log_level = getenv("LOG_LEVEL") or "INFO"
 
     config = {}
     omitted_keys = []
     redacted_keys = []
     newlines = False
+    log_none = False
     msg_key = "msg"
     error_key = "error"
     redact_value = "[REDACTED]"
     enabled = True
 
     mixin = None
 
@@ -107,14 +108,17 @@
 
         if config.get("enabled") and isinstance(config["enabled"], bool):
             self.enabled = config["enabled"]
 
         if config.get("redact_value") and isinstance(config["redact_value"], str):
             self.redact_value = config["redact_value"]
 
+        if config.get("log_none") and isinstance(config["log_none"], bool):
+            self.log_none = config["log_none"]
+
     def log(self, level, data, message=None):
         level_num = LogLevel.get(level)
 
         if not level_num or not isinstance(level_num, int):
             raise Exception(f"Invalid log level: {level}")
 
         if self.log_level == "SILENT" or level_num == 0 or not self.enabled:
@@ -164,14 +168,19 @@
                         del to_log[key]
 
             if len(self.redacted_keys):
                 for key in self.redacted_keys:
                     if key in to_log:
                         to_log[key] = self.redact_value
 
+            if not self.log_none:
+                for key in list(to_log.keys()):
+                    if to_log[key] is None:
+                        del to_log[key]
+
             try:
                 json_to_log = json.dumps(to_log, cls=DecimalEncoder)
                 if self.newlines:
                     json_to_log += "\n"
                 print(json_to_log)
             except Exception as e:
                 print(f"Error logging: {e}")
```

### Comparing `pyno_logger-0.0.8/pyno_logger.egg-info/PKG-INFO` & `pyno_logger-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyno-logger
-Version: 0.0.8
+Name: pyno_logger
+Version: 0.0.9
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,29 +32,33 @@
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
-- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
+- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". If set, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict. Defaults to `INFO`.
 
-- `base` (optional): Dictionary with any base configuration that is applied to all logs.
+- `base` (optional): Dictionary with any base configuration that is applied to all logs. Defaults to `{}`.
 
-- `enabled` (optional): Boolean value that sets the enabled state of the logger.
+- `enabled` (optional): Boolean value that sets the enabled state of the logger. Defaults to `True`.
+
+- `log_none` (optional): Boolean value that determines if `None` values are logged in JSON output. Defaults to `False`.
 
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
 
-- `redact_value` (optional): Custom value for any keys that are redacted during a log.
+- `redact_value` (optional): Custom value for any keys that are redacted during a log. Defaults to `[REDACTED]`.
+
+- `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string. Defaults to `[]`.
+
+- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission. Defaults to `[]`.
 
-- `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
-- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission.
-- `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
+- `newlines` (optional): Boolean value that specifies whether to append a newline character to the end of each log message. Defaults to `False`.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
 ### Logging Methods
```

