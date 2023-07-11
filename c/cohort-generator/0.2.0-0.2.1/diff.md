# Comparing `tmp/cohort-generator-0.2.0.tar.gz` & `tmp/cohort-generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohort-generator-0.2.0.tar", last modified: Wed Jun 14 08:26:51 2023, max compression
+gzip compressed data, was "cohort-generator-0.2.1.tar", last modified: Tue Jul 11 14:30:33 2023, max compression
```

## Comparing `cohort-generator-0.2.0.tar` & `cohort-generator-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/cohort_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/ohdsi/cohort_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-14 08:26:29.000000 cohort-generator-0.2.0/ohdsi/cohort_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-14 08:26:29.000000 cohort-generator-0.2.0/ohdsi/cohort_generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-14 08:26:29.000000 cohort-generator-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/cohort_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/ohdsi/cohort_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-11 14:30:22.000000 cohort-generator-0.2.1/ohdsi/cohort_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-11 14:30:22.000000 cohort-generator-0.2.1/ohdsi/cohort_generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 14:30:22.000000 cohort-generator-0.2.1/setup.py
```

### Comparing `cohort-generator-0.2.0/PKG-INFO` & `cohort-generator-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohort-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
```

### Comparing `cohort-generator-0.2.0/cohort_generator.egg-info/PKG-INFO` & `cohort-generator-0.2.1/cohort_generator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohort-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
```

### Comparing `cohort-generator-0.2.0/ohdsi/cohort_generator/__init__.py` & `cohort-generator-0.2.1/ohdsi/cohort_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `cohort-generator-0.2.0/ohdsi/cohort_generator/main.py` & `cohort-generator-0.2.1/ohdsi/cohort_generator/main.py`

 * *Files identical despite different names*

### Comparing `cohort-generator-0.2.0/setup.py` & `cohort-generator-0.2.1/setup.py`

 * *Files identical despite different names*

