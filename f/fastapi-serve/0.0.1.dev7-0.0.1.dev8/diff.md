# Comparing `tmp/fastapi-serve-0.0.1.dev7.tar.gz` & `tmp/fastapi-serve-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.1.dev7.tar", last modified: Tue Jul 11 14:49:26 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.1.dev8.tar", last modified: Tue Jul 11 14:52:00 2023, max compression
```

## Comparing `fastapi-serve-0.0.1.dev7.tar` & `fastapi-serve-0.0.1.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:26.587529 fastapi-serve-0.0.1.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 14:49:22.000000 fastapi-serve-0.0.1.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 14:49:26.587529 fastapi-serve-0.0.1.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 14:49:22.000000 fastapi-serve-0.0.1.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:26.587529 fastapi-serve-0.0.1.dev7/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 14:49:22.000000 fastapi-serve-0.0.1.dev7/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:26.587529 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 14:49:26.000000 fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:49:26.587529 fastapi-serve-0.0.1.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-11 14:49:22.000000 fastapi-serve-0.0.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/setup.py
```

### Comparing `fastapi-serve-0.0.1.dev7/LICENSE` & `fastapi-serve-0.0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.1.dev7/PKG-INFO` & `fastapi-serve-0.0.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.1.dev7 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.1.dev8 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/now Project-URL: Tracker, https://github.com/jina-ai/now/
 issues Keywords: jina fastapi restapi cloud docker kubernetes Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `fastapi-serve-0.0.1.dev7/README.md` & `fastapi-serve-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.1.dev7/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.1.dev7 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.1.dev8 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/now Project-URL: Tracker, https://github.com/jina-ai/now/
 issues Keywords: jina fastapi restapi cloud docker kubernetes Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `fastapi-serve-0.0.1.dev7/setup.py` & `fastapi-serve-0.0.1.dev8/setup.py`

 * *Files identical despite different names*

