# Comparing `tmp/comex-0.1.3.tar.gz` & `tmp/comex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.1.3.tar", last modified: Thu Jun 22 04:19:09 2023, max compression
+gzip compressed data, was "comex-0.1.4.tar", last modified: Tue Jul 11 12:51:11 2023, max compression
```

## Comparing `comex-0.1.3.tar` & `comex-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-27 09:03:42.000000 comex-0.1.3/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)    13520 2023-06-22 04:19:09.860000 comex-0.1.3/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)    12903 2023-06-22 04:08:47.000000 comex-0.1.3/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-06-22 04:19:09.860000 comex-0.1.3/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-27 09:03:43.000000 comex-0.1.3/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)      104 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/__main__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     3664 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/cli.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/AST/
--rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/codeviews/AST/AST.py
--rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/AST/AST_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/AST/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/CFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG.py
--rwxrwxrwx   0 noble      (501) staff       (20)    97324 2023-06-22 04:17:23.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG_csharp.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)    78345 2023-06-22 04:17:23.000000 comex-0.1.3/src/comex/codeviews/CFG/CFG_java.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/CFG/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/CST/
--rwxrwxrwx   0 noble      (501) staff       (20)     2542 2023-06-22 04:11:17.000000 comex-0.1.3/src/comex/codeviews/CST/CST_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/CST/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/DFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-05-31 12:50:30.000000 comex-0.1.3/src/comex/codeviews/DFG/DFG_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/DFG/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/SDFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     4581 2023-06-09 05:17:59.000000 comex-0.1.3/src/comex/codeviews/SDFG/SDFG.py
--rwxrwxrwx   0 noble      (501) staff       (20)    57510 2023-06-22 04:11:17.000000 comex-0.1.3/src/comex/codeviews/SDFG/SDFG_csharp.py
--rwxrwxrwx   0 noble      (501) staff       (20)    61649 2023-06-18 03:38:41.000000 comex-0.1.3/src/comex/codeviews/SDFG/SDFG_java.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/SDFG/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/codeviews/combined_graph/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/combined_graph/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/codeviews/combined_graph/combined_driver.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/tree_parser/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/tree_parser/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)    11275 2023-06-22 04:11:17.000000 comex-0.1.3/src/comex/tree_parser/cs_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)     6210 2023-06-08 11:12:38.000000 comex-0.1.3/src/comex/tree_parser/custom_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)    10039 2023-06-08 11:12:38.000000 comex-0.1.3/src/comex/tree_parser/java_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1818 2023-05-29 09:20:48.000000 comex-0.1.3/src/comex/tree_parser/parser_driver.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex/utils/
--rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/utils/DFG_utils.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.3/src/comex/utils/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)    26499 2023-06-14 16:12:07.000000 comex-0.1.3/src/comex/utils/cs_nodes.py
--rwxrwxrwx   0 noble      (501) staff       (20)    25220 2023-06-07 04:40:53.000000 comex-0.1.3/src/comex/utils/java_nodes.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1134 2023-06-07 04:40:53.000000 comex-0.1.3/src/comex/utils/postprocessor.py
--rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/utils/preprocessor.py
--rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-05-27 09:03:43.000000 comex-0.1.3/src/comex/utils/src_parser.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-22 04:19:09.810000 comex-0.1.3/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)    13520 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-06-22 04:19:09.000000 comex-0.1.3/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-27 09:03:42.000000 comex-0.1.4/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)    14479 2023-07-11 12:51:11.640000 comex-0.1.4/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)    13862 2023-07-11 12:00:46.000000 comex-0.1.4/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-07-11 12:51:11.640000 comex-0.1.4/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-06-30 03:53:49.000000 comex-0.1.4/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      104 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/__main__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     3654 2023-07-08 22:33:09.000000 comex-0.1.4/src/comex/cli.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/AST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/AST/AST.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/AST/AST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/AST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/CFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CFG/CFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    97324 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CFG/CFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CFG/CFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    78345 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CFG/CFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/CST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     2542 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CST/CST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/CST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/DFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-06-30 06:38:47.000000 comex-0.1.4/src/comex/codeviews/DFG/DFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/DFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/SDFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4581 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/SDFG/SDFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    57510 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/SDFG/SDFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    61649 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/SDFG/SDFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/SDFG/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/codeviews/combined_graph/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/combined_graph/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/codeviews/combined_graph/combined_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/tree_parser/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/tree_parser/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    11275 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/tree_parser/cs_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     6210 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/tree_parser/custom_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    10039 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/tree_parser/java_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1818 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/tree_parser/parser_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex/utils/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/DFG_utils.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    26499 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/cs_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    25220 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/java_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1134 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/postprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/preprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-06-30 03:53:49.000000 comex-0.1.4/src/comex/utils/src_parser.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-07-11 12:51:11.590000 comex-0.1.4/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)    14479 2023-07-11 12:51:11.000000 comex-0.1.4/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-07-11 12:51:11.000000 comex-0.1.4/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-07-11 12:51:11.000000 comex-0.1.4/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-07-11 12:51:11.000000 comex-0.1.4/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-07-11 12:51:11.000000 comex-0.1.4/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-07-11 12:51:11.000000 comex-0.1.4/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.1.3/LICENSE` & `comex-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/PKG-INFO` & `comex-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: comex
-Version: 0.1.3
-Summary: Generate combined multi-code view graphs
-Home-page: https://github.com/IBM/tree-sitter-codeviews
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
+If you wish to learn more about the approach taken, here are some conference talks and publications:
+- ASE 2023 demonstration: [COMEX: A Tool for Generating Customized Source Code Representations](https://arxiv.org/abs/2307.04693)
+- ICSE 2023 tutorial: [The Landscape of Source Code Representation Learning in AI-Driven Software Engineering Tasks](https://research.ibm.com/publications/the-landscape-of-source-code-representation-learning-in-ai-driven-software-engineering-tasks)
+
+## Cite Comex
+If you use Comex in your research, please cite our work by using the following BibTeX entry:
+```
+@misc{das2023comex,
+      title={COMEX: A Tool for Generating Customized Source Code Representations}, 
+      author={Debeshee Das and Noble Saji Mathews and Alex Mathai and Srikanth Tamilselvam and Kranthi Sedamaki and Sridhar Chimalakonda and Atul Kumar},
+      year={2023},
+      eprint={2307.04693},
+      archivePrefix={arXiv},
+      primaryClass={cs.SE}
+}
+```
+
 ---
 ## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
```

### Comparing `comex-0.1.3/README.md` & `comex-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,48 @@
+Metadata-Version: 2.1
+Name: comex
+Version: 0.1.4
+Summary: Generate combined multi-code view graphs
+Home-page: https://github.com/IBM/tree-sitter-codeviews
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
+If you wish to learn more about the approach taken, here are some conference talks and publications:
+- ASE 2023 demonstration: [COMEX: A Tool for Generating Customized Source Code Representations](https://arxiv.org/abs/2307.04693)
+- ICSE 2023 tutorial: [The Landscape of Source Code Representation Learning in AI-Driven Software Engineering Tasks](https://research.ibm.com/publications/the-landscape-of-source-code-representation-learning-in-ai-driven-software-engineering-tasks)
+
+## Cite Comex
+If you use Comex in your research, please cite our work by using the following BibTeX entry:
+```
+@misc{das2023comex,
+      title={COMEX: A Tool for Generating Customized Source Code Representations}, 
+      author={Debeshee Das and Noble Saji Mathews and Alex Mathai and Srikanth Tamilselvam and Kranthi Sedamaki and Sridhar Chimalakonda and Atul Kumar},
+      year={2023},
+      eprint={2307.04693},
+      archivePrefix={arXiv},
+      primaryClass={cs.SE}
+}
+```
+
 ---
 ## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
```

### Comparing `comex-0.1.3/setup.cfg` & `comex-0.1.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.1.3
+version = 0.1.4
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.1.3/src/comex/cli.py` & `comex-0.1.4/src/comex/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     }
     """),
         code_file: Optional[Path] = typer.Option(None, help="./test_file,java"),
         graphs: str = typer.Option("ast,dfg", help="ast, cfg, dfg"),
         output: str = typer.Option("dot", help="all/json/dot (dot generates png as well)"),
         blacklisted: str = typer.Option("", help="Nodes to be removed from the AST"),
         collapsed: bool = typer.Option(False, help="Collapses all occurrences of a variable into one node"),
-        statements: bool = typer.Option(True, help="Converts DFG output to statement level and uses RDA"),
+        # statements: bool = typer.Option(True, help="Converts DFG output to statement level and uses RDA"),
         last_def: bool = typer.Option(False, help="Adds last definition information to the DFG"),
         last_use: bool = typer.Option(False, help="Adds last use information to the DFG"),
         throw_parse_error: bool = typer.Option(False, help="Throws an error if the code cannot be parsed"),
         debug: bool = typer.Option(False, help="Enables debug logs"),
 ):
     """
     Comex
@@ -61,15 +61,15 @@
             "minimized": bool(blacklisted),
             "blacklisted": blacklisted.split(",")
         },
         "DFG": {
             "exists": False,
             "collapsed": collapsed,
             "minimized": False,
-            "statements": statements,
+            "statements": True,
             "last_def": last_def,
             "last_use": last_use
         },
         "CFG": {
             "exists": False,
         }
     }
@@ -82,15 +82,15 @@
             "blacklisted": blacklisted.split(",")
         }
     if "dfg" in graphs.lower():
         codeviews["DFG"] = {
             "exists": True,
             "collapsed": collapsed,
             "minimized": False,
-            "statements": statements,
+            "statements": True,
             "last_def": last_def,
             "last_use": last_use
         }
     if "cfg" in graphs.lower():
         codeviews["CFG"] = {
             "exists": True,
         }
