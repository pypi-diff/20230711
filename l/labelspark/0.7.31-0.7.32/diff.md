# Comparing `tmp/labelspark-0.7.31.tar.gz` & `tmp/labelspark-0.7.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelspark-0.7.31.tar", last modified: Tue Jul 11 02:24:13 2023, max compression
+gzip compressed data, was "labelspark-0.7.32.tar", last modified: Tue Jul 11 21:54:23 2023, max compression
```

## Comparing `labelspark-0.7.31.tar` & `labelspark-0.7.32.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:24:13.490230 labelspark-0.7.31/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 02:24:03.000000 labelspark-0.7.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-11 02:24:13.490230 labelspark-0.7.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-11 02:24:03.000000 labelspark-0.7.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:24:13.490230 labelspark-0.7.31/labelspark/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/add_json_answers_to_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/bronze_to_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)    33789 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/create_labelbox_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/dataframe_schema_enrichment.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/dictionary_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/flatten_bronze_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/get_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/get_videoframe_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/is_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/jsonToDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/spark_schema_to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/update_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-11 02:24:03.000000 labelspark-0.7.31/labelspark/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:24:13.490230 labelspark-0.7.31/labelspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-11 02:24:13.000000 labelspark-0.7.31/labelspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-11 02:24:13.000000 labelspark-0.7.31/labelspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 02:24:13.000000 labelspark-0.7.31/labelspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 02:24:13.000000 labelspark-0.7.31/labelspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 02:24:13.000000 labelspark-0.7.31/labelspark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:24:13.490230 labelspark-0.7.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-11 02:24:03.000000 labelspark-0.7.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:54:23.230970 labelspark-0.7.32/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 21:54:14.000000 labelspark-0.7.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-11 21:54:23.230970 labelspark-0.7.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-11 21:54:14.000000 labelspark-0.7.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:54:23.230970 labelspark-0.7.32/labelspark/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/add_json_answers_to_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/bronze_to_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33989 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/create_labelbox_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/dataframe_schema_enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/dictionary_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/flatten_bronze_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/get_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/get_videoframe_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/is_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/jsonToDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/spark_schema_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/update_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:54:23.230970 labelspark-0.7.32/labelspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:54:23.230970 labelspark-0.7.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-11 21:54:14.000000 labelspark-0.7.32/setup.py
```

### Comparing `labelspark-0.7.31/LICENSE` & `labelspark-0.7.32/LICENSE`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/PKG-INFO` & `labelspark-0.7.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.31
+Version: 0.7.32
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `labelspark-0.7.31/README.md` & `labelspark-0.7.32/README.md`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/__init__.py` & `labelspark-0.7.32/labelspark/__init__.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/add_json_answers_to_dictionary.py` & `labelspark-0.7.32/labelspark/add_json_answers_to_dictionary.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/api_key.py` & `labelspark-0.7.32/labelspark/api_key.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/bronze_to_silver.py` & `labelspark-0.7.32/labelspark/bronze_to_silver.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/client.py` & `labelspark-0.7.32/labelspark/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         if verbose:
             print(f"Success: DataFrame generated")
         
         return df        
     
     def export_to_delta_table(self, project, 
         include_metadata:bool=False, include_performance:bool=False, include_agreement:bool=False,
-        verbose:bool=False, mask_method:str="png", divider="///", table_path="", write_mode="overwrite", spark:pyspark.sql.SparkSession=None, spark_config:dict={}):
+        verbose:bool=False, mask_method:str="png", divider="///", table_path="", write_mode="append", spark:pyspark.sql.SparkSession=None, spark_config:dict={}):
         """ Creates a Spark Dataframe and saves it to a Databricks Delta Table
         Args:
             project                 :   Required (str / lablebox.Project) - Labelbox Project ID or lablebox.Project object to export labels from
             include_metadata        :   Optional (bool) - If included, exports metadata fields
             include_performance     :   Optional (bool) - If included, exports labeling performance
             include_agreement       :   Optional (bool) - If included, exports consensus scores       
             verbose                 :   Optional (bool) - If True, prints details about code execution; if False, prints minimal information
@@ -104,14 +104,17 @@
                                                 
                                             - GCS:
                                                 {
                                                     "jars": [<path to gcs-connector-hadoop2-latest.jar file>],
                                                     "credentials": <path to GCS service account json keyfile>
                                                 }"""
 
+        if write_mode not in ['append', 'overwrite']:
+            raise ValueError(f"The Delta Table write mode must be either 'append' or 'overwrite', the write mode provided is {write_mode}")
+        
         if spark is None:
             spark = self.get_spark_session(table_path, spark_config)
         sc = spark.sparkContext
         
         flattened_labels_dict = export_and_flatten_labels(
             client=self.lb_client, project=project, 
             include_metadata=include_metadata, include_performance=include_performance, include_agreement=include_agreement,
```

### Comparing `labelspark-0.7.31/labelspark/connector.py` & `labelspark-0.7.32/labelspark/connector.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/create_dataset.py` & `labelspark-0.7.32/labelspark/create_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/create_labelbox_dataset.py` & `labelspark-0.7.32/labelspark/create_labelbox_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/dataframe_schema_enrichment.py` & `labelspark-0.7.32/labelspark/dataframe_schema_enrichment.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/flatten_bronze_table.py` & `labelspark-0.7.32/labelspark/flatten_bronze_table.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/get_annotations.py` & `labelspark-0.7.32/labelspark/get_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/get_videoframe_annotations.py` & `labelspark-0.7.32/labelspark/get_videoframe_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/spark_schema_to_string.py` & `labelspark-0.7.32/labelspark/spark_schema_to_string.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/update_metadata.py` & `labelspark-0.7.32/labelspark/update_metadata.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark/uploader.py` & `labelspark-0.7.32/labelspark/uploader.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/labelspark.egg-info/PKG-INFO` & `labelspark-0.7.32/labelspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.31
+Version: 0.7.32
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `labelspark-0.7.31/labelspark.egg-info/SOURCES.txt` & `labelspark-0.7.32/labelspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.31/setup.py` & `labelspark-0.7.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelspark',
-    version='0.7.31',
+    version='0.7.32',
     author='Labelbox',
     author_email="raphael@labelbox.com",      
     packages=find_packages(),
     url='https://github.com/Labelbox/LabelSpark.git',
     description='Labelbox Connector for Databricks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

