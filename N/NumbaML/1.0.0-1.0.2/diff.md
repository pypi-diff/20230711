# Comparing `tmp/NumbaML-1.0.0.tar.gz` & `tmp/NumbaML-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NumbaML-1.0.0.tar", last modified: Fri Jul  7 11:40:51 2023, max compression
+gzip compressed data, was "NumbaML-1.0.2.tar", last modified: Tue Jul 11 06:36:17 2023, max compression
```

## Comparing `NumbaML-1.0.0.tar` & `NumbaML-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:40:51.376962 NumbaML-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:40:51.376962 NumbaML-1.0.0/NumbaML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-07 11:40:51.000000 NumbaML-1.0.0/NumbaML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-07 11:40:51.000000 NumbaML-1.0.0/NumbaML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:40:51.000000 NumbaML-1.0.0/NumbaML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 11:40:51.000000 NumbaML-1.0.0/NumbaML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 11:40:51.000000 NumbaML-1.0.0/NumbaML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-07 11:40:51.376962 NumbaML-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-07 11:40:41.000000 NumbaML-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:40:51.376962 NumbaML-1.0.0/numbaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-07 11:40:41.000000 NumbaML-1.0.0/numbaml/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:40:51.376962 NumbaML-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-07 11:40:41.000000 NumbaML-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:40:51.376962 NumbaML-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-07 11:40:41.000000 NumbaML-1.0.0/tests/test_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-07 11:40:41.000000 NumbaML-1.0.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 11:40:41.000000 NumbaML-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/NumbaML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-11 06:36:17.285541 NumbaML-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-11 06:36:05.000000 NumbaML-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/numbaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:36:17.285541 NumbaML-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 06:36:05.000000 NumbaML-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-11 06:36:05.000000 NumbaML-1.0.2/tests/test_linear_model.py
```

### Comparing `NumbaML-1.0.0/NumbaML.egg-info/PKG-INFO` & `NumbaML-1.0.2/NumbaML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumbaML
-Version: 1.0.0
+Version: 1.0.2
 Summary: Linear regression with Numba
 Home-page: https://github.com/jcatankard/NumbaML
 Author: Josh Tankard
 Description-Content-Type: text/markdown
 
 # Regression modelling with Numba
```

### Comparing `NumbaML-1.0.0/PKG-INFO` & `NumbaML-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumbaML
-Version: 1.0.0
+Version: 1.0.2
 Summary: Linear regression with Numba
 Home-page: https://github.com/jcatankard/NumbaML
 Author: Josh Tankard
 Description-Content-Type: text/markdown
 
 # Regression modelling with Numba
```

### Comparing `NumbaML-1.0.0/README.md` & `NumbaML-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.0/numbaml/confidence_intervals.py` & `NumbaML-1.0.2/numbaml/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.0/numbaml/fit.py` & `NumbaML-1.0.2/numbaml/fit.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.0/numbaml/linear_model.py` & `NumbaML-1.0.2/numbaml/linear_model.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.0/numbaml/metrics.py` & `NumbaML-1.0.2/numbaml/metrics.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.0/numbaml/model_selection.py` & `NumbaML-1.0.2/numbaml/model_selection.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.0/numbaml/scoring.py` & `NumbaML-1.0.2/numbaml/scoring.py`

 * *Files identical despite different names*

