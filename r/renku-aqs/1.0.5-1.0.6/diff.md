# Comparing `tmp/renku-aqs-1.0.5.tar.gz` & `tmp/renku-aqs-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-aqs-1.0.5.tar", last modified: Mon Jun  5 21:24:13 2023, max compression
+gzip compressed data, was "renku-aqs-1.0.6.tar", last modified: Tue Jul 11 12:12:07 2023, max compression
```

## Comparing `renku-aqs-1.0.5.tar` & `renku-aqs-1.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      187 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/.gitignore
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11358 2021-06-14 15:54:58.000000 renku-aqs-1.0.5/LICENSE
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      114 2021-06-14 15:54:58.000000 renku-aqs-1.0.5/MANIFEST.in
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/PKG-INFO
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     6340 2023-02-22 13:05:10.000000 renku-aqs-1.0.5/README.md
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        5 2023-06-05 17:42:57.000000 renku-aqs-1.0.5/VERSION
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      345 2021-06-14 15:54:58.000000 renku-aqs-1.0.5/concepts.md
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1659 2021-06-28 10:31:11.000000 renku-aqs-1.0.5/example.md
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.843607 renku-aqs-1.0.5/readme_imgs/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)  1891362 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/animation_expansion_retraction.gif
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    22497 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/enable_disable_configuration-graph.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   302729 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_display_graph_complete.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   150316 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    36993 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an_no-oda-info.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   146690 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_show-graph.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    61174 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/expanded_plan.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    71535 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/hierarchical_view.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52046 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/reduced_plan.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52899 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/subgraph.png
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.843607 renku-aqs-1.0.5/renku_aqs.egg-info/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/PKG-INFO
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1066 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      171 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/entry_points.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2021-12-08 07:18:18.000000 renku-aqs-1.0.5/renku_aqs.egg-info/not-zip-safe
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      120 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/requires.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        9 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/top_level.txt
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/renkuaqs/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5975 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/__init__.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      606 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/config.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2092 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/renkuaqs/graph_config.yaml
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     7384 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/graph_graphical_config.json
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     8836 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/graph_nodes_subset_config.json
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      421 2023-02-10 17:08:04.000000 renku-aqs-1.0.5/renkuaqs/graph_reduction_config.json
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    50791 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/graph_utils.py
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/renkuaqs/icons/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3416 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/renkuaqs/icons/graph_icon.svg
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11874 2023-03-14 09:55:25.000000 renku-aqs-1.0.5/renkuaqs/javascript_graph_utils.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    42892 2023-05-26 14:38:27.000000 renku-aqs-1.0.5/renkuaqs/ontology.ttl
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    18708 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/plugin.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        0 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/requirements.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       38 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/setup.cfg
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2399 2023-06-05 21:24:05.000000 renku-aqs-1.0.5/setup.py
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/tests/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3093 2023-02-08 14:37:58.000000 renku-aqs-1.0.5/tests/test_example.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      187 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/.gitignore
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11358 2021-06-14 15:54:58.000000 renku-aqs-1.0.6/LICENSE
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      114 2021-06-14 15:54:58.000000 renku-aqs-1.0.6/MANIFEST.in
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     6340 2023-02-22 13:05:10.000000 renku-aqs-1.0.6/README.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        5 2023-07-11 12:11:05.000000 renku-aqs-1.0.6/VERSION
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      345 2021-06-14 15:54:58.000000 renku-aqs-1.0.6/concepts.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1659 2021-06-28 10:31:11.000000 renku-aqs-1.0.6/example.md
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/readme_imgs/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)  1891362 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/animation_expansion_retraction.gif
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    22497 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/enable_disable_configuration-graph.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   302729 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_display_graph_complete.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   150316 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    36993 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an_no-oda-info.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   146690 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_show-graph.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    61174 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/expanded_plan.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    71535 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/hierarchical_view.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52046 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/reduced_plan.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52899 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/subgraph.png
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/renku_aqs.egg-info/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1066 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      171 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/entry_points.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2021-12-08 07:18:18.000000 renku-aqs-1.0.6/renku_aqs.egg-info/not-zip-safe
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      120 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        9 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/top_level.txt
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/renkuaqs/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5975 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/__init__.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      606 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/config.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2092 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/renkuaqs/graph_config.yaml
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     7384 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/graph_graphical_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     8836 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/graph_nodes_subset_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      421 2023-02-10 17:08:04.000000 renku-aqs-1.0.6/renkuaqs/graph_reduction_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    50791 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/graph_utils.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/renkuaqs/icons/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3416 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/renkuaqs/icons/graph_icon.svg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11874 2023-03-14 09:55:25.000000 renku-aqs-1.0.6/renkuaqs/javascript_graph_utils.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    42892 2023-05-26 14:38:27.000000 renku-aqs-1.0.6/renkuaqs/ontology.ttl
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    18752 2023-07-11 12:03:33.000000 renku-aqs-1.0.6/renkuaqs/plugin.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        0 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/requirements.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       38 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/setup.cfg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2399 2023-07-11 12:10:22.000000 renku-aqs-1.0.6/setup.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/tests/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3093 2023-02-08 14:37:58.000000 renku-aqs-1.0.6/tests/test_example.py
```

### Comparing `renku-aqs-1.0.5/LICENSE` & `renku-aqs-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/PKG-INFO` & `renku-aqs-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku-aqs
-Version: 1.0.5
+Version: 1.0.6
 Summary: Renku AQS plugin
 Author: Gabriele Barni, Volodymyr Savchenko
 Author-email: 
 License: Apache License 2.0
 Keywords: Renku AQS
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `renku-aqs-1.0.5/README.md` & `renku-aqs-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/example.md` & `renku-aqs-1.0.6/example.md`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/animation_expansion_retraction.gif` & `renku-aqs-1.0.6/readme_imgs/animation_expansion_retraction.gif`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/enable_disable_configuration-graph.png` & `renku-aqs-1.0.6/readme_imgs/enable_disable_configuration-graph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/example_display_graph_complete.png` & `renku-aqs-1.0.6/readme_imgs/example_display_graph_complete.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an.png` & `renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an_no-oda-info.png` & `renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an_no-oda-info.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/example_show-graph.png` & `renku-aqs-1.0.6/readme_imgs/example_show-graph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/expanded_plan.png` & `renku-aqs-1.0.6/readme_imgs/expanded_plan.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/hierarchical_view.png` & `renku-aqs-1.0.6/readme_imgs/hierarchical_view.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/reduced_plan.png` & `renku-aqs-1.0.6/readme_imgs/reduced_plan.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/readme_imgs/subgraph.png` & `renku-aqs-1.0.6/readme_imgs/subgraph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renku_aqs.egg-info/PKG-INFO` & `renku-aqs-1.0.6/renku_aqs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku-aqs
-Version: 1.0.5
+Version: 1.0.6
 Summary: Renku AQS plugin
 Author: Gabriele Barni, Volodymyr Savchenko
 Author-email: 
 License: Apache License 2.0
 Keywords: Renku AQS
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `renku-aqs-1.0.5/renku_aqs.egg-info/SOURCES.txt` & `renku-aqs-1.0.6/renku_aqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/__init__.py` & `renku-aqs-1.0.6/renkuaqs/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/config.py` & `renku-aqs-1.0.6/renkuaqs/config.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/graph_config.yaml` & `renku-aqs-1.0.6/renkuaqs/graph_config.yaml`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/graph_graphical_config.json` & `renku-aqs-1.0.6/renkuaqs/graph_graphical_config.json`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/graph_nodes_subset_config.json` & `renku-aqs-1.0.6/renkuaqs/graph_nodes_subset_config.json`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/graph_utils.py` & `renku-aqs-1.0.6/renkuaqs/graph_utils.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/icons/graph_icon.svg` & `renku-aqs-1.0.6/renkuaqs/icons/graph_icon.svg`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/javascript_graph_utils.py` & `renku-aqs-1.0.6/renkuaqs/javascript_graph_utils.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/ontology.ttl` & `renku-aqs-1.0.6/renkuaqs/ontology.ttl`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/renkuaqs/plugin.py` & `renku-aqs-1.0.6/renkuaqs/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 
 from pathlib import Path
 from renku.domain_model.provenance.annotation import Annotation
 from renku.domain_model.project_context import project_context
 from renku.core.plugin import hookimpl
 from IPython.display import Image, HTML
 from prettytable import PrettyTable
-from aqsconverters.io import AQS_DIR, COMMON_DIR
+from aqsconverters.io import AQS_ANNOTATION_DIR, COMMON_DIR
 from renkuaqs.config import ENTITY_METADATA_AQS_DIR
 from nb2workflow import ontology
 
 import renkuaqs.graph_utils as graph_utils
 
 
 class AQS(object):
     def __init__(self, run):
         self.run = run
 
     @property
     def renku_aqs_path(self):
         """Return a ``Path`` instance of Renku AQS metadata folder."""
-        return Path(project_context.metadata_path).joinpath(AQS_DIR).joinpath(COMMON_DIR)
+        return Path(project_context.metadata_path).joinpath(AQS_ANNOTATION_DIR).joinpath(COMMON_DIR)
 
     @property
     def aqs_annotation_path(self):
         """Return a ``Path`` instance of Renku AQS specific annotation."""
         return Path(ENTITY_METADATA_AQS_DIR)
 
     def load_model(self, path):
@@ -70,15 +70,15 @@
 
 
 @hookimpl
 def activity_annotations(activity):
     """``process_run_annotations`` hook implementation."""
     aqs = AQS(activity)
 
-    sitecustomize_path = pathlib.Path(os.path.join(project_context.metadata_path, AQS_DIR, "sitecustomize.py"))
+    sitecustomize_path = pathlib.Path(os.path.join(project_context.metadata_path, AQS_ANNOTATION_DIR, "sitecustomize.py"))
     if sitecustomize_path.exists():
         sitecustomize_path.unlink()
 
     annotations = []
 
     print("process_run_annotations")
     print(aqs.renku_aqs_path)
@@ -137,15 +137,15 @@
     return annotations
 
 
 @hookimpl
 def pre_run(tool):
     print(f"\033[31mhere we will prepare hooks for astroquery, tool given is {tool}\033[0m")
 
-    sitecustomize_dir = Path(project_context.metadata_path, AQS_DIR)
+    sitecustomize_dir = Path(project_context.metadata_path, AQS_ANNOTATION_DIR)
 
     if not sitecustomize_dir.exists():
         sitecustomize_dir.mkdir(parents=True)
 
     os.environ["PYTHONPATH"] = f"{sitecustomize_dir}:" + os.environ.get('PYTHONPATH', "")
 
     sitecustomize_path = os.path.join(sitecustomize_dir, "sitecustomize.py")
```

### Comparing `renku-aqs-1.0.5/setup.py` & `renku-aqs-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.5/tests/test_example.py` & `renku-aqs-1.0.6/tests/test_example.py`

 * *Files identical despite different names*

