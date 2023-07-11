# Comparing `tmp/untouched-0.2.6.tar.gz` & `tmp/untouched-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untouched-0.2.6.tar", max compression
+gzip compressed data, was "untouched-0.2.7.tar", max compression
```

## Comparing `untouched-0.2.6.tar` & `untouched-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1783 2023-07-10 23:55:50.971863 untouched-0.2.6/README.md
--rw-r--r--   0        0        0      378 2023-07-11 19:44:52.545666 untouched-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.2.6/src/untouched/__init__.py
--rw-r--r--   0        0        0     2637 2023-07-10 23:46:39.295971 untouched-0.2.6/src/untouched/builder.py
--rw-r--r--   0        0        0      623 2023-07-11 19:43:26.031000 untouched-0.2.6/src/untouched/builder.pyi
--rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.2.6/src/untouched/registry.py
--rw-r--r--   0        0        0      489 2023-07-11 19:44:05.532353 untouched-0.2.6/src/untouched/registry.pyi
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 untouched-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1783 2023-07-10 23:55:50.971863 untouched-0.2.7/README.md
+-rw-r--r--   0        0        0      378 2023-07-11 19:56:15.708069 untouched-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.2.7/src/untouched/__init__.py
+-rw-r--r--   0        0        0     2637 2023-07-10 23:46:39.295971 untouched-0.2.7/src/untouched/builder.py
+-rw-r--r--   0        0        0      623 2023-07-11 19:43:26.031000 untouched-0.2.7/src/untouched/builder.pyi
+-rw-r--r--   0        0        0        0 2023-07-11 19:55:51.102929 untouched-0.2.7/src/untouched/py.typed
+-rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.2.7/src/untouched/registry.py
+-rw-r--r--   0        0        0      489 2023-07-11 19:44:05.532353 untouched-0.2.7/src/untouched/registry.pyi
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 untouched-0.2.7/PKG-INFO
```

### Comparing `untouched-0.2.6/README.md` & `untouched-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `untouched-0.2.6/src/untouched/builder.py` & `untouched-0.2.7/src/untouched/builder.py`

 * *Files identical despite different names*

### Comparing `untouched-0.2.6/src/untouched/builder.pyi` & `untouched-0.2.7/src/untouched/builder.pyi`

 * *Files identical despite different names*

### Comparing `untouched-0.2.6/src/untouched/registry.py` & `untouched-0.2.7/src/untouched/registry.py`

 * *Files identical despite different names*

### Comparing `untouched-0.2.6/PKG-INFO` & `untouched-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untouched
-Version: 0.2.6
+Version: 0.2.7
 Summary: Immutable builder, carbon copy of lann/builder package in GoLang.
 Author: damacaner
 Author-email: caner@damacana.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

