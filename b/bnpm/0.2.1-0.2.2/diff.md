# Comparing `tmp/bnpm-0.2.1.tar.gz` & `tmp/bnpm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnpm-0.2.1.tar", last modified: Sun Jul  2 00:20:47 2023, max compression
+gzip compressed data, was "bnpm-0.2.2.tar", last modified: Tue Jul 11 19:39:44 2023, max compression
```

## Comparing `bnpm-0.2.1.tar` & `bnpm-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.644057 bnpm-0.2.1/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-02 00:20:47.644194 bnpm-0.2.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.642288 bnpm-0.2.1/bnpm/
--rwxrwxrwx   0 root         (0) root         (0)      907 2023-07-02 00:16:12.000000 bnpm-0.2.1/bnpm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.1/bnpm/ca2p_preprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.1/bnpm/classification.py
--rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.1/bnpm/clustering.py
--rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.1/bnpm/container_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.1/bnpm/cross_validation.py
--rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.1/bnpm/cupy_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.1/bnpm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.1/bnpm/dtw.py
--rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.1/bnpm/email_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.1/bnpm/featurization.py
--rwxrwxrwx   0 root         (0) root         (0)    23399 2023-06-29 05:55:34.000000 bnpm-0.2.1/bnpm/file_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    11769 2023-06-10 18:47:53.000000 bnpm-0.2.1/bnpm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.1/bnpm/image_processing.py
--rwxrwxrwx   0 root         (0) root         (0)    22721 2023-06-09 18:03:17.000000 bnpm-0.2.1/bnpm/indexing.py
--rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.1/bnpm/linear_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.1/bnpm/math_functions.py
--rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.1/bnpm/misc.py
--rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.1/bnpm/optimization.py
--rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.1/bnpm/other_peoples_code.py
--rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.1/bnpm/parallel_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.1/bnpm/path_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    38452 2023-06-17 22:18:41.000000 bnpm-0.2.1/bnpm/plotting_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.1/bnpm/resource_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)    34625 2023-06-19 08:21:29.000000 bnpm-0.2.1/bnpm/server.py
--rwxrwxrwx   0 root         (0) root         (0)    29980 2023-06-17 04:30:32.000000 bnpm-0.2.1/bnpm/similarity.py
--rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.1/bnpm/spectral.py
--rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.1/bnpm/stats.py
--rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.1/bnpm/timeSeries.py
--rwxrwxrwx   0 root         (0) root         (0)    13307 2023-06-17 04:43:28.000000 bnpm-0.2.1/bnpm/torch_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.1/bnpm/video.py
--rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.1/bnpm/welford_moving.py
--rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.1/bnpm/welford_moving_2D.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.643578 bnpm-0.2.1/bnpm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.643836 bnpm-0.2.1/demos/
--rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.2.1/demos/slurmDispatcher.py
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-02 00:20:47.644610 bnpm-0.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-10 00:46:32.000000 bnpm-0.2.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.435567 bnpm-0.2.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 19:39:44.435679 bnpm-0.2.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.433843 bnpm-0.2.2/bnpm/
+-rwxrwxrwx   0 root         (0) root         (0)      907 2023-07-11 19:38:00.000000 bnpm-0.2.2/bnpm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.2/bnpm/ca2p_preprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.2/bnpm/classification.py
+-rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.2/bnpm/clustering.py
+-rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.2/bnpm/container_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.2/bnpm/cross_validation.py
+-rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.2/bnpm/cupy_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.2/bnpm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.2/bnpm/dtw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.2/bnpm/email_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.2/bnpm/featurization.py
+-rwxrwxrwx   0 root         (0) root         (0)    23399 2023-06-29 05:55:34.000000 bnpm-0.2.2/bnpm/file_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    11769 2023-06-10 18:47:53.000000 bnpm-0.2.2/bnpm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.2/bnpm/image_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)    23809 2023-07-11 01:29:59.000000 bnpm-0.2.2/bnpm/indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.2/bnpm/linear_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.2/bnpm/math_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.2/bnpm/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.2/bnpm/optimization.py
+-rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.2/bnpm/other_peoples_code.py
+-rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.2/bnpm/parallel_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.2/bnpm/path_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    40543 2023-07-11 00:22:09.000000 bnpm-0.2.2/bnpm/plotting_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.2/bnpm/resource_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)    34760 2023-07-11 19:35:57.000000 bnpm-0.2.2/bnpm/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    31408 2023-07-11 01:31:23.000000 bnpm-0.2.2/bnpm/similarity.py
+-rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.2/bnpm/spectral.py
+-rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.2/bnpm/stats.py
+-rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.2/bnpm/timeSeries.py
+-rwxrwxrwx   0 root         (0) root         (0)    23576 2023-07-06 21:06:01.000000 bnpm-0.2.2/bnpm/torch_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.2/bnpm/video.py
+-rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.2/bnpm/welford_moving.py
+-rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.2/bnpm/welford_moving_2D.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.435101 bnpm-0.2.2/bnpm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      895 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.435350 bnpm-0.2.2/demos/
+-rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.2.2/demos/slurmDispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-11 19:39:44.436046 bnpm-0.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-10 00:46:32.000000 bnpm-0.2.2/setup.py
```

### Comparing `bnpm-0.2.1/LICENSE` & `bnpm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/PKG-INFO` & `bnpm-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
```

### Comparing `bnpm-0.2.1/README.md` & `bnpm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/__init__.py` & `bnpm-0.2.2/bnpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             'torch_helpers',
             'video',
         ]
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

