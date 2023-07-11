# Comparing `tmp/pycltools-1.1.5.2.tar.gz` & `tmp/pycltools-1.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.5.2.tar", last modified: Tue Jul 11 14:48:52 2023, max compression
+gzip compressed data, was "pycltools-1.1.5.3.tar", last modified: Tue Jul 11 15:00:52 2023, max compression
```

## Comparing `pycltools-1.1.5.2.tar` & `pycltools-1.1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46248 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46278 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:00:52.000000 pycltools-1.1.5.3/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:00:52.190820 pycltools-1.1.5.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 15:00:41.000000 pycltools-1.1.5.3/setup.py
```

### Comparing `pycltools-1.1.5.2/LICENSE` & `pycltools-1.1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.2/PKG-INFO` & `pycltools-1.1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.2
+Version: 1.1.5.3
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycltools-1.1.5.2/README.md` & `pycltools-1.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.2/pycltools/__init__.py` & `pycltools-1.1.5.3/pycltools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.5.2"
+__version__ = "1.1.5.3"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "adrien.leger@nanoporetech.com"
 __url__ = "https://github.com/a-slide/pycltools"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pycltools-1.1.5.2/pycltools/pycltools.py` & `pycltools-1.1.5.3/pycltools/pycltools.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import pysam as ps
 from tqdm import tqdm
 import numpy as np
 from matplotlib import pyplot as pl
 
 ##~~~~~~~ DEFINE CONSTANTS ~~~~~~~#
 
+MAX_SEED_VALUE = 2**32
+
 COLOR_CODES = {
     "white": 29,
     "grey": 30,
     "red": 31,
     "green": 32,
     "yellow": 33,
     "blue": 34,
@@ -1276,15 +1278,15 @@
         Overall number of sequences to be generated
     * seed: None or int
         If given the random generator will behave in a deterministic way
     """
     # Set seed if needed
     if seed is None:
         random.seed(None)
-        seed = random.randint(0, sys.maxsize)
+        seed = random.randint(0, MAX_SEED_VALUE)
         
     random.seed(seed)
     np.random.seed(seed)  
 
     kmer_c = Counter()
 
     seq_l = []
@@ -1494,15 +1496,15 @@
         self.skip_previous_seed = skip_previous_seed
         self.verbose = verbose
         if skip_previous_seed:
             self.previous_seeds = set()
         random.seed(self.seed)
 
     def __call__ (self):
-        seed = random.randint(0, sys.maxsize)
+        seed = random.randint(0, MAX_SEED_VALUE)
         if self.skip_previous_seed:
             if seed in self.previous_seeds:
                 if self.verbose:
                     print(f"Seed {seed} already known. Incrementing")
                 while seed in self.previous_seeds:
                     seed += 1
             self.previous_seeds.add(seed)
```

### Comparing `pycltools-1.1.5.2/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.5.3/pycltools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.2
+Version: 1.1.5.3
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

