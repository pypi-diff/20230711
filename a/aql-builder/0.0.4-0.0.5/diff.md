# Comparing `tmp/aql-builder-0.0.4.tar.gz` & `tmp/aql-builder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aql-builder-0.0.4.tar", last modified: Tue Jul 11 03:58:24 2023, max compression
+gzip compressed data, was "aql-builder-0.0.5.tar", last modified: Tue Jul 11 04:22:35 2023, max compression
```

## Comparing `aql-builder-0.0.4.tar` & `aql-builder-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:58:24.926107 aql-builder-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)    11341 2023-07-11 02:37:58.000000 aql-builder-0.0.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     4023 2023-07-11 03:58:24.926107 aql-builder-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-11 02:37:58.000000 aql-builder-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:58:24.926107 aql-builder-0.0.4/aql_builder/
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-07-11 03:54:53.000000 aql-builder-0.0.4/aql_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5676 2023-07-11 02:37:58.000000 aql-builder-0.0.4/aql_builder/assumptions.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-11 02:37:58.000000 aql-builder-0.0.4/aql_builder/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    33010 2023-07-11 02:37:58.000000 aql-builder-0.0.4/aql_builder/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:58:24.926107 aql-builder-0.0.4/aql_builder.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4023 2023-07-11 03:58:24.000000 aql-builder-0.0.4/aql_builder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      320 2023-07-11 03:58:24.000000 aql-builder-0.0.4/aql_builder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:58:24.000000 aql-builder-0.0.4/aql_builder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-11 03:58:24.000000 aql-builder-0.0.4/aql_builder.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 03:58:24.000000 aql-builder-0.0.4/aql_builder.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:58:24.926107 aql-builder-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 03:54:53.000000 aql-builder-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:58:24.926107 aql-builder-0.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)    31554 2023-07-11 02:37:58.000000 aql-builder-0.0.4/tests/test_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:22:35.281833 aql-builder-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)    11341 2022-12-20 00:21:34.000000 aql-builder-0.0.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     4023 2023-07-11 04:22:35.281833 aql-builder-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-11 02:21:38.000000 aql-builder-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:22:35.281833 aql-builder-0.0.5/aql_builder/
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2023-07-11 04:21:43.000000 aql-builder-0.0.5/aql_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5676 2022-12-20 00:21:34.000000 aql-builder-0.0.5/aql_builder/assumptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-20 00:21:34.000000 aql-builder-0.0.5/aql_builder/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    33010 2022-12-20 00:21:34.000000 aql-builder-0.0.5/aql_builder/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:22:35.281833 aql-builder-0.0.5/aql_builder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4023 2023-07-11 04:22:35.000000 aql-builder-0.0.5/aql_builder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-11 04:22:35.000000 aql-builder-0.0.5/aql_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 04:22:35.000000 aql-builder-0.0.5/aql_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-11 04:22:35.000000 aql-builder-0.0.5/aql_builder.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 04:22:35.000000 aql-builder-0.0.5/aql_builder.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 04:22:35.281833 aql-builder-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 03:39:38.000000 aql-builder-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:22:35.281833 aql-builder-0.0.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    31554 2022-12-20 00:21:34.000000 aql-builder-0.0.5/tests/test_builder.py
```

### Comparing `aql-builder-0.0.4/LICENSE.txt` & `aql-builder-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.4/PKG-INFO` & `aql-builder-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aql-builder
-Version: 0.0.4
+Version: 0.0.5
 Summary: ArangoDB AQL builder
 Home-page: https://foss.heptapod.net/aquapenguin/aql-builder
 Maintainer: Aqua Penguin
 Maintainer-email: aqua.penguin.34@gmail.com
 Project-URL: Source, https://foss.heptapod.net/aquapenguin/aql-builder
 Project-URL: Tracker, https://foss.heptapod.net/aquapenguin/aql-builder/-/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aql-builder-0.0.4/README.md` & `aql-builder-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.4/aql_builder/__init__.py` & `aql-builder-0.0.5/aql_builder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from aql_builder import types
 
 # pylint: disable=protected-access
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 
 class _AQLBuilderMeta(type):
 
 	def __call__(cls, obj=None):
 		return types.auto_cast_token(obj)
```

### Comparing `aql-builder-0.0.4/aql_builder/assumptions.py` & `aql-builder-0.0.5/aql_builder/assumptions.py`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.4/aql_builder/types.py` & `aql-builder-0.0.5/aql_builder/types.py`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.4/aql_builder.egg-info/PKG-INFO` & `aql-builder-0.0.5/aql_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aql-builder
-Version: 0.0.4
+Version: 0.0.5
 Summary: ArangoDB AQL builder
 Home-page: https://foss.heptapod.net/aquapenguin/aql-builder
 Maintainer: Aqua Penguin
 Maintainer-email: aqua.penguin.34@gmail.com
 Project-URL: Source, https://foss.heptapod.net/aquapenguin/aql-builder
 Project-URL: Tracker, https://foss.heptapod.net/aquapenguin/aql-builder/-/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aql-builder-0.0.4/setup.py` & `aql-builder-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.4/tests/test_builder.py` & `aql-builder-0.0.5/tests/test_builder.py`

 * *Files identical despite different names*

