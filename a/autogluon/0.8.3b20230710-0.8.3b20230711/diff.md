# Comparing `tmp/autogluon-0.8.3b20230710.tar.gz` & `tmp/autogluon-0.8.3b20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.3b20230710.tar", last modified: Mon Jul 10 09:04:50 2023, max compression
+gzip compressed data, was "autogluon-0.8.3b20230711.tar", last modified: Tue Jul 11 09:04:43 2023, max compression
```

## Comparing `autogluon-0.8.3b20230710.tar` & `autogluon-0.8.3b20230711.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-10 09:04:02.000000 autogluon-0.8.3b20230710/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:04:02.000000 autogluon-0.8.3b20230710/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:50.368187 autogluon-0.8.3b20230710/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:04:50.000000 autogluon-0.8.3b20230710/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:04:43.608643 autogluon-0.8.3b20230711/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-11 09:04:43.608643 autogluon-0.8.3b20230711/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:04:43.608643 autogluon-0.8.3b20230711/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-11 09:03:55.000000 autogluon-0.8.3b20230711/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:04:43.604643 autogluon-0.8.3b20230711/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:04:43.604643 autogluon-0.8.3b20230711/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:04:43.608643 autogluon-0.8.3b20230711/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:03:55.000000 autogluon-0.8.3b20230711/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:04:43.604643 autogluon-0.8.3b20230711/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:04:43.000000 autogluon-0.8.3b20230711/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.3b20230710/PKG-INFO` & `autogluon-0.8.3b20230711/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230710
+Version: 0.8.3b20230711
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.3b20230710/setup.py` & `autogluon-0.8.3b20230711/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.3b20230710/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.3b20230711/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230710
+Version: 0.8.3b20230711
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

