# Comparing `tmp/labelspark-0.7.29.tar.gz` & `tmp/labelspark-0.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelspark-0.7.29.tar", last modified: Mon Jul 10 14:04:04 2023, max compression
+gzip compressed data, was "labelspark-0.7.30.tar", last modified: Mon Jul 10 17:23:00 2023, max compression
```

## Comparing `labelspark-0.7.29.tar` & `labelspark-0.7.30.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:04:04.693280 labelspark-0.7.29/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 14:03:54.000000 labelspark-0.7.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-10 14:04:04.693280 labelspark-0.7.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 14:03:54.000000 labelspark-0.7.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:04:04.693280 labelspark-0.7.29/labelspark/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/add_json_answers_to_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/bronze_to_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/create_labelbox_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/dataframe_schema_enrichment.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/dictionary_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/flatten_bronze_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/get_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/get_videoframe_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/is_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/jsonToDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/spark_schema_to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/update_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:04:04.693280 labelspark-0.7.29/labelspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:04:04.693280 labelspark-0.7.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-10 14:03:54.000000 labelspark-0.7.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:23:00.931468 labelspark-0.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 17:22:52.000000 labelspark-0.7.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-10 17:23:00.931468 labelspark-0.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 17:22:52.000000 labelspark-0.7.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:23:00.931468 labelspark-0.7.30/labelspark/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/add_json_answers_to_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/bronze_to_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/create_labelbox_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/dataframe_schema_enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/dictionary_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/flatten_bronze_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/get_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/get_videoframe_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/is_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/jsonToDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/spark_schema_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/update_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-10 17:22:52.000000 labelspark-0.7.30/labelspark/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:23:00.931468 labelspark-0.7.30/labelspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-10 17:23:00.000000 labelspark-0.7.30/labelspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 17:23:00.000000 labelspark-0.7.30/labelspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:23:00.000000 labelspark-0.7.30/labelspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 17:23:00.000000 labelspark-0.7.30/labelspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 17:23:00.000000 labelspark-0.7.30/labelspark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:23:00.931468 labelspark-0.7.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-10 17:22:52.000000 labelspark-0.7.30/setup.py
```

### Comparing `labelspark-0.7.29/LICENSE` & `labelspark-0.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/PKG-INFO` & `labelspark-0.7.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.29
+Version: 0.7.30
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `labelspark-0.7.29/README.md` & `labelspark-0.7.30/README.md`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/__init__.py` & `labelspark-0.7.30/labelspark/__init__.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/add_json_answers_to_dictionary.py` & `labelspark-0.7.30/labelspark/add_json_answers_to_dictionary.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/api_key.py` & `labelspark-0.7.30/labelspark/api_key.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/bronze_to_silver.py` & `labelspark-0.7.30/labelspark/bronze_to_silver.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/client.py` & `labelspark-0.7.30/labelspark/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import pyspark
 from labelbox import Client as labelboxClient
-from labelspark.labelspark.uploader import create_upload_dict
-from labelspark.labelspark.connector import check_pyspark, get_col_names, get_unique_values
-from labelbase.labelbase.connector import validate_columns, determine_actions
-from labelbase.labelbase.uploader import create_global_key_to_data_row_id_dict, batch_create_data_rows, batch_rows_to_project, batch_upload_annotations
-from labelbase.labelbase.downloader import export_and_flatten_labels
-from labelpandas.labelpandas.client import Client as lp_client
-# from labelpandas.labelpandas.client import upsert_data_rows_from_table
-from itertools import chain
-from pyspark.sql.types import StructType, StructField, ArrayType, IntegerType, DoubleType, StringType, DataType
+from labelspark.uploader import create_upload_dict
+from labelspark.connector import check_pyspark, get_col_names, get_unique_values
+from labelbase.connector import validate_columns, determine_actions
+from labelbase.uploader import create_global_key_to_data_row_id_dict, batch_create_data_rows, batch_rows_to_project, batch_upload_annotations
+from labelbase.downloader import export_and_flatten_labels
 import json
 from delta import *
 from uuid import uuid4
-from labelbase.labelbase.downloader import *
-from labelbase.labelbase.uploader import *
-from labelbase.labelbase.connector import *
-from labelspark.labelspark import connector, uploader
+from labelbase.downloader import *
+from labelbase.uploader import *
+from labelbase.connector import *
+from labelspark import connector, uploader
 
 class Client:
     """ A Databricks Client, containing a Labelbox Client, to-be-run a Databricks notebook
     Args:
         lb_api_key                  :   Required (str) - Labelbox API Key
         lb_endpoint                 :   Optinoal (bool) - Labelbox GraphQL endpoint
         lb_enable_experimental      :   Optional (bool) - If `True` enables experimental Labelbox SDK features
@@ -211,15 +207,14 @@
         """
         # Create/identify the following values:
             # row_data_col      : column with name "row_data"
             # global_key_col    : column with name "global_key" - defaults to row_data_col
             # external_id_col   : column with name "external_id" - defaults to global_key_col
             # project_id_col    : column with name "project_id" - defaults to ""
             # dataset_id_col    : column with name "dataset_id" - defaults to ""
-            # external_id_col   : column with name "external_id" - defaults to global_key_col        
             # metadata_index    : Dictonary where {key=metadata_field_name : value=metadata_type} - defaults to {}
             # attachment_index  : Dictonary where {key=column_name : value=attachment_type} - defaults to {}
             # annotation_index  : Dictonary where {key=column_name : value=top_level_feature_name} - defaults to {}
         x = validate_columns(
             client=self.lb_client, table=table,
             get_columns_function=get_col_names,
             get_unique_values_function=get_unique_values,
```

### Comparing `labelspark-0.7.29/labelspark/connector.py` & `labelspark-0.7.30/labelspark/connector.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/create_dataset.py` & `labelspark-0.7.30/labelspark/create_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/create_labelbox_dataset.py` & `labelspark-0.7.30/labelspark/create_labelbox_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/dataframe_schema_enrichment.py` & `labelspark-0.7.30/labelspark/dataframe_schema_enrichment.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/flatten_bronze_table.py` & `labelspark-0.7.30/labelspark/flatten_bronze_table.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/get_annotations.py` & `labelspark-0.7.30/labelspark/get_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/get_videoframe_annotations.py` & `labelspark-0.7.30/labelspark/get_videoframe_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/spark_schema_to_string.py` & `labelspark-0.7.30/labelspark/spark_schema_to_string.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/update_metadata.py` & `labelspark-0.7.30/labelspark/update_metadata.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark/uploader.py` & `labelspark-0.7.30/labelspark/uploader.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/labelspark.egg-info/PKG-INFO` & `labelspark-0.7.30/labelspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.29
+Version: 0.7.30
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `labelspark-0.7.29/labelspark.egg-info/SOURCES.txt` & `labelspark-0.7.30/labelspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.29/setup.py` & `labelspark-0.7.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelspark',
-    version='0.7.29',
+    version='0.7.30',
     author='Labelbox',
     author_email="raphael@labelbox.com",      
     packages=find_packages(),
     url='https://github.com/Labelbox/LabelSpark.git',
     description='Labelbox Connector for Databricks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

