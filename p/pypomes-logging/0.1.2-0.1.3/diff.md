# Comparing `tmp/pypomes_logging-0.1.2.tar.gz` & `tmp/pypomes_logging-0.1.3.tar.gz`

## Comparing `pypomes_logging-0.1.2.tar` & `pypomes_logging-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypomes_logging-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/PKG-INFO
```

### Comparing `pypomes_logging-0.1.2/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.1.3/src/pypomes_logging/logging_pomes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,146 @@
 import logging
 import os
 import tempfile
 from datetime import datetime
 from dateutil import parser
 from io import BytesIO
 from typing import Final, TextIO
-from pypomes_core.datetime_pomes import DATETIME_FORMAT_INV
-from pypomes_core.env_pomes import APP_PREFIX, env_get_str
+from pypomes_core import APP_PREFIX, DATETIME_FORMAT_INV, env_get_str
 
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID", f"{APP_PREFIX}")
-LOGGIN_FILE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE",
-                                      os.path.join(tempfile.gettempdir(), f"{APP_PREFIX}.log"))
-LOGGING_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_MODE", "a")
+LOGGING_FORMAT: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID",
+                                         "{asctime} {levelname:1.1} {thread:5d} "
+                                         "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
+LOGGING_STYLE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_STYLE", "{")
+
+LOGGING_FILE_PATH: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_PATH",
+                                            os.path.join(tempfile.gettempdir(), f"{APP_PREFIX}.log"))
+LOGGING_FILE_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_MODE", "a")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
 match env_get_str(f"{APP_PREFIX}_LOGGING_LEVEL"):
-    case "debug":
+    case "d" | "debug":
         LOGGING_LEVEL: Final[int] = logging.DEBUG
-    case "info":
+    case "i" | "info":
         LOGGING_LEVEL: Final[int] = logging.INFO
-    case "warn":
+    case "w" | "warning":
         LOGGING_LEVEL: Final[int] = logging.WARN
-    case "error":
+    case "e" | "error":
         LOGGING_LEVEL: Final[int] = logging.ERROR
-    case _:  # "critical"
+    case "c" | "critical":
         LOGGING_LEVEL: Final[int] = logging.CRITICAL
