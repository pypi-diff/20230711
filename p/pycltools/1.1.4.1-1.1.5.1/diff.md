# Comparing `tmp/pycltools-1.1.4.1.tar.gz` & `tmp/pycltools-1.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.4.1.tar", last modified: Tue Jul 11 14:30:52 2023, max compression
+gzip compressed data, was "pycltools-1.1.5.1.tar", last modified: Tue Jul 11 14:45:31 2023, max compression
```

## Comparing `pycltools-1.1.4.1.tar` & `pycltools-1.1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:52.495248 pycltools-1.1.4.1/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46240 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46240 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/setup.py
```

### Comparing `pycltools-1.1.4.1/LICENSE` & `pycltools-1.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.4.1/PKG-INFO` & `pycltools-1.1.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.4.1
+Version: 1.1.5.1
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
-Home-page: https://github.com/a-slide/pycoQC
+Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
-Author-email: aleg@ebi.ac.uk
+Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
```

### Comparing `pycltools-1.1.4.1/README.md` & `pycltools-1.1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,13 +74,11 @@
 
 List of all functions contained in the package with a short description: [functions list Notebook](https://a-slide.github.io/pycltools/pycltools_functions_list.html)
 
 Detailed usage of most of the functions with basic tests: [Tests Notebook](https://a-slide.github.io/pycltools/pycltools_tests.html)
 
 ## Authors and Contact
 
-Adrien Leger - 2019
-
-EMBL EBI
+Adrien Leger - 2023
 
 * <aleg@ebi.ac.uk>
 * [Github](https://github.com/a-slide)
```

### Comparing `pycltools-1.1.4.1/pycltools/__init__.py` & `pycltools-1.1.5.1/pycltools/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.4.1"
+__version__ = "1.1.5.1"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
-__email__ = "aleg@ebi.ac.uk"
-__url__ = "https://github.com/a-slide/pycoQC"
+__email__ = "adrien.leger@nanoporetech.com"
+__url__ = "https://github.com/a-slide/pycltools"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
```

### Comparing `pycltools-1.1.4.1/pycltools/pycltools.py` & `pycltools-1.1.5.1/pycltools/pycltools.py`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.4.1/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.5.1/pycltools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.4.1
+Version: 1.1.5.1
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
-Home-page: https://github.com/a-slide/pycoQC
+Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
-Author-email: aleg@ebi.ac.uk
+Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
```

