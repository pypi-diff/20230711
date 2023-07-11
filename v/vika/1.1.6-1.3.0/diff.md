# Comparing `tmp/vika-1.1.6.tar.gz` & `tmp/vika-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vika-1.1.6.tar", last modified: Tue Jan  3 11:42:58 2023, max compression
+gzip compressed data, was "dist/vika-1.3.0.tar", last modified: Tue Jul 11 07:06:35 2023, max compression
```

## Comparing `vika-1.1.6.tar` & `vika-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_create_field.py
--rw-r--r--   0 runner    (1001) docker     (122)      914 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_create_datasheet.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_delete_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_get_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_delete_field.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_create_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_get_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_update_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_create_embed_link.py
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_get_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-01-03 11:42:49.000000 vika-1.1.6/test/test_get_spaces.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-03 11:42:58.000000 vika-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    14924 2023-01-03 11:42:49.000000 vika-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/vika.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-01-03 11:42:58.000000 vika-1.1.6/vika.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-03 11:42:58.000000 vika-1.1.6/vika.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-01-03 11:42:58.000000 vika-1.1.6/vika.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-03 11:42:58.000000 vika-1.1.6/vika.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17993 2023-01-03 11:42:58.000000 vika-1.1.6/vika.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-01-03 11:42:49.000000 vika-1.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    17993 2023-01-03 11:42:58.000000 vika-1.1.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/vika/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/vika/node/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-01-03 11:42:49.000000 vika-1.1.6/vika/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-01-03 11:42:49.000000 vika-1.1.6/vika/node/node_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-01-03 11:42:49.000000 vika-1.1.6/vika/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-01-03 11:42:49.000000 vika-1.1.6/vika/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/vika/space/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-01-03 11:42:49.000000 vika-1.1.6/vika/space/space.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-01-03 11:42:49.000000 vika-1.1.6/vika/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-01-03 11:42:49.000000 vika-1.1.6/vika/space/space_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/vika/datasheet/
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/record.py
--rw-r--r--   0 runner    (1001) docker     (122)     8964 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/view_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/query_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/datasheet_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/field_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10632 2023-01-03 11:42:49.000000 vika-1.1.6/vika/datasheet/datasheet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4165 2023-01-03 11:42:49.000000 vika-1.1.6/vika/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-01-03 11:42:49.000000 vika-1.1.6/vika/apitable.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-01-03 11:42:49.000000 vika-1.1.6/vika/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-03 11:42:58.000000 vika-1.1.6/vika/types/
--rw-r--r--   0 runner    (1001) docker     (122)     3097 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/response.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/record.py
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/embedlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/node.py
--rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/field.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/space.py
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/view.py
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-01-03 11:42:49.000000 vika-1.1.6/vika/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-01-03 11:42:49.000000 vika-1.1.6/vika/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    14924 2023-07-11 07:06:27.000000 vika-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 07:06:35.000000 vika-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-11 07:06:27.000000 vika-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/space/
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-11 07:06:27.000000 vika-1.3.0/vika/space/space_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-11 07:06:27.000000 vika-1.3.0/vika/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-11 07:06:27.000000 vika-1.3.0/vika/space/space.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/datasheet/
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/datasheet_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10632 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/datasheet.py
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/query_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8957 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/record.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/view_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4165 2023-07-11 07:06:27.000000 vika-1.3.0/vika/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-11 07:06:27.000000 vika-1.3.0/vika/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/node/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-11 07:06:27.000000 vika-1.3.0/vika/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-07-11 07:06:27.000000 vika-1.3.0/vika/node/node_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-11 07:06:27.000000 vika-1.3.0/vika/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-11 07:06:27.000000 vika-1.3.0/vika/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/embedlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/unit_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/field.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/record.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/space.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-11 07:06:27.000000 vika-1.3.0/vika/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-11 07:06:27.000000 vika-1.3.0/vika/apitable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/team.py
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/member.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/unit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/role.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_records.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_datasheet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_delete_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_records.py
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_delete_records.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_update_records.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_embed_link.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17993 2023-07-11 07:06:35.000000 vika-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17993 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/SOURCES.txt
```

### Comparing `vika-1.1.6/test/test_utils.py` & `vika-1.3.0/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from apitable.utils import query_parse
+from vika.utils import query_parse
 
 
 class TestUtils(unittest.TestCase):
 
     def test_query_parse(self):
         field_key_map = {}
         self.assertEqual(query_parse(field_key_map, a=1), "{a}=1")
```

### Comparing `vika-1.1.6/test/test_get_nodes.py` & `vika-1.3.0/test/test_get_nodes.py`

 * *Files 8% similar despite different names*

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

### Comparing `vika-1.1.6/test/test_create_field.py` & `vika-1.3.0/test/test_create_field.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_create_datasheet.py` & `vika-1.3.0/test/test_create_datasheet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import warnings
 from vika import Vika
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

### Comparing `vika-1.1.6/test/test_delete_records.py` & `vika-1.3.0/test/test_delete_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_get_fields.py` & `vika-1.3.0/test/test_get_fields.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_delete_field.py` & `vika-1.3.0/test/test_delete_field.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_create_records.py` & `vika-1.3.0/test/test_create_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_get_views.py` & `vika-1.3.0/test/test_get_views.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_update_records.py` & `vika-1.3.0/test/test_update_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_upload_file.py` & `vika-1.3.0/test/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/test/test_get_records.py` & `vika-1.3.0/test/test_get_records.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import unittest
 import warnings
 
 from vika import Vika
