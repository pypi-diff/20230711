# Comparing `tmp/apitable-1.2.0.tar.gz` & `tmp/apitable-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apitable-1.2.0.tar", last modified: Mon Mar 13 07:42:56 2023, max compression
+gzip compressed data, was "dist/apitable-1.2.1.tar", last modified: Tue Jul 11 02:11:03 2023, max compression
```

## Comparing `apitable-1.2.0.tar` & `apitable-1.2.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-03-13 07:42:56.000000 apitable-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-03-13 07:42:47.000000 apitable-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/apitable.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable/datasheet/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/datasheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/datasheet_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/query_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/datasheet/view_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable/node/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/node/node_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable/space/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/space/space_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable/types/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/embedlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/space.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/types/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-13 07:42:47.000000 apitable-1.2.0/apitable/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-03-13 07:42:55.000000 apitable-1.2.0/apitable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-13 07:42:56.000000 apitable-1.2.0/apitable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 07:42:55.000000 apitable-1.2.0/apitable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-13 07:42:55.000000 apitable-1.2.0/apitable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 07:42:55.000000 apitable-1.2.0/apitable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 07:42:56.000000 apitable-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-13 07:42:47.000000 apitable-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:42:56.000000 apitable-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_create_datasheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_create_embed_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_create_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_create_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_delete_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_delete_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_get_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_get_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_get_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_get_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_update_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_upload_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-13 07:42:47.000000 apitable-1.2.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-07-11 02:11:03.000000 apitable-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-11 02:10:52.000000 apitable-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/apitable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable/datasheet/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/datasheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/datasheet_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/query_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/datasheet/view_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/node/node_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable/space/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/space/space_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/embedlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/unit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/types/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-11 02:10:52.000000 apitable-1.2.1/apitable/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 02:11:03.000000 apitable-1.2.1/apitable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:11:03.000000 apitable-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 02:10:52.000000 apitable-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:11:03.000000 apitable-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_create_datasheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_create_embed_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_create_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_create_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_delete_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_delete_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_get_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_get_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_get_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_get_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_update_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-11 02:10:52.000000 apitable-1.2.1/test/test_utils.py
```

### Comparing `apitable-1.2.0/PKG-INFO` & `apitable-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: apitable
-Version: 1.2.0
+Version: 1.2.1
 Summary: Apitable Python SDK
 Home-page: https://github.com/apitable/apitable-sdks
 Author: apitable
 Author-email: dev@apitable.com
 License: UNKNOWN
 Description: # APITable.py