### Comparing `bnpm-0.2.1/bnpm/ca2p_preprocessing.py` & `bnpm-0.2.2/bnpm/ca2p_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/classification.py` & `bnpm-0.2.2/bnpm/classification.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/clustering.py` & `bnpm-0.2.2/bnpm/clustering.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/container_helpers.py` & `bnpm-0.2.2/bnpm/container_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/cross_validation.py` & `bnpm-0.2.2/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/cupy_helpers.py` & `bnpm-0.2.2/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/decomposition.py` & `bnpm-0.2.2/bnpm/decomposition.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/dtw.py` & `bnpm-0.2.2/bnpm/dtw.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/email_helpers.py` & `bnpm-0.2.2/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/featurization.py` & `bnpm-0.2.2/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/file_helpers.py` & `bnpm-0.2.2/bnpm/file_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/h5_handling.py` & `bnpm-0.2.2/bnpm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/image_processing.py` & `bnpm-0.2.2/bnpm/image_processing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/indexing.py` & `bnpm-0.2.2/bnpm/indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -768,10 +768,44 @@
         weights = torch.as_tensor(weights).type(k[0][0].dtype).to(k[0][0].device) if weights is not None else torch.ones(len(k)).type(k[0][0].dtype).to(k[0][0].device)
 
     rank = len(k)
     n_modes = len(k[0])
     dense = zeros([k[0][m].shape[0] for m in range(n_modes)]).type(k[0][0].dtype).to(k[0][0].device)
     for r in range(rank):
         ## take the outer product of the n vectors in each mode and add to the dense tensor
-        dense += einsum(','.join([chr(97+m) for m in range(n_modes)]) + '->' + ''.join([chr(97+m) for m in range(n_modes)]), *k[r]) * weights[r]
+        str_einsum = ','.join([chr(97+m) for m in range(n_modes)]) + '->' + ''.join([chr(97+m) for m in range(n_modes)])
+        dense += einsum(str_einsum, *k[r]) * weights[r]
 
+    return dense
+
+def cp_to_dense(cp, weights=None):
+    """
+    Converts a list (of length n_modes) of 2D arrays (of shape (len_dim, rank))
+     [CP format] to a dense tensor (of shape (len_dim, len_dim, ...))
+    RH 2022
+
+    Args:
+        cp (list of np.ndarray):
+            List of 2D arrays in CP format.
+            Tensorly uses this format for their 'cp' format.
+
+    Returns:
+        dense (np.ndarray):
+            Dense tensor
+    """
+    rank = cp[0].shape[1]
+    n_modes = len(cp)
+    str_einsum = ','.join([chr(97+m)+'r' for m in range(n_modes)]) + '->' + ''.join([chr(97+m) for m in range(n_modes)])
+    if weights is None:
+        weights = np.ones(rank)
+
+    ## check if numpy or torch
+    if isinstance(cp[0], np.ndarray):
+        einsum = np.einsum
+        weights = np.array(weights).astype(cp[0].dtype)
+    elif isinstance(cp[0], torch.Tensor):
+        einsum = torch.einsum
+        weights = torch.as_tensor(weights).type(cp[0].dtype).to(cp[0].device)
+
+    dense = einsum(str_einsum, *[cp[m] * weights for m in range(n_modes)])
+    
     return dense
