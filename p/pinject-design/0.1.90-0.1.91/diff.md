# Comparing `tmp/pinject_design-0.1.90.tar.gz` & `tmp/pinject_design-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinject_design-0.1.90.tar", max compression
+gzip compressed data, was "pinject_design-0.1.91.tar", max compression
```

## Comparing `pinject_design-0.1.90.tar` & `pinject_design-0.1.91.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.90/LICENSE
--rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.90/pinject_design/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.90/pinject_design/di/__init__.py
--rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.90/pinject_design/di/app_designed.py
--rw-r--r--   0        0        0     2442 2023-05-06 03:52:35.678286 pinject_design-0.1.90/pinject_design/di/app_injected.py
--rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.90/pinject_design/di/applicative.py
--rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.90/pinject_design/di/ast.py
--rw-r--r--   0        0        0     7338 2023-05-04 06:32:55.349238 pinject_design-0.1.90/pinject_design/di/design.py
--rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.90/pinject_design/di/designed.py
--rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.90/pinject_design/di/dynamic_proxy.py
--rw-r--r--   0        0        0    28337 2023-07-04 16:13:18.254578 pinject_design-0.1.90/pinject_design/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.90/pinject_design/di/implicit_globals.py
--rw-r--r--   0        0        0    29340 2023-07-11 07:44:55.289012 pinject_design-0.1.90/pinject_design/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.90/pinject_design/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.90/pinject_design/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.90/pinject_design/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.90/pinject_design/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.90/pinject_design/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.90/pinject_design/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.90/pinject_design/di/session.py
--rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.90/pinject_design/di/sessioned.py
--rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.90/pinject_design/di/static_proxy.py
--rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.90/pinject_design/di/test_ast.py
--rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.90/pinject_design/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.90/pinject_design/di/test_graph.py
--rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.90/pinject_design/di/test_injected.py
--rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.90/pinject_design/di/test_proxiable.py
--rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.90/pinject_design/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.90/pinject_design/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.90/pinject_design/global_configs
--rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.90/pinject_design/global_configs.py
--rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.90/pinject_design/graph_inspection.py
--rw-r--r--   0        0        0     1612 2023-07-11 09:19:43.794158 pinject_design-0.1.90/pinject_design/helper_structure.py
--rw-r--r--   0        0        0     6272 2023-07-11 09:19:43.787170 pinject_design-0.1.90/pinject_design/helpers.py
--rw-r--r--   0        0        0     2285 2023-07-11 08:45:24.185649 pinject_design-0.1.90/pinject_design/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.90/pinject_design/nx_graph_util.py
--rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.90/pinject_design/pinject_design.iml
--rw-r--r--   0        0        0    20978 2023-07-11 09:23:48.233461 pinject_design-0.1.90/pinject_design/run_config_utils.py
--rw-r--r--   0        0        0     1590 2023-07-11 09:19:43.796587 pinject_design-0.1.90/pinject_design/run_config_utils_v2.py
--rw-r--r--   0        0        0      938 2023-07-11 09:19:43.784630 pinject_design-0.1.90/pinject_design/test_package/__init__.py
--rw-r--r--   0        0        0      234 2023-07-11 09:19:43.781955 pinject_design-0.1.90/pinject_design/test_package/child/__init__.py
--rw-r--r--   0        0        0      284 2023-07-11 08:16:07.010761 pinject_design-0.1.90/pinject_design/test_package/child/module1.py
--rw-r--r--   0        0        0    19787 2023-07-05 04:39:53.268769 pinject_design-0.1.90/pinject_design/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.90/pinject_design/viz/__init__.py
--rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.90/pinject_design/viz/graph.py
--rw-r--r--   0        0        0      639 2023-07-11 09:23:55.316472 pinject_design-0.1.90/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.90/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.91/LICENSE
+-rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.91/pinject_design/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.91/pinject_design/di/__init__.py
+-rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.91/pinject_design/di/app_designed.py
+-rw-r--r--   0        0        0     2442 2023-05-06 03:52:35.678286 pinject_design-0.1.91/pinject_design/di/app_injected.py
+-rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.91/pinject_design/di/applicative.py
+-rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.91/pinject_design/di/ast.py
+-rw-r--r--   0        0        0     7338 2023-05-04 06:32:55.349238 pinject_design-0.1.91/pinject_design/di/design.py
+-rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.91/pinject_design/di/designed.py
+-rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.91/pinject_design/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    28337 2023-07-04 16:13:18.254578 pinject_design-0.1.91/pinject_design/di/graph.py
+-rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.91/pinject_design/di/implicit_globals.py
+-rw-r--r--   0        0        0    29340 2023-07-11 07:44:55.289012 pinject_design-0.1.91/pinject_design/di/injected.py
+-rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.91/pinject_design/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.91/pinject_design/di/permissioned/__init__.py
+-rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.91/pinject_design/di/permissioned/blueprint.py
+-rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.91/pinject_design/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.91/pinject_design/di/provider.py
+-rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.91/pinject_design/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.91/pinject_design/di/session.py
+-rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.91/pinject_design/di/sessioned.py
+-rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.91/pinject_design/di/static_proxy.py
+-rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.91/pinject_design/di/test_ast.py
+-rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.91/pinject_design/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.91/pinject_design/di/test_graph.py
+-rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.91/pinject_design/di/test_injected.py
+-rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.91/pinject_design/di/test_proxiable.py
+-rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.91/pinject_design/di/util.py
+-rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.91/pinject_design/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.91/pinject_design/global_configs
+-rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.91/pinject_design/global_configs.py
+-rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.91/pinject_design/graph_inspection.py
+-rw-r--r--   0        0        0     1612 2023-07-11 09:19:43.794158 pinject_design-0.1.91/pinject_design/helper_structure.py
+-rw-r--r--   0        0        0     6272 2023-07-11 09:19:43.787170 pinject_design-0.1.91/pinject_design/helpers.py
+-rw-r--r--   0        0        0     2285 2023-07-11 08:45:24.185649 pinject_design-0.1.91/pinject_design/module_inspector.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.91/pinject_design/nx_graph_util.py
+-rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.91/pinject_design/pinject_design.iml
+-rw-r--r--   0        0        0    20791 2023-07-11 09:25:18.780147 pinject_design-0.1.91/pinject_design/run_config_utils.py
+-rw-r--r--   0        0        0     1590 2023-07-11 09:19:43.796587 pinject_design-0.1.91/pinject_design/run_config_utils_v2.py
+-rw-r--r--   0        0        0      938 2023-07-11 09:19:43.784630 pinject_design-0.1.91/pinject_design/test_package/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-11 09:19:43.781955 pinject_design-0.1.91/pinject_design/test_package/child/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-11 08:16:07.010761 pinject_design-0.1.91/pinject_design/test_package/child/module1.py
+-rw-r--r--   0        0        0    19787 2023-07-05 04:39:53.268769 pinject_design-0.1.91/pinject_design/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.91/pinject_design/viz/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.91/pinject_design/viz/graph.py
+-rw-r--r--   0        0        0      639 2023-07-11 09:25:31.468372 pinject_design-0.1.91/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.91/PKG-INFO
```

### Comparing `pinject_design-0.1.90/LICENSE` & `pinject_design-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/app_designed.py` & `pinject_design-0.1.91/pinject_design/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/app_injected.py` & `pinject_design-0.1.91/pinject_design/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/applicative.py` & `pinject_design-0.1.91/pinject_design/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/ast.py` & `pinject_design-0.1.91/pinject_design/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/design.py` & `pinject_design-0.1.91/pinject_design/di/design.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/designed.py` & `pinject_design-0.1.91/pinject_design/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/dynamic_proxy.py` & `pinject_design-0.1.91/pinject_design/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/graph.py` & `pinject_design-0.1.91/pinject_design/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/injected.py` & `pinject_design-0.1.91/pinject_design/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/injected_analysis.py` & `pinject_design-0.1.91/pinject_design/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/permissioned/blueprint.py` & `pinject_design-0.1.91/pinject_design/di/permissioned/blueprint.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/proxiable.py` & `pinject_design-0.1.91/pinject_design/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/session.py` & `pinject_design-0.1.91/pinject_design/di/session.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/sessioned.py` & `pinject_design-0.1.91/pinject_design/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/static_proxy.py` & `pinject_design-0.1.91/pinject_design/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/test_dynamic_proxy.py` & `pinject_design-0.1.91/pinject_design/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/test_graph.py` & `pinject_design-0.1.91/pinject_design/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/test_injected.py` & `pinject_design-0.1.91/pinject_design/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/test_proxiable.py` & `pinject_design-0.1.91/pinject_design/di/test_proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/di/util.py` & `pinject_design-0.1.91/pinject_design/di/util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/exceptions.py` & `pinject_design-0.1.91/pinject_design/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/graph_inspection.py` & `pinject_design-0.1.91/pinject_design/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/helper_structure.py` & `pinject_design-0.1.91/pinject_design/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/helpers.py` & `pinject_design-0.1.91/pinject_design/helpers.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/module_inspector.py` & `pinject_design-0.1.91/pinject_design/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/nx_graph_util.py` & `pinject_design-0.1.91/pinject_design/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/run_config_utils.py` & `pinject_design-0.1.91/pinject_design/run_config_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,21 +585,17 @@
 
     return inspect_module_for_type(module_path, accept)
 
 
 @injected_function
 def get_designs_from_meta_var(
         var_path_to_file_path,
-        logger,
         /,
         meta: ModuleVarSpec
 ) -> List[ModuleVarSpec]:
-    logger.info(f"trying to import designs from {meta.var_path}")
-    mod_path = '.'.join(meta.var_path.split(".")[:-1])
-    logger.info(f"estimated mod_path:{mod_path}")
     return get_designs_from_module(var_path_to_file_path(meta.var_path))
 
 
 @injected_function
 def var_path_to_file_path(project_root: Path, /, var_path: str) -> Path:
     module_path = '.'.join(var_path.split(".")[:-1])
     return Path(str(project_root / module_path.replace(".", os.path.sep)) + ".py")
```

### Comparing `pinject_design-0.1.90/pinject_design/run_config_utils_v2.py` & `pinject_design-0.1.91/pinject_design/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/test_package/__init__.py` & `pinject_design-0.1.91/pinject_design/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pinject_design/visualize_di.py` & `pinject_design-0.1.91/pinject_design/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.90/pyproject.toml` & `pinject_design-0.1.91/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinject-design"
-version = "0.1.90"
+version = "0.1.91"
 description = "immutable wrapper for pinject"
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 makefun = "*"
```

### Comparing `pinject_design-0.1.90/PKG-INFO` & `pinject_design-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinject-design
-Version: 0.1.90
+Version: 0.1.91
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

