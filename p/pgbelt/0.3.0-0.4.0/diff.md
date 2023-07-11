# Comparing `tmp/pgbelt-0.3.0.tar.gz` & `tmp/pgbelt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgbelt-0.3.0.tar", max compression
+gzip compressed data, was "pgbelt-0.4.0.tar", max compression
```

## Comparing `pgbelt-0.3.0.tar` & `pgbelt-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10758 2023-06-29 22:26:55.117648 pgbelt-0.3.0/LICENSE
--rw-r--r--   0        0        0     2047 2023-06-29 22:26:55.117648 pgbelt-0.3.0/README.md
--rw-r--r--   0        0        0      137 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/__init__.py
--rw-r--r--   0        0        0      462 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/__init__.py
--rw-r--r--   0        0        0     5849 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/convenience.py
--rw-r--r--   0        0        0     5292 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/helpers.py
--rw-r--r--   0        0        0     3043 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/login.py
--rw-r--r--   0        0        0     8215 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/preflight.py
--rw-r--r--   0        0        0     3148 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/schema.py
--rw-r--r--   0        0        0     5082 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/setup.py
--rw-r--r--   0        0        0     3190 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/status.py
--rw-r--r--   0        0        0     8080 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/sync.py
--rw-r--r--   0        0        0     3754 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/cmd/teardown.py
--rw-r--r--   0        0        0       35 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/config/__init__.py
--rw-r--r--   0        0        0     3817 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/config/config.py
--rw-r--r--   0        0        0     5421 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/config/models.py
--rw-r--r--   0        0        0     5247 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/config/remote.py
--rw-r--r--   0        0        0      186 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/main.py
--rw-r--r--   0        0        0       40 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/util/__init__.py
--rw-r--r--   0        0        0      583 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/util/asyncfuncs.py
--rw-r--r--   0        0        0     9698 2023-06-29 22:26:55.121648 pgbelt-0.3.0/pgbelt/util/dump.py
--rw-r--r--   0        0        0     1424 2023-06-29 22:26:55.125648 pgbelt-0.3.0/pgbelt/util/logs.py
--rw-r--r--   0        0        0    12313 2023-06-29 22:26:55.125648 pgbelt-0.3.0/pgbelt/util/pglogical.py
--rw-r--r--   0        0        0    13669 2023-06-29 22:26:55.125648 pgbelt-0.3.0/pgbelt/util/postgres.py
--rw-r--r--   0        0        0     1202 2023-06-29 22:26:55.125648 pgbelt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 pgbelt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-07-11 01:37:54.668294 pgbelt-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2047 2023-07-11 01:37:54.668294 pgbelt-0.4.0/README.md
+-rw-r--r--   0        0        0      137 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/__init__.py
+-rw-r--r--   0        0        0      462 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/__init__.py
+-rw-r--r--   0        0        0     5849 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/convenience.py
+-rw-r--r--   0        0        0     5292 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/helpers.py
+-rw-r--r--   0        0        0     3043 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/login.py
+-rw-r--r--   0        0        0     8215 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/preflight.py
+-rw-r--r--   0        0        0     3148 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/schema.py
+-rw-r--r--   0        0        0     5082 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/setup.py
+-rw-r--r--   0        0        0     3190 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/status.py
+-rw-r--r--   0        0        0     8080 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/sync.py
+-rw-r--r--   0        0        0     3754 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/cmd/teardown.py
+-rw-r--r--   0        0        0       35 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/config/__init__.py
+-rw-r--r--   0        0        0     3817 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/config/config.py
+-rw-r--r--   0        0        0     5421 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/config/models.py
+-rw-r--r--   0        0        0     5247 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/config/remote.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/main.py
+-rw-r--r--   0        0        0       40 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/util/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/util/asyncfuncs.py
+-rw-r--r--   0        0        0     9698 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/util/dump.py
+-rw-r--r--   0        0        0     1699 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/util/logs.py
+-rw-r--r--   0        0        0    12313 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/util/pglogical.py
+-rw-r--r--   0        0        0    13669 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pgbelt/util/postgres.py
+-rw-r--r--   0        0        0     1202 2023-07-11 01:37:54.672294 pgbelt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 pgbelt-0.4.0/PKG-INFO
```

### Comparing `pgbelt-0.3.0/LICENSE` & `pgbelt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/README.md` & `pgbelt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/convenience.py` & `pgbelt-0.4.0/pgbelt/cmd/convenience.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/helpers.py` & `pgbelt-0.4.0/pgbelt/cmd/helpers.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/login.py` & `pgbelt-0.4.0/pgbelt/cmd/login.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/preflight.py` & `pgbelt-0.4.0/pgbelt/cmd/preflight.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/schema.py` & `pgbelt-0.4.0/pgbelt/cmd/schema.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/setup.py` & `pgbelt-0.4.0/pgbelt/cmd/setup.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/status.py` & `pgbelt-0.4.0/pgbelt/cmd/status.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/sync.py` & `pgbelt-0.4.0/pgbelt/cmd/sync.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/cmd/teardown.py` & `pgbelt-0.4.0/pgbelt/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/config/config.py` & `pgbelt-0.4.0/pgbelt/config/config.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/config/models.py` & `pgbelt-0.4.0/pgbelt/config/models.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/config/remote.py` & `pgbelt-0.4.0/pgbelt/config/remote.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/util/asyncfuncs.py` & `pgbelt-0.4.0/pgbelt/util/asyncfuncs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/util/dump.py` & `pgbelt-0.4.0/pgbelt/util/dump.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/util/logs.py` & `pgbelt-0.4.0/pgbelt/util/logs.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,29 @@
     return f"logs/{db}/{dc}/logs.txt"
 
 
 def get_logger(db: str, dc: str, kind: str = "") -> logging.Logger:
     # When we set up a logger for that db that emits to a file
     logger = logging.getLogger(f"dbup.{db}.{dc}")
     if not logger.handlers:
