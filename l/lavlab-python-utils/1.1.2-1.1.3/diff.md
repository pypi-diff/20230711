# Comparing `tmp/lavlab-python-utils-1.1.2.tar.gz` & `tmp/lavlab-python-utils-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.1.2.tar", last modified: Tue Jul 11 12:58:40 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.1.3.tar", last modified: Tue Jul 11 14:49:03 2023, max compression
```

## Comparing `lavlab-python-utils-1.1.2.tar` & `lavlab-python-utils-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    27566 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 12:58:40.000000 lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 12:58:40.000000 lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:58:40.000000 lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 12:58:40.000000 lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 12:58:40.000000 lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:58:40.790101 lavlab-python-utils-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/test/test_omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 12:58:29.000000 lavlab-python-utils-1.1.2/test/test_python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.221859 lavlab-python-utils-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:49:03.221859 lavlab-python-utils-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.1.2/PKG-INFO` & `lavlab-python-utils-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.1.2/pyproject.toml` & `lavlab-python-utils-1.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lavlab-python-utils"
 description = "LaViolette Lab utility package"
-version = "1.1.2"
+version = "1.1.3"
 
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 
 readme = "README.rst"
 classifiers = [
```

### Comparing `lavlab-python-utils-1.1.2/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.1.3/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.2/src/lavlab/omero_util.py` & `lavlab-python-utils-1.1.3/src/lavlab/omero_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 """
 Helper functions that handle high-level operations and translating asynchronous requests for easy development.
 """
 import os
 import asyncio
 import tempfile
 
@@ -516,16 +517,16 @@
     get tiles for timepoints
 
 Returns
 -------
 list
     List of (z,c,t,(x,y,w,h)) tiles for use in getTiles.
     """
-    width = range(img.getSizeX())
-    height = range(img.getSizeY())
+    width = img.getSizeX()
+    height = img.getSizeY()
     z_indexes = range(img.getSizeZ())
     timepoints = range(img.getSizeT())
     channels = range(img.getSizeC())
 
     img._prepareRenderingEngine()
     tile_size = img._re.getTileSize()
     img._re.close()
```

### Comparing `lavlab-python-utils-1.1.2/src/lavlab/python_util.py` & `lavlab-python-utils-1.1.3/src/lavlab/python_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 """
 Contains general utilities for lavlab's python scripts.
 """
 import os
 import asyncio
 
 import numpy as np
```

### Comparing `lavlab-python-utils-1.1.2/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.1.2/test/test_omero_util.py` & `lavlab-python-utils-1.1.3/test/test_omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.2/test/test_python_utils.py` & `lavlab-python-utils-1.1.3/test/test_python_utils.py`

 * *Files identical despite different names*

