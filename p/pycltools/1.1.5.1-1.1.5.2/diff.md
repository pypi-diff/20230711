# Comparing `tmp/pycltools-1.1.5.1.tar.gz` & `tmp/pycltools-1.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.5.1.tar", last modified: Tue Jul 11 14:45:31 2023, max compression
+gzip compressed data, was "pycltools-1.1.5.2.tar", last modified: Tue Jul 11 14:48:52 2023, max compression
```

## Comparing `pycltools-1.1.5.1.tar` & `pycltools-1.1.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46240 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:45:31.000000 pycltools-1.1.5.1/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:45:31.328738 pycltools-1.1.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:45:20.000000 pycltools-1.1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46248 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:48:52.000000 pycltools-1.1.5.2/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:48:52.303358 pycltools-1.1.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:48:39.000000 pycltools-1.1.5.2/setup.py
```

### Comparing `pycltools-1.1.5.1/LICENSE` & `pycltools-1.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.1/PKG-INFO` & `pycltools-1.1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.1
+Version: 1.1.5.2
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycltools-1.1.5.1/README.md` & `pycltools-1.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.1/pycltools/__init__.py` & `pycltools-1.1.5.2/pycltools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.5.1"
+__version__ = "1.1.5.2"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "adrien.leger@nanoporetech.com"
 __url__ = "https://github.com/a-slide/pycltools"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pycltools-1.1.5.1/pycltools/pycltools.py` & `pycltools-1.1.5.2/pycltools/pycltools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1253,14 +1253,15 @@
     bases=["A", "G", "T", "C"],
     kmer_len=3,
     hp_max=3,
     seq_len=100,
     n_seq=10,
     seed=None,
     include_rc=False,
+    verbose=False,
 ):
     """
     Generate a list of sequences with an optimized kmer content.
     * how
         min = Always choose the kmer with the lower kmer count in the previous sequence. Random in case of ties
         weights = Bases are randomly picked based on a probability invertly corelated to the kmer counts in the previous sequence
     * bases = ["A","T","C","G"],
@@ -1457,15 +1458,15 @@
     * min_mapq
         minimal score to be considered high mapq
     """
     counter_dict = defaultdict(Counter)
     for bam in glob.glob(fp):
 
         label = bam.split("/")[-1].split(".")[0]
-        jprint("Parse bam {}".format(label), bold=True)
+        cprint("Parse bam {}".format(label))
 
         with ps.AlignmentFile(bam, "rb") as f:
             for read in f:
                 if read.is_unmapped:
                     counter_dict[label]["unmapped"] += 1
                 elif read.is_secondary:
                     counter_dict[label]["secondary"] += 1
```

### Comparing `pycltools-1.1.5.1/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.5.2/pycltools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.1
+Version: 1.1.5.2
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

