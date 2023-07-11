# Comparing `tmp/dotenver-1.2.2.tar.gz` & `tmp/dotenver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenver-1.2.2.tar", last modified: Tue Jul 11 13:50:51 2023, max compression
+gzip compressed data, was "dotenver-1.3.0.tar", last modified: Tue Jul 11 14:03:38 2023, max compression
```

## Comparing `dotenver-1.2.2.tar` & `dotenver-1.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1536 2021-06-12 14:19:12.000000 dotenver-1.2.2/LICENSE
--rw-r--r--   0        0        0     2237 2023-07-11 13:46:41.246272 dotenver-1.2.2/README.rst
--rw-r--r--   0        0        0       22 2023-07-11 13:48:18.562037 dotenver-1.2.2/dotenver/__init__.py
--rw-r--r--   0        0        0     3764 2021-06-12 14:19:12.000000 dotenver-1.2.2/dotenver/cli.py
--rw-r--r--   0        0        0     8187 2021-06-12 14:19:12.000000 dotenver-1.2.2/dotenver/dotenver.py
--rw-r--r--   0        0        0     1103 2023-07-11 13:50:51.990958 dotenver-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-06-12 14:19:12.000000 dotenver-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0     8216 2023-07-11 13:46:41.247126 dotenver-1.2.2/tests/test_dotenver.py
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 dotenver-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1536 2021-06-12 14:19:12.000000 dotenver-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2237 2023-07-11 13:46:41.246272 dotenver-1.3.0/README.rst
+-rw-r--r--   0        0        0       22 2023-07-11 13:59:29.956138 dotenver-1.3.0/dotenver/__init__.py
+-rw-r--r--   0        0        0     3764 2021-06-12 14:19:12.000000 dotenver-1.3.0/dotenver/cli.py
+-rw-r--r--   0        0        0     8187 2021-06-12 14:19:12.000000 dotenver-1.3.0/dotenver/dotenver.py
+-rw-r--r--   0        0        0     1069 2023-07-11 14:03:38.653825 dotenver-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-06-12 14:19:12.000000 dotenver-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     8216 2023-07-11 13:46:41.247126 dotenver-1.3.0/tests/test_dotenver.py
+-rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 dotenver-1.3.0/PKG-INFO
```

### Comparing `dotenver-1.2.2/LICENSE` & `dotenver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.2/README.rst` & `dotenver-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.2/dotenver/cli.py` & `dotenver-1.3.0/dotenver/cli.py`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.2/dotenver/dotenver.py` & `dotenver-1.3.0/dotenver/dotenver.py`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.2/pyproject.toml` & `dotenver-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 authors = [
     { name = "Federico Jaramillo Martínez", email = "federicojaramillom@gmail.com" },
 ]
 requires-python = ">=3.7,<4.0"
 dependencies = [
-    "jinja2<4.0,>=2.0",
-    "faker<2.0,>=1.0",
-    "colorama<1.0.0,>=0.4.1",
+    "jinja2",
+    "faker",
+    "colorama",
 ]
 name = "dotenver"
-version = "1.2.2"
+version = "1.3.0"
 description = "Automatically generate .env files from .env.example template files"
 readme = "README.rst"
 keywords = [
     "dotenv",
     "template",
 ]
 classifiers = [
```

### Comparing `dotenver-1.2.2/tests/test_dotenver.py` & `dotenver-1.3.0/tests/test_dotenver.py`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.2/PKG-INFO` & `dotenver-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dotenver
-Version: 1.2.2
+Version: 1.3.0
 Summary: Automatically generate .env files from .env.example template files
 Keywords: dotenv template
 Author-Email: Federico Jaramillo Martínez <federicojaramillom@gmail.com>
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Project-URL: Repository, https://github.com/jmfederico/dotenver
 Requires-Python: <4.0,>=3.7
-Requires-Dist: jinja2<4.0,>=2.0
-Requires-Dist: faker<2.0,>=1.0
-Requires-Dist: colorama<1.0.0,>=0.4.1
+Requires-Dist: jinja2
+Requires-Dist: faker
+Requires-Dist: colorama
 Description-Content-Type: text/x-rst
 
 ============================
 Python DotEnver
 ============================
 
 .. image:: https://badge.fury.io/py/dotenver.svg
```

