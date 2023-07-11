# Comparing `tmp/fedml_azure-2.0.0.dev0.tar.gz` & `tmp/fedml_azure-2.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_azure-2.0.0.dev0.tar", last modified: Wed May 11 21:51:23 2022, max compression
+gzip compressed data, was "fedml_azure-2.0.1.dev0.tar", last modified: Tue Jul 11 21:18:53 2023, max compression
```

## Comparing `fedml_azure-2.0.0.dev0.tar` & `fedml_azure-2.0.1.dev0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2022-05-11 21:51:23.507809 fedml_azure-2.0.0.dev0/
--rw-r--r--   0 I550585    (501) staff       (20)    11307 2022-04-20 22:04:39.000000 fedml_azure-2.0.0.dev0/LICENSE.txt
--rw-r--r--   0 I550585    (501) staff       (20)      349 2022-05-11 21:51:23.507163 fedml_azure-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      103 2021-09-30 23:53:45.000000 fedml_azure-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 I550585    (501) staff       (20)       38 2022-05-11 21:51:23.508005 fedml_azure-2.0.0.dev0/setup.cfg
--rw-r--r--   0 I550585    (501) staff       (20)      757 2022-05-11 21:50:54.000000 fedml_azure-2.0.0.dev0/setup.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2022-05-11 21:51:23.476946 fedml_azure-2.0.0.dev0/src/
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2022-05-11 21:51:23.499773 fedml_azure-2.0.0.dev0/src/fedml_azure/
--rw-r--r--   0 I550585    (501) staff       (20)      182 2022-03-25 19:46:30.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)    11107 2022-03-28 22:49:40.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/compute_creation.py
--rw-r--r--   0 I550585    (501) staff       (20)     9031 2022-03-28 20:08:48.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/dbconnection.py
--rw-r--r--   0 I550585    (501) staff       (20)    16929 2022-04-20 22:05:13.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/deployment.py
--rw-r--r--   0 I550585    (501) staff       (20)    14315 2022-04-01 19:53:04.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/dwc_azureml.py
--rw-r--r--   0 I550585    (501) staff       (20)     4982 2022-04-01 00:04:17.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/environment_creation.py
--rw-r--r--   0 I550585    (501) staff       (20)     1682 2022-04-01 01:44:09.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/install_validate.sh
--rw-r--r--   0 I550585    (501) staff       (20)      380 2021-10-01 17:36:33.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/internal_config.json
--rw-r--r--   0 I550585    (501) staff       (20)     7737 2022-04-01 01:25:39.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)     9867 2022-04-01 01:45:51.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/kyma_deployment.py
--rw-r--r--   0 I550585    (501) staff       (20)      656 2022-03-28 22:10:56.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/logger.py
--rw-r--r--   0 I550585    (501) staff       (20)     3112 2022-03-28 23:02:33.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/resource_creation.py
--rw-r--r--   0 I550585    (501) staff       (20)     4949 2022-03-29 02:53:37.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/script_generator.py
--rw-r--r--   0 I550585    (501) staff       (20)      652 2022-03-28 23:03:10.000000 fedml_azure-2.0.0.dev0/src/fedml_azure/script_generator_helper.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2022-05-11 21:51:23.505845 fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/
--rw-r--r--   0 I550585    (501) staff       (20)      349 2022-05-11 21:51:22.000000 fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      707 2022-05-11 21:51:23.000000 fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/SOURCES.txt
--rw-r--r--   0 I550585    (501) staff       (20)        1 2022-05-11 21:51:23.000000 fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/dependency_links.txt
--rw-r--r--   0 I550585    (501) staff       (20)       19 2022-05-11 21:51:23.000000 fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/requires.txt
--rw-r--r--   0 I550585    (501) staff       (20)       12 2022-05-11 21:51:23.000000 fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/top_level.txt
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.995678 fedml_azure-2.0.1.dev0/
+-rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/LICENSE.txt
+-rw-r--r--   0 I550585    (501) staff       (20)      349 2023-07-11 21:18:53.995155 fedml_azure-2.0.1.dev0/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      103 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/pyproject.toml
+-rw-r--r--   0 I550585    (501) staff       (20)       38 2023-07-11 21:18:53.995812 fedml_azure-2.0.1.dev0/setup.cfg
+-rw-r--r--   0 I550585    (501) staff       (20)      757 2023-07-11 21:17:15.000000 fedml_azure-2.0.1.dev0/setup.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.973683 fedml_azure-2.0.1.dev0/src/
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.989743 fedml_azure-2.0.1.dev0/src/fedml_azure/
+-rw-r--r--   0 I550585    (501) staff       (20)      182 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)    11107 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/compute_creation.py
+-rw-r--r--   0 I550585    (501) staff       (20)    15864 2023-07-11 21:16:30.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/dbconnection.py
+-rw-r--r--   0 I550585    (501) staff       (20)    16929 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/deployment.py
+-rw-r--r--   0 I550585    (501) staff       (20)    14315 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/dwc_azureml.py
+-rw-r--r--   0 I550585    (501) staff       (20)     4982 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/environment_creation.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1682 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/install_validate.sh
+-rw-r--r--   0 I550585    (501) staff       (20)      380 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/internal_config.json
+-rw-r--r--   0 I550585    (501) staff       (20)     7737 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     9867 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deployment.py
+-rw-r--r--   0 I550585    (501) staff       (20)      656 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/logger.py
+-rw-r--r--   0 I550585    (501) staff       (20)     3112 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/resource_creation.py
+-rw-r--r--   0 I550585    (501) staff       (20)     4949 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator.py
+-rw-r--r--   0 I550585    (501) staff       (20)      652 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator_helper.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.994253 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/
+-rw-r--r--   0 I550585    (501) staff       (20)      349 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      707 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 I550585    (501) staff       (20)        1 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       19 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/requires.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       12 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/top_level.txt
```

### Comparing `fedml_azure-2.0.0.dev0/LICENSE.txt` & `fedml_azure-2.0.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/setup.py` & `fedml_azure-2.0.1.dev0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="fedml_azure",
-    version="2.0.0.dev0",
+    version="2.0.1.dev0",
     author="SAP SE",
     description="A python library for building machine learning models on AzureML using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/compute_creation.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/compute_creation.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/deployment.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/deployment.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/dwc_azureml.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/dwc_azureml.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/environment_creation.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/environment_creation.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/install_validate.sh` & `fedml_azure-2.0.1.dev0/src/fedml_azure/install_validate.sh`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/kyma_deploy.sh` & `fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/kyma_deployment.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deployment.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/logger.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/resource_creation.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/resource_creation.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/script_generator.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure/script_generator_helper.py` & `fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator_helper.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.0.dev0/src/fedml_azure.egg-info/SOURCES.txt` & `fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

