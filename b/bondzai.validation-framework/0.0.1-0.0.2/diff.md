# Comparing `tmp/bondzai.validation-framework-0.0.1.tar.gz` & `tmp/bondzai.validation-framework-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.validation-framework-0.0.1.tar", last modified: Tue Jul 11 18:23:26 2023, max compression
+gzip compressed data, was "bondzai.validation-framework-0.0.2.tar", last modified: Tue Jul 11 19:03:39 2023, max compression
```

## Comparing `bondzai.validation-framework-0.0.1.tar` & `bondzai.validation-framework-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:23:26.869066 bondzai.validation-framework-0.0.1/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-11 18:23:26.869176 bondzai.validation-framework-0.0.1/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:23:26.862287 bondzai.validation-framework-0.0.1/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:23:26.866544 bondzai.validation-framework-0.0.1/bondzai/validation_framework/
--rw-r--r--   0 theo       (501) staff       (20)       21 2023-07-11 18:23:15.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2913 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/connector_handler.py
--rw-r--r--   0 theo       (501) staff       (20)    10835 2023-07-11 18:23:15.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/dataset_handler.py
--rw-r--r--   0 theo       (501) staff       (20)     9244 2023-07-11 18:23:15.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/event_catcher.py
--rw-r--r--   0 theo       (501) staff       (20)     3540 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/log_handler.py
--rw-r--r--   0 theo       (501) staff       (20)     9752 2023-07-11 18:23:15.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/result_handler.py
--rw-r--r--   0 theo       (501) staff       (20)     2028 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/bondzai/validation_framework/tar_handler.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:23:26.868854 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      793 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      134 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       22 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:23:26.000000 bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/zip-safe
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:23:26.867068 bondzai.validation-framework-0.0.1/examples/
--rw-r--r--   0 theo       (501) staff       (20)     5098 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/examples/live_scenario.py
--rw-r--r--   0 theo       (501) staff       (20)    12310 2023-07-11 18:23:15.000000 bondzai.validation-framework-0.0.1/examples/scenario.py
--rw-r--r--   0 theo       (501) staff       (20)       76 2023-07-11 18:21:12.000000 bondzai.validation-framework-0.0.1/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      882 2023-07-11 18:23:26.869840 bondzai.validation-framework-0.0.1/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.087244 bondzai.validation-framework-0.0.2/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-11 19:03:39.087345 bondzai.validation-framework-0.0.2/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.081330 bondzai.validation-framework-0.0.2/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.084702 bondzai.validation-framework-0.0.2/bondzai/validation_framework/
+-rw-r--r--   0 theo       (501) staff       (20)       21 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2913 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/connector_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)    10835 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/dataset_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)     9244 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/event_catcher.py
+-rw-r--r--   0 theo       (501) staff       (20)     3540 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/log_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)     9752 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/result_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)     2028 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/tar_handler.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.087031 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      793 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)      134 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       22 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 19:03:38.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/zip-safe
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.085214 bondzai.validation-framework-0.0.2/examples/
+-rw-r--r--   0 theo       (501) staff       (20)     5098 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/examples/live_scenario.py
+-rw-r--r--   0 theo       (501) staff       (20)    12310 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/examples/scenario.py
+-rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      882 2023-07-11 19:03:39.087930 bondzai.validation-framework-0.0.2/setup.cfg
```

### Comparing `bondzai.validation-framework-0.0.1/NOTICE` & `bondzai.validation-framework-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/PKG-INFO` & `bondzai.validation-framework-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.validation-framework
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bondzai Validation Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,validation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.validation-framework-0.0.1/bondzai/validation_framework/connector_handler.py` & `bondzai.validation-framework-0.0.2/bondzai/validation_framework/connector_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/bondzai/validation_framework/dataset_handler.py` & `bondzai.validation-framework-0.0.2/bondzai/validation_framework/dataset_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/bondzai/validation_framework/event_catcher.py` & `bondzai.validation-framework-0.0.2/bondzai/validation_framework/event_catcher.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/bondzai/validation_framework/log_handler.py` & `bondzai.validation-framework-0.0.2/bondzai/validation_framework/log_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/bondzai/validation_framework/result_handler.py` & `bondzai.validation-framework-0.0.2/bondzai/validation_framework/result_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/bondzai/validation_framework/tar_handler.py` & `bondzai.validation-framework-0.0.2/bondzai/validation_framework/tar_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/PKG-INFO` & `bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.validation-framework
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bondzai Validation Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,validation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.validation-framework-0.0.1/bondzai.validation_framework.egg-info/SOURCES.txt` & `bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/examples/live_scenario.py` & `bondzai.validation-framework-0.0.2/examples/live_scenario.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/examples/scenario.py` & `bondzai.validation-framework-0.0.2/examples/scenario.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.1/setup.cfg` & `bondzai.validation-framework-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 zip_safe = True
 include_package_data = True
 namespace_packages = 
 	bondzai
 install_requires = 
 	asciiplot==1.0.0
 	bondzai.gateway-sdk==0.0.8
-	numpy==1.25.0
+	numpy==1.24.3
 	PyYAML==6.0
 	texttable==1.6.7
 	typing_extensions==4.7.1
 
 [options.extras_require]
 dev = 
 	pylint==2.15.9
```

