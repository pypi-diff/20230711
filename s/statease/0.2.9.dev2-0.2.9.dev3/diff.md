# Comparing `tmp/statease-0.2.9.dev2.tar.gz` & `tmp/statease-0.2.9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statease-0.2.9.dev2.tar", last modified: Tue Jul 11 15:52:16 2023, max compression
+gzip compressed data, was "statease-0.2.9.dev3.tar", last modified: Tue Jul 11 15:57:20 2023, max compression
```

## Comparing `statease-0.2.9.dev2.tar` & `statease-0.2.9.dev3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/statease/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/row_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/statease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:20.009617 statease-0.2.9.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-11 15:57:20.009617 statease-0.2.9.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:57:20.009617 statease-0.2.9.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:20.009617 statease-0.2.9.dev3/statease/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/row_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-11 15:57:00.000000 statease-0.2.9.dev3/statease/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:20.009617 statease-0.2.9.dev3/statease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-11 15:57:20.000000 statease-0.2.9.dev3/statease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-11 15:57:20.000000 statease-0.2.9.dev3/statease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:57:20.000000 statease-0.2.9.dev3/statease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:57:20.000000 statease-0.2.9.dev3/statease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 15:57:20.000000 statease-0.2.9.dev3/statease.egg-info/top_level.txt
```

### Comparing `statease-0.2.9.dev2/LICENSE` & `statease-0.2.9.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/PKG-INFO` & `statease-0.2.9.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statease
-Version: 0.2.9.dev2
+Version: 0.2.9.dev3
 Summary:  Python interface to Stat-Ease 360.
 Home-page: https://statease.com/docs/se360/python-integration/
 Author: Stat-Ease, Inc.
 Author-email: support@statease.com
 License: Other/Proprietary License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `statease-0.2.9.dev2/setup.py` & `statease-0.2.9.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.2.9.dev2'
+VERSION = '0.2.9.dev3'
 DOCLINES = (__doc__ or '').split("\n")
 
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Manufacturing",
     "Intended Audience :: End Users/Desktop",
```

### Comparing `statease-0.2.9.dev2/statease/analysis.py` & `statease-0.2.9.dev3/statease/analysis.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease/client.py` & `statease-0.2.9.dev3/statease/client.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease/factor.py` & `statease-0.2.9.dev3/statease/factor.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease/information.py` & `statease-0.2.9.dev3/statease/information.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease/node.py` & `statease-0.2.9.dev3/statease/node.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease/optimizer.py` & `statease-0.2.9.dev3/statease/optimizer.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease/response.py` & `statease-0.2.9.dev3/statease/response.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.9.dev2/statease.egg-info/PKG-INFO` & `statease-0.2.9.dev3/statease.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statease
-Version: 0.2.9.dev2
+Version: 0.2.9.dev3
 Summary:  Python interface to Stat-Ease 360.
 Home-page: https://statease.com/docs/se360/python-integration/
 Author: Stat-Ease, Inc.
 Author-email: support@statease.com
 License: Other/Proprietary License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