+        skip_file_handler = False
+
         try:
             makedirs(log_file_dir(db, dc))
         except FileExistsError:
             pass
+        # We will allow OSError (not being able to write to disk)
+        # Just don't add the File Handler
+        except OSError:
+            skip_file_handler = True
+            pass
 
-        handler = logging.FileHandler(log_file_path(db, dc), mode="w")
-        handler.setFormatter(logging.Formatter(FORMATTER, style="{"))
-        # always log everything to the file
-        logger.setLevel(logging.DEBUG)
-        logger.addHandler(handler)
+        if not skip_file_handler:
+            handler = logging.FileHandler(log_file_path(db, dc), mode="w")
+            handler.setFormatter(logging.Formatter(FORMATTER, style="{"))
+            # always log everything to the file
+            logger.setLevel(logging.DEBUG)
+            logger.addHandler(handler)
 
     # if you pass kind then you can get a logger for a specific thing,
     # and your logs will end up annotated with the kind
     return logging.getLogger(f"dbup.{db}.{dc}.{kind}") if kind else logger
```

### Comparing `pgbelt-0.3.0/pgbelt/util/pglogical.py` & `pgbelt-0.4.0/pgbelt/util/pglogical.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pgbelt/util/postgres.py` & `pgbelt-0.4.0/pgbelt/util/postgres.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.3.0/pyproject.toml` & `pgbelt-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgbelt"
-version = "0.3.0"
+version = "0.4.0"
 description = "A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication."
 authors = ["Varjitt Jeeva <varjitt.jeeva@autodesk.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pgbelt", from = "./" },
 ]
```

### Comparing `pgbelt-0.3.0/PKG-INFO` & `pgbelt-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgbelt
-Version: 0.3.0
+Version: 0.4.0
 Summary: A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.
 Author: Varjitt Jeeva
 Author-email: varjitt.jeeva@autodesk.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgbelt Version: 0.3.0 Summary: A CLI tool used to
+Metadata-Version: 2.1 Name: pgbelt Version: 0.4.0 Summary: A CLI tool used to
 manage Postgres data migrations from beginning to end, for a single database or
 a fleet, leveraging pglogical replication. Author: Varjitt Jeeva Author-email:
 varjitt.jeeva@autodesk.com Requires-Python: >=3.9 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiofiles (>=0.8,<23.2) Requires-Dist:
 asyncpg (>=0.27.0,<0.28.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-
```

