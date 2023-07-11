# Comparing `tmp/yetl-framework-1.6.6.dev3.tar.gz` & `tmp/yetl-framework-1.6.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.6.6.dev3.tar", last modified: Sat Jul  8 11:02:35 2023, max compression
+gzip compressed data, was "yetl-framework-1.6.6.dev4.tar", last modified: Tue Jul 11 14:33:33 2023, max compression
```

## Comparing `yetl-framework-1.6.6.dev3.tar` & `yetl-framework-1.6.6.dev4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.760224 yetl-framework-1.6.6.dev3/
--rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-08 11:02:35.760224 yetl-framework-1.6.6.dev3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-08 11:02:35.760224 yetl-framework-1.6.6.dev3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1251 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.756224 yetl-framework-1.6.6.dev3/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.756224 yetl-framework-1.6.6.dev3/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.756224 yetl-framework-1.6.6.dev3/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16286 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.756224 yetl-framework-1.6.6.dev3/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.756224 yetl-framework-1.6.6.dev3/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4920 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.760224 yetl-framework-1.6.6.dev3/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-08 11:01:31.000000 yetl-framework-1.6.6.dev3/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 11:02:35.760224 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-08 11:02:35.000000 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-08 11:02:35.000000 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-08 11:02:35.000000 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-08 11:02:35.000000 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       73 2023-07-08 11:02:35.000000 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-08 11:02:35.000000 yetl-framework-1.6.6.dev3/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.921040 yetl-framework-1.6.6.dev4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-11 14:33:33.921040 yetl-framework-1.6.6.dev4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-11 14:33:33.921040 yetl-framework-1.6.6.dev4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1251 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.917040 yetl-framework-1.6.6.dev4/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.917040 yetl-framework-1.6.6.dev4/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.917040 yetl-framework-1.6.6.dev4/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16741 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.917040 yetl-framework-1.6.6.dev4/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.921040 yetl-framework-1.6.6.dev4/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4980 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.921040 yetl-framework-1.6.6.dev4/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-11 14:32:30.000000 yetl-framework-1.6.6.dev4/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 14:33:33.921040 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-11 14:33:33.000000 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-11 14:33:33.000000 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-11 14:33:33.000000 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-11 14:33:33.000000 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       73 2023-07-11 14:33:33.000000 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-11 14:33:33.000000 yetl-framework-1.6.6.dev4/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.6.6.dev3/PKG-INFO` & `yetl-framework-1.6.6.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.6.dev3
+Version: 1.6.6.dev4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.6.dev3/README.md` & `yetl-framework-1.6.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/setup.py` & `yetl-framework-1.6.6.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.6.6.dev3",
+    version="1.6.6.dev4",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.6.6.dev3/yetl/__main__.py` & `yetl-framework-1.6.6.dev4/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/cli/_init.py` & `yetl-framework-1.6.6.dev4/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.6.6.dev4/yetl/cli/metadata_provider/_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     table = "table"
     sql = "sql"
     id = "id"
     depends_on = "depends_on"
     deltalake = "deltalake"
     identity = "identity"
     partition_by = "partition_by"
+    cluster_by = "cluster_by"
     delta_constraints = "delta_constraints"
     z_order_by = "z_order_by"
     delta_properties = "delta_properties"
     exception_thresholds = "exception_thresholds"
     warning_thresholds = "warning_thresholds"
     invalid_ratio = "invalid_ratio"
     invalid_rows = "invalid_rows"
@@ -48,14 +49,15 @@
         ColumnNames.table: str,
         ColumnNames.sql: str,
         ColumnNames.id: str,
         ColumnNames.depends_on: str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
+        f"{ColumnNames.deltalake}_{ColumnNames.cluster_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": int,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_rows}": np.float64,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.max_rows}": np.float64,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.min_rows}": np.float64,
@@ -76,14 +78,15 @@
     sql: str = Field(default=None)
     id: str = Field(default=None)
     depends_on: str = Field(default=None)
     deltalake_delta_properties: str = Field(default=None)
     custom_properties: Dict[str, Any] = Field(default=None)
     deltalake_identity: str = Field(default=None)
     deltalake_partition_by: str = Field(default=None)
