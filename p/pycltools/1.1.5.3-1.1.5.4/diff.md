# Comparing `tmp/pycltools-1.1.5.3.tar.gz` & `tmp/pycltools-1.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.5.3.tar", last modified: Tue Jul 11 15:00:52 2023, max compression
+gzip compressed data, was "pycltools-1.1.5.4.tar", last modified: Tue Jul 11 15:15:53 2023, max compression
```

## Comparing `pycltools-1.1.5.3.tar` & `pycltools-1.1.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46278 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:15:53.699073 pycltools-1.1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:15:53.699073 pycltools-1.1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:15:53.695073 pycltools-1.1.5.4/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46273 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:15:53.695073 pycltools-1.1.5.4/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:15:53.699073 pycltools-1.1.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/setup.py
```

### Comparing `pycltools-1.1.5.3/LICENSE` & `pycltools-1.1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.3/PKG-INFO` & `pycltools-1.1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.3
+Version: 1.1.5.4
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycltools-1.1.5.3/README.md` & `pycltools-1.1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.3/pycltools/__init__.py` & `pycltools-1.1.5.4/pycltools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.5.3"
+__version__ = "1.1.5.4"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "adrien.leger@nanoporetech.com"
 __url__ = "https://github.com/a-slide/pycltools"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pycltools-1.1.5.3/pycltools/pycltools.py` & `pycltools-1.1.5.4/pycltools/pycltools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1295,15 +1295,15 @@
         
     elif n_seq == 1 and type(seq_len) == int:
         seq_len = [seq_len,]
         
     elif type(seq_len) in (list, set, tuple) and len(seq_len) != n_seq:
         raise ValueError ("n_seq is not the same length as seq_len")
 
-    for slen in tqdm.tqdm(seq_len, disable=True):
+    for slen in tqdm(seq_len, disable=True):
         
         seq = []
 
         # First base
         hp = 1
         seq.append(random.choice(bases))
```

### Comparing `pycltools-1.1.5.3/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.5.4/pycltools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.3
+Version: 1.1.5.4
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

