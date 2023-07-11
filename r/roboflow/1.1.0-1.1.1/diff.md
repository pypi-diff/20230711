# Comparing `tmp/roboflow-1.1.0.tar.gz` & `tmp/roboflow-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.1.0.tar", last modified: Wed Jun 21 16:51:26 2023, max compression
+gzip compressed data, was "roboflow-1.1.1.tar", last modified: Tue Jul 11 21:33:44 2023, max compression
```

## Comparing `roboflow-1.1.0.tar` & `roboflow-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-06-21 16:50:54.000000 roboflow-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-06-21 16:51:26.742029 roboflow-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-21 16:50:54.000000 roboflow-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 16:50:54.000000 roboflow-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.726028 roboflow-1.1.0/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.730028 roboflow-1.1.0/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23093 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.730028 roboflow-1.1.0/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:51:26.742029 roboflow-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-21 16:50:54.000000 roboflow-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-11 21:33:17.000000 roboflow-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-11 21:33:44.297987 roboflow-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-11 21:33:17.000000 roboflow-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 21:33:17.000000 roboflow-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:33:44.297987 roboflow-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 21:33:17.000000 roboflow-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/test_versions.py
```

### Comparing `roboflow-1.1.0/LICENSE` & `roboflow-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/PKG-INFO` & `roboflow-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.1.0
+Version: 1.1.1
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.1.0 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.1.1 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.1.0/README.md` & `roboflow-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/__init__.py` & `roboflow-1.1.1/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.1.0/roboflow/archive/plot.py` & `roboflow-1.1.1/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/config.py` & `roboflow-1.1.1/roboflow/config.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/core/project.py` & `roboflow-1.1.1/roboflow/core/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -613,12 +613,103 @@
                 )
         else:
             annotation_success = True
 
         overall_success = success and annotation_success
         return overall_success
 
+    def search(
+        self,
+        like_image: str = None,
+        prompt: str = None,
+        offset: int = 0,
+        limit: int = 100,
+        tag: str = None,
+        class_name: str = None,
+        in_dataset: str = None,
+        batch: bool = False,
+        batch_id: str = None,
+        fields: list = ["id", "created", "name", "labels"],
+    ):
+        payload = {}
+
+        if like_image is not None:
+            payload["like_image"] = like_image
+
+        if prompt is not None:
+            payload["prompt"] = prompt
+
+        if offset is not None:
+            payload["offset"] = offset
+
+        if limit is not None:
+            payload["limit"] = limit
+
+        if tag is not None:
+            payload["tag"] = tag
+
+        if class_name is not None:
+            payload["class_name"] = class_name
+
+        if in_dataset is not None:
+            payload["in_dataset"] = in_dataset
+
+        if batch is not None:
+            payload["batch"] = batch
+
+        if batch_id is not None:
+            payload["batch_id"] = batch_id
+
+        payload["fields"] = fields
+
+        data = requests.post(
+            API_URL
+            + "/"
+            + self.__workspace
+            + "/"
+            + self.__project_name
+            + "/search?api_key="
+            + self.__api_key,
+            json=payload,
+        )
+
+        return data.json()["results"]
+
+    def search_all(
+        self,
+        like_image: str = None,
+        prompt: str = None,
+        offset: int = 0,
+        limit: int = 100,
+        tag: str = None,
+        class_name: str = None,
+        in_dataset: str = None,
+        batch: bool = False,
+        batch_id: str = None,
+        fields: list = ["id", "created"],
+    ):
+        while True:
+            data = self.search(
+                like_image=like_image,
+                prompt=prompt,
+                offset=offset,
+                limit=limit,
+                tag=tag,
+                class_name=class_name,
+                in_dataset=in_dataset,
+                batch=batch,
+                batch_id=batch_id,
+                fields=fields,
+            )
+
+            yield data
+
+            if len(data) < limit:
+                break
+
+            offset += limit
+
     def __str__(self):
         # String representation of project
         json_str = {"name": self.name, "type": self.type, "workspace": self.__workspace}
 
         return json.dumps(json_str, indent=2)
```

### Comparing `roboflow-1.1.0/roboflow/core/version.py` & `roboflow-1.1.1/roboflow/core/version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/core/workspace.py` & `roboflow-1.1.1/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/models/classification.py` & `roboflow-1.1.1/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/models/inference.py` & `roboflow-1.1.1/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/models/instance_segmentation.py` & `roboflow-1.1.1/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/models/object_detection.py` & `roboflow-1.1.1/roboflow/models/object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/models/semantic_segmentation.py` & `roboflow-1.1.1/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/util/active_learning_utils.py` & `roboflow-1.1.1/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/util/clip_compare_utils.py` & `roboflow-1.1.1/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/util/image_utils.py` & `roboflow-1.1.1/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/util/prediction.py` & `roboflow-1.1.1/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/util/two_stage_utils.py` & `roboflow-1.1.1/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow/util/versions.py` & `roboflow-1.1.1/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/roboflow.egg-info/PKG-INFO` & `roboflow-1.1.1/roboflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.1.0
+Version: 1.1.1
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.1.0 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.1.1 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.1.0/roboflow.egg-info/SOURCES.txt` & `roboflow-1.1.1/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/setup.py` & `roboflow-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/models/test_instance_segmentation.py` & `roboflow-1.1.1/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/models/test_object_detection.py` & `roboflow-1.1.1/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/models/test_semantic_segmentation.py` & `roboflow-1.1.1/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/test_project.py` & `roboflow-1.1.1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/test_queries.py` & `roboflow-1.1.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/test_version.py` & `roboflow-1.1.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/util/test_image_utils.py` & `roboflow-1.1.1/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.0/tests/util/test_versions.py` & `roboflow-1.1.1/tests/util/test_versions.py`

 * *Files identical despite different names*

