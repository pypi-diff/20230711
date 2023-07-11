# Comparing `tmp/fastchecks-0.1.0rc7.tar.gz` & `tmp/fastchecks-0.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0rc7.tar", max compression
+gzip compressed data, was "fastchecks-0.1.0rc8.tar", max compression
```

## Comparing `fastchecks-0.1.0rc7.tar` & `fastchecks-0.1.0rc8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4889 2023-07-11 10:14:23.709259 fastchecks-0.1.0rc7/README.md
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc7/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc7/fastchecks/check.py
--rw-r--r--   0        0        0    11388 2023-07-11 10:09:09.131089 fastchecks-0.1.0rc7/fastchecks/cli.py
--rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc7/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc7/fastchecks/log.py
--rw-r--r--   0        0        0      892 2023-07-11 10:03:13.456792 fastchecks-0.1.0rc7/fastchecks/meta.py
--rw-r--r--   0        0        0     6958 2023-07-11 09:12:31.873884 fastchecks-0.1.0rc7/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc7/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc7/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc7/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc7/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc7/fastchecks/vutil.py
--rw-r--r--   0        0        0     1963 2023-07-11 10:15:39.403127 fastchecks-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0     4889 2023-07-11 10:14:23.709259 fastchecks-0.1.0rc8/README.md
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc8/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc8/fastchecks/check.py
+-rw-r--r--   0        0        0    11388 2023-07-11 10:09:09.131089 fastchecks-0.1.0rc8/fastchecks/cli.py
+-rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc8/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc8/fastchecks/log.py
+-rw-r--r--   0        0        0      892 2023-07-11 10:03:13.456792 fastchecks-0.1.0rc8/fastchecks/meta.py
+-rw-r--r--   0        0        0     6992 2023-07-11 10:23:34.114164 fastchecks-0.1.0rc8/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc8/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc8/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc8/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc8/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc8/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1963 2023-07-11 10:24:39.451237 fastchecks-0.1.0rc8/pyproject.toml
+-rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc8/PKG-INFO
```

### Comparing `fastchecks-0.1.0rc7/README.md` & `fastchecks-0.1.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/__init__.py` & `fastchecks-0.1.0rc8/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/check.py` & `fastchecks-0.1.0rc8/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/cli.py` & `fastchecks-0.1.0rc8/fastchecks/cli.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/conf.py` & `fastchecks-0.1.0rc8/fastchecks/conf.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/log.py` & `fastchecks-0.1.0rc8/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/meta.py` & `fastchecks-0.1.0rc8/fastchecks/meta.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/runner.py` & `fastchecks-0.1.0rc8/fastchecks/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
                 async with asyncio.timeout(delay=timeout_init_sec):
                     inited = await common_single_pg_datastore_init(ctx.checks._pool, timeout=timeout_init_sec)
 
                 require(inited, "The postgres database could not be initialized")
         except:
             logging.critical(
-                f"Could not initialize the postgres database after {timeout_init_sec}s -- does the DB exist?",
+                f"Could not initialize the postgres database after {timeout_init_sec}s -- does the DB exist or do you have enough permissions?",
                 exc_info=False,
             )
             await ctx.close()
             sys.exit(2)
 
         return ctx
```

### Comparing `fastchecks-0.1.0rc7/fastchecks/sockets/__init__.py` & `fastchecks-0.1.0rc8/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.1.0rc8/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/types.py` & `fastchecks-0.1.0rc8/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/util.py` & `fastchecks-0.1.0rc8/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/fastchecks/vutil.py` & `fastchecks-0.1.0rc8/fastchecks/vutil.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc7/pyproject.toml` & `fastchecks-0.1.0rc8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.1.0-rc.7"
+version = "0.1.0-rc.8"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
```

### Comparing `fastchecks-0.1.0rc7/PKG-INFO` & `fastchecks-0.1.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.1.0rc7
+Version: 0.1.0rc8
 Summary: 🚥 Fast website monitoring backend service
 Home-page: https://github.com/juanmirocks/fastchecks
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

