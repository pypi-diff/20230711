# Comparing `tmp/relics_run_api-0.1.0.tar.gz` & `tmp/relics_run_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relics_run_api-0.1.0.tar", max compression
+gzip compressed data, was "relics_run_api-0.1.1.tar", max compression
```

## Comparing `relics_run_api-0.1.0.tar` & `relics_run_api-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1861 2023-07-11 05:38:09.294345 relics_run_api-0.1.0/README.md
--rw-r--r--   0        0        0      359 2023-07-06 23:09:57.318352 relics_run_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      453 2023-07-11 04:58:01.087621 relics_run_api-0.1.0/relics_run_api/__init__.py
--rw-r--r--   0        0        0       74 2023-07-06 19:34:21.444404 relics_run_api-0.1.0/relics_run_api/base.py
--rw-r--r--   0        0        0      853 2023-07-09 21:27:32.255101 relics_run_api-0.1.0/relics_run_api/common.py
--rw-r--r--   0        0        0     3759 2023-07-11 04:19:41.291061 relics_run_api-0.1.0/relics_run_api/history.py
--rw-r--r--   0        0        0     4205 2023-07-11 04:44:55.474112 relics_run_api-0.1.0/relics_run_api/index.py
--rw-r--r--   0        0        0     3058 2023-07-11 04:34:19.355250 relics_run_api-0.1.0/relics_run_api/market_data.py
--rw-r--r--   0        0        0     2754 2023-07-11 04:59:02.762503 relics_run_api-0.1.0/relics_run_api/output.py
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 relics_run_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-11 05:57:12.801523 relics_run_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2172 2023-07-11 05:55:00.742843 relics_run_api-0.1.1/README.md
+-rw-r--r--   0        0        0      388 2023-07-11 05:58:37.468318 relics_run_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-11 04:58:01.087621 relics_run_api-0.1.1/relics_run_api/__init__.py
+-rw-r--r--   0        0        0       74 2023-07-06 19:34:21.444404 relics_run_api-0.1.1/relics_run_api/base.py
+-rw-r--r--   0        0        0      853 2023-07-09 21:27:32.255101 relics_run_api-0.1.1/relics_run_api/common.py
+-rw-r--r--   0        0        0     3759 2023-07-11 04:19:41.291061 relics_run_api-0.1.1/relics_run_api/history.py
+-rw-r--r--   0        0        0     4205 2023-07-11 04:44:55.474112 relics_run_api-0.1.1/relics_run_api/index.py
+-rw-r--r--   0        0        0     3058 2023-07-11 04:34:19.355250 relics_run_api-0.1.1/relics_run_api/market_data.py
+-rw-r--r--   0        0        0     2754 2023-07-11 04:59:02.762503 relics_run_api-0.1.1/relics_run_api/output.py
+-rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 relics_run_api-0.1.1/PKG-INFO
```

### Comparing `relics_run_api-0.1.0/README.md` & `relics_run_api-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Relics.run API
 
+[![PyPI](https://img.shields.io/pypi/v/relics-run-api) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/relics-run-api) ![PyPI - Format](https://img.shields.io/pypi/format/relics-run-api) ![PyPI - License](https://img.shields.io/pypi/l/relics-run-api)](https://pypi.org/project/relics-run-api/)
+
 This is an unofficial API for the [Relics.run](https://relics.run/) website.
 
 The API is currently in development and is subject to change.
 Through the API, you can access the same data that is available on the website.
 This API only facilitates the retrieval of data through functions.
 
 ## Usage
```

### Comparing `relics_run_api-0.1.0/relics_run_api/common.py` & `relics_run_api-0.1.1/relics_run_api/common.py`

 * *Files identical despite different names*

### Comparing `relics_run_api-0.1.0/relics_run_api/history.py` & `relics_run_api-0.1.1/relics_run_api/history.py`

 * *Files identical despite different names*

### Comparing `relics_run_api-0.1.0/relics_run_api/index.py` & `relics_run_api-0.1.1/relics_run_api/index.py`

 * *Files identical despite different names*

### Comparing `relics_run_api-0.1.0/relics_run_api/market_data.py` & `relics_run_api-0.1.1/relics_run_api/market_data.py`

 * *Files identical despite different names*

### Comparing `relics_run_api-0.1.0/relics_run_api/output.py` & `relics_run_api-0.1.1/relics_run_api/output.py`

 * *Files identical despite different names*