```

### Comparing `comex-0.1.3/src/comex/codeviews/AST/AST.py` & `comex-0.1.4/src/comex/codeviews/AST/AST.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/AST/AST_driver.py` & `comex-0.1.4/src/comex/codeviews/AST/AST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/CFG/CFG.py` & `comex-0.1.4/src/comex/codeviews/CFG/CFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/CFG/CFG_csharp.py` & `comex-0.1.4/src/comex/codeviews/CFG/CFG_csharp.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/CFG/CFG_driver.py` & `comex-0.1.4/src/comex/codeviews/CFG/CFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/CFG/CFG_java.py` & `comex-0.1.4/src/comex/codeviews/CFG/CFG_java.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/CST/CST_driver.py` & `comex-0.1.4/src/comex/codeviews/CST/CST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/DFG/DFG_driver.py` & `comex-0.1.4/src/comex/codeviews/DFG/DFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/SDFG/SDFG.py` & `comex-0.1.4/src/comex/codeviews/SDFG/SDFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/SDFG/SDFG_csharp.py` & `comex-0.1.4/src/comex/codeviews/SDFG/SDFG_csharp.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/SDFG/SDFG_java.py` & `comex-0.1.4/src/comex/codeviews/SDFG/SDFG_java.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/codeviews/combined_graph/combined_driver.py` & `comex-0.1.4/src/comex/codeviews/combined_graph/combined_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/tree_parser/cs_parser.py` & `comex-0.1.4/src/comex/tree_parser/cs_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/tree_parser/custom_parser.py` & `comex-0.1.4/src/comex/tree_parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/tree_parser/java_parser.py` & `comex-0.1.4/src/comex/tree_parser/java_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/tree_parser/parser_driver.py` & `comex-0.1.4/src/comex/tree_parser/parser_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/utils/DFG_utils.py` & `comex-0.1.4/src/comex/utils/DFG_utils.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/utils/cs_nodes.py` & `comex-0.1.4/src/comex/utils/cs_nodes.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/utils/java_nodes.py` & `comex-0.1.4/src/comex/utils/java_nodes.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/utils/postprocessor.py` & `comex-0.1.4/src/comex/utils/postprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/utils/preprocessor.py` & `comex-0.1.4/src/comex/utils/preprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex/utils/src_parser.py` & `comex-0.1.4/src/comex/utils/src_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.3/src/comex.egg-info/PKG-INFO` & `comex-0.1.4/src/comex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -18,14 +18,31 @@
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
+If you wish to learn more about the approach taken, here are some conference talks and publications:
+- ASE 2023 demonstration: [COMEX: A Tool for Generating Customized Source Code Representations](https://arxiv.org/abs/2307.04693)
+- ICSE 2023 tutorial: [The Landscape of Source Code Representation Learning in AI-Driven Software Engineering Tasks](https://research.ibm.com/publications/the-landscape-of-source-code-representation-learning-in-ai-driven-software-engineering-tasks)
+
+## Cite Comex
+If you use Comex in your research, please cite our work by using the following BibTeX entry:
+```
+@misc{das2023comex,
+      title={COMEX: A Tool for Generating Customized Source Code Representations}, 
+      author={Debeshee Das and Noble Saji Mathews and Alex Mathai and Srikanth Tamilselvam and Kranthi Sedamaki and Sridhar Chimalakonda and Atul Kumar},
+      year={2023},
+      eprint={2307.04693},
+      archivePrefix={arXiv},
+      primaryClass={cs.SE}
+}
+```
+
 ---
 ## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
```

### Comparing `comex-0.1.3/src/comex.egg-info/SOURCES.txt` & `comex-0.1.4/src/comex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

