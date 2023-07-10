# Comparing `tmp/summo-0.0.4.tar.gz` & `tmp/summo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summo-0.0.4.tar", last modified: Wed Jul  5 03:07:49 2023, max compression
+gzip compressed data, was "summo-0.0.5.tar", last modified: Mon Jul 10 23:07:12 2023, max compression
```

## Comparing `summo-0.0.4.tar` & `summo-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 03:07:39.000000 summo-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-05 03:07:49.633726 summo-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-05 03:07:39.000000 summo-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-05 03:07:39.000000 summo-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:07:49.633726 summo-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/src/summo/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 03:07:39.000000 summo-0.0.4/src/summo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 03:07:39.000000 summo-0.0.4/src/summo/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/src/summo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-05 03:07:39.000000 summo-0.0.4/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 23:07:03.000000 summo-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-10 23:07:12.787935 summo-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 23:07:03.000000 summo-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-10 23:07:03.000000 summo-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:07:12.787935 summo-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/src/summo/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:07:03.000000 summo-0.0.5/src/summo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-10 23:07:03.000000 summo-0.0.5/src/summo/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/src/summo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-10 23:07:03.000000 summo-0.0.5/tests/test_summary.py
```

### Comparing `summo-0.0.4/LICENSE` & `summo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `summo-0.0.4/PKG-INFO` & `summo-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: summo
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: tests
 Provides-Extra: typing
 License-File: LICENSE
 
 # Summo
 
 Summo is a Python package to summarize a dataset information
 
@@ -40,20 +41,24 @@
     },
     "columns": {
         "a": {
             "na_count": 2,
             "na_pct": 0.4,
             "unique": False,
             "dtype": "float64",
+            "median": 2.0,
+            "mean": 1.666666, 
         },
         "b": {
             "na_count": 1,
             "na_pct": 0.2,
             "unique": False,
             "dtype": "float64",
+            "median": 5.0,
+            "mean": 5.0, 
         },
         "c": {
             "na_count": 2,
             "na_pct": 0.4,
             "unique": False,
             "dtype": "object",
         },
```

### Comparing `summo-0.0.4/README.md` & `summo-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,20 +29,24 @@
     },
     "columns": {
         "a": {
             "na_count": 2,
             "na_pct": 0.4,
             "unique": False,
             "dtype": "float64",
+            "median": 2.0,
+            "mean": 1.666666, 
         },
         "b": {
             "na_count": 1,
             "na_pct": 0.2,
             "unique": False,
             "dtype": "float64",
+            "median": 5.0,
+            "mean": 5.0, 
         },
         "c": {
             "na_count": 2,
             "na_pct": 0.4,
             "unique": False,
             "dtype": "object",
         },
```

### Comparing `summo-0.0.4/pyproject.toml` & `summo-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "summo"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 requires-python = ">=3.9"
 readme = "README.md"
 license = { text = "MIT License" }
 authors = [{ name = "Rafael Sanabria", email = "rafael.d.sanabria@gmail.com" }]
 dependencies = ["pandas >= 2.0.0"]
 classifiers = []
 
 # consider including tox, build, twine
 [project.optional-dependencies]
 dev = ["pytest >= 7.3", "black >= 23.3.0", "ruff>=0.0.275"]
+tests = ["pytest >= 7.3", "deepdiff >= 6.3.1"]
 typing = ["pandas-stubs > 2.0.0"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.black]
 line-length = 100
@@ -39,15 +40,15 @@
 legacy_tox_ini = """
   [tox]
   min_version = 4.0
   env_list = format, linter, type, py39, py310, py311
 
   [testenv]
   deps = 
-    pytest >= 7.3
+    .[tests]
   commands = pytest
 
   [testenv:format]
   skip_install = true
   deps =
     black >= 23.0
   commands = black {posargs: src tests}
```

### Comparing `summo-0.0.4/src/summo.egg-info/PKG-INFO` & `summo-0.0.5/src/summo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: summo
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: tests
 Provides-Extra: typing
 License-File: LICENSE
 
 # Summo
 
 Summo is a Python package to summarize a dataset information
 
@@ -40,20 +41,24 @@
     },
     "columns": {
         "a": {
             "na_count": 2,
             "na_pct": 0.4,
             "unique": False,
             "dtype": "float64",
+            "median": 2.0,
+            "mean": 1.666666, 
         },
         "b": {
             "na_count": 1,
             "na_pct": 0.2,
             "unique": False,
             "dtype": "float64",
+            "median": 5.0,
+            "mean": 5.0, 
         },
         "c": {
             "na_count": 2,
             "na_pct": 0.4,
             "unique": False,
             "dtype": "object",
         },
```

