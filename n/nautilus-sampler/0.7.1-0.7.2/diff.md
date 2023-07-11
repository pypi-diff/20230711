# Comparing `tmp/nautilus_sampler-0.7.1.tar.gz` & `tmp/nautilus_sampler-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus_sampler-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nautilus_sampler-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nautilus_sampler-0.7.1.tar` & `nautilus_sampler-0.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     8644 2023-07-07 10:14:17.431483 nautilus_sampler-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-04-08 20:18:18.001727 nautilus_sampler-0.7.1/LICENSE
--rw-r--r--   0        0        0     2938 2023-07-07 10:08:39.691790 nautilus_sampler-0.7.1/README.md
--rw-r--r--   0        0        0      218 2023-07-07 10:14:38.112204 nautilus_sampler-0.7.1/nautilus/__init__.py
--rw-r--r--   0        0        0      316 2023-04-14 03:07:30.928925 nautilus_sampler-0.7.1/nautilus/bounds/__init__.py
--rw-r--r--   0        0        0    22429 2023-06-07 11:06:55.121515 nautilus_sampler-0.7.1/nautilus/bounds/basic.py
--rw-r--r--   0        0        0    17901 2023-07-07 10:09:46.370971 nautilus_sampler-0.7.1/nautilus/bounds/neural.py
--rw-r--r--   0        0        0    13354 2023-06-22 17:16:37.897613 nautilus_sampler-0.7.1/nautilus/bounds/union.py
--rw-r--r--   0        0        0     5757 2023-07-07 10:09:46.370971 nautilus_sampler-0.7.1/nautilus/neural.py
--rw-r--r--   0        0        0     5967 2023-04-08 20:18:18.032727 nautilus_sampler-0.7.1/nautilus/prior.py
--rw-r--r--   0        0        0    49690 2023-06-22 17:16:37.899613 nautilus_sampler-0.7.1/nautilus/sampler.py
--rw-r--r--   0        0        0      676 2023-04-08 20:18:18.032727 nautilus_sampler-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3871 2023-06-04 02:02:40.543916 nautilus_sampler-0.7.1/tests/test_blobs.py
--rw-r--r--   0        0        0    14060 2023-06-22 17:16:37.953613 nautilus_sampler-0.7.1/tests/test_bounds.py
--rw-r--r--   0        0        0     5647 2023-06-22 17:16:37.954613 nautilus_sampler-0.7.1/tests/test_io.py
--rw-r--r--   0        0        0      486 2023-04-14 03:07:30.932925 nautilus_sampler-0.7.1/tests/test_neural.py
--rw-r--r--   0        0        0     1040 2023-06-04 02:02:40.544916 nautilus_sampler-0.7.1/tests/test_pool.py
--rw-r--r--   0        0        0     3714 2023-04-08 20:18:18.033727 nautilus_sampler-0.7.1/tests/test_prior.py
--rw-r--r--   0        0        0     7563 2023-06-22 17:16:37.954613 nautilus_sampler-0.7.1/tests/test_sampler.py
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 nautilus_sampler-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     8939 2023-07-11 16:32:28.271839 nautilus_sampler-0.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-04-08 20:18:18.001727 nautilus_sampler-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2938 2023-07-08 19:26:05.239116 nautilus_sampler-0.7.2/README.md
+-rw-r--r--   0        0        0      218 2023-07-11 16:32:35.207827 nautilus_sampler-0.7.2/nautilus/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-14 03:07:30.928925 nautilus_sampler-0.7.2/nautilus/bounds/__init__.py
+-rw-r--r--   0        0        0    22429 2023-06-07 11:06:55.121515 nautilus_sampler-0.7.2/nautilus/bounds/basic.py
+-rw-r--r--   0        0        0    17805 2023-07-09 14:37:27.324400 nautilus_sampler-0.7.2/nautilus/bounds/neural.py
+-rw-r--r--   0        0        0    13354 2023-06-22 17:16:37.897613 nautilus_sampler-0.7.2/nautilus/bounds/union.py
+-rw-r--r--   0        0        0     5757 2023-07-08 19:26:05.241116 nautilus_sampler-0.7.2/nautilus/neural.py
+-rw-r--r--   0        0        0     5967 2023-04-08 20:18:18.032727 nautilus_sampler-0.7.2/nautilus/prior.py
+-rw-r--r--   0        0        0    49708 2023-07-09 14:40:56.064078 nautilus_sampler-0.7.2/nautilus/sampler.py
+-rw-r--r--   0        0        0      676 2023-04-08 20:18:18.032727 nautilus_sampler-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3871 2023-06-04 02:02:40.543916 nautilus_sampler-0.7.2/tests/test_blobs.py
+-rw-r--r--   0        0        0    14060 2023-06-22 17:16:37.953613 nautilus_sampler-0.7.2/tests/test_bounds.py
+-rw-r--r--   0        0        0     5647 2023-06-22 17:16:37.954613 nautilus_sampler-0.7.2/tests/test_io.py
+-rw-r--r--   0        0        0      486 2023-04-14 03:07:30.932925 nautilus_sampler-0.7.2/tests/test_neural.py
+-rw-r--r--   0        0        0     1040 2023-06-04 02:02:40.544916 nautilus_sampler-0.7.2/tests/test_pool.py
+-rw-r--r--   0        0        0     3714 2023-04-08 20:18:18.033727 nautilus_sampler-0.7.2/tests/test_prior.py
+-rw-r--r--   0        0        0     7563 2023-06-22 17:16:37.954613 nautilus_sampler-0.7.2/tests/test_sampler.py
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 nautilus_sampler-0.7.2/PKG-INFO
```

### Comparing `nautilus_sampler-0.7.1/CHANGELOG.md` & `nautilus_sampler-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to nautilus will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [Unreleased]
+
+## [0.7.2] - 2023-07-11
+
+### Changed
+- The sampler should now deal better with likelihood plateaus.
+
+### Fixed
+- The prior function now always receives a copy of the points, preventing buggy behavior if the user's prior function does the prior transform on the original array.
+
 ## [0.7.1] - 2023-07-07
 
 ### Fixed
 - Parallelization with MPIPoolExecutor should now work correctly.
 
 ## [0.7.0] - 2023-06-20
