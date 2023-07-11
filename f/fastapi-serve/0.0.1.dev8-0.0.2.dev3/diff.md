# Comparing `tmp/fastapi-serve-0.0.1.dev8.tar.gz` & `tmp/fastapi-serve-0.0.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.1.dev8.tar", last modified: Tue Jul 11 14:52:00 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.2.dev3.tar", last modified: Tue Jul 11 15:10:53 2023, max compression
```

## Comparing `fastapi-serve-0.0.1.dev8.tar` & `fastapi-serve-0.0.2.dev3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 14:52:00.000000 fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:52:00.522381 fastapi-serve-0.0.1.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-11 14:51:53.000000 fastapi-serve-0.0.1.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:53.268398 fastapi-serve-0.0.2.dev3/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 15:10:52.000000 fastapi-serve-0.0.2.dev3/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 15:10:53.000000 fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:10:53.272398 fastapi-serve-0.0.2.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 15:10:47.000000 fastapi-serve-0.0.2.dev3/setup.py
```

### Comparing `fastapi-serve-0.0.1.dev8/LICENSE` & `fastapi-serve-0.0.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.1.dev8/PKG-INFO` & `fastapi-serve-0.0.2.dev3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.1.dev8
+Version: 0.0.2.dev3
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
-Project-URL: Source, https://github.com/jina-ai/now
-Project-URL: Tracker, https://github.com/jina-ai/now/issues
+Project-URL: Source, https://github.com/jina-ai/fastapi-serve/
+Project-URL: Tracker, https://github.com/jina-ai/fastapi-serve/issues
 Keywords: jina fastapi restapi cloud docker kubernetes
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.1.dev8 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev3 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
-github.com/jina-ai/now Project-URL: Tracker, https://github.com/jina-ai/now/
-issues Keywords: jina fastapi restapi cloud docker kubernetes Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Intended Audience :: Science/Research Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Environment :: Console Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Description-Content-Type: text/markdown Provides-Extra: test
-License-File: LICENSE
+github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
+jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
+kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Education Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
+Console Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
+Provides-Extra: test License-File: LICENSE
  ***** FastAPI-Serve: FastAPI to the Cloud, Batteries Included! âï¸ðð
                                      *****
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
 Welcome to **fastapi-serve**, a framework designed to take the pain out of
 deploying your local FastAPI applications to the cloud. Built using our open-
```

### Comparing `fastapi-serve-0.0.1.dev8/README.md` & `fastapi-serve-0.0.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.1.dev8/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.2.dev3/fastapi_serve.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.1.dev8
+Version: 0.0.2.dev3
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
-Project-URL: Source, https://github.com/jina-ai/now
-Project-URL: Tracker, https://github.com/jina-ai/now/issues
+Project-URL: Source, https://github.com/jina-ai/fastapi-serve/
+Project-URL: Tracker, https://github.com/jina-ai/fastapi-serve/issues
 Keywords: jina fastapi restapi cloud docker kubernetes
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.1.dev8 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev3 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
-github.com/jina-ai/now Project-URL: Tracker, https://github.com/jina-ai/now/
-issues Keywords: jina fastapi restapi cloud docker kubernetes Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Intended Audience :: Science/Research Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Environment :: Console Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Description-Content-Type: text/markdown Provides-Extra: test
-License-File: LICENSE
+github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
+jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
+kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Education Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
+Console Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
+Provides-Extra: test License-File: LICENSE
  ***** FastAPI-Serve: FastAPI to the Cloud, Batteries Included! âï¸ðð
                                      *****
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
 Welcome to **fastapi-serve**, a framework designed to take the pain out of
 deploying your local FastAPI applications to the cloud. Built using our open-
```

### Comparing `fastapi-serve-0.0.1.dev8/setup.py` & `fastapi-serve-0.0.2.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,12 @@
         "Environment :: Console",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     project_urls={
         "Documentation": "https://docs.jina.ai",
-        "Source": "https://github.com/jina-ai/now",
-        "Tracker": "https://github.com/jina-ai/now/issues",
+        "Source": "https://github.com/jina-ai/fastapi-serve/",
+        "Tracker": "https://github.com/jina-ai/fastapi-serve/issues",
     },
     keywords="jina fastapi restapi cloud docker kubernetes",
 )
```