+    case _:
+        LOGGING_LEVEL: Final[int] = logging.NOTSET
 
 logging.basicConfig(level=LOGGING_LEVEL,
-                    filename=LOGGIN_FILE,
-                    filemode=LOGGING_MODE,
+                    filename=LOGGING_FILE_PATH,
+                    filemode=LOGGING_FILE_MODE,
                     datefmt=DATETIME_FORMAT_INV,
                     style="{",
                     format="{asctime} {levelname:1.1} {thread:5d} "
                            "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
 for _handler in logging.root.handlers:
     _handler.addFilter(logging.Filter(LOGGING_ID))
 
 
-def logging_entries(errors: list[str], log_level: str, log_from: str, log_to: str) -> BytesIO:
+def logging_get_entries(errors: list[str], log_level: str, log_from: str, log_to: str) -> BytesIO:
 
     def get_level(level: str) -> int:
 
         result: int | None
         match level:
-            case None | "N" | "n":
-                result = logging.NOTSET         # 0
-            case "D" | "d":
+            case "d" | "debug":
                 result = logging.DEBUG          # 10
-            case "I" | "i":
+            case "i" | "info":
                 result = logging.INFO           # 20
-            case "W" | "w":
+            case "w" | "warning":
                 result = logging.WARN           # 30
-            case "E" | "e":
+            case "e" | "error":
                 result = logging.ERROR          # 40
-            case "C" | "c":
+            case "c" | "critical":
                 result = logging.CRITICAL       # 50
             case _:
-                result = None
+                result = logging.NOTSET         # 0
 
         return result
 
     # inicializa variável de retorno
     result: BytesIO | None = None
 
-    # oobtem o nível de log
+    # obtain the logging level
     logging_level: int = get_level(log_level)
-    if log_level is None:
-        errors.append(f"Valor '{log_level}' do atributo 'level' inválido")
 
-    # obtem a estampa inicial
+    # obtain the initial timestap
     from_stamp: datetime | None = None
     if log_from is not None:
         from_stamp = parser.parse(log_from)
         if from_stamp is None:
-            errors.append(f"Valor '{from_stamp}' do atributo 'from' inválido")
+            errors.append(f"Value '{from_stamp}' of 'from' attribute invalid")
 
-    # obtem a estampa final
+    # obtaind the final timestamp
     to_stamp: datetime | None = None
     if log_to is not None:
         to_stamp = parser.parse(log_to)
         if to_stamp is None or \
            (from_stamp is not None and from_stamp > to_stamp):
-            errors.append(f"Valor '{to_stamp}' do atributo 'to' inválido")
+            errors.append(f"Value '{to_stamp}' of 'to' attribute invalid")
 
-    # o arquivo de log existe ?
-    if not os.path.exists(LOGGIN_FILE):
-        # não, reporte o erro
-        errors.append(f"Arquivo '{LOGGIN_FILE}' não encontrado")
+    # does the log file exist ?
+    if not os.path.exists(LOGGING_FILE_PATH):
+        # no, report the error
+        errors.append(f"File '{LOGGING_FILE_PATH}' not found")
 
-    # houve erro ?
+    # any error ?
     if len(errors) == 0:
-        # não, prossiga
+        # no, proceed
         result = BytesIO()
-        with open(LOGGIN_FILE, "r") as f:
+        with open(LOGGING_FILE_PATH, "r") as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(maxsplit=3)
                 level: int = get_level(items[2])
                 if level >= logging_level:
                     timestamp: datetime = parser.parse(f"{items[0]} {items[1]}")
                     if (from_stamp is None or timestamp >= from_stamp) and \
                        (to_stamp is None or timestamp <= to_stamp):
                         result.write(line.encode())
                 line = f.readline()
 
     return result
 
 
-def log_errors(errors: list[str], output_dev: TextIO = None):
+def logging_log_msgs(msgs: list[str], log_level: str = None, output_dev: TextIO = None):
     """
-    Escreve no *logger*, e opcionalmente, em *output_dev*
-    (tipicamente, *sys.stdout* ou *sys.stderr*), os erros em *errors*.
+    Write messages in *msgs* to *PYPOMES_LOGGER*, and to *output_dev*
+    (tipically, *sys.stdout* ou *sys.stderr*).
 
-    :param errors: a lista de erros
-    :param output_dev: dispositivo de saída onde o erro deve ser impresso
+    :param msgs: the messages list
+    :param log_level: the logging level (None for no log printing)
+    :param output_dev: output device where the message is to be printed (None for no device printing)
     """
-    # percorre a lista de erros
-    for error in errors:
-        # escreve o erro no log
-        PYPOMES_LOGGER.error(error)
+    # traverse the messages list
+    for msg in msgs:
+        # write the message
+        match log_level:
+            case "c" | "critical":
+                PYPOMES_LOGGER.critical(msg)
+            case "d" | "debug":
+                PYPOMES_LOGGER.debug(msg)
+            case "i" | "info":
+                PYPOMES_LOGGER.info(msg)
+            case "w" | "warning":
+                PYPOMES_LOGGER.warning(msg)
+            case "e" | "error":
+                PYPOMES_LOGGER.error(msg)
 
         # o dispositivo de saída foi definido ?
         if output_dev is not None:
             # sim, escreva o erro nesse dispositivo
-            output_dev.write(error)
+            output_dev.write(msg)
 
             # o dispositivo de saída é 'stderr' ou 'stdout' ?
             if output_dev.name.startswith("<std"):
                 # sim, mude de linha
                 output_dev.write("\n")
```

### Comparing `pypomes_logging-0.1.2/LICENSE` & `pypomes_logging-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.1.2/pyproject.toml` & `pypomes_logging-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.1.2",
-    "pypomes_core>=0.1.2",
+    "pypomes_core>=0.1.4",
     "python-dateutil>=2.8.2",
     "setuptools>=68.0.0",
     "wheel>=0.40.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Logging"
```

### Comparing `pypomes_logging-0.1.2/PKG-INFO` & `pypomes_logging-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_logging
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.1.2
+Requires-Dist: pypomes-core>=0.1.4
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.40.0
```

