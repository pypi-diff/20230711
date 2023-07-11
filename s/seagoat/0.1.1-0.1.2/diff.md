# Comparing `tmp/seagoat-0.1.1.tar.gz` & `tmp/seagoat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.1.1.tar", max compression
+gzip compressed data, was "seagoat-0.1.2.tar", max compression
```

## Comparing `seagoat-0.1.1.tar` & `seagoat-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-07-11 18:39:34.444967 seagoat-0.1.1/LICENSE
--rw-r--r--   0        0        0      771 2023-07-11 13:40:38.554139 seagoat-0.1.1/README.md
--rw-r--r--   0        0        0     1217 2023-07-11 19:05:23.382485 seagoat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/__init__.py
--rw-r--r--   0        0        0     1583 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/cache.py
--rw-r--r--   0        0        0      196 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/common.py
--rw-r--r--   0        0        0     4477 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/engine.py
--rw-r--r--   0        0        0     3474 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/file.py
--rw-r--r--   0        0        0     1827 2023-07-11 19:03:35.755526 seagoat-0.1.1/seagoat/main.py
--rw-r--r--   0        0        0     2664 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/repository.py
--rw-r--r--   0        0        0     1626 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/result.py
--rw-r--r--   0        0        0     1876 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1208 2023-07-11 13:40:38.560806 seagoat-0.1.1/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 seagoat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-11 18:39:34.444967 seagoat-0.1.2/LICENSE
+-rw-r--r--   0        0        0      771 2023-07-11 13:40:38.554139 seagoat-0.1.2/README.md
+-rw-r--r--   0        0        0     1217 2023-07-11 19:13:50.387003 seagoat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/__init__.py
+-rw-r--r--   0        0        0     1583 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/cache.py
+-rw-r--r--   0        0        0      196 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/common.py
+-rw-r--r--   0        0        0     4477 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/engine.py
+-rw-r--r--   0        0        0     3474 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/file.py
+-rw-r--r--   0        0        0     1862 2023-07-11 19:13:50.387003 seagoat-0.1.2/seagoat/main.py
+-rw-r--r--   0        0        0     2664 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/repository.py
+-rw-r--r--   0        0        0     1626 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/result.py
+-rw-r--r--   0        0        0     1876 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1208 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 seagoat-0.1.2/PKG-INFO
```

### Comparing `seagoat-0.1.1/LICENSE` & `seagoat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/README.md` & `seagoat-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/pyproject.toml` & `seagoat-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.1.1"
+version = "0.1.2"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.main:seagoat"
```

### Comparing `seagoat-0.1.1/seagoat/cache.py` & `seagoat-0.1.2/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/seagoat/engine.py` & `seagoat-0.1.2/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/seagoat/file.py` & `seagoat-0.1.2/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/seagoat/main.py` & `seagoat-0.1.2/seagoat/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from functools import cache
 import os
 import sys
 import click
 from pygments import highlight
 from pygments.lexers import get_lexer_for_filename
 from pygments.formatters import TerminalFormatter
 from pygments.lexers.javascript import JavascriptLexer, TypeScriptLexer
 
 from seagoat.engine import Engine
 
 
+@cache
 def get_highlighted_lines(file_name: str):
     with open(file_name, "r", encoding="utf-8") as source_code_file:
         code = source_code_file.read()
 
     if file_name.endswith(".md"):
         return code.splitlines()
```

### Comparing `seagoat-0.1.1/seagoat/repository.py` & `seagoat-0.1.2/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/seagoat/result.py` & `seagoat-0.1.2/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/seagoat/sources/chroma.py` & `seagoat-0.1.2/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/seagoat/sources/ripgrep.py` & `seagoat-0.1.2/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.1/PKG-INFO` & `seagoat-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.1.1
+Version: 0.1.2
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