```

### Comparing `bnpm-0.2.1/bnpm/linear_regression.py` & `bnpm-0.2.2/bnpm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/math_functions.py` & `bnpm-0.2.2/bnpm/math_functions.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/misc.py` & `bnpm-0.2.2/bnpm/misc.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/optimization.py` & `bnpm-0.2.2/bnpm/optimization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/other_peoples_code.py` & `bnpm-0.2.2/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/parallel_helpers.py` & `bnpm-0.2.2/bnpm/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/path_helpers.py` & `bnpm-0.2.2/bnpm/path_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/plotting_helpers.py` & `bnpm-0.2.2/bnpm/plotting_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -453,15 +453,18 @@
         [0.6,0,1],
         [0.8,0,0.8],
         [1,0,0.6],
     ],
     under=[0,0,0],
     over=[0.5,0.5,0.5],
     bad=[0.9,0.9,0.9],
-    name='none'):
+    input_values=[0,1],
+    N=256,
+    name='none'
+):
     """Create a colormap from a sequence of rgb values.
     Stolen with love from Alex (https://gist.github.com/ahwillia/3e022cdd1fe82627cbf1f2e9e2ad80a7ex)
     
     Args:
         colors (list):
             List of RGB values
         name (str):
@@ -482,30 +485,61 @@
     n_colors = len(colors)
     if n_colors <= 1:
         raise ValueError('Must specify at least two colors')
 
     # convert colors to rgb
     colors = [colorConverter.to_rgb(c) for c in colors]
 
+    ## prep input_values
+    input_values = np.array(input_values)
+    ### assert monotonic
+    if not np.all(np.diff(input_values) > 0):
+        raise ValueError('input_values must be monotonically increasing')
+    fn_norm = lambda x: (x - input_values.min()) / np.ptp(input_values)
+    input_values_norm = fn_norm(input_values)
+    ### assert either n_inputs is 2 or n_colors
+    if len(input_values) == 2:
+        input_values_norm = np.linspace(0., 1., n_colors, endpoint=True)
+    elif len(input_values) != n_colors:
+        raise ValueError('length of input_values must be either 2 or equal to the length of colors')
+
     # set up colormap
-    r, g, b = colors[0]
-    cdict = {'red': [(0.0, r, r)], 'green': [(0.0, g, g)], 'blue': [(0.0, b, b)]}
-    for i, (r, g, b) in enumerate(colors[1:]):
-        idx = (i+1) / (n_colors-1)
+    cdict = {'red': [], 'green': [], 'blue': []}
+    for i, (r, g, b) in enumerate(colors):
+        idx = input_values_norm[i]
+        # print(idx)
         cdict['red'].append((idx, r, r))
         cdict['green'].append((idx, g, g))
         cdict['blue'].append((idx, b, b))
 
-    cmap = LinearSegmentedColormap(name, {k: tuple(v) for k, v in cdict.items()})
+    cmap = LinearSegmentedColormap(
+        name=name, 
+        segmentdata={k: tuple(v) for k, v in cdict.items()},
+        N=N,
+    )
                                    
     cmap.set_bad(bad)
     cmap.set_over(over)
     cmap.set_under(under)
 
-    return cmap
+    import matplotlib
+    class LSC_norm(matplotlib.colors.LinearSegmentedColormap):
+        def __init__(self, name=name, N=N):
+            super().__init__(name=name, segmentdata={k: tuple(v) for k, v in cdict.items()}, N=N)
+            self.set_bad(bad)
+            self.set_over(over)
+            self.set_under(under)
+
+        def __call__(self, X, alpha=None, bytes=False):
+            X_norm = fn_norm(X)
+            return super().__call__(X_norm, alpha=alpha, bytes=bytes)
+        
+    cmap_out = LSC_norm(name=name, N=N)
+
+    return cmap_out
 
 class Cmap_conjunctive:
     """
     Combines multiple colormaps into a single colormap by
      multiplying their values together.
     RH 2022
     """
@@ -1064,14 +1098,20 @@
             # return self.labels_
             return self.labels_.items()
         elif kind == 'dataframe':
             # return {'index': np.array([x[0] for x in self.labels_], dtype=np.int64), 'label': np.array([x[1] for x in self.labels_])}
             return {'index': np.array(list(self.labels_.keys()), dtype=np.int64), 'label': np.array(list(self.labels_.values()), dtype=str)}
 
 
+def rgb_to_hex(r, g, b):
+    if isinstance(r, float):
+        r, g, b = (int(v*255) for v in (r,g,b))
+    return '#{:02x}{:02x}{:02x}'.format(r, g, b)
+
+
 ########################################################################################################################
 ########################################## OTHER PLOTTING LIBRARIES ####################################################
 ########################################################################################################################
 
 def export_svg_hv_bokeh(obj, path_save):
     """
     Save a scatterplot from holoviews as an svg file.
