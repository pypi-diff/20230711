# Comparing `tmp/dotenver-1.2.1.tar.gz` & `tmp/dotenver-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenver-1.2.1.tar", max compression
+gzip compressed data, was "dotenver-1.2.2.tar", last modified: Tue Jul 11 13:50:51 2023, max compression
```

## Comparing `dotenver-1.2.1.tar` & `dotenver-1.2.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1536 2021-06-12 14:19:12.642512 dotenver-1.2.1/LICENSE
--rw-r--r--   0        0        0     2195 2021-06-12 14:19:12.642639 dotenver-1.2.1/README.rst
--rw-r--r--   0        0        0       22 2021-06-12 14:19:12.642796 dotenver-1.2.1/dotenver/__init__.py
--rw-r--r--   0        0        0     3764 2021-06-12 14:19:12.642923 dotenver-1.2.1/dotenver/cli.py
--rw-r--r--   0        0        0     8187 2021-06-12 14:19:12.643070 dotenver-1.2.1/dotenver/dotenver.py
--rw-r--r--   0        0        0     1016 2021-06-12 14:19:12.643186 dotenver-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3354 2021-06-12 14:23:08.837000 dotenver-1.2.1/setup.py
--rw-r--r--   0        0        0     3444 2021-06-12 14:23:08.837339 dotenver-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1536 2021-06-12 14:19:12.000000 dotenver-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2237 2023-07-11 13:46:41.246272 dotenver-1.2.2/README.rst
+-rw-r--r--   0        0        0       22 2023-07-11 13:48:18.562037 dotenver-1.2.2/dotenver/__init__.py
+-rw-r--r--   0        0        0     3764 2021-06-12 14:19:12.000000 dotenver-1.2.2/dotenver/cli.py
+-rw-r--r--   0        0        0     8187 2021-06-12 14:19:12.000000 dotenver-1.2.2/dotenver/dotenver.py
+-rw-r--r--   0        0        0     1103 2023-07-11 13:50:51.990958 dotenver-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-06-12 14:19:12.000000 dotenver-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     8216 2023-07-11 13:46:41.247126 dotenver-1.2.2/tests/test_dotenver.py
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 dotenver-1.2.2/PKG-INFO
```

### Comparing `dotenver-1.2.1/LICENSE` & `dotenver-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.1/README.rst` & `dotenver-1.2.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ============================
 Python DotEnver
 ============================
 
 .. image:: https://badge.fury.io/py/dotenver.svg
     :target: https://badge.fury.io/py/dotenver
 
-.. image:: https://travis-ci.org/jmfederico/dotenver.svg?branch=master
-    :target: https://travis-ci.org/jmfederico/dotenver
+.. image:: https://github.com/jmfederico/dotenver/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/jmfederico/dotenver/actions/workflows/tests.yml
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
 
 A Python app to generate dotenv (.env) files from templates.
```

### Comparing `dotenver-1.2.1/dotenver/cli.py` & `dotenver-1.2.2/dotenver/cli.py`

 * *Files identical despite different names*

### Comparing `dotenver-1.2.1/dotenver/dotenver.py` & `dotenver-1.2.2/dotenver/dotenver.py`

 * *Files identical despite different names*

