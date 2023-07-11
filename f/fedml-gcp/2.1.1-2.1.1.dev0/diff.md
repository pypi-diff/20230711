# Comparing `tmp/fedml_gcp-2.1.1.tar.gz` & `tmp/fedml_gcp-2.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_gcp-2.1.1.tar", last modified: Tue Jul 11 18:58:06 2023, max compression
+gzip compressed data, was "fedml_gcp-2.1.1.dev0.tar", last modified: Wed Jun 21 18:24:58 2023, max compression
```

## Comparing `fedml_gcp-2.1.1.tar` & `fedml_gcp-2.1.1.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 18:58:06.138666 fedml_gcp-2.1.1/
--rw-r--r--   0 I542957    (501) staff       (20)     1271 2023-07-11 18:58:06.137972 fedml_gcp-2.1.1/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      900 2023-07-10 19:16:51.000000 fedml_gcp-2.1.1/README.md
--rw-r--r--   0 I542957    (501) staff       (20)      103 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/pyproject.toml
--rw-r--r--   0 I542957    (501) staff       (20)       38 2023-07-11 18:58:06.138851 fedml_gcp-2.1.1/setup.cfg
--rw-r--r--   0 I542957    (501) staff       (20)     1065 2023-07-11 18:56:37.000000 fedml_gcp-2.1.1/setup.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 18:58:06.062283 fedml_gcp-2.1.1/src/
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 18:58:06.121549 fedml_gcp-2.1.1/src/fedml_gcp/
--rw-r--r--   0 I542957    (501) staff       (20)      118 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/__init__.py
--rw-r--r--   0 I542957    (501) staff       (20)      808 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/build_and_push.sh
--rw-r--r--   0 I542957    (501) staff       (20)    15864 2023-07-10 19:16:51.000000 fedml_gcp-2.1.1/src/fedml_gcp/dbconnection.py
--rw-r--r--   0 I542957    (501) staff       (20)     9433 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/dwcgcp.py
--rw-r--r--   0 I542957    (501) staff       (20)      199 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/install_kubectl.sh
--rw-r--r--   0 I542957    (501) staff       (20)      656 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/logger.py
--rw-r--r--   0 I542957    (501) staff       (20)      393 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/model.py
--rw-r--r--   0 I542957    (501) staff       (20)     8470 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1/src/fedml_gcp/script_generator.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 18:58:06.136708 fedml_gcp-2.1.1/src/fedml_gcp.egg-info/
--rw-r--r--   0 I542957    (501) staff       (20)     1271 2023-07-11 18:58:06.000000 fedml_gcp-2.1.1/src/fedml_gcp.egg-info/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      443 2023-07-11 18:58:06.000000 fedml_gcp-2.1.1/src/fedml_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 I542957    (501) staff       (20)        1 2023-07-11 18:58:06.000000 fedml_gcp-2.1.1/src/fedml_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 I542957    (501) staff       (20)       67 2023-07-11 18:58:06.000000 fedml_gcp-2.1.1/src/fedml_gcp.egg-info/requires.txt
--rw-r--r--   0 I542957    (501) staff       (20)       10 2023-07-11 18:58:06.000000 fedml_gcp-2.1.1/src/fedml_gcp.egg-info/top_level.txt
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-21 18:24:58.624422 fedml_gcp-2.1.1.dev0/
+-rw-r--r--   0 I542957    (501) staff       (20)     1276 2023-06-21 18:24:58.622527 fedml_gcp-2.1.1.dev0/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      900 2023-06-21 18:18:57.000000 fedml_gcp-2.1.1.dev0/README.md
+-rw-r--r--   0 I542957    (501) staff       (20)      103 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/pyproject.toml
+-rw-r--r--   0 I542957    (501) staff       (20)       38 2023-06-21 18:24:58.624606 fedml_gcp-2.1.1.dev0/setup.cfg
+-rw-r--r--   0 I542957    (501) staff       (20)     1070 2023-06-21 18:21:23.000000 fedml_gcp-2.1.1.dev0/setup.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-21 18:24:58.596445 fedml_gcp-2.1.1.dev0/src/
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-21 18:24:58.605857 fedml_gcp-2.1.1.dev0/src/fedml_gcp/
+-rw-r--r--   0 I542957    (501) staff       (20)      118 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/__init__.py
+-rw-r--r--   0 I542957    (501) staff       (20)      808 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/build_and_push.sh
+-rw-r--r--   0 I542957    (501) staff       (20)    15864 2023-06-21 18:19:15.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/dbconnection.py
+-rw-r--r--   0 I542957    (501) staff       (20)     9433 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/dwcgcp.py
+-rw-r--r--   0 I542957    (501) staff       (20)      199 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/install_kubectl.sh
+-rw-r--r--   0 I542957    (501) staff       (20)      656 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/logger.py
+-rw-r--r--   0 I542957    (501) staff       (20)      393 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/model.py
+-rw-r--r--   0 I542957    (501) staff       (20)     8470 2023-03-13 18:48:47.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp/script_generator.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-21 18:24:58.619759 fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/
+-rw-r--r--   0 I542957    (501) staff       (20)     1276 2023-06-21 18:24:58.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      443 2023-06-21 18:24:58.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 I542957    (501) staff       (20)        1 2023-06-21 18:24:58.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       67 2023-06-21 18:24:58.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/requires.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       10 2023-06-21 18:24:58.000000 fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/top_level.txt
```

### Comparing `fedml_gcp-2.1.1/PKG-INFO` & `fedml_gcp-2.1.1.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml_gcp
-Version: 2.1.1
+Version: 2.1.1.dev0
 Summary: A python library for building machine learning models on Google Cloud Platform using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_gcp-2.1.1/README.md` & `fedml_gcp-2.1.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `fedml_gcp-2.1.1/setup.py` & `fedml_gcp-2.1.1.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setuptools.setup(
     name="fedml_gcp",
-    version="2.1.1",
+    version="2.1.1.dev0",
     author="SAP SE",
     description="A python library for building machine learning models on Google Cloud Platform using a federated data source",
     license='Apache License 2.0',
     license_files=['LICENSE.txt'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `fedml_gcp-2.1.1/src/fedml_gcp/build_and_push.sh` & `fedml_gcp-2.1.1.dev0/src/fedml_gcp/build_and_push.sh`

 * *Files identical despite different names*

### Comparing `fedml_gcp-2.1.1/src/fedml_gcp/dbconnection.py` & `fedml_gcp-2.1.1.dev0/src/fedml_gcp/dbconnection.py`

 * *Files identical despite different names*

### Comparing `fedml_gcp-2.1.1/src/fedml_gcp/dwcgcp.py` & `fedml_gcp-2.1.1.dev0/src/fedml_gcp/dwcgcp.py`

 * *Files identical despite different names*

### Comparing `fedml_gcp-2.1.1/src/fedml_gcp/logger.py` & `fedml_gcp-2.1.1.dev0/src/fedml_gcp/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_gcp-2.1.1/src/fedml_gcp/script_generator.py` & `fedml_gcp-2.1.1.dev0/src/fedml_gcp/script_generator.py`

 * *Files identical despite different names*

### Comparing `fedml_gcp-2.1.1/src/fedml_gcp.egg-info/PKG-INFO` & `fedml_gcp-2.1.1.dev0/src/fedml_gcp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml-gcp
-Version: 2.1.1
+Version: 2.1.1.dev0
 Summary: A python library for building machine learning models on Google Cloud Platform using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