@@ -1083,8 +1123,34 @@
         path_save (str):
             Path to save the svg file.
     """
     import holoviews as hv
     import bokeh
     plot_state = hv.renderer('bokeh').get_plot(obj).state
     plot_state.output_backend = 'svg'
-    bokeh.io.export_svgs(plot_state, filename=path_save)
+    bokeh.io.export_svgs(plot_state, filename=path_save)
+
+def plot_lines_bokeh(x=None, y=None, figsize=(500,500)):
+    import bokeh.plotting as bp
+    # y = y.cpu().numpy() if isinstance(y, torch.Tensor) else y
+    # x = x.cpu().numpy() if isinstance(x, torch.Tensor) else x
+    if y is None:
+        y = x
+        y = y[:,None] if y.ndim == 1 else y
+        x = np.arange(y.shape[0])
+        
+    cmap = simple_cmap(
+#         colors=[[0,0,1],[0,1,0],[1,0,0]],
+    )
+    p = bp.figure()
+    for i_line in range(y.shape[1]):
+        p.line(
+            x=x, 
+            y=y[:,i_line], 
+            color=rgb_to_hex(*cmap(i_line / (y.shape[1]-1))[:3]),
+            line_width=2,
+        )
+        
+    p.frame_height=figsize[0]
+    p.frame_width=figsize[1]
+    bp.show(p)
+    return p
```

### Comparing `bnpm-0.2.1/bnpm/resource_tracking.py` & `bnpm-0.2.2/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/server.py` & `bnpm-0.2.2/bnpm/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import copy
 import time
 import typing
 import sys
 
 from . import container_helpers
 
-def batch_run(paths_scripts, 
-                params_list, 
-                sbatch_config_list, 
-                max_n_jobs=2,
-                dir_save='/n/data1/hms/neurobio/sabatini/rich/analysis/', 
-                name_save='jobNum_', 
-                verbose=True,
-                ):
+def batch_run(
+    paths_scripts, 
+    params_list, 
+    sbatch_config_list, 
+    max_n_jobs=2,
+    dir_save='/n/data1/hms/neurobio/sabatini/rich/analysis/', 
+    name_save='jobNum_', 
+    verbose=True,
+):
     r"""
     Run a batch of jobs.
     Workflow 1: run a single script over a sweep of parameters
         - Make a script that takes in the set of parameters
            you wish to sweep over as variables.
         - Prepend the script to take in string arguments
            pointing to a param_config file (maybe a dict).
@@ -114,14 +115,17 @@
             - Name of each job (used as inner directory name)
             - If str, then will be used for all jobs 
             - Job iteration always appended to the end.
             - If List, then must have len(params_list) items.
         verbose (bool):
             - Whether or not to print progress
     """
+    import json
+    import os
+    import shutil
 
     # make sure the arguments are matched in length
     n_jobs = max(len(paths_scripts), len(params_list), len(sbatch_config_list))
     if max_n_jobs is not None:
         if n_jobs > max_n_jobs:
             raise ValueError(f'Too many jobs requested: max_n_jobs={max_n_jobs} > n_jobs={n_jobs}')
 
@@ -144,26 +148,27 @@
     for ii in range(n_jobs):
         dir_save_job = dir_save / f'{name_save[ii]}{ii}'
         dir_save_job.mkdir(parents=True, exist_ok=True)
         # save the shell scripts
         save_path_sbatchConfig = dir_save_job / 'sbatch_config.sh'
         with open(save_path_sbatchConfig, 'w') as f:
             f.write(sbatch_config_list[ii])
+        # save the script
+        path_script_job = dir_save_job / Path(paths_scripts[ii]).name
+        shutil.copyfile(paths_scripts[ii], path_script_job);
         # save the parameters        
-        save_path_params = dir_save_job / 'params.json'
-        with open(save_path_params, 'w') as f:
+        path_params_job = dir_save_job / 'params.json'
+        with open(path_params_job, 'w') as f:
             json.dump(params_list[ii], f)
     
         # run the job
         if verbose:
             print(f'Submitting job: {name_save[ii]} {ii}')
         # ! sbatch --job-name=${name_save}_${ii} --output=${dir_save_job}/log.txt --error=${dir_save_job}/err.txt --time=${sbatch_config_list[ii]["time"]} --mem=${sbatch_config_list[ii]["mem"]} --cpus-per-task=${sbatch_config_list[ii]["cpus"]} --wrap="${paths_scripts[ii]} ${params_list[ii]} ${sbatch_config_list[ii]} ${dir_save_job}"
-        # with open()
-        os.system(f'sbatch {save_path_sbatchConfig} {paths_scripts[ii]} {save_path_params} {dir_save_job}')
-
+        os.system(f'sbatch {save_path_sbatchConfig} {paths_scripts[ii]} {path_params_job} {dir_save_job}')
 
 
 ###############################
 ### MASTER CONTROLLER STUFF ###
 ###############################
 
 import paramiko
@@ -232,14 +237,15 @@
         self.client.connect(
             hostname=hostname,
             username=username,
             password=password,
             port=port, 
             key_filename=key_filename,
             look_for_keys=look_for_keys, 
+            allow_agent=look_for_keys,
         )
         self.ssh = self.client.invoke_shell()
 
     def send(self, cmd='ls', append_enter=True):
         """
         Send a command to the remote server.
         Args:
