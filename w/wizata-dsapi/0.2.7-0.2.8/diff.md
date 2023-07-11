# Comparing `tmp/wizata-dsapi-0.2.7.tar.gz` & `tmp/wizata-dsapi-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.7.tar", last modified: Mon Jul 10 14:02:28 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.2.8.tar", last modified: Tue Jul 11 12:31:02 2023, max compression
```

## Comparing `wizata-dsapi-0.2.7.tar` & `wizata-dsapi-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 14:02:28.900266 wizata-dsapi-0.2.7/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-07-10 14:02:28.899267 wizata-dsapi-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-10 14:02:28.900266 wizata-dsapi-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-10 13:55:20.000000 wizata-dsapi-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:02:28.873571 wizata-dsapi-0.2.7/wizata_dsapi/
--rw-rw-rw-   0        0        0     1014 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.7/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.7/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.7/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.7/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.7/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.7/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.7/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.7/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.7/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.7/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.7/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.7/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     7221 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.7/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2762 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.7/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56463 2023-07-10 14:00:26.000000 wizata-dsapi-0.2.7/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:02:28.898266 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 12:31:02.322145 wizata-dsapi-0.2.8/
+-rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-07-11 12:31:02.321662 wizata-dsapi-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.2.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:31:02.322641 wizata-dsapi-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-11 12:30:48.000000 wizata-dsapi-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:31:02.298178 wizata-dsapi-0.2.8/wizata_dsapi/
+-rw-rw-rw-   0        0        0     1014 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     5763 2023-06-19 13:45:53.000000 wizata-dsapi-0.2.8/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     6145 2023-07-11 12:30:48.000000 wizata-dsapi-0.2.8/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14903 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.8/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.2.8/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     9999 2023-06-21 05:55:35.000000 wizata-dsapi-0.2.8/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    17900 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.8/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    18221 2023-07-06 16:17:20.000000 wizata-dsapi-0.2.8/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.2.8/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     7221 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2599 2023-06-22 14:06:45.000000 wizata-dsapi-0.2.8/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2762 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56463 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:31:02.319690 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-07-11 12:31:02.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.7/LICENSE.txt` & `wizata-dsapi-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/setup.py` & `wizata-dsapi-0.2.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.2.7',
+    version='0.2.8',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/__init__.py` & `wizata-dsapi-0.2.8/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.2.8/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.2.8/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.2.8/wizata_dsapi/datapoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import uuid
 from enum import Enum
 from .api_dto import ApiDto
 
 
-class Category:
+class Category(ApiDto):
 
     def __init__(self,
                  category_id: uuid.UUID = None,
                  name: str = None):
         if category_id is None:
             self.category_id = uuid.uuid4()
         else:
             self.category_id = category_id
         self.name = name
 
+    def api_id(self) -> str:
+        return str(self.category_id).upper()
+
+    def endpoint(self) -> str:
+        return "Categories"
+
     def from_json(self, obj):
         if "id" in obj.keys():
             self.category_id = uuid.UUID(obj["id"])
 
         if "name" in obj.keys():
             self.name = obj["name"]
 
@@ -26,25 +32,31 @@
             "id": str(self.category_id)
         }
         if self.name is not None and self.name != '':
             obj["name"] = self.name
         return obj
 
 
-class Label:
+class Label(ApiDto):
 
     def __init__(self,
                  label_id: uuid.UUID = None,
                  name: str = None):
         if label_id is None:
             self.label_id = uuid.uuid4()
         else:
             self.label_id = label_id
         self.name = name
 
+    def api_id(self) -> str:
+        return str(self.label_id).upper()
+
+    def endpoint(self) -> str:
+        return "Labels"
+
     def from_json(self, obj):
         if "id" in obj.keys():
             self.label_id = uuid.UUID(obj["id"])
 
         if "name" in obj.keys():
             self.name = obj["name"]
 
@@ -53,25 +65,31 @@
             "id": str(self.label_id)
         }
         if self.name is not None and self.name != '':
             obj["name"] = self.name
         return obj
 
 
-class Unit:
+class Unit(ApiDto):
 
     def __init__(self,
                  unit_id: uuid.UUID = None,
                  short_name: str = None):
         if unit_id is None:
             self.unit_id = uuid.uuid4()
         else:
             self.unit_id = unit_id
         self.short_name = short_name
 
+    def api_id(self) -> str:
+        return str(self.unit_id).upper()
+
+    def endpoint(self) -> str:
+        return "Units"
+
     def from_json(self, obj):
         """
         Load the datapoint entity from a dictionary.
 
         :param obj: Dict version of the datapoint.
         """
         if "id" in obj.keys():
```

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.2.8/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.2.8/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/execution.py` & `wizata-dsapi-0.2.8/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/experiment.py` & `wizata-dsapi-0.2.8/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.2.8/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.2.8/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.2.8/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/plot.py` & `wizata-dsapi-0.2.8/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/request.py` & `wizata-dsapi-0.2.8/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/script.py` & `wizata-dsapi-0.2.8/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/template.py` & `wizata-dsapi-0.2.8/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/twin.py` & `wizata-dsapi-0.2.8/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.2.8/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.2.8/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.2.8/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.7/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.2.8/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

