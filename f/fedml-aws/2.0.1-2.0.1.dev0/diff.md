# Comparing `tmp/fedml_aws-2.0.1.tar.gz` & `tmp/fedml_aws-2.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_aws-2.0.1.tar", last modified: Tue Jul 11 19:01:50 2023, max compression
+gzip compressed data, was "fedml_aws-2.0.1.dev0.tar", last modified: Wed Jul  5 22:02:52 2023, max compression
```

## Comparing `fedml_aws-2.0.1.tar` & `fedml_aws-2.0.1.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 19:01:50.370869 fedml_aws-2.0.1/
--rw-r--r--   0 I542957    (501) staff       (20)     1252 2023-07-11 19:01:50.370195 fedml_aws-2.0.1/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      889 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/README.md
--rw-r--r--   0 I542957    (501) staff       (20)      103 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/pyproject.toml
--rw-r--r--   0 I542957    (501) staff       (20)       38 2023-07-11 19:01:50.371042 fedml_aws-2.0.1/setup.cfg
--rw-r--r--   0 I542957    (501) staff       (20)      938 2023-07-11 19:01:37.000000 fedml_aws-2.0.1/setup.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 19:01:50.343693 fedml_aws-2.0.1/src/
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 19:01:50.352469 fedml_aws-2.0.1/src/fedml_aws/
--rw-r--r--   0 I542957    (501) staff       (20)      175 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/__init__.py
--rw-r--r--   0 I542957    (501) staff       (20)     2352 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/build_and_push.sh
--rw-r--r--   0 I542957    (501) staff       (20)    15864 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/dbconnection.py
--rw-r--r--   0 I542957    (501) staff       (20)    22560 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/dwcsagemaker.py
--rw-r--r--   0 I542957    (501) staff       (20)      199 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/install_kubectl.sh
--rw-r--r--   0 I542957    (501) staff       (20)      656 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/logger.py
--rw-r--r--   0 I542957    (501) staff       (20)     4647 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/predictor.py
--rw-r--r--   0 I542957    (501) staff       (20)    16482 2023-07-11 19:00:23.000000 fedml_aws-2.0.1/src/fedml_aws/script_generator.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-11 19:01:50.368876 fedml_aws-2.0.1/src/fedml_aws.egg-info/
--rw-r--r--   0 I542957    (501) staff       (20)     1252 2023-07-11 19:01:50.000000 fedml_aws-2.0.1/src/fedml_aws.egg-info/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      467 2023-07-11 19:01:50.000000 fedml_aws-2.0.1/src/fedml_aws.egg-info/SOURCES.txt
--rw-r--r--   0 I542957    (501) staff       (20)        1 2023-07-11 19:01:50.000000 fedml_aws-2.0.1/src/fedml_aws.egg-info/dependency_links.txt
--rw-r--r--   0 I542957    (501) staff       (20)       36 2023-07-11 19:01:50.000000 fedml_aws-2.0.1/src/fedml_aws.egg-info/requires.txt
--rw-r--r--   0 I542957    (501) staff       (20)       10 2023-07-11 19:01:50.000000 fedml_aws-2.0.1/src/fedml_aws.egg-info/top_level.txt
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-05 22:02:52.511929 fedml_aws-2.0.1.dev0/
+-rw-r--r--   0 I542957    (501) staff       (20)     1257 2023-07-05 22:02:52.511257 fedml_aws-2.0.1.dev0/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      889 2023-07-05 21:55:20.000000 fedml_aws-2.0.1.dev0/README.md
+-rw-r--r--   0 I542957    (501) staff       (20)      103 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/pyproject.toml
+-rw-r--r--   0 I542957    (501) staff       (20)       38 2023-07-05 22:02:52.512093 fedml_aws-2.0.1.dev0/setup.cfg
+-rw-r--r--   0 I542957    (501) staff       (20)      943 2023-07-05 22:02:06.000000 fedml_aws-2.0.1.dev0/setup.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-05 22:02:52.417646 fedml_aws-2.0.1.dev0/src/
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-05 22:02:52.494096 fedml_aws-2.0.1.dev0/src/fedml_aws/
+-rw-r--r--   0 I542957    (501) staff       (20)      175 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/__init__.py
+-rw-r--r--   0 I542957    (501) staff       (20)     2352 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/build_and_push.sh
+-rw-r--r--   0 I542957    (501) staff       (20)    15864 2023-06-28 21:02:54.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/dbconnection.py
+-rw-r--r--   0 I542957    (501) staff       (20)    22560 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/dwcsagemaker.py
+-rw-r--r--   0 I542957    (501) staff       (20)      199 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/install_kubectl.sh
+-rw-r--r--   0 I542957    (501) staff       (20)      656 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/logger.py
+-rw-r--r--   0 I542957    (501) staff       (20)     4647 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/predictor.py
+-rw-r--r--   0 I542957    (501) staff       (20)    16482 2023-06-28 21:02:27.000000 fedml_aws-2.0.1.dev0/src/fedml_aws/script_generator.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-07-05 22:02:52.509978 fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/
+-rw-r--r--   0 I542957    (501) staff       (20)     1257 2023-07-05 22:02:52.000000 fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      467 2023-07-05 22:02:52.000000 fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 I542957    (501) staff       (20)        1 2023-07-05 22:02:52.000000 fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       36 2023-07-05 22:02:52.000000 fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/requires.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       10 2023-07-05 22:02:52.000000 fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/top_level.txt
```

### Comparing `fedml_aws-2.0.1/PKG-INFO` & `fedml_aws-2.0.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml_aws
-Version: 2.0.1
+Version: 2.0.1.dev0
 Summary: A python library for building machine learning models on AWS Sagemaker using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_aws-2.0.1/README.md` & `fedml_aws-2.0.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/setup.py` & `fedml_aws-2.0.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="fedml_aws",
-    version="2.0.1",
+    version="2.0.1.dev0",
     author="SAP SE",
     description="A python library for building machine learning models on AWS Sagemaker using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `fedml_aws-2.0.1/src/fedml_aws/build_and_push.sh` & `fedml_aws-2.0.1.dev0/src/fedml_aws/build_and_push.sh`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/src/fedml_aws/dbconnection.py` & `fedml_aws-2.0.1.dev0/src/fedml_aws/dbconnection.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/src/fedml_aws/dwcsagemaker.py` & `fedml_aws-2.0.1.dev0/src/fedml_aws/dwcsagemaker.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/src/fedml_aws/logger.py` & `fedml_aws-2.0.1.dev0/src/fedml_aws/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/src/fedml_aws/predictor.py` & `fedml_aws-2.0.1.dev0/src/fedml_aws/predictor.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/src/fedml_aws/script_generator.py` & `fedml_aws-2.0.1.dev0/src/fedml_aws/script_generator.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.1/src/fedml_aws.egg-info/PKG-INFO` & `fedml_aws-2.0.1.dev0/src/fedml_aws.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml-aws
-Version: 2.0.1
+Version: 2.0.1.dev0
 Summary: A python library for building machine learning models on AWS Sagemaker using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

