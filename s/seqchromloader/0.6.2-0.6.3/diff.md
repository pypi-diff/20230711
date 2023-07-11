# Comparing `tmp/seqchromloader-0.6.2.tar.gz` & `tmp/seqchromloader-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.6.2.tar", last modified: Thu Jun 22 19:54:57 2023, max compression
+gzip compressed data, was "seqchromloader-0.6.3.tar", last modified: Tue Jul 11 18:48:50 2023, max compression
```

## Comparing `seqchromloader-0.6.2.tar` & `seqchromloader-0.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 19:54:57.720191 seqchromloader-0.6.2/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-22 19:54:57.719856 seqchromloader-0.6.2/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.2/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 19:54:57.712088 seqchromloader-0.6.2/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.2/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12749 2023-06-22 19:45:04.000000 seqchromloader-0.6.2/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14608 2023-06-22 01:59:36.000000 seqchromloader-0.6.2/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7280 2023-06-20 14:39:51.000000 seqchromloader-0.6.2/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 19:54:57.718499 seqchromloader-0.6.2/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-22 19:54:57.000000 seqchromloader-0.6.2/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-06-22 19:54:57.000000 seqchromloader-0.6.2/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-06-22 19:54:57.000000 seqchromloader-0.6.2/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-06-22 19:54:57.000000 seqchromloader-0.6.2/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-06-22 19:54:57.000000 seqchromloader-0.6.2/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-06-22 19:54:57.720266 seqchromloader-0.6.2/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-06-22 19:46:14.000000 seqchromloader-0.6.2/setup.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 19:54:57.719198 seqchromloader-0.6.2/tests/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    13030 2023-06-22 19:52:40.000000 seqchromloader-0.6.2/tests/test_writer_loader.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.367218 seqchromloader-0.6.3/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-11 18:48:50.366933 seqchromloader-0.6.3/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.3/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.347955 seqchromloader-0.6.3/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.3/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12749 2023-06-22 19:45:04.000000 seqchromloader-0.6.3/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14864 2023-07-11 18:46:36.000000 seqchromloader-0.6.3/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7280 2023-06-20 14:39:51.000000 seqchromloader-0.6.3/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.365960 seqchromloader-0.6.3/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-07-11 18:48:50.367296 seqchromloader-0.6.3/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-07-11 18:47:48.000000 seqchromloader-0.6.3/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.366497 seqchromloader-0.6.3/tests/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    13030 2023-06-22 19:52:40.000000 seqchromloader-0.6.3/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.6.2/PKG-INFO` & `seqchromloader-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.2
+Version: 0.6.3
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.2/README.md` & `seqchromloader-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.2/seqchromloader/loader.py` & `seqchromloader-0.6.3/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.2/seqchromloader/utils.py` & `seqchromloader-0.6.3/seqchromloader/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             filtered_chromosomes.append(filtered_record)
         # merge the retained chromosomes
         corods_out = pd.concat(filtered_chromosomes)
     else:
         corods_out = coords
     return corods_out
 
-def make_random_shift(coords, L, buffer=0):
+def make_random_shift(coords, L, buffer=0, rng=None):
     """
     This function takes as input a set of bed coordinates dataframe 
     It finds the mid-point for each record or Interval in the bed file,
     shifts the mid-point, and generates a windows of length L.
 
     If training window length is L, then we must ensure that the
     peak center is still within the training window.
@@ -92,23 +92,27 @@
     
     :param coords: input coordinate dataframe, first 3 columns are: [chrom, start, end]
     :type coords: pandas.DataFrame
     :param L: training/shifting window size, the shifted midpoint should fall into the range -L/2 + buffer ~ L/2 + buffer
     :type L: integer
     :param buffer: buffer size
     :type buffer: integer
+    :param rng: random number generator from numpy, optional
+    :type rng: np.random.Generator
     :rtype: shifted coordinate dataframe
-    
     """
     low = int(-L/2 + buffer)
     high = int(L/2 - buffer + 1)
 
+    if rng is None:
+        rng = np.random.default_rng()
+
     return (coords.assign(midpoint=lambda x: (x["start"]+x["end"])/2)
             .astype({"midpoint": int})
-            .assign(midpoint=lambda x: x["midpoint"] + np.random.randint(low=low, high=high, size=len(coords)))
+            .assign(midpoint=lambda x: x["midpoint"] + rng.integers(low=low, high=high, size=len(coords)))
             .apply(lambda s: pd.Series([s["chrom"], int(s["midpoint"]-L/2), int(s["midpoint"]+L/2)],
                                         index=["chrom", "start", "end"]), axis=1))
 
 def make_flank(coords, L, d):
     """
     Make flanking regions by:
     1. Shift midpoint by d
@@ -125,15 +129,16 @@
     return (coords.assign(midpoint=lambda x: (x["start"]+x["end"])/2)
                 .astype({"midpoint": int})
                 .assign(midpoint=lambda x: x["midpoint"] + d)
                 .apply(lambda s: pd.Series([s["chrom"], int(s["midpoint"]-L/2), int(s["midpoint"]+L/2)],
                                             index=["chrom", "start", "end"]), axis=1))
 
     
-def random_coords(gs:str=None, genome:str=None, incl:BedTool=None, excl:BedTool=None, l=500, n=1000):
+def random_coords(gs:str=None, genome:str=None, incl:BedTool=None, excl:BedTool=None,
+                  l=500, n=1000, seed=1):
     """
     Randomly sample n intervals of length l from the genome,
     shuffle to make all intervals inside the desired regions 
     and outside exclusion regions
     
     :param gs: genome size file path, only one of `gs` and `genome` is required
     :type gs: string
@@ -143,30 +148,32 @@
     :type incl: BedTool object
     :param incl: regions that chopped regions shouldn't overlap with
     :type excl: BedTool object
     :param l: random interval size
     :type l: integer
     :param n: number of random intervals generated
     :type n: integer
+    :param seed: random seed
+    :type seed: integer
     """
     random_kwargs = {}
     shuffle_kwargs = {}
     if genome:
         random_kwargs.update({"genome": genome}); shuffle_kwargs.update({"genome": genome})
     elif gs:
         random_kwargs.update({"g": gs}); shuffle_kwargs.update({"g": gs})
     else:
         raise Exception("Either gs or genome should be provided!")
     
     if incl: shuffle_kwargs.update({"incl": incl.fn})
     if excl: shuffle_kwargs.update({"excl": excl.fn})
     
     return (BedTool()
-            .random(l=l, n=n, **random_kwargs)
-            .shuffle(**shuffle_kwargs)
+            .random(l=l, n=n, seed=seed, **random_kwargs)
+            .shuffle(seed=seed, **shuffle_kwargs)
             .to_dataframe()[["chrom", "start", "end"]])
 
 def chop_genome(chroms:list=None, incl:BedTool=None, excl:BedTool=None, gs=None, genome=None, stride=500, l=500):
     """
     Given a genome size file and chromosome list,
     chop these chromosomes into intervals of length l,
     with include/exclude regions specified
```

### Comparing `seqchromloader-0.6.2/seqchromloader/writer.py` & `seqchromloader-0.6.3/seqchromloader/writer.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.2/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.6.3/seqchromloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.2
+Version: 0.6.3
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.2/setup.py` & `seqchromloader-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.6.2",
+    version="0.6.3",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

### Comparing `seqchromloader-0.6.2/tests/test_writer_loader.py` & `seqchromloader-0.6.3/tests/test_writer_loader.py`

 * *Files identical despite different names*