+    deltalake_cluster_by: str = Field(default=None)
     deltalake_delta_constraints: str = Field(default=None)
     deltalake_z_order_by: str = Field(default=None)
     deltalake_vacuum: Union[int, None] = Field(default=None)
     warning_thresholds_invalid_ratio: float = Field(default=None)
     warning_thresholds_invalid_rows: int = Field(default=None)
     warning_thresholds_max_rows: int = Field(default=None)
     warning_thresholds_min_rows: int = Field(default=None)
@@ -147,14 +150,15 @@
             [
                 self.sql is not None,
                 self.id is not None,
                 self.depends_on is not None,
                 self.deltalake_delta_properties is not None,
                 self.deltalake_identity is not None,
                 self.deltalake_partition_by is not None,
+                self.deltalke_cluster_by is not None,
                 self.deltalake_delta_constraints is not None,
                 self.deltalake_z_order_by is not None,
                 self._has_warning_thresholds(),
                 self._has_exception_thresholds(),
             ]
         )
 
@@ -229,14 +233,18 @@
                 table[ColumnNames.id.name] = self._get_list(self.id)
             if self.sql is not None and self.sql.lower() == "y":
                 table["sql"] = "../sql/{{database}}/{{table}}.sql"
             if self.deltalake_partition_by is not None:
                 table[ColumnNames.partition_by.name] = self._get_list(
                     self.deltalake_partition_by
                 )
+            if self.deltalake_cluster_by is not None:
+                table[ColumnNames.cluster_by.name] = self._get_list(
+                    self.deltalake_cluster_by
+                )
             if self.deltalake_z_order_by is not None:
                 table[ColumnNames.z_order_by.name] = self._get_list(
                     self.deltalake_z_order_by
                 )
             if self.deltalake_vacuum is not None:
                 table[ColumnNames.vacuum.name] = self._get_list(self.deltalake_vacuum)
             if self.deltalake_delta_properties is not None:
@@ -273,14 +281,15 @@
         ColumnNames.table: str,
         ColumnNames.sql: str,
         ColumnNames.id: str,
         ColumnNames.depends_on: str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
+        f"{ColumnNames.deltalake}_{ColumnNames.cluster_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": str,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_rows}": np.float64,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.max_rows}": np.float64,
         f"{ColumnNames.warning_thresholds}_{ColumnNames.min_rows}": np.float64,
```

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/__init__.py` & `yetl-framework-1.6.6.dev4/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_config.py` & `yetl-framework-1.6.6.dev4/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_decorators.py` & `yetl-framework-1.6.6.dev4/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_logging_config.py` & `yetl-framework-1.6.6.dev4/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_project.py` & `yetl-framework-1.6.6.dev4/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_spark_context.py` & `yetl-framework-1.6.6.dev4/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_tables.py` & `yetl-framework-1.6.6.dev4/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_timeslice.py` & `yetl-framework-1.6.6.dev4/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/_utils.py` & `yetl-framework-1.6.6.dev4/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/deltalake.py` & `yetl-framework-1.6.6.dev4/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/table/_deltalake.py` & `yetl-framework-1.6.6.dev4/yetl/config/table/_deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     _spark: DeltaLakeFn = PrivateAttr(default=None)
     depends_on: List[str] = Field(default=[])
     delta_properties: Dict[str, str] = Field(default=None)
     delta_constraints: Dict[str, str] = Field(default=None)
     partition_by: Union[List[str], str] = Field(default=None)
+    cluster_by: Union[List[str], str] = Field(default=None)
     z_order_by: Union[List[str], str] = Field(default=None)
     vacuum: int = Field(default=31)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     stage: StageType = Field(...)
     managed: bool = Field(default=False)
```

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/table/_factory.py` & `yetl-framework-1.6.6.dev4/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/table/_read.py` & `yetl-framework-1.6.6.dev4/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/config/table/_table.py` & `yetl-framework-1.6.6.dev4/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/workflow/_dlt.py` & `yetl-framework-1.6.6.dev4/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.6.6.dev4/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev3/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.6.6.dev4/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.6.dev3
+Version: 1.6.6.dev4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.6.dev3/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.6.6.dev4/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