```

### Comparing `bnpm-0.2.1/bnpm/similarity.py` & `bnpm-0.2.2/bnpm/similarity.py`

 * *Files 4% similar despite different names*

```diff
@@ -631,14 +631,50 @@
         d = np.sqrt(1-(x+b))**a # fn 5: sqrt(1-x)
     if fn_toUse == 6:
         d = -np.log((x*a)+b) # fn 6: -log(x)
     
     return d + eps
     
 
+def cp_reconstruction_EV(tensor_dense, tensor_CP):
+    """
+    Explained variance of a reconstructed tensor using
+    by a CP tensor (similar to kruskal tensor).
+    RH 2023
+
+    Args:
+        tensor_dense (np.ndarray or torch.Tensor):
+            Dense tensor to be reconstructed. shape (n_samples, n_features)
+        tensor_CP (tensorly CPTensor or list of np.ndarray/torch.Tensor):
+            CP tensor.
+            If a list of factors, then each factor should be a 2D array of shape
+            (n_samples, rank).
+            Can also be a tensorly CPTensor object.
+    """
+    tensor_rec = None
+    try:
+        import tensorly as tl
+        if isinstance(tensor_CP, tl.cp_tensor.CPTensor):
+            tensor_rec = tl.cp_to_tensor(tensor_CP)
+    except ImportError as e:
+        raise ImportError('tensorly not installed. Please install tensorly or provide a list of factors as the tensor_CP argument.')
+    
+    if tensor_rec is None:
+        assert isinstance(tensor_CP, list), 'tensor_CP must be a list of factors'
+        assert all([isinstance(f, (np.ndarray, torch.Tensor)) for f in tensor_CP]), 'tensor_CP must be a list of factors'
+        tensor_rec = indexing.cp_to_dense(tensor_CP)
+
+    if isinstance(tensor_dense, torch.Tensor):
+        var = torch.var
+    elif isinstance(tensor_dense, np.ndarray):
+        var = np.var
+    ev = 1 - (var(tensor_dense - tensor_rec) / var(tensor_dense))
+    return ev
+    
+
 ##########################################    
 ########### Linear Assignment ############
 ##########################################
 
 def best_permutation(mat1 , mat2 , method='pearson'):
     '''
     This function compares the representations of two sets of vectors (columns
```

### Comparing `bnpm-0.2.1/bnpm/spectral.py` & `bnpm-0.2.2/bnpm/spectral.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/stats.py` & `bnpm-0.2.2/bnpm/stats.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/timeSeries.py` & `bnpm-0.2.2/bnpm/timeSeries.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/video.py` & `bnpm-0.2.2/bnpm/video.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/welford_moving.py` & `bnpm-0.2.2/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm/welford_moving_2D.py` & `bnpm-0.2.2/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/bnpm.egg-info/PKG-INFO` & `bnpm-0.2.2/bnpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
```

### Comparing `bnpm-0.2.1/bnpm.egg-info/SOURCES.txt` & `bnpm-0.2.2/bnpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/demos/slurmDispatcher.py` & `bnpm-0.2.2/demos/slurmDispatcher.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.1/setup.py` & `bnpm-0.2.2/setup.py`

 * *Files identical despite different names*