```

### Comparing `nautilus_sampler-0.7.1/LICENSE` & `nautilus_sampler-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/README.md` & `nautilus_sampler-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/nautilus/bounds/basic.py` & `nautilus_sampler-0.7.2/nautilus/bounds/basic.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/nautilus/bounds/neural.py` & `nautilus_sampler-0.7.2/nautilus/bounds/neural.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module implementing multi-dimensional neural network-based bounds."""
 
 import numpy as np
 from functools import partial
-from scipy.stats import percentileofscore
+from scipy.stats import rankdata
 from threadpoolctl import threadpool_limits
 
 from .basic import Ellipsoid, UnitCubeEllipsoidMixture
 from .union import Union
 from ..neural import NeuralNetworkEmulator
 
 
@@ -78,21 +78,20 @@
 
         # Train the network.
         select = bound.outer_bound.contains(points)
         points = points[select]
         log_l = log_l[select]
 
         points_t = bound.outer_bound.transform(points)
-        perc = np.argsort(np.argsort(log_l)) / float(len(log_l))
-        perc_min = percentileofscore(log_l, log_l_min) / 100
         score = np.zeros(len(points))
-        select = perc < perc_min
-        if np.any(select):
-            score[select] = 0.5 * (perc[select] / perc_min)
-        score[~select] = 1 - 0.5 * (1 - perc[~select]) / (1 - perc_min)
+        select = log_l > log_l_min
+        score[select] = 0.5 * (
+            1 + (rankdata(log_l[select]) - 0.5) / np.sum(select))
+        score[~select] = 0.5 * (
+            (rankdata(log_l[~select]) - 0.5) / np.sum(~select))
         bound.emulator = NeuralNetworkEmulator.train(
             points_t, score, n_networks=n_networks,
             neural_network_kwargs=neural_network_kwargs, pool=pool)
 
         bound.score_predict_min = np.polyval(np.polyfit(
             score, bound.emulator.predict(points_t), 3), 0.5)
 
@@ -117,14 +116,15 @@
         points = np.atleast_2d(points)
 
         in_bound = self.outer_bound.contains(points)
         if np.any(in_bound) and self.emulator is not None:
             points_t = self.outer_bound.transform(points)
             in_bound[in_bound] = (self.emulator.predict(points_t[in_bound]) >
                                   self.score_predict_min)
+
         return in_bound
 
     def write(self, group):
         """Write the bound to an HDF5 group.
 
         Parameters
         ----------
```

### Comparing `nautilus_sampler-0.7.1/nautilus/bounds/union.py` & `nautilus_sampler-0.7.2/nautilus/bounds/union.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/nautilus/neural.py` & `nautilus_sampler-0.7.2/nautilus/neural.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/nautilus/prior.py` & `nautilus_sampler-0.7.2/nautilus/prior.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/nautilus/sampler.py` & `nautilus_sampler-0.7.2/nautilus/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,17 +711,17 @@
         else:
             if self.pass_dict:
                 transform = self.prior.unit_to_dictionary
             else:
                 transform = self.prior.unit_to_physical
 
         if not self.vectorized:
-            args = list(map(transform, points))
+            args = list(map(transform, np.copy(points)))
         else:
-            args = transform(points)
+            args = transform(np.copy(points))
 
         # Evaluate the likelihood.
         if self.vectorized:
             result = self.likelihood(args)
             if isinstance(result, tuple):
                 result = list(zip(*result))
         elif self.pool_l is not None:
```

### Comparing `nautilus_sampler-0.7.1/pyproject.toml` & `nautilus_sampler-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/tests/test_blobs.py` & `nautilus_sampler-0.7.2/tests/test_blobs.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/tests/test_bounds.py` & `nautilus_sampler-0.7.2/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/tests/test_io.py` & `nautilus_sampler-0.7.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/tests/test_pool.py` & `nautilus_sampler-0.7.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/tests/test_prior.py` & `nautilus_sampler-0.7.2/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/tests/test_sampler.py` & `nautilus_sampler-0.7.2/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `nautilus_sampler-0.7.1/PKG-INFO` & `nautilus_sampler-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus-sampler
-Version: 0.7.1
+Version: 0.7.2
 Summary: Neural Network-Boosted Importance Sampling for Bayesian Statistics
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
```

