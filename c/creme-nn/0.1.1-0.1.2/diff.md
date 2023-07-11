# Comparing `tmp/creme-nn-0.1.1.tar.gz` & `tmp/creme-nn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/creme-nn-0.1.1.tar", last modified: Mon Jul  3 19:29:52 2023, max compression
+gzip compressed data, was "dist/creme-nn-0.1.2.tar", last modified: Tue Jul 11 03:34:24 2023, max compression
```

## Comparing `creme-nn-0.1.1.tar` & `creme-nn-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 19:29:52.232789 creme-nn-0.1.1/
--rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-03 19:29:52.232500 creme-nn-0.1.1/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     1135 2023-07-03 02:58:16.000000 creme-nn-0.1.1/README.md
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 19:29:52.230173 creme-nn-0.1.1/creme/
--rwxr-xr-x   0 peter      (501) staff       (20)        0 2023-06-21 13:18:10.000000 creme-nn-0.1.1/creme/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)    18592 2023-07-03 18:04:20.000000 creme-nn-0.1.1/creme/creme.py
--rw-r--r--   0 peter      (501) staff       (20)     4406 2023-07-03 01:23:19.000000 creme-nn-0.1.1/creme/custom_model.py
--rwxr-xr-x   0 peter      (501) staff       (20)     4580 2023-06-26 02:40:44.000000 creme-nn-0.1.1/creme/shuffle.py
--rw-r--r--   0 peter      (501) staff       (20)     4340 2023-07-03 01:28:26.000000 creme-nn-0.1.1/creme/utils.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 19:29:52.232030 creme-nn-0.1.1/creme_nn.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      264 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)       89 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)        6 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2023-07-03 19:29:52.232904 creme-nn-0.1.1/setup.cfg
--rw-r--r--   0 peter      (501) staff       (20)     1385 2023-07-03 19:29:37.000000 creme-nn-0.1.1/setup.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-11 03:34:24.173588 creme-nn-0.1.2/
+-rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-11 03:34:24.173329 creme-nn-0.1.2/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     1326 2023-07-04 12:35:04.000000 creme-nn-0.1.2/README.md
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-11 03:34:24.171511 creme-nn-0.1.2/creme/
+-rwxr-xr-x   0 peter      (501) staff       (20)        0 2023-06-21 13:18:10.000000 creme-nn-0.1.2/creme/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)    18701 2023-07-11 03:25:04.000000 creme-nn-0.1.2/creme/creme.py
+-rw-r--r--   0 peter      (501) staff       (20)     4406 2023-07-03 01:23:19.000000 creme-nn-0.1.2/creme/custom_model.py
+-rwxr-xr-x   0 peter      (501) staff       (20)     4580 2023-06-26 02:40:44.000000 creme-nn-0.1.2/creme/shuffle.py
+-rw-r--r--   0 peter      (501) staff       (20)     4215 2023-07-11 03:24:21.000000 creme-nn-0.1.2/creme/utils.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-11 03:34:24.172971 creme-nn-0.1.2/creme_nn.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-11 03:34:24.000000 creme-nn-0.1.2/creme_nn.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      264 2023-07-11 03:34:24.000000 creme-nn-0.1.2/creme_nn.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2023-07-11 03:34:24.000000 creme-nn-0.1.2/creme_nn.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)       89 2023-07-11 03:34:24.000000 creme-nn-0.1.2/creme_nn.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)        6 2023-07-11 03:34:24.000000 creme-nn-0.1.2/creme_nn.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)       38 2023-07-11 03:34:24.173682 creme-nn-0.1.2/setup.cfg
+-rw-r--r--   0 peter      (501) staff       (20)     1385 2023-07-11 03:33:51.000000 creme-nn-0.1.2/setup.py
```

### Comparing `creme-nn-0.1.1/PKG-INFO` & `creme-nn-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creme-nn
-Version: 0.1.1
+Version: 0.1.2
 Summary: An in silico perturbation framework to interpret large-scale genomic deep learning
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `creme-nn-0.1.1/README.md` & `creme-nn-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,9 +6,16 @@
 
 [CREME](https://www.youtube.com/watch?v=PBwAxmrE194) (Cis-Regulatory Element Model Explanations) is an in silico perturbation framework designed to examine large-scale DNNs trained on regulatory genomics data. CREME can provide interpretations at various scales, including a coarse-grained CRE-level view as well as a fine-grained motif-level view. CREME can be used to identify cis-regulatory elements (CREs) that directly enhance or silence target genes. CREME can also be used to map CRE distance from transcription start sites and gene expression, as well as the intricate complexity of higher-order CRE interactions. 
 
 
 CREME is based on the notion that by fitting experimental data, the DNN essentially approximates the underlying "function" of the experimental assay. Thus, the trained DNN can be treated as a surrogate for the experimental assay, enabling in silico "measurements" for any  sequence. CREME comprises a suite of perturbation experiments to uncover how DNNs learn rules of interactions between CREs and their target genes
 
 
+Paper: https://www.biorxiv.org/content/10.1101/2023.07.03.547592v1 
 
+Tutorial and full documentation on Readthedocs.org comding soon...
+
+CREME is pip installable:
+```
+pip install creme-nn
+```
```