+        
         [![Latest Version](https://shields.mitmproxy.org/pypi/v/apitable.svg)](https://pypi.python.org/pypi/apitable)
         
         It is the official package for the Fusion API of APITable, and provides an API similar to the Django ORM style.
         
         # Requirements
+        
         python3.6 +
         
         If you want to call apitable rest api, you need get the API Token first: visit the workbench of APITable, click the avatar in the lower left corner, and go to User Center > Developer Configuration. Click to generate Token (you need to bind your email for the first time).
         
         # Installation
+        
         ```shell
         pip install --upgrade apitable
         ```
         
         # Getting started
         
         ## Example
@@ -139,14 +142,15 @@
         bug = apitable.datasheet("dstn2lEFltyGHe2j86", field_key="id", field_key_map={
             "title": "flddpSLHEzDPQ",
             "state": "fldwvNDf9teD2",
         })
         ```
         
         # Documentation
+        
         ## records
         
         `dst.records` manage records in datasheets.
         
         | Method           | Parameter             | Type        | Description                                                                                                                                                                    | Example                                                                                                        |
         | ---------------- | --------------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
         | create           | dict                  | Record      | Create a single record                                                                                                                                                         | `dst.records.create({"title":"new title"})`                                                                    |
@@ -182,15 +186,15 @@
         | Method/Attribute | Parameter | Type | Description                                                              | Example         |
         | ---------------- | --------- | ---- | ------------------------------------------------------------------------ | --------------- |
         | json             | /         | dict | Returns all field values of the current record                           | `record.json()` |
         | \_id             | /         | str  | \_id is a reserved attribute, returns the recordId of the current record | `record._id`    |
         
         ## Field
         
-        The mapping relationship between Field and Python data structure. The data with empty cells in the dimension table is always null, and the records returned by the API will not contain fields with null values.
+        The mapping relationship between Field and Python data structure. The data with empty cells in the datasheet is always null, and the records returned by the API will not contain fields with null values.
         
         | Field Type       | Data type           |
         | ---------------- | ------------------- |
         | SingleText       | str                 |
         | Text             | str                 |
         | SingleSelect     | str                 |
         | MultiSelect      | str[]               |
@@ -210,15 +214,15 @@
         | Rating           | int                 |
         | CreatedBy        | unit object         |
         | LastModifiedBy   | unit object         |
         | MagicLink        | str[]               |
         | MagicLookUp      | any[]               |
         | Formula          | str / bool          |
         
-        ## all 
+        ## all
         
         all method will automatically handle paging loading all resources
         
         _When the paging-related parameters (pageNum, pageSize) are passed in, the SDK will no longer automatically load all records, and only return the specified page data_。
         
         > Try to avoid using the dst.records.all method without parameters to get all the data.
         > The API can obtain a maximum of 1000 pieces of data per request. If your data volume is too large, it is close to the limit of 50000. In the case of no parameters, calling all will serially request the API 50 times. Not only is it very slow, but it consumes API request credit.
@@ -254,17 +258,16 @@
         | filterByFormula | str                | Returns matching records using formulas as filter criteria                                                  |                                       |
         | maxRecords      | int                | Limit the number of records returned, the default is 5000                                                   |                                       |
         | cellFormat      | 'json' or 'string' | Defaults to 'json', when specified as 'string' all values will be automatically converted to string format. |                                       |
         | fieldKey        | 'name' or 'id'     | Specifies the field query and returned key. The column name 'name' is used by default.                      |                                       |
         
         See: [Tutorial getting started with formulas](https://help.apitable.com/docs/guide/tutorial-getting-started-with-formulas)
         
-        
-        
         ## FAQ
+        
         ### Can I get the field type (meta) information of the datasheet?
         
         Can be get through the fields/views API.
         
         ### Can option be created automatically?
         
         If you write to a non-existent option, the option will be created automatically
@@ -278,19 +281,23 @@
         10 records. In the future, we will adjust the size of this limit according to the actual situation.
         
         ### Can more records be fetched per request?
         
         The current maximum is 1000 records. In the future, we will adjust the size of this limit according to the actual situation.
         
         # Development and test
+        
         Create a new `.env`, the content can refer to `.env.example`.
+        
         ```shell
         cp .env .env.example
         ```
+        
         Then modify the test code in the `test/` folder for testing.
+        
         ```shell
         pipenv install --pre
         pipenv shell
         python -m unittest test
         ```
         
 Platform: UNKNOWN
```

### Comparing `apitable-1.2.0/README.md` & `apitable-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # APITable.py
+
 [![Latest Version](https://shields.mitmproxy.org/pypi/v/apitable.svg)](https://pypi.python.org/pypi/apitable)
 
 It is the official package for the Fusion API of APITable, and provides an API similar to the Django ORM style.
 
 # Requirements
+
 python3.6 +
 
 If you want to call apitable rest api, you need get the API Token first: visit the workbench of APITable, click the avatar in the lower left corner, and go to User Center > Developer Configuration. Click to generate Token (you need to bind your email for the first time).
 
 # Installation
+
 ```shell
 pip install --upgrade apitable
 ```
 
 # Getting started
 
 ## Example
@@ -131,14 +134,15 @@
 bug = apitable.datasheet("dstn2lEFltyGHe2j86", field_key="id", field_key_map={
     "title": "flddpSLHEzDPQ",
     "state": "fldwvNDf9teD2",
 })
 ```
 
 # Documentation
+
 ## records
 
 `dst.records` manage records in datasheets.
 
 | Method           | Parameter             | Type        | Description                                                                                                                                                                    | Example                                                                                                        |
 | ---------------- | --------------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
 | create           | dict                  | Record      | Create a single record                                                                                                                                                         | `dst.records.create({"title":"new title"})`                                                                    |
@@ -174,15 +178,15 @@
 | Method/Attribute | Parameter | Type | Description                                                              | Example         |
 | ---------------- | --------- | ---- | ------------------------------------------------------------------------ | --------------- |
 | json             | /         | dict | Returns all field values of the current record                           | `record.json()` |
 | \_id             | /         | str  | \_id is a reserved attribute, returns the recordId of the current record | `record._id`    |
 
 ## Field
 
-The mapping relationship between Field and Python data structure. The data with empty cells in the dimension table is always null, and the records returned by the API will not contain fields with null values.
+The mapping relationship between Field and Python data structure. The data with empty cells in the datasheet is always null, and the records returned by the API will not contain fields with null values.
 
 | Field Type       | Data type           |
 | ---------------- | ------------------- |
 | SingleText       | str                 |
 | Text             | str                 |
 | SingleSelect     | str                 |
 | MultiSelect      | str[]               |
@@ -202,15 +206,15 @@
 | Rating           | int                 |
 | CreatedBy        | unit object         |
 | LastModifiedBy   | unit object         |
 | MagicLink        | str[]               |
 | MagicLookUp      | any[]               |
 | Formula          | str / bool          |
 
-## all 
+## all
 
 all method will automatically handle paging loading all resources
 
 _When the paging-related parameters (pageNum, pageSize) are passed in, the SDK will no longer automatically load all records, and only return the specified page data_。
 
 > Try to avoid using the dst.records.all method without parameters to get all the data.
 > The API can obtain a maximum of 1000 pieces of data per request. If your data volume is too large, it is close to the limit of 50000. In the case of no parameters, calling all will serially request the API 50 times. Not only is it very slow, but it consumes API request credit.
@@ -246,17 +250,16 @@
 | filterByFormula | str                | Returns matching records using formulas as filter criteria                                                  |                                       |
 | maxRecords      | int                | Limit the number of records returned, the default is 5000                                                   |                                       |
 | cellFormat      | 'json' or 'string' | Defaults to 'json', when specified as 'string' all values will be automatically converted to string format. |                                       |
 | fieldKey        | 'name' or 'id'     | Specifies the field query and returned key. The column name 'name' is used by default.                      |                                       |
 
 See: [Tutorial getting started with formulas](https://help.apitable.com/docs/guide/tutorial-getting-started-with-formulas)
 
-
-
 ## FAQ
+
 ### Can I get the field type (meta) information of the datasheet?
 
 Can be get through the fields/views API.
 
 ### Can option be created automatically?
 
 If you write to a non-existent option, the option will be created automatically
@@ -270,17 +273,21 @@
 10 records. In the future, we will adjust the size of this limit according to the actual situation.
 
 ### Can more records be fetched per request?
 
 The current maximum is 1000 records. In the future, we will adjust the size of this limit according to the actual situation.
 
 # Development and test
+
 Create a new `.env`, the content can refer to `.env.example`.
+
 ```shell
 cp .env .env.example
 ```
+
 Then modify the test code in the `test/` folder for testing.
+
 ```shell
 pipenv install --pre
 pipenv shell
 python -m unittest test
 ```
```

### Comparing `apitable-1.2.0/apitable/apitable.py` & `apitable-1.2.1/apitable/apitable.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/datasheet/datasheet.py` & `apitable-1.2.1/apitable/datasheet/datasheet.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/datasheet/datasheet_manager.py` & `apitable-1.2.1/apitable/datasheet/datasheet_manager.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/datasheet/field_manager.py` & `apitable-1.2.1/apitable/datasheet/field_manager.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/datasheet/query_set.py` & `apitable-1.2.1/apitable/datasheet/query_set.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/datasheet/record.py` & `apitable-1.2.1/apitable/datasheet/record.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/datasheet/record_manager.py` & `apitable-1.2.1/apitable/datasheet/record_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         raise Exception(resp.message)
 
     def all(self, **kwargs):
         """
         Filter records by query conditions, see get records query params https://developers.apitable.com/api-reference#operation/get-records
         @param kwargs:
             - viewId: 'viewId1',View ID. Defaults to the first view in the Apitable. The request will return the filtered/sorted results in the view, and you can use the fields parameter to filter unwanted field data
-            - sort: [{ 'Field name or ID': 'asc' }] sorts the records of the specified dimensional grid. An array of multiple "sort objects". Support order: 'asc' and reverse order: 'desc'. Note: The sorting conditions specified by this parameter will override the sorting conditions in the view.
+            - sort: [{ 'Field name or ID': 'asc' }] sorts the records of the specified datasheet. An array of multiple "sort objects". Support order: 'asc' and reverse order: 'desc'. Note: The sorting conditions specified by this parameter will override the sorting conditions in the view.
             - recordIds: ['recordId1', 'recordId2'], array of recordIds. If this parameter is included, the records array specified in the parameter is returned. The returned values are sorted in the order passed in the array. Filtering and sorting are ignored at this time. No paging, at most 1000 items per query
             - fields: ['title', 'detail', 'Citations'], specify the field to be returned (the default is the field name, or it can be specified as the field Id through fieldKey). If this parameter is included, the returned record collection will be filtered, and only the specified fields will be returned.
             - filterByFormula: '{Citations} >  0', use formulas as filter conditions to return matching records, visit https://help.apitable.com/docs/guide/tutorial-getting-started-with-formulas to learn how to use formulas
             - maxRecords: 5000, limits the total number of records returned. If this value is less than the actual total number of records in the table, the total number of records returned is limited to this value.
             - cellFormat: 'json', cell value type, the default is 'json', when specified as 'string', all values will be automatically converted to string format.
             - fieldKey: 'name', specifies the field's query and returned key. The column name 'name' is used by default. When specified as 'id', fieldId will be used as the query and return method (using id can avoid the problem of code failure caused by modification of column names)
         @return:
```

### Comparing `apitable-1.2.0/apitable/exceptions.py` & `apitable-1.2.1/apitable/exceptions.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/node/node_manager.py` & `apitable-1.2.1/apitable/node/node_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib.parse import urljoin
 
 from apitable.types.response import (
     GETNodeListResponse,
-    GETNodeDetailResponse
+    GETNodeDetailResponse,
+    GETSearchNodeListResponse
 )
 from apitable.utils import handle_response
 
 
 class NodeManager:
     def __init__(self, apitable: 'Apitable', **kwargs):
         self.apitable = apitable
@@ -23,14 +24,26 @@
 
     def _get_node_detail(self, node_id: str) -> GETNodeDetailResponse:
         node_detail_resp = self.apitable.request.get(
             urljoin(self.apitable.api_base, f"/fusion/v1/nodes/{node_id}")
         )
         return handle_response(node_detail_resp, GETNodeDetailResponse)
 
+    def _search_nodes(self, space_id: str, **kwargs) -> GETSearchNodeListResponse:
+        search_node_list_resp = self.apitable.request.get(
+            urljoin(self.apitable.api_base, f"/fusion/v2/spaces/{space_id}/nodes"),
+            params=kwargs
+        )
+        return handle_response(search_node_list_resp, GETSearchNodeListResponse)
+    
+    def search(self, **kwargs):
+        space_id = kwargs.get('spaceId', self.space_id)
+        nodes_resp = self._search_nodes(space_id, **kwargs)
+        return nodes_resp.data.nodes
+
     def all(self, **kwargs):
         """
         apitable.nodes.all(spaceId='spcxxxxxx') Get the list of files in the root of the specified space
         """
         space_id = kwargs.get('spaceId', self.space_id)
         nodes_resp = self._get_nodes(space_id)
         return nodes_resp.data.nodes
```

### Comparing `apitable-1.2.0/apitable/request.py` & `apitable-1.2.1/apitable/request.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/space/space.py` & `apitable-1.2.1/apitable/space/space.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from apitable.node import NodeManager
-from apitable.utils import get_dst_id, handle_response
+from urllib.parse import urljoin
+
 from apitable.datasheet import Datasheet, DatasheetManager
+from apitable.node import NodeManager
 from apitable.types.response import PostDatasheetMetaResponse
-from urllib.parse import urljoin
+from apitable.unit import Member, Role, Team
+from apitable.utils import get_dst_id, handle_response
 
 
 class Space:
     def __init__(self, apitable: 'Apitable', space_id: str):
         self.apitable = apitable
         self.id = space_id
 
@@ -14,14 +16,35 @@
     def nodes(self):
         return NodeManager(self.apitable, space_id=self.id)
 
     @property
     def datasheets(self):
         return DatasheetManager(self)
 
+    @property
+    def member(self):
+        """
+        Space member.
+        """
+        return Member(self)
+
+    @property
+    def role(self):
+        """
+        Space role.
+        """
+        return Role(self)
+
+    @property
+    def team(self):
+        """
+        Space team.
+        """
+        return Team(self)
+
     def datasheet(self, dst_id_or_url, **kwargs):
         """
         @param dst_id_or_url: Datasheet ID or URL
         @param kwargs:
             - field_key: 'id' or 'name' 
             - field_key_map: Field Mapping Dictionary. More info: https://github.com/apitable/apitable-sdks/tree/develop/apitable.py#Field-mapping
         @return:
```

### Comparing `apitable-1.2.0/apitable/space/space_manager.py` & `apitable-1.2.1/apitable/space/space_manager.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/types/embedlink.py` & `apitable-1.2.1/apitable/types/embedlink.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/types/field.py` & `apitable-1.2.1/apitable/types/field.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/types/record.py` & `apitable-1.2.1/apitable/types/record.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable/types/response.py` & `apitable-1.2.1/apitable/types/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Any, List, Optional
 
 from apitable.types.embedlink import EmbedLinkThemeEnum, EmbedLinkPayload
-from apitable.types.node import NodeListItem, NodeDetail
+from apitable.types.node import NodeListItem, NodeDetail, NodeSearchInfo
 from apitable.types.space import SpaceListItem
 from apitable.types.record import RawRecord
 from apitable.types.view import MetaView
 from apitable.types.field import MetaField
 from pydantic import BaseModel
 
 
@@ -106,14 +106,20 @@
 class GETNodeListResponseData(BaseModel):
     nodes: List[NodeListItem]
 
 
 class GETNodeListResponse(ResponseBase):
     data: GETNodeListResponseData
 
+class GETSearchNodeListResponseData(BaseModel):
+    nodes: List[NodeSearchInfo]
+
+class GETSearchNodeListResponse(ResponseBase):
+    data: GETSearchNodeListResponseData
+
 
 class GETNodeDetailResponse(ResponseBase):
     data: NodeDetail
 
 
 class PostDatasheetMetaResponseData(BaseModel):
     id: str
```

### Comparing `apitable-1.2.0/apitable/utils.py` & `apitable-1.2.1/apitable/utils.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/apitable.egg-info/PKG-INFO` & `apitable-1.2.1/apitable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: apitable
-Version: 1.2.0
+Version: 1.2.1
 Summary: Apitable Python SDK
 Home-page: https://github.com/apitable/apitable-sdks
 Author: apitable
 Author-email: dev@apitable.com
 License: UNKNOWN
 Description: # APITable.py
+        
         [![Latest Version](https://shields.mitmproxy.org/pypi/v/apitable.svg)](https://pypi.python.org/pypi/apitable)
         
         It is the official package for the Fusion API of APITable, and provides an API similar to the Django ORM style.
         
         # Requirements
+        
         python3.6 +
         
         If you want to call apitable rest api, you need get the API Token first: visit the workbench of APITable, click the avatar in the lower left corner, and go to User Center > Developer Configuration. Click to generate Token (you need to bind your email for the first time).
         
         # Installation
+        
         ```shell
         pip install --upgrade apitable
         ```
         
         # Getting started
         
         ## Example
@@ -139,14 +142,15 @@
         bug = apitable.datasheet("dstn2lEFltyGHe2j86", field_key="id", field_key_map={
             "title": "flddpSLHEzDPQ",
             "state": "fldwvNDf9teD2",
         })
         ```
         
         # Documentation
+        
         ## records
         
         `dst.records` manage records in datasheets.
         
         | Method           | Parameter             | Type        | Description                                                                                                                                                                    | Example                                                                                                        |
         | ---------------- | --------------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
         | create           | dict                  | Record      | Create a single record                                                                                                                                                         | `dst.records.create({"title":"new title"})`                                                                    |
@@ -182,15 +186,15 @@
         | Method/Attribute | Parameter | Type | Description                                                              | Example         |
         | ---------------- | --------- | ---- | ------------------------------------------------------------------------ | --------------- |
         | json             | /         | dict | Returns all field values of the current record                           | `record.json()` |
         | \_id             | /         | str  | \_id is a reserved attribute, returns the recordId of the current record | `record._id`    |
         
         ## Field
         
-        The mapping relationship between Field and Python data structure. The data with empty cells in the dimension table is always null, and the records returned by the API will not contain fields with null values.
+        The mapping relationship between Field and Python data structure. The data with empty cells in the datasheet is always null, and the records returned by the API will not contain fields with null values.
         
         | Field Type       | Data type           |
         | ---------------- | ------------------- |
         | SingleText       | str                 |
         | Text             | str                 |
         | SingleSelect     | str                 |
         | MultiSelect      | str[]               |
@@ -210,15 +214,15 @@
         | Rating           | int                 |
         | CreatedBy        | unit object         |
         | LastModifiedBy   | unit object         |
         | MagicLink        | str[]               |
         | MagicLookUp      | any[]               |
         | Formula          | str / bool          |
         
-        ## all 
+        ## all
         
         all method will automatically handle paging loading all resources
         
         _When the paging-related parameters (pageNum, pageSize) are passed in, the SDK will no longer automatically load all records, and only return the specified page data_。
         
         > Try to avoid using the dst.records.all method without parameters to get all the data.
         > The API can obtain a maximum of 1000 pieces of data per request. If your data volume is too large, it is close to the limit of 50000. In the case of no parameters, calling all will serially request the API 50 times. Not only is it very slow, but it consumes API request credit.
@@ -254,17 +258,16 @@
         | filterByFormula | str                | Returns matching records using formulas as filter criteria                                                  |                                       |
         | maxRecords      | int                | Limit the number of records returned, the default is 5000                                                   |                                       |
         | cellFormat      | 'json' or 'string' | Defaults to 'json', when specified as 'string' all values will be automatically converted to string format. |                                       |
         | fieldKey        | 'name' or 'id'     | Specifies the field query and returned key. The column name 'name' is used by default.                      |                                       |
         
         See: [Tutorial getting started with formulas](https://help.apitable.com/docs/guide/tutorial-getting-started-with-formulas)
         
-        
-        
         ## FAQ
+        
         ### Can I get the field type (meta) information of the datasheet?
         
         Can be get through the fields/views API.
         
         ### Can option be created automatically?
         
         If you write to a non-existent option, the option will be created automatically
@@ -278,19 +281,23 @@
         10 records. In the future, we will adjust the size of this limit according to the actual situation.
         
         ### Can more records be fetched per request?
         
         The current maximum is 1000 records. In the future, we will adjust the size of this limit according to the actual situation.
         
         # Development and test
+        
         Create a new `.env`, the content can refer to `.env.example`.
+        
         ```shell
         cp .env .env.example
         ```
+        
         Then modify the test code in the `test/` folder for testing.
+        
         ```shell
         pipenv install --pre
         pipenv shell
         python -m unittest test
         ```
         
 Platform: UNKNOWN
```

### Comparing `apitable-1.2.0/apitable.egg-info/SOURCES.txt` & `apitable-1.2.1/apitable.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 apitable/types/__init__.py
 apitable/types/embedlink.py
 apitable/types/field.py
 apitable/types/node.py
 apitable/types/record.py
 apitable/types/response.py
 apitable/types/space.py
+apitable/types/unit_model.py
 apitable/types/view.py
 test/test_create_datasheet.py
 test/test_create_embed_link.py
 test/test_create_field.py
 test/test_create_records.py
 test/test_delete_field.py
 test/test_delete_records.py
```

### Comparing `apitable-1.2.0/setup.py` & `apitable-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_create_datasheet.py` & `apitable-1.2.1/test/test_create_datasheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import warnings
 from apitable import Apitable
 from . import DOMAIN, TOKEN, SPACE_ID, FOLDER_ID
 
 
-class TestCreateFields(unittest.TestCase):
+class TestCreateDatasheet(unittest.TestCase):
     """Apitable Python SDK create datasheet test class
     - Datasheet Creation SDK Test
     """
 
     def setUp(self):
         """Create a datasheet test class object initial hook:"""
         warnings.simplefilter("ignore", ResourceWarning)
```

### Comparing `apitable-1.2.0/test/test_create_embed_link.py` & `apitable-1.2.1/test/test_create_embed_link.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_create_field.py` & `apitable-1.2.1/test/test_create_field.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_create_records.py` & `apitable-1.2.1/test/test_create_records.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_delete_field.py` & `apitable-1.2.1/test/test_delete_field.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_delete_records.py` & `apitable-1.2.1/test/test_delete_records.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_get_fields.py` & `apitable-1.2.1/test/test_get_fields.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_get_nodes.py` & `apitable-1.2.1/test/test_get_nodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,20 @@
         apitable.set_api_base(DOMAIN)
         self.apitable = apitable
 
     def test_space_root_nodes_all(self):
         space_root_nodes = self.apitable.space(SPACE_ID).nodes.all()
         self.assertIsInstance(space_root_nodes, list)
         first_node = space_root_nodes[0]
-        self.assertIn(first_node.type, ["Datasheet", "Folder"])
+        self.assertIn(first_node.type, ["Datasheet", "Folder", "Mirror"])
 
     def test_get_node_detail(self):
         node = self.apitable.nodes.get(FOLDER_ID)
         self.assertEqual(node.id, FOLDER_ID)
         self.assertIsNotNone(node.children)
 
+    def test_search_nodes(self):
+        nodes = self.apitable.nodes.search(spaceId=SPACE_ID, type='Folder')
+        self.assertIsInstance(nodes, list)
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `apitable-1.2.0/test/test_get_records.py` & `apitable-1.2.1/test/test_get_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import unittest
 import warnings
 
 from apitable import Apitable
-from . import TOKEN, DOMAIN, SPACE_ID, DATASHEET_ID, VIEW_ID
+from . import TOKEN, DOMAIN, SPACE_ID, DATASHEET_ID_FOR_GET, VIEW_ID
 
 
 class TestGetRecords(unittest.TestCase):
     def setUp(self):
         warnings.simplefilter("ignore", ResourceWarning)
         apitable = Apitable(TOKEN)
         apitable.set_api_base(DOMAIN)
-        self.dst = apitable.space(SPACE_ID).datasheet(DATASHEET_ID)
+        self.dst = apitable.space(SPACE_ID).datasheet(DATASHEET_ID_FOR_GET)
 
     def test_record_count(self):
         self.assertEqual(self.dst.records.all().count(), 1)
 
     def test_record_filter_get(self):
         self.assertEqual(
             self.dst.records.filter(title="apitable").get().title, "apitable"
```

### Comparing `apitable-1.2.0/test/test_get_spaces.py` & `apitable-1.2.1/test/test_get_spaces.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_get_views.py` & `apitable-1.2.1/test/test_get_views.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_update_records.py` & `apitable-1.2.1/test/test_update_records.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_upload_file.py` & `apitable-1.2.1/test/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `apitable-1.2.0/test/test_utils.py` & `apitable-1.2.1/test/test_utils.py`

 * *Files identical despite different names*