-from . import TOKEN, DOMAIN, SPACE_ID, DATASHEET_ID, VIEW_ID
+from . import TOKEN, DOMAIN, SPACE_ID, DATASHEET_ID_FOR_GET, VIEW_ID
 
 
 class TestGetRecords(unittest.TestCase):
     def setUp(self):
         warnings.simplefilter("ignore", ResourceWarning)
         apitable = Vika(TOKEN)
         apitable.set_api_base(DOMAIN)
-        self.dst = apitable.space(SPACE_ID).datasheet(DATASHEET_ID)
+        self.dst = apitable.space(SPACE_ID).datasheet(DATASHEET_ID_FOR_GET)
 
     def test_record_count(self):
         self.assertEqual(self.dst.records.all().count(), 1)
 
     def test_record_filter_get(self):
         self.assertEqual(
             self.dst.records.filter(title="apitable").get().title, "apitable"
```

### Comparing `vika-1.1.6/test/test_get_spaces.py` & `vika-1.3.0/test/test_get_spaces.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/README.md` & `vika-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika.egg-info/SOURCES.txt` & `vika-1.3.0/vika.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -41,8 +41,14 @@
 vika/types/__init__.py
 vika/types/embedlink.py
 vika/types/field.py
 vika/types/node.py
 vika/types/record.py
 vika/types/response.py
 vika/types/space.py
-vika/types/view.py
+vika/types/unit_model.py
+vika/types/view.py
+vika/unit/__init__.py
+vika/unit/member.py
+vika/unit/role.py
+vika/unit/team.py
+vika/unit/unit.py
```

### Comparing `vika-1.1.6/vika.egg-info/PKG-INFO` & `vika-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vika
-Version: 1.1.6
+Version: 1.3.0
 Summary: 维格表官方 Python SDK
 Home-page: https://github.com/vikadata/vika.py
 Author: vikadata
 Author-email: dev@vikadata.com
 License: UNKNOWN
 Description: > ⚠️ 请参考[迁移指南](https://github.com/vikadata/vika.py/blob/master/docs/upgrade_to_v1.md) 从 0.1.x 升级至 1.x 版本，旧版本我们将不再维护!
```

### Comparing `vika-1.1.6/setup.py` & `vika-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author="vikadata",
     author_email="dev@vikadata.com",
     description="维格表官方 Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vikadata/vika.py",
     packages=[
-        "vika", "vika.datasheet", "vika.types", "vika.node", "vika.space"
+        "vika", "vika.datasheet", "vika.types", "vika.node", "vika.space", "vika.unit"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

### Comparing `vika-1.1.6/PKG-INFO` & `vika-1.3.0/vika.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vika
-Version: 1.1.6
+Version: 1.3.0
 Summary: 维格表官方 Python SDK
 Home-page: https://github.com/vikadata/vika.py
 Author: vikadata
 Author-email: dev@vikadata.com
 License: UNKNOWN
 Description: > ⚠️ 请参考[迁移指南](https://github.com/vikadata/vika.py/blob/master/docs/upgrade_to_v1.md) 从 0.1.x 升级至 1.x 版本，旧版本我们将不再维护!
```

### Comparing `vika-1.1.6/vika/node/node_manager.py` & `vika-1.3.0/vika/node/node_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib.parse import urljoin
 
 from vika.types.response import (
     GETNodeListResponse,
-    GETNodeDetailResponse
+    GETNodeDetailResponse,
+    GETSearchNodeListResponse
 )
 from vika.utils import handle_response
 
 
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

### Comparing `vika-1.1.6/vika/request.py` & `vika-1.3.0/vika/request.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/space/space.py` & `vika-1.3.0/vika/space/space.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from vika.node import NodeManager
-from vika.utils import get_dst_id, handle_response
+from urllib.parse import urljoin
+
 from vika.datasheet import Datasheet, DatasheetManager
+from vika.node import NodeManager
 from vika.types.response import PostDatasheetMetaResponse
-from urllib.parse import urljoin
+from vika.unit import Member, Role, Team
+from vika.utils import get_dst_id, handle_response
 
 
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

### Comparing `vika-1.1.6/vika/space/space_manager.py` & `vika-1.3.0/vika/space/space_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/datasheet/record.py` & `vika-1.3.0/vika/datasheet/record.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/datasheet/record_manager.py` & `vika-1.3.0/vika/datasheet/record_manager.py`

 * *Files 1% similar despite different names*

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

### Comparing `vika-1.1.6/vika/datasheet/query_set.py` & `vika-1.3.0/vika/datasheet/query_set.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/datasheet/datasheet_manager.py` & `vika-1.3.0/vika/datasheet/datasheet_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/datasheet/field_manager.py` & `vika-1.3.0/vika/datasheet/field_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/datasheet/datasheet.py` & `vika-1.3.0/vika/datasheet/datasheet.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/utils.py` & `vika-1.3.0/vika/utils.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/apitable.py` & `vika-1.3.0/vika/apitable.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/exceptions.py` & `vika-1.3.0/vika/exceptions.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/types/response.py` & `vika-1.3.0/vika/types/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Any, List, Optional
 
 from vika.types.embedlink import EmbedLinkThemeEnum, EmbedLinkPayload
-from vika.types.node import NodeListItem, NodeDetail
+from vika.types.node import NodeListItem, NodeDetail, NodeSearchInfo
 from vika.types.space import SpaceListItem
 from vika.types.record import RawRecord
 from vika.types.view import MetaView
 from vika.types.field import MetaField
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

### Comparing `vika-1.1.6/vika/types/record.py` & `vika-1.3.0/vika/types/record.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/types/embedlink.py` & `vika-1.3.0/vika/types/embedlink.py`

 * *Files identical despite different names*

### Comparing `vika-1.1.6/vika/types/field.py` & `vika-1.3.0/vika/types/field.py`

 * *Files identical despite different names*

