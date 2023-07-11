# Comparing `tmp/atro_pylog-0.1.4.tar.gz` & `tmp/atro_pylog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_pylog-0.1.4.tar", max compression
+gzip compressed data, was "atro_pylog-0.2.0.tar", max compression
```

## Comparing `atro_pylog-0.1.4.tar` & `atro_pylog-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1763 2023-07-02 10:28:41.837142 atro_pylog-0.1.4/pylog/__init__.py
--rw-r--r--   0        0        0     1050 2023-07-02 10:20:33.596546 atro_pylog-0.1.4/pylog/level.py
--rw-r--r--   0        0        0      363 2023-07-02 10:20:33.596546 atro_pylog-0.1.4/pylog/logger_type.py
--rw-r--r--   0        0        0     1106 2023-07-05 06:56:40.494773 atro_pylog-0.1.4/pylog/opentelemetry_setup.py
--rw-r--r--   0        0        0      127 2023-07-02 10:20:33.596546 atro_pylog-0.1.4/pylog/rich_setup.py
--rw-r--r--   0        0        0      649 2023-07-05 06:53:13.387261 atro_pylog-0.1.4/pylog/settings.py
--rw-r--r--   0        0        0      641 2023-07-05 20:24:18.948672 atro_pylog-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 atro_pylog-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1717 2023-07-11 20:05:26.775535 atro_pylog-0.2.0/atro_pylog/__init__.py
+-rw-r--r--   0        0        0     1050 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/level.py
+-rw-r--r--   0        0        0      363 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/logger_type.py
+-rw-r--r--   0        0        0     1096 2023-07-11 19:59:20.704545 atro_pylog-0.2.0/atro_pylog/opentelemetry_setup.py
+-rw-r--r--   0        0        0      127 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/rich_setup.py
+-rw-r--r--   0        0        0      649 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/settings.py
+-rw-r--r--   0        0        0      636 2023-07-11 20:05:06.008434 atro_pylog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 atro_pylog-0.2.0/PKG-INFO
```

### Comparing `atro_pylog-0.1.4/pylog/__init__.py` & `atro_pylog-0.2.0/atro_pylog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import sys
-import traceback
 from pathlib import Path
 
+import stackprinter
+
 sys.path.append(Path(__file__).resolve().parent.parent.as_posix())
 
-from pylog.level import level_to_str, str_to_level  # noqa E402
-from pylog.logger_type import LoggerType  # noqa E402
-from pylog.logger_type import str_to_logger_type  # noqa E402
-from pylog.opentelemetry_setup import open_telemetry_logger_setup  # noqa E402
-from pylog.rich_setup import rich_handler  # noqa E402
-from pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings  # noqa E402
+from atro_pylog.level import level_to_str, str_to_level  # noqa E402
+from atro_pylog.logger_type import LoggerType  # noqa E402
+from atro_pylog.logger_type import str_to_logger_type  # noqa E402
+from atro_pylog.opentelemetry_setup import open_telemetry_logger_setup  # noqa E402
+from atro_pylog.rich_setup import rich_handler  # noqa E402
+from atro_pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings  # noqa E402
 
 logger = logging.getLogger(__name__)
 
 
 def exception_handler(exc_type, exc_value, exc_traceback):
-    logger.critical(f"Exception: \n {str(exc_value)} \n {''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))}")
+    logger.critical(stackprinter.format(exc_value))
 
 
 def set_logger(base_settings: BaseLoggerSettings = BaseLoggerSettings(), open_telemetry_settings: OpenTelemetryLoggerSettings = OpenTelemetryLoggerSettings()):
     sys.excepthook = exception_handler
     handlers = []
 
     types = [str_to_logger_type(type.strip()) for type in base_settings.type.split(";")]
```

### Comparing `atro_pylog-0.1.4/pylog/level.py` & `atro_pylog-0.2.0/atro_pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro_pylog-0.1.4/pylog/opentelemetry_setup.py` & `atro_pylog-0.2.0/atro_pylog/opentelemetry_setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 
-from pylog.settings import OpenTelemetryLoggerSettings
+from atro_pylog.settings import OpenTelemetryLoggerSettings
 
 
 def open_telemetry_logger_setup(level: int, settings: OpenTelemetryLoggerSettings):
     trace.set_tracer_provider(TracerProvider())
     logger_provider = LoggerProvider(  # type: ignore
         resource=Resource.create(
             {
                 "service.name": settings.service_name,
                 "service.instance.id": settings.instance_id,
             },
         ),
     )
     set_logger_provider(logger_provider)
-    exporter = OTLPLogExporter(insecure=True, endpoint=settings.endpoint)
+    exporter = OTLPLogExporter(endpoint=settings.endpoint)
     logger_provider.add_log_record_processor(BatchLogRecordProcessor(exporter))
     return LoggingHandler(level=level, logger_provider=logger_provider)
```

### Comparing `atro_pylog-0.1.4/pylog/settings.py` & `atro_pylog-0.2.0/atro_pylog/settings.py`

 * *Files identical despite different names*

### Comparing `atro_pylog-0.1.4/pyproject.toml` & `atro_pylog-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "atro-pylog"
-version = "0.1.4"
+version = "0.2.0"
 description = "A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging)."
 authors = ["Atropos <pypi.rising@atro.xyz>"]
-packages = [{ include = "pylog" }]
+packages = [{ include = "atro_pylog" }]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.7,<4.0"
 rich = "*"
-opentelemetry-api = "*"
-opentelemetry-exporter-otlp-proto-http = "*"
-opentelemetry-sdk = "*"
-pydantic = "*"
-pydantic-settings = "*"
+opentelemetry-api = "^1.18.0"
+opentelemetry-exporter-otlp-proto-http = "^1.18.0"
+opentelemetry-sdk = "^1.18.0"
+pydantic = "^2.0.0"
+pydantic-settings = "^2.0.0"
 python-dotenv = "*"
-
-[tool.poetry.dev-dependencies]
-pytest = "*"
-twine = "*"
-wheel = "*"
+stackprinter = "^0.2.10"
```

### Comparing `atro_pylog-0.1.4/PKG-INFO` & `atro_pylog-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.1.4
+Version: 0.2.0
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: opentelemetry-api
-Requires-Dist: opentelemetry-exporter-otlp-proto-http
-Requires-Dist: opentelemetry-sdk
-Requires-Dist: pydantic
-Requires-Dist: pydantic-settings
+Requires-Dist: opentelemetry-api (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.18.0,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv
 Requires-Dist: rich
+Requires-Dist: stackprinter (>=0.2.10,<0.3.0)
```

