# Comparing `tmp/mcemtools-0.2.0.tar.gz` & `tmp/mcemtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.2.0.tar", last modified: Tue Jul 11 03:57:10 2023, max compression
+gzip compressed data, was "mcemtools-0.3.0.tar", last modified: Tue Jul 11 04:13:27 2023, max compression
```

## Comparing `mcemtools-0.2.0.tar` & `mcemtools-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 03:57:00.000000 mcemtools-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-11 03:57:00.000000 mcemtools-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 03:57:00.000000 mcemtools-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 03:57:00.000000 mcemtools-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 03:57:00.000000 mcemtools-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-11 03:57:10.011534 mcemtools-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 03:57:00.000000 mcemtools-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.007534 mcemtools-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 03:57:10.000000 mcemtools-0.2.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 03:57:00.000000 mcemtools-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 03:57:10.015534 mcemtools-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-11 03:57:00.000000 mcemtools-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 03:57:00.000000 mcemtools-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-11 03:57:00.000000 mcemtools-0.2.0/tests/test_mcemtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:13:27.289460 mcemtools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 04:13:15.000000 mcemtools-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-11 04:13:15.000000 mcemtools-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 04:13:15.000000 mcemtools-0.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 04:13:15.000000 mcemtools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 04:13:15.000000 mcemtools-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-11 04:13:27.289460 mcemtools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 04:13:15.000000 mcemtools-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:13:27.285460 mcemtools-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 04:13:15.000000 mcemtools-0.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:13:27.285460 mcemtools-0.3.0/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-11 04:13:15.000000 mcemtools-0.3.0/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:13:27.289460 mcemtools-0.3.0/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 04:13:27.000000 mcemtools-0.3.0/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 04:13:15.000000 mcemtools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 04:13:27.289460 mcemtools-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 04:13:15.000000 mcemtools-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:13:27.289460 mcemtools-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 04:13:15.000000 mcemtools-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 04:13:15.000000 mcemtools-0.3.0/tests/test_mcemtools.py
```

### Comparing `mcemtools-0.2.0/CONTRIBUTING.rst` & `mcemtools-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/LICENSE` & `mcemtools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/PKG-INFO` & `mcemtools-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -74,7 +74,13 @@
 * First release on PyPI.
 
 0.2.0 (2023-07-11)
 ------------------
 
 * Many functions used for 4D-STEM analysis have been added.
 * OOP is avoided as much as possible.
+
+0.3.0 (2023-07-11)
+------------------
+
+* Tests are increasing in number
+* init includes import of mcemtools
```

### Comparing `mcemtools-0.2.0/README.rst` & `mcemtools-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/docs/Makefile` & `mcemtools-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/docs/conf.py` & `mcemtools-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/docs/installation.rst` & `mcemtools-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/docs/make.bat` & `mcemtools-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/mcemtools/analysis.py` & `mcemtools-0.3.0/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/mcemtools/masking.py` & `mcemtools-0.3.0/mcemtools/masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/mcemtools/mcemtools.py` & `mcemtools-0.3.0/mcemtools/mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/mcemtools/tensor_svd.py` & `mcemtools-0.3.0/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/mcemtools/transforms.py` & `mcemtools-0.3.0/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.3.0/mcemtools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -74,7 +74,13 @@
 * First release on PyPI.
 
 0.2.0 (2023-07-11)
 ------------------
 
 * Many functions used for 4D-STEM analysis have been added.
 * OOP is avoided as much as possible.
+
+0.3.0 (2023-07-11)
+------------------
+
+* Tests are increasing in number
+* init includes import of mcemtools
```

### Comparing `mcemtools-0.2.0/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.3.0/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.2.0/setup.py` & `mcemtools-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
-_version = '0.2.0'
+_version = '0.3.0'
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['Click>=7.0', ]
+requirements = ['numpy']
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Alireza Sadri",
     author_email='Alireza.Sadri@monash.edu',
     python_requires='>=3.7',
```