### Comparing `creme-nn-0.1.1/creme/creme.py` & `creme-nn-0.1.2/creme/creme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from . import shuffle 
+from . import shuffle
 
 ############################################################################################
 # TSS Context Dependence Test
 ############################################################################################
 
 def context_dependence_test(model, x, tile_pos, num_shuffle, mean=True):
     """
@@ -383,15 +383,15 @@
         max_index = optimization(pred_mut)
         pred_per_round.append(pred_mut[max_index])
 
         # add coordinates to fixed_tiles
         fixed_tiles.append(available_tiles[max_index])
 
         # update available positions 
-        utils.remove_tss_tile(available_tiles, max_index)
+        remove_tss_tile(available_tiles, max_index)
 
     return pred_wt[0], np.array(pred_per_round), fixed_tiles 
 
 
 
 ############################################################################################
 # CRE Multiplicity Test
@@ -483,15 +483,15 @@
 
         # find largest effect size
         max_index = optimization(pred_mut)
         max_positions.append(available_tiles[max_index])
         pred_per_round.append(pred_mut[max_index])
 
         # update available positions 
-        utils.remove_tss_tile(available_tiles, max_index)
+        remove_tss_tile(available_tiles, max_index)
 
     return pred_control, np.array(pred_per_round), max_positions 
 
 
 
 ########################################################################################
 # Normalization functions
@@ -520,11 +520,13 @@
 
 
 def reduce_pred_index(pred, bin_index=448):
     """Reduce multivariate prediction by selecting an index"""
     return pred[:, bin_index]
 
 
-
+def remove_tss_tile(tiles, tile_index):
+    """Remove a tile form a list of tile coordinates."""
+    del tiles[tile_index]
```

### Comparing `creme-nn-0.1.1/creme/custom_model.py` & `creme-nn-0.1.2/creme/custom_model.py`

 * *Files identical despite different names*

### Comparing `creme-nn-0.1.1/creme/shuffle.py` & `creme-nn-0.1.2/creme/shuffle.py`

 * *Files identical despite different names*

### Comparing `creme-nn-0.1.1/creme/utils.py` & `creme-nn-0.1.2/creme/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,19 +107,14 @@
     for i in np.arange(center_end, L, window):
         if i + window < L:
             other_tiles.append([i, i+window])
 
     return center_tile, other_tiles 
 
 
-def remove_tss_tile(tiles, tile_index):
-    """Remove a tile form a list of tile coordinates."""
-    del tiles[tile_index]
-
-
 def make_dir(dir_path):
     """ Make directory if doesn't exist."""
     if not os.path.isdir(dir_path):
         os.mkdir(dir_path)
     return dir_path
```

### Comparing `creme-nn-0.1.1/creme_nn.egg-info/PKG-INFO` & `creme-nn-0.1.2/creme_nn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creme-nn
-Version: 0.1.1
+Version: 0.1.2
 Summary: An in silico perturbation framework to interpret large-scale genomic deep learning
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `creme-nn-0.1.1/setup.py` & `creme-nn-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="creme-nn",
     # TODO: Consider using https://github.com/python-versioneer/python-versioneer to
     # get version information from git.
-    version="0.1.1",
+    version="0.1.2",
     description="An in silico perturbation framework to interpret large-scale genomic deep learning",
     # author='A. Random Developer',
     # author_email='author@example.com',
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

