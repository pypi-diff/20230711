# Comparing `tmp/bwd-0.1.0.tar.gz` & `tmp/bwd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwd-0.1.0.tar", max compression
+gzip compressed data, was "bwd-0.1.1.tar", max compression
```

## Comparing `bwd-0.1.0.tar` & `bwd-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.0/LICENSE
--rw-r--r--   0        0        0      854 2023-07-10 21:58:45.218230 bwd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      495 2022-05-17 20:40:56.204982 bwd-0.1.0/src/bwd/__init__.py
--rw-r--r--   0        0        0     4204 2023-07-10 21:49:37.009554 bwd-0.1.0/src/bwd/bwd.py
--rw-r--r--   0        0        0     4107 2023-07-10 21:48:49.286458 bwd-0.1.0/src/bwd/bwd_random.py
--rw-r--r--   0        0        0     4745 2023-07-10 21:51:11.360429 bwd-0.1.0/src/bwd/multi_bwd.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bwd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.1/LICENSE
+-rw-r--r--   0        0        0      854 2023-07-11 11:01:58.243429 bwd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      495 2022-05-17 20:40:56.204982 bwd-0.1.1/src/bwd/__init__.py
+-rw-r--r--   0        0        0     4204 2023-07-10 21:49:37.009554 bwd-0.1.1/src/bwd/bwd.py
+-rw-r--r--   0        0        0     4107 2023-07-10 21:48:49.286458 bwd-0.1.1/src/bwd/bwd_random.py
+-rw-r--r--   0        0        0     4745 2023-07-10 21:51:11.360429 bwd-0.1.1/src/bwd/multi_bwd.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bwd-0.1.1/PKG-INFO
```

### Comparing `bwd-0.1.0/LICENSE` & `bwd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bwd-0.1.0/pyproject.toml` & `bwd-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bwd"
-version = "0.1.0"
+version = "0.1.1"
 description = "A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)"
 authors = ["Drew Dimmery <drew.dimmery@gmail.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = "^1.22.3"
```

### Comparing `bwd-0.1.0/src/bwd/bwd.py` & `bwd-0.1.1/src/bwd/bwd.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.0/src/bwd/bwd_random.py` & `bwd-0.1.1/src/bwd/bwd_random.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.0/src/bwd/multi_bwd.py` & `bwd-0.1.1/src/bwd/multi_bwd.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.0/PKG-INFO` & `bwd-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwd
-Version: 0.1.0
+Version: 0.1.1
 Summary: A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)
 License: Apache-2.0
 Author: Drew Dimmery
 Author-email: drew.dimmery@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

