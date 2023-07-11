# Comparing `tmp/cereslib-0.4.1rc1.tar.gz` & `tmp/cereslib-0.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cereslib-0.4.1rc1.tar", max compression
+gzip compressed data, was "cereslib-0.4.2rc1.tar", max compression
```

## Comparing `cereslib-0.4.1rc1.tar` & `cereslib-0.4.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      130 2023-06-22 07:45:10.855428 cereslib-0.4.1rc1/AUTHORS
--rw-r--r--   0        0        0     7651 2023-06-22 07:45:10.855428 cereslib-0.4.1rc1/LICENSE
--rw-r--r--   0        0        0     1544 2023-06-22 07:45:10.855428 cereslib-0.4.1rc1/NEWS
--rw-r--r--   0        0        0     4872 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/README.md
--rw-r--r--   0        0        0      759 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/__init__.py
--rw-r--r--   0        0        0       91 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/_version.py
--rw-r--r--   0        0        0        0 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/dfutils/__init__.py
--rw-r--r--   0        0        0     2586 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/dfutils/filter.py
--rw-r--r--   0        0        0     3595 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/dfutils/format.py
--rw-r--r--   0        0        0        0 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/enrich/__init__.py
--rw-r--r--   0        0        0    31880 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/enrich/enrich.py
--rw-r--r--   0        0        0        0 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/events/__init__.py
--rw-r--r--   0        0        0    34868 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/cereslib/events/events.py
--rw-r--r--   0        0        0     1359 2023-06-22 07:45:10.859429 cereslib-0.4.1rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/__init__.py
--rw-r--r--   0        0        0      379 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/enrich/authors.csv
--rw-r--r--   0        0        0      106 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/enrich/onion.csv
--rw-r--r--   0        0        0      111 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/enrich/pairprogramming.csv
--rw-r--r--   0        0        0      292 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/enrich/timedifference.csv
--rw-r--r--   0        0        0      610 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/enrich/uuids.csv
--rw-r--r--   0        0        0     9538 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/events/git.json
--rw-r--r--   0        0        0       97 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/data/projects_map.json
--rw-r--r--   0        0        0     3904 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/manual_test_events.py
--rwxr-xr-x   0        0        0     1075 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/run_tests.py
--rw-r--r--   0        0        0    11014 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/test_enrich.py
--rw-r--r--   0        0        0     2433 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/test_filter.py
--rw-r--r--   0        0        0     1894 2023-06-22 07:45:10.863429 cereslib-0.4.1rc1/tests/test_format.py
--rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 cereslib-0.4.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-07-11 14:01:44.413792 cereslib-0.4.2rc1/AUTHORS
+-rw-r--r--   0        0        0     7651 2023-07-11 14:01:44.413792 cereslib-0.4.2rc1/LICENSE
+-rw-r--r--   0        0        0     1624 2023-07-11 14:01:44.413792 cereslib-0.4.2rc1/NEWS
+-rw-r--r--   0        0        0     4872 2023-07-11 14:01:44.413792 cereslib-0.4.2rc1/README.md
+-rw-r--r--   0        0        0      759 2023-07-11 14:01:44.413792 cereslib-0.4.2rc1/cereslib/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/_version.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/dfutils/__init__.py
+-rw-r--r--   0        0        0     2586 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/dfutils/filter.py
+-rw-r--r--   0        0        0     3595 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/dfutils/format.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/enrich/__init__.py
+-rw-r--r--   0        0        0    31880 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/enrich/enrich.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/events/__init__.py
+-rw-r--r--   0        0        0    34868 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/cereslib/events/events.py
+-rw-r--r--   0        0        0     1359 2023-07-11 14:01:44.417792 cereslib-0.4.2rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/__init__.py
+-rw-r--r--   0        0        0      379 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/enrich/authors.csv
+-rw-r--r--   0        0        0      106 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/enrich/onion.csv
+-rw-r--r--   0        0        0      111 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/enrich/pairprogramming.csv
+-rw-r--r--   0        0        0      292 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/enrich/timedifference.csv
+-rw-r--r--   0        0        0      610 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/enrich/uuids.csv
+-rw-r--r--   0        0        0     9538 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/events/git.json
+-rw-r--r--   0        0        0       97 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/data/projects_map.json
+-rw-r--r--   0        0        0     3904 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/manual_test_events.py
+-rwxr-xr-x   0        0        0     1075 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    11014 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/test_enrich.py
+-rw-r--r--   0        0        0     2433 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/test_filter.py
+-rw-r--r--   0        0        0     1894 2023-07-11 14:01:44.421793 cereslib-0.4.2rc1/tests/test_format.py
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 cereslib-0.4.2rc1/PKG-INFO
```

### Comparing `cereslib-0.4.1rc1/LICENSE` & `cereslib-0.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/NEWS` & `cereslib-0.4.2rc1/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## cereslib 0.4.1 - (2023-06-28)
+  
+  * Update Poetry's package dependencies
+
 ## cereslib 0.4.0 - (2023-04-21)
 
 **New features:**
 
  * Support for more languages and file types\
    The library is able to detect the new file formats and language
    formats. This list includes JavaScript, TypeScript, Terraform, among
```

### Comparing `cereslib-0.4.1rc1/README.md` & `cereslib-0.4.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/cereslib/__init__.py` & `cereslib-0.4.2rc1/cereslib/__init__.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/cereslib/dfutils/filter.py` & `cereslib-0.4.2rc1/cereslib/dfutils/filter.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/cereslib/dfutils/format.py` & `cereslib-0.4.2rc1/cereslib/dfutils/format.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/cereslib/enrich/enrich.py` & `cereslib-0.4.2rc1/cereslib/enrich/enrich.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/cereslib/events/events.py` & `cereslib-0.4.2rc1/cereslib/events/events.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/pyproject.toml` & `cereslib-0.4.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cereslib"
-version = "0.4.1-rc.1"
+version = "0.4.2-rc.1"
 description = "GrimoireLab: Unify, eventize and enrich information from Perceval"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `cereslib-0.4.1rc1/tests/data/enrich/uuids.csv` & `cereslib-0.4.2rc1/tests/data/enrich/uuids.csv`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/tests/data/events/git.json` & `cereslib-0.4.2rc1/tests/data/events/git.json`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/tests/manual_test_events.py` & `cereslib-0.4.2rc1/tests/manual_test_events.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/tests/run_tests.py` & `cereslib-0.4.2rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/tests/test_enrich.py` & `cereslib-0.4.2rc1/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/tests/test_filter.py` & `cereslib-0.4.2rc1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/tests/test_format.py` & `cereslib-0.4.2rc1/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.4.1rc1/PKG-INFO` & `cereslib-0.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cereslib
-Version: 0.4.1rc1
+Version: 0.4.2rc1
 Summary: GrimoireLab: Unify, eventize and enrich information from Perceval
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

