# Comparing `tmp/bsimx-0.2.0.tar.gz` & `tmp/bsimx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsimx-0.2.0.tar", max compression
+gzip compressed data, was "bsimx-0.2.1.tar", max compression
```

## Comparing `bsimx-0.2.0.tar` & `bsimx-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0      645 2023-07-04 05:02:37.222850 bsimx-0.2.0/README.md
--rw-r--r--   0        0        0      529 2023-07-04 05:15:56.442853 bsimx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6406 2023-07-04 05:02:37.242850 bsimx-0.2.0/src/bsimx.py
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 bsimx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      645 2023-07-04 05:02:37.222850 bsimx-0.2.1/README.md
+-rw-r--r--   0        0        0      603 2023-07-11 02:28:01.468981 bsimx-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6407 2023-07-11 02:11:32.668967 bsimx-0.2.1/src/bsimx/__init__.py
+-rw-r--r--   0        0        0  1619458 2023-07-11 02:24:31.858957 bsimx-0.2.1/src/bsimx/static/bundle.js
+-rw-r--r--   0        0        0    11679 2023-07-11 02:24:31.478957 bsimx-0.2.1/src/bsimx/static/style.css
+-rw-r--r--   0        0        0      960 2023-07-11 02:24:30.448957 bsimx-0.2.1/src/bsimx/templates/index.html
+-rw-r--r--   0        0        0      748 2023-07-11 02:10:34.608964 bsimx-0.2.1/src/bsimx/type.py
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 bsimx-0.2.1/PKG-INFO
```

### Comparing `bsimx-0.2.0/README.md` & `bsimx-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bsimx-0.2.0/pyproject.toml` & `bsimx-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 [tool.poetry]
 name = "bsimx"
-version = "0.2.0"
+version = "0.2.1"
 description = "The agent-based modeling tool with deck.gl, networkx and osmnx."
 authors = ["s-uei <uei.shunsuke@kagawa-u.ac.jp>"]
 readme = "README.md"
+include = [
+    "src/**/*.html",
+    "src/**/*.js",
+    "src/**/*.css",
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 networkx = "^2.8.8"
 osmnx = "^1.3.0"
 flask = "^2.2.3"
 pydantic = "^1.10.9"
```

### Comparing `bsimx-0.2.0/src/bsimx.py` & `bsimx-0.2.1/src/bsimx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Optional, Any, Union
 import networkx as nx
 import json
 from flask import Flask, render_template
 import json
 
-from type import (
+from .type import (
     AgentResult,
     AreaBounds,
     EdgeResult,
     NodeResult,
     Position,
     RouteResult,
     SimulationResult,
```

### Comparing `bsimx-0.2.0/PKG-INFO` & `bsimx-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsimx
-Version: 0.2.0
+Version: 0.2.1
 Summary: The agent-based modeling tool with deck.gl, networkx and osmnx.
 Author: s-uei
 Author-email: uei.shunsuke@kagawa-u.ac.jp
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

