# Comparing `tmp/pycltools-1.1.3.9.tar.gz` & `tmp/pycltools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.3.9.tar", last modified: Wed Mar 17 16:57:01 2021, max compression
+gzip compressed data, was "pycltools-1.1.4.tar", last modified: Tue Jul 11 14:18:03 2023, max compression
```

## Comparing `pycltools-1.1.3.9.tar` & `pycltools-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 16:57:01.017242 pycltools-1.1.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2021-03-17 16:57:01.017242 pycltools-1.1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2021-03-17 16:56:50.000000 pycltools-1.1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 16:57:01.013242 pycltools-1.1.3.9/pycltools/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2021-03-17 16:56:50.000000 pycltools-1.1.3.9/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    86553 2021-03-17 16:56:50.000000 pycltools-1.1.3.9/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 16:57:01.017242 pycltools-1.1.3.9/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2021-03-17 16:57:00.000000 pycltools-1.1.3.9/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-03-17 16:57:00.000000 pycltools-1.1.3.9/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-17 16:57:00.000000 pycltools-1.1.3.9/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-03-17 16:57:00.000000 pycltools-1.1.3.9/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-17 16:57:00.000000 pycltools-1.1.3.9/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-17 16:57:01.017242 pycltools-1.1.3.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      130 2021-03-17 16:56:50.000000 pycltools-1.1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:18:03.619540 pycltools-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:17:52.000000 pycltools-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 14:18:03.619540 pycltools-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-11 14:17:52.000000 pycltools-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:18:03.619540 pycltools-1.1.4/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-11 14:17:52.000000 pycltools-1.1.4/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45124 2023-07-11 14:17:52.000000 pycltools-1.1.4/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:18:03.619540 pycltools-1.1.4/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:18:03.619540 pycltools-1.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:17:52.000000 pycltools-1.1.4/setup.py
```

### Comparing `pycltools-1.1.3.9/pycltools/__init__.py` & `pycltools-1.1.4/pycltools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.3.9"
+__version__ = "1.1.4"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "aleg@ebi.ac.uk"
 __url__ = "https://github.com/a-slide/pycoQC"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
@@ -15,17 +15,15 @@
     "Programming Language :: Python :: 3",
 ]
 
 __install_requires__ = [
     "pysam>=0.14.0",
     "pandas>=0.23.0",
     "numpy>=1.14.0",
-    "notebook>=5.6.0",
     "tqdm>=4.23.4",
-    "httplib2",
     "matplotlib>=3.0.0",
 ]
 __python_requires__ = ">=3"
 __description__ = "pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation..."
 
 # Collect info in a dictionnary for setup.py
 setup_dict = {
```

