# Comparing `tmp/pycltools-1.1.5.4.tar.gz` & `tmp/pycltools-1.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.5.4.tar", last modified: Tue Jul 11 15:15:53 2023, max compression
+gzip compressed data, was "pycltools-1.1.5.5.tar", last modified: Tue Jul 11 15:33:56 2023, max compression
```

## Comparing `pycltools-1.1.5.4.tar` & `pycltools-1.1.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:15:53.699073 pycltools-1.1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:15:53.699073 pycltools-1.1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:15:53.695073 pycltools-1.1.5.4/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46273 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:15:53.695073 pycltools-1.1.5.4/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:15:53.000000 pycltools-1.1.5.4/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:15:53.699073 pycltools-1.1.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 15:15:41.000000 pycltools-1.1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:33:56.334192 pycltools-1.1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:33:56.330192 pycltools-1.1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:33:56.330192 pycltools-1.1.5.5/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46778 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:33:56.330192 pycltools-1.1.5.5/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:33:56.334192 pycltools-1.1.5.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/setup.py
```

### Comparing `pycltools-1.1.5.4/LICENSE` & `pycltools-1.1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.4/PKG-INFO` & `pycltools-1.1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.4
+Version: 1.1.5.5
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycltools-1.1.5.4/README.md` & `pycltools-1.1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.4/pycltools/__init__.py` & `pycltools-1.1.5.5/pycltools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.5.4"
+__version__ = "1.1.5.5"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "adrien.leger@nanoporetech.com"
 __url__ = "https://github.com/a-slide/pycltools"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pycltools-1.1.5.4/pycltools/pycltools.py` & `pycltools-1.1.5.5/pycltools/pycltools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1255,14 +1255,16 @@
     bases=["A", "G", "T", "C"],
     kmer_len=3,
     hp_max=3,
     seq_len=100,
     n_seq=10,
     seed=None,
     include_rc=False,
+    init_seq=None,
+    init_counter=None,
     verbose=False,
 ):
     """
     Generate a list of sequences with an optimized kmer content.
     * how
         min = Always choose the kmer with the lower kmer count in the previous sequence. Random in case of ties
         weights = Bases are randomly picked based on a probability invertly corelated to the kmer counts in the previous sequence
@@ -1272,26 +1274,39 @@
         Length of kmer to optimize the distribution
     * hp_max: int (default 3)
         Maximal length of homopolymers
     * seq_len: int or list (default 100)
         Length of sequences to be generated
     * n_seq: int (default 10)
         Overall number of sequences to be generated
+    * init_seq: str (default None)
+        Sequence to initialise the kmer counter from
+    * init_counter: str (default None)
+        Kmer counter to initialise from
     * seed: None or int
         If given the random generator will behave in a deterministic way
     """
     # Set seed if needed
     if seed is None:
         random.seed(None)
         seed = random.randint(0, MAX_SEED_VALUE)
         
     random.seed(seed)
     np.random.seed(seed)  
 
     kmer_c = Counter()
+    if init_seq and len(init_seq) >= kmer_len:
+        for i in range(0, len(init_seq) - kmer_len):
+            kmer = init_seq[i:i+kmer_len]
+            if set(kmer).difference(set(bases)):
+                continue
+            kmer_c[kmer]+=1
+
+    if init_counter:
+        kmer_c = init_counter
 
     seq_l = []
     if n_seq > 1 and type(seq_len) == int:
         seq_len = list(itertools.repeat(seq_len, n_seq))
         
     elif n_seq == 1 and type(seq_len) == int:
         seq_len = [seq_len,]
```

### Comparing `pycltools-1.1.5.4/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.5.5/pycltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.4
+Version: 1.1.5.5
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

