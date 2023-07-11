# Comparing `tmp/airflow-provider-lakefs-0.46.1.tar.gz` & `tmp/airflow-provider-lakefs-0.46.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-lakefs-0.46.1.tar", last modified: Wed May  3 07:44:59 2023, max compression
+gzip compressed data, was "airflow-provider-lakefs-0.46.2.tar", last modified: Tue Jul 11 10:47:16 2023, max compression
```

## Comparing `airflow-provider-lakefs-0.46.1.tar` & `airflow-provider-lakefs-0.46.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.122530 airflow-provider-lakefs-0.46.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 07:44:49.000000 airflow-provider-lakefs-0.46.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-03 07:44:59.122530 airflow-provider-lakefs-0.46.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-03 07:44:49.000000 airflow-provider-lakefs-0.46.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.118530 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-03 07:44:59.000000 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 07:44:59.000000 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:44:59.000000 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 07:44:59.000000 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 07:44:59.000000 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 07:44:59.000000 airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.118530 airflow-provider-lakefs-0.46.1/lakefs_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-03 07:44:49.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.118530 airflow-provider-lakefs-0.46.1/lakefs_provider/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:49.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/example_dags/lakefs-dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.118530 airflow-provider-lakefs-0.46.1/lakefs_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/hooks/lakefs_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.118530 airflow-provider-lakefs-0.46.1/lakefs_provider/links/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/links/lakefs_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.122530 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/commit_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/create_branch_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/create_symlink_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/get_commit_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/get_object_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/merge_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/upload_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/operators/with_metadata_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:59.122530 airflow-provider-lakefs-0.46.1/lakefs_provider/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/sensors/commit_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/lakefs_provider/sensors/file_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:44:59.122530 airflow-provider-lakefs-0.46.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 07:44:50.000000 airflow-provider-lakefs-0.46.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.553331 airflow-provider-lakefs-0.46.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-11 10:47:16.553331 airflow-provider-lakefs-0.46.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.549331 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-11 10:47:16.000000 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-11 10:47:16.000000 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:47:16.000000 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 10:47:16.000000 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 10:47:16.000000 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:47:16.000000 airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.549331 airflow-provider-lakefs-0.46.2/lakefs_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.549331 airflow-provider-lakefs-0.46.2/lakefs_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/example_dags/lakefs-dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.549331 airflow-provider-lakefs-0.46.2/lakefs_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/hooks/lakefs_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.549331 airflow-provider-lakefs-0.46.2/lakefs_provider/links/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/links/lakefs_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.553331 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/commit_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/create_branch_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/create_symlink_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/get_commit_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/get_object_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/merge_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/upload_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/operators/with_metadata_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:16.553331 airflow-provider-lakefs-0.46.2/lakefs_provider/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/sensors/commit_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/lakefs_provider/sensors/file_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:47:16.553331 airflow-provider-lakefs-0.46.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 10:47:06.000000 airflow-provider-lakefs-0.46.2/setup.py
```

### Comparing `airflow-provider-lakefs-0.46.1/LICENSE` & `airflow-provider-lakefs-0.46.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/PKG-INFO` & `airflow-provider-lakefs-0.46.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-lakefs
-Version: 0.46.1
+Version: 0.46.2
 Summary: A lakeFS provider package built by Treeverse.
 Home-page: https://lakefs.io
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `airflow-provider-lakefs-0.46.1/README.md` & `airflow-provider-lakefs-0.46.2/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/PKG-INFO` & `airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-lakefs
-Version: 0.46.1
+Version: 0.46.2
 Summary: A lakeFS provider package built by Treeverse.
 Home-page: https://lakefs.io
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `airflow-provider-lakefs-0.46.1/airflow_provider_lakefs.egg-info/SOURCES.txt` & `airflow-provider-lakefs-0.46.2/airflow_provider_lakefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/__init__.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/example_dags/lakefs-dag.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/example_dags/lakefs-dag.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/hooks/lakefs_hook.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/hooks/lakefs_hook.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/links/lakefs_link.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/links/lakefs_link.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/commit_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/commit_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/create_branch_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/create_branch_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/create_symlink_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/create_symlink_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/get_commit_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/get_commit_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/get_object_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/get_object_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/merge_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/merge_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/upload_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/upload_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/operators/with_metadata_operator.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/operators/with_metadata_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 
     # DAG metadata to add to commit, expanded after fetching appropriate
     # metadata.  The key of each metadata item will be prefixed
     # "::lakefs::".
     __metadata_templates = {
         "dag_run_id": "{{dag_run.run_id}}",
         "dag_id": "{{dag.dag_id}}",
-        "logical_date": "{{logical_date}}",
+        "logical_date[iso8601]": "{{logical_date}}",
         "data_interval_start[iso8601]": "{{data_interval_start}}",
         "data_interval_end[iso8601]": "{{data_interval_end}}",
-        "last_scheduling_decision": "{{dag_run.last_scheduling_decision}}",
+        "last_scheduling_decision[iso8601]": "{{dag_run.last_scheduling_decision}}",
         "run_type": "{{dag_run.run_type}}",
-        "external_trigger": "{{dag_run.external_trigger}}",
-        "conf": "{{params}}",
+        "external_trigger[boolean]": "{{dag_run.external_trigger}}",
         "note": "{{dag_run.note}}",
         # build_airflow_url_with_query can only run from a Flask app
         # context.  Fake URLs instead.
         "url[url:id]": '{{endpoint_url}}/api/v1/dags/{{dag.dag_id}}/dagRuns/{{dag_run.run_id}}',
         "url[url:ui]": '{{endpoint_url}}/dags/{{dag.dag_id}}/graph?dag_run_id={{dag_run.run_id}}&root=&logical_date={{logical_date}}',
     }
```

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/sensors/commit_sensor.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/sensors/commit_sensor.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/lakefs_provider/sensors/file_sensor.py` & `airflow-provider-lakefs-0.46.2/lakefs_provider/sensors/file_sensor.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.46.1/setup.py` & `airflow-provider-lakefs-0.46.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 """Perform the package airflow-provider-lakeFS setup."""
 setup(
     name='airflow-provider-lakefs',
-    version='0.46.1',
+    version='0.46.2',
     description='A lakeFS provider package built by Treeverse.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         "apache_airflow_provider": [
             "provider_info=lakefs_provider.__init__:get_provider_info"
         ]
```

