# Comparing `tmp/azureml-assets-1.5.0.tar.gz` & `tmp/azureml-assets-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.5.0.tar", last modified: Thu Jul  6 13:04:25 2023, max compression
+gzip compressed data, was "azureml-assets-1.5.1.tar", last modified: Tue Jul 11 18:59:13 2023, max compression
```

## Comparing `azureml-assets-1.5.0.tar` & `azureml-assets-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.770660 azureml-assets-1.5.0/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.770660 azureml-assets-1.5.0/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16797 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6897 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17280 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-06 13:04:25.000000 azureml-assets-1.5.0/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-06 13:04:25.000000 azureml-assets-1.5.0/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 13:04:25.000000 azureml-assets-1.5.0/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-06 13:04:25.000000 azureml-assets-1.5.0/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-06 13:04:25.000000 azureml-assets-1.5.0/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-06 13:04:25.774659 azureml-assets-1.5.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-06 13:03:44.000000 azureml-assets-1.5.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.134351 azureml-assets-1.5.1/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.134351 azureml-assets-1.5.1/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17053 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17280 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/setup.py
```

### Comparing `azureml-assets-1.5.0/PKG-INFO` & `azureml-assets-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.5.0
+Version: 1.5.1
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.5.0/azureml/assets/__init__.py` & `azureml-assets-1.5.1/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/asset_utils.py` & `azureml-assets-1.5.1/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/config.py` & `azureml-assets-1.5.1/azureml/assets/config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/copy_assets.py` & `azureml-assets-1.5.1/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/deployment_config.py` & `azureml-assets-1.5.1/azureml/assets/deployment_config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/environment/build.py` & `azureml-assets-1.5.1/azureml/assets/environment/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from typing import List, Tuple
 
 import azureml.assets as assets
 import azureml.assets.util as util
 from azureml.assets.util import logger
 
 TASK_FILENAME = "_acr_build_task.yaml"
-STEP_TIMEOUT_SECONDS = 60 * 90
+BUILD_STEP_TIMEOUT_SECONDS = 60 * 90
+SCAN_STEP_TIMEOUT_SECONDS = 60 * 20
+TRIVY_TIMEOUT = "15m0s"
 SUCCESS_COUNT = "success_count"
 FAILED_COUNT = "failed_count"
 COUNTERS = [SUCCESS_COUNT, FAILED_COUNT]
 
 
 def create_acr_task(image_name: str,
                     build_context_dir: Path,
@@ -48,37 +50,42 @@
 
     Returns:
         Path: The task file.
     """
     # Start task with just the build step
     task = {
         'version': 'v1.1.0',
-        'stepTimeout': STEP_TIMEOUT_SECONDS,
+        'stepTimeout': BUILD_STEP_TIMEOUT_SECONDS,
         'steps': [{
             'id': "build",
             'build': f"-t $Registry/{image_name} -f {dockerfile} ."
         }]}
 
+    # Add output conda export command
+    task['steps'].append({
+        'id': 'conda_export',
+        'cmd': f"$Registry/{image_name} conda env export",
+        'ignoreErrors': True
+    })
+
     # Add test command if provided
     if test_command:
         task['steps'].append({
             'id': 'test',
             'cmd': f"$Registry/{image_name} {test_command}"
         })
 
         if trivy_url is not None:
             task['steps'].append({
                 'id': 'scan',
-                'cmd': (
-                        f"$Registry/{image_name} "
-                        f"curl -sSfL -o trivy.deb {trivy_url} && "
-                        "dpkg -i trivy.deb && "
-                        "trivy fs --scanners vuln /"
-                    ),
-                'ignoreErrors': True
+                'stepTimeout': SCAN_STEP_TIMEOUT_SECONDS,
+                'cmd': f"aquasec/trivy -q --timeout {TRIVY_TIMEOUT} image --scanners vuln --ignore-unfixed "
+                       f"$Registry/{image_name}",
+                'ignoreErrors': True,
+                'privileged': True
             })
 
     # Add push step if requested
     if push:
         task['steps'].append({
             'id': 'push',
             'push': [f"$Registry/{image_name}"]
```

### Comparing `azureml-assets-1.5.0/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.5.1/azureml/assets/environment/pin_image_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         response = _urlopen_with_retries(f"https://{hostname}/v2/{repo}/tags/list")
     except Exception as e:
         raise Exception(f"Failed to retrieve tags for {repo}: {e}")
     tags = json.loads(response.read().decode("utf-8")).get("tags", [])
 
     # Filter tags and sort in descending order because this should be faster
     tags_sorted = sorted([t for t in tags if t != LATEST_TAG and
-                         (regex is None or regex.search(t) is not None)], reverse=True)
+                         (regex is None or regex.fullmatch(t) is not None)], reverse=True)
 
     # Handle regex
     if regex is not None:
         # Use the most recent matching tag
         if tags_sorted:
             latest_tag = tags_sorted[0]
         else:
```

### Comparing `azureml-assets-1.5.0/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.5.1/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.5.1/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.5.1/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.5.1/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/model/utils.py` & `azureml-assets-1.5.1/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/tag_released_assets.py` & `azureml-assets-1.5.1/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/update_assets.py` & `azureml-assets-1.5.1/azureml/assets/update_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/update_spec.py` & `azureml-assets-1.5.1/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/util/__init__.py` & `azureml-assets-1.5.1/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/util/logger.py` & `azureml-assets-1.5.1/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/util/template.py` & `azureml-assets-1.5.1/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/util/util.py` & `azureml-assets-1.5.1/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml/assets/validate_assets.py` & `azureml-assets-1.5.1/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.5.1/azureml_assets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.5.0
+Version: 1.5.1
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.5.0/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.5.1/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.0/setup.py` & `azureml-assets-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.5.0",
+   version="1.5.1",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

