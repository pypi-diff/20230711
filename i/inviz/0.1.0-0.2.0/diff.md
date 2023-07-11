# Comparing `tmp/inviz-0.1.0.tar.gz` & `tmp/inviz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.1.0.tar", last modified: Sun Jun 18 03:23:29 2023, max compression
+gzip compressed data, was "inviz-0.2.0.tar", last modified: Tue Jul 11 00:27:56 2023, max compression
```

## Comparing `inviz-0.1.0.tar` & `inviz-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-18 03:23:29.022444 inviz-0.1.0/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.1.0/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.1.0/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-06-18 03:23:29.022444 inviz-0.1.0/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1643 2023-06-15 14:20:14.000000 inviz-0.1.0/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-18 03:23:29.022444 inviz-0.1.0/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-18 03:23:29.022444 inviz-0.1.0/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       89 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)     6472 2023-06-18 03:02:43.000000 inviz-0.1.0/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-06-18 03:23:29.022444 inviz-0.1.0/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1100 2023-06-18 03:02:43.000000 inviz-0.1.0/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-11 00:27:56.098684 inviz-0.2.0/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.0/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.0/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-07-11 00:27:56.098684 inviz-0.2.0/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1643 2023-06-15 14:20:14.000000 inviz-0.2.0/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-11 00:27:56.088684 inviz-0.2.0/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-11 00:27:56.098684 inviz-0.2.0/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       89 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10342 2023-07-10 23:57:56.000000 inviz-0.2.0/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-11 00:27:56.098684 inviz-0.2.0/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1100 2023-07-11 00:03:27.000000 inviz-0.2.0/setup.py
```

### Comparing `inviz-0.1.0/LICENSE` & `inviz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.1.0/PKG-INFO` & `inviz-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.1.0
+Version: 0.2.0
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.1.0/README.md` & `inviz-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.1.0/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.0/inviz/inviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.1.0
+Version: 0.2.0
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.1.0/setup.py` & `inviz-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.1.0",
+    version = "0.2.0",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
```

