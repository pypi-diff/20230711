# Comparing `tmp/pycltools-1.1.4.tar.gz` & `tmp/pycltools-1.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.4.tar", last modified: Tue Jul 11 14:18:03 2023, max compression
+gzip compressed data, was "pycltools-1.1.4.1.tar", last modified: Tue Jul 11 14:30:52 2023, max compression
```

## Comparing `pycltools-1.1.4.tar` & `pycltools-1.1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:18:03.619540 pycltools-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:17:52.000000 pycltools-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 14:18:03.619540 pycltools-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-11 14:17:52.000000 pycltools-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:18:03.619540 pycltools-1.1.4/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-11 14:17:52.000000 pycltools-1.1.4/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45124 2023-07-11 14:17:52.000000 pycltools-1.1.4/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:18:03.619540 pycltools-1.1.4/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:18:03.000000 pycltools-1.1.4/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:18:03.619540 pycltools-1.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:17:52.000000 pycltools-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:52.495248 pycltools-1.1.4.1/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46240 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:30:52.000000 pycltools-1.1.4.1/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:52.499248 pycltools-1.1.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 14:30:40.000000 pycltools-1.1.4.1/setup.py
```

### Comparing `pycltools-1.1.4/LICENSE` & `pycltools-1.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.4/PKG-INFO` & `pycltools-1.1.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.4
+Version: 1.1.4.1
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycoQC
 Author: Adrien Leger
 Author-email: aleg@ebi.ac.uk
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycltools-1.1.4/README.md` & `pycltools-1.1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.4/pycltools/__init__.py` & `pycltools-1.1.4.1/pycltools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.4"
+__version__ = "1.1.4.1"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "aleg@ebi.ac.uk"
 __url__ = "https://github.com/a-slide/pycoQC"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pycltools-1.1.4/pycltools/pycltools.py` & `pycltools-1.1.4.1/pycltools/pycltools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1474,7 +1474,37 @@
                 else:
                     counter_dict[label]["primary"] += 1
                     counter_dict[label]["primary bases"] += read.infer_read_length()
                     if read.mapping_quality >= min_mapq:
                         counter_dict[label]["primary high mapq"] += 1
 
     return pd.DataFrame(counter_dict)
+
+class random_seed_gen ():
+    def __init__(self, seed=None, skip_previous_seed=False, verbose=False):
+        """
+        Initiate a random seed generator object
+        * seed: int or None (default None)
+            Initial state. If None the first state is chosen randomly            
+        * skip_previous_seed: bool (default False)
+            If True track previously drawn seeds and make sure they are not used again
+        * verbose: bool (default False)
+        """
+        self.seed=seed
+        self.skip_previous_seed = skip_previous_seed
+        self.verbose = verbose
+        if skip_previous_seed:
+            self.previous_seeds = set()
+        random.seed(self.seed)
+
+    def __call__ (self):
+        seed = random.randint(0, sys.maxsize)
+        if self.skip_previous_seed:
+            if seed in self.previous_seeds:
+                if self.verbose:
+                    print(f"Seed {seed} already known. Incrementing")
+                while seed in self.previous_seeds:
+                    seed += 1
+            self.previous_seeds.add(seed)
+
+        random.seed(seed)
+        self.seed = seed
```

### Comparing `pycltools-1.1.4/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.4.1/pycltools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.4
+Version: 1.1.4.1
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycoQC
 Author: Adrien Leger
 Author-email: aleg@ebi.ac.uk
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

