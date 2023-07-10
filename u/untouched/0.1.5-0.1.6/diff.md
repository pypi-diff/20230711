# Comparing `tmp/untouched-0.1.5.tar.gz` & `tmp/untouched-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untouched-0.1.5.tar", max compression
+gzip compressed data, was "untouched-0.1.6.tar", max compression
```

## Comparing `untouched-0.1.5.tar` & `untouched-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1942 2023-07-10 23:44:26.091213 untouched-0.1.5/README.md
--rw-r--r--   0        0        0      378 2023-07-10 23:43:57.479050 untouched-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.1.5/src/untouched/__init__.py
--rw-r--r--   0        0        0     2650 2023-07-10 23:40:43.753947 untouched-0.1.5/src/untouched/builder.py
--rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.1.5/src/untouched/registry.py
--rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 untouched-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1942 2023-07-10 23:44:26.091213 untouched-0.1.6/README.md
+-rw-r--r--   0        0        0      378 2023-07-10 23:46:20.230862 untouched-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.1.6/src/untouched/__init__.py
+-rw-r--r--   0        0        0     2686 2023-07-10 23:45:55.170720 untouched-0.1.6/src/untouched/builder.py
+-rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.1.6/src/untouched/registry.py
+-rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 untouched-0.1.6/PKG-INFO
```

### Comparing `untouched-0.1.5/README.md` & `untouched-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `untouched-0.1.5/src/untouched/builder.py` & `untouched-0.1.6/src/untouched/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import collections.abc
 from typing import Any, Dict, Optional, TypeVar
 
-from src.untouched.registry import Registry
+# import registry with most certain way possible
+from .registry import Registry
 
 # any subclass of Builder will be able to use the methods defined in Builder, or the methods defined in its subclasses
 T = TypeVar('T', bound='Builder')
 
 
 class Builder:
     """
```

### Comparing `untouched-0.1.5/src/untouched/registry.py` & `untouched-0.1.6/src/untouched/registry.py`

 * *Files identical despite different names*

### Comparing `untouched-0.1.5/PKG-INFO` & `untouched-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untouched
-Version: 0.1.5
+Version: 0.1.6
 Summary: Immutable builder, carbon copy of lann/builder package in GoLang.
 Author: damacaner
 Author-email: caner@damacana.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

