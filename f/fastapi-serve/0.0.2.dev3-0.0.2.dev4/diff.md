# Comparing `tmp/fastapi-serve-0.0.2.dev3.tar.gz` & `tmp/fastapi-serve-0.0.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.2.dev3.tar", last modified: Tue Jul 11 15:10:53 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.2.dev4.tar", last modified: Tue Jul 11 16:57:39 2023, max compression
```

## Comparing `fastapi-serve-0.0.2.dev3.tar` & `fastapi-serve-0.0.2.dev4.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:53.268398 fastapi-serve-0.0.2.dev3/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 15:10:52.000000 fastapi-serve-0.0.2.dev3/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.190368 fastapi-serve-0.0.2.dev4/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 16:57:38.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.190368 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/setup.py
```

### Comparing `fastapi-serve-0.0.2.dev3/LICENSE` & `fastapi-serve-0.0.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev3/PKG-INFO` & `fastapi-serve-0.0.2.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev3
+Version: 0.0.2.dev4
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
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev3 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev4 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev3/README.md` & `fastapi-serve-0.0.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev3
+Version: 0.0.2.dev4
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
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev3 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev4 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev3/setup.py` & `fastapi-serve-0.0.2.dev4/setup.py`

 * *Files identical despite different names*

