# Comparing `tmp/rally_cli-0.1.8.tar.gz` & `tmp/rally_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rally_cli-0.1.8.tar", max compression
+gzip compressed data, was "rally_cli-0.1.9.tar", max compression
```

## Comparing `rally_cli-0.1.8.tar` & `rally_cli-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1084 2022-12-03 16:21:03.678510 rally_cli-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     1733 2022-12-03 16:21:03.462509 rally_cli-0.1.8/README.md
--rw-r--r--   0        0        0      753 2022-12-12 17:05:16.777725 rally_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      130 2022-12-03 16:21:03.562510 rally_cli-0.1.8/rallycli/__init__.py
--rw-r--r--   0        0        0      233 2022-12-03 16:21:03.534510 rally_cli-0.1.8/rallycli/apis/__init__.py
--rw-r--r--   0        0        0     7482 2022-12-03 16:21:03.522510 rally_cli-0.1.8/rallycli/apis/artifact_api.py
--rw-r--r--   0        0        0     3860 2022-12-03 16:21:03.530510 rally_cli-0.1.8/rallycli/apis/attdefinition_api.py
--rw-r--r--   0        0        0     3392 2022-12-03 16:21:03.550510 rally_cli-0.1.8/rallycli/apis/project_api.py
--rw-r--r--   0        0        0     4562 2022-12-03 16:21:03.526510 rally_cli-0.1.8/rallycli/apis/scm_api.py
--rw-r--r--   0        0        0      965 2022-12-03 16:21:03.546510 rally_cli-0.1.8/rallycli/apis/timebox_api.py
--rw-r--r--   0        0        0     2569 2022-12-03 16:21:03.518509 rally_cli-0.1.8/rallycli/apis/user_api.py
--rw-r--r--   0        0        0    18982 2022-12-03 16:21:03.498510 rally_cli-0.1.8/rallycli/base_api.py
--rw-r--r--   0        0        0      135 2022-12-03 16:21:03.506510 rally_cli-0.1.8/rallycli/errors/__init__.py
--rw-r--r--   0        0        0     3449 2022-12-03 16:21:03.502509 rally_cli-0.1.8/rallycli/errors/decorators.py
--rw-r--r--   0        0        0     3818 2022-12-03 16:21:03.510510 rally_cli-0.1.8/rallycli/errors/rally_errors.py
--rw-r--r--   0        0        0      279 2022-12-03 16:21:03.482509 rally_cli-0.1.8/rallycli/models/__init__.py
--rw-r--r--   0        0        0     3780 2022-12-12 16:56:13.166884 rally_cli-0.1.8/rallycli/models/artifact_models.py
--rw-r--r--   0        0        0     7220 2022-12-03 16:21:03.474510 rally_cli-0.1.8/rallycli/models/base_models.py
--rw-r--r--   0        0        0      270 2022-12-03 16:21:03.486509 rally_cli-0.1.8/rallycli/models/memento.py
--rw-r--r--   0        0        0     3891 2022-12-03 16:21:03.474510 rally_cli-0.1.8/rallycli/models/models.py
--rw-r--r--   0        0        0      924 2022-12-03 16:21:03.490510 rally_cli-0.1.8/rallycli/models/type_names.py
--rw-r--r--   0        0        0     3605 2022-12-03 16:21:03.558510 rally_cli-0.1.8/rallycli/rally_api.py
--rw-r--r--   0        0        0     2381 2022-12-12 16:55:52.449664 rally_cli-0.1.8/rallycli/session_builder.py
--rw-r--r--   0        0        0       39 2022-12-03 16:21:03.598510 rally_cli-0.1.8/rallycli/utils/__init__.py
--rw-r--r--   0        0        0      407 2022-12-03 16:21:03.570510 rally_cli-0.1.8/rallycli/utils/logging.py
--rw-r--r--   0        0        0     3882 2022-12-03 16:21:03.578510 rally_cli-0.1.8/rallycli/utils/orig_utils.py
--rw-r--r--   0        0        0      605 2022-12-03 16:21:03.574510 rally_cli-0.1.8/rallycli/utils/timer.py
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 rally_cli-0.1.8/setup.py
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 rally_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 16:21:03.678510 rally_cli-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     1733 2022-12-03 16:21:03.462509 rally_cli-0.1.9/README.md
+-rw-r--r--   0        0        0      753 2023-07-11 14:11:01.793001 rally_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      130 2022-12-03 16:21:03.562510 rally_cli-0.1.9/rallycli/__init__.py
+-rw-r--r--   0        0        0      233 2022-12-03 16:21:03.534510 rally_cli-0.1.9/rallycli/apis/__init__.py
+-rw-r--r--   0        0        0     7482 2022-12-03 16:21:03.522510 rally_cli-0.1.9/rallycli/apis/artifact_api.py
+-rw-r--r--   0        0        0     3860 2022-12-03 16:21:03.530510 rally_cli-0.1.9/rallycli/apis/attdefinition_api.py
+-rw-r--r--   0        0        0     3392 2022-12-03 16:21:03.550510 rally_cli-0.1.9/rallycli/apis/project_api.py
+-rw-r--r--   0        0        0     4562 2022-12-03 16:21:03.526510 rally_cli-0.1.9/rallycli/apis/scm_api.py
+-rw-r--r--   0        0        0      965 2022-12-03 16:21:03.546510 rally_cli-0.1.9/rallycli/apis/timebox_api.py
+-rw-r--r--   0        0        0     2569 2022-12-03 16:21:03.518509 rally_cli-0.1.9/rallycli/apis/user_api.py
+-rw-r--r--   0        0        0    18982 2022-12-03 16:21:03.498510 rally_cli-0.1.9/rallycli/base_api.py
+-rw-r--r--   0        0        0      135 2022-12-03 16:21:03.506510 rally_cli-0.1.9/rallycli/errors/__init__.py
+-rw-r--r--   0        0        0     3449 2022-12-03 16:21:03.502509 rally_cli-0.1.9/rallycli/errors/decorators.py
+-rw-r--r--   0        0        0     3818 2022-12-03 16:21:03.510510 rally_cli-0.1.9/rallycli/errors/rally_errors.py
+-rw-r--r--   0        0        0      279 2022-12-03 16:21:03.482509 rally_cli-0.1.9/rallycli/models/__init__.py
+-rw-r--r--   0        0        0     3780 2022-12-12 16:56:13.166884 rally_cli-0.1.9/rallycli/models/artifact_models.py
+-rw-r--r--   0        0        0     7220 2022-12-03 16:21:03.474510 rally_cli-0.1.9/rallycli/models/base_models.py
+-rw-r--r--   0        0        0      270 2022-12-03 16:21:03.486509 rally_cli-0.1.9/rallycli/models/memento.py
+-rw-r--r--   0        0        0     3891 2022-12-03 16:21:03.474510 rally_cli-0.1.9/rallycli/models/models.py
+-rw-r--r--   0        0        0      924 2022-12-03 16:21:03.490510 rally_cli-0.1.9/rallycli/models/type_names.py
+-rw-r--r--   0        0        0     3605 2022-12-03 16:21:03.558510 rally_cli-0.1.9/rallycli/rally_api.py
+-rw-r--r--   0        0        0     2381 2022-12-12 16:55:52.449664 rally_cli-0.1.9/rallycli/session_builder.py
+-rw-r--r--   0        0        0       39 2022-12-03 16:21:03.598510 rally_cli-0.1.9/rallycli/utils/__init__.py
+-rw-r--r--   0        0        0      407 2022-12-03 16:21:03.570510 rally_cli-0.1.9/rallycli/utils/logging.py
+-rw-r--r--   0        0        0     3882 2022-12-03 16:21:03.578510 rally_cli-0.1.9/rallycli/utils/orig_utils.py
+-rw-r--r--   0        0        0      605 2022-12-03 16:21:03.574510 rally_cli-0.1.9/rallycli/utils/timer.py
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 rally_cli-0.1.9/PKG-INFO
```

### Comparing `rally_cli-0.1.8/LICENSE.txt` & `rally_cli-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/README.md` & `rally_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/pyproject.toml` & `rally_cli-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rally-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = "Rally software API Client"
 authors = ["J. Andres Guerrero <juguerre@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rallycli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `rally_cli-0.1.8/rallycli/apis/artifact_api.py` & `rally_cli-0.1.9/rallycli/apis/artifact_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/apis/attdefinition_api.py` & `rally_cli-0.1.9/rallycli/apis/attdefinition_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/apis/project_api.py` & `rally_cli-0.1.9/rallycli/apis/project_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/apis/scm_api.py` & `rally_cli-0.1.9/rallycli/apis/scm_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/apis/timebox_api.py` & `rally_cli-0.1.9/rallycli/apis/timebox_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/apis/user_api.py` & `rally_cli-0.1.9/rallycli/apis/user_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/base_api.py` & `rally_cli-0.1.9/rallycli/base_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/errors/decorators.py` & `rally_cli-0.1.9/rallycli/errors/decorators.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/errors/rally_errors.py` & `rally_cli-0.1.9/rallycli/errors/rally_errors.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/models/artifact_models.py` & `rally_cli-0.1.9/rallycli/models/artifact_models.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/models/base_models.py` & `rally_cli-0.1.9/rallycli/models/base_models.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/models/models.py` & `rally_cli-0.1.9/rallycli/models/models.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/models/type_names.py` & `rally_cli-0.1.9/rallycli/models/type_names.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/rally_api.py` & `rally_cli-0.1.9/rallycli/rally_api.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/session_builder.py` & `rally_cli-0.1.9/rallycli/session_builder.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/utils/orig_utils.py` & `rally_cli-0.1.9/rallycli/utils/orig_utils.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/rallycli/utils/timer.py` & `rally_cli-0.1.9/rallycli/utils/timer.py`

 * *Files identical despite different names*

### Comparing `rally_cli-0.1.8/PKG-INFO` & `rally_cli-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rally-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Rally software API Client
 License: MIT
 Author: J. Andres Guerrero
 Author-email: juguerre@gmail.com
 Requires-Python: >=3.8.0,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

