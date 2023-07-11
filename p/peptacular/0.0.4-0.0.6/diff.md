# Comparing `tmp/peptacular-0.0.4.tar.gz` & `tmp/peptacular-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptacular-0.0.4.tar", last modified: Tue May  2 16:52:35 2023, max compression
+gzip compressed data, was "peptacular-0.0.6.tar", last modified: Tue Jul 11 20:24:34 2023, max compression
```

## Comparing `peptacular-0.0.4.tar` & `peptacular-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:52:35.951821 peptacular-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 16:52:23.000000 peptacular-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-02 16:52:35.951821 peptacular-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 16:52:23.000000 peptacular-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-02 16:52:23.000000 peptacular-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:52:35.951821 peptacular-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 16:52:23.000000 peptacular-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:52:35.947821 peptacular-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:52:35.947821 peptacular-0.0.4/src/peptacular/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 16:52:23.000000 peptacular-0.0.4/src/peptacular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 16:52:23.000000 peptacular-0.0.4/src/peptacular/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-02 16:52:23.000000 peptacular-0.0.4/src/peptacular/peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-02 16:52:23.000000 peptacular-0.0.4/src/peptacular/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-02 16:52:23.000000 peptacular-0.0.4/src/peptacular/refseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 16:52:23.000000 peptacular-0.0.4/src/peptacular/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:52:35.951821 peptacular-0.0.4/src/peptacular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-02 16:52:35.000000 peptacular-0.0.4/src/peptacular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 16:52:35.000000 peptacular-0.0.4/src/peptacular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:52:35.000000 peptacular-0.0.4/src/peptacular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 16:52:35.000000 peptacular-0.0.4/src/peptacular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 16:52:35.000000 peptacular-0.0.4/src/peptacular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:52:35.951821 peptacular-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-02 16:52:23.000000 peptacular-0.0.4/tests/test_peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-05-02 16:52:23.000000 peptacular-0.0.4/tests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-02 16:52:23.000000 peptacular-0.0.4/tests/test_refstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 20:24:21.000000 peptacular-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-11 20:24:34.846794 peptacular-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-11 20:24:21.000000 peptacular-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-11 20:24:21.000000 peptacular-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:24:34.846794 peptacular-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 20:24:21.000000 peptacular-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/src/peptacular/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/refseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24396 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/src/peptacular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-07-11 20:24:21.000000 peptacular-0.0.6/tests/test_peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-11 20:24:21.000000 peptacular-0.0.6/tests/test_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-11 20:24:21.000000 peptacular-0.0.6/tests/test_refstring.py
```

### Comparing `peptacular-0.0.4/LICENSE` & `peptacular-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.4/PKG-INFO` & `peptacular-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.4
+Version: 0.0.6
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.4/README.md` & `peptacular-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.4/pyproject.toml` & `peptacular-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "regex",
+    "numpy"
 ]
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project.urls]
 repository = "https://github.com/pgarrett-scripps/peptacular.git"
```

### Comparing `peptacular-0.0.4/src/peptacular/refseq.py` & `peptacular-0.0.6/src/peptacular/refseq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from typing import Union
 
 
 class RefString:
     """A string-like class that stores a memory view of the string and slices by reference"""
     def __init__(self, value: Union[str, memoryview]):
         """Initializes a RefString object.
@@ -87,7 +88,10 @@
         return RefString(str(self).ljust(width, fillchar))
 
     def rjust(self, width, fillchar=' '):
         return RefString(str(self).rjust(width, fillchar))
 
     def center(self, width, fillchar=' '):
         return RefString(str(self).center(width, fillchar))
+
+    def __add__(self, other):
+        return RefString(str(self) + str(other))
```

### Comparing `peptacular-0.0.4/src/peptacular.egg-info/PKG-INFO` & `peptacular-0.0.6/src/peptacular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.4
+Version: 0.0.6
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.4/tests/test_refstring.py` & `peptacular-0.0.6/tests/test_refstring.py`

 * *Files identical despite different names*

