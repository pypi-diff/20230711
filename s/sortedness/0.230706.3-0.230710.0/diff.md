# Comparing `tmp/sortedness-0.230706.3.tar.gz` & `tmp/sortedness-0.230710.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedness-0.230706.3.tar", max compression
+gzip compressed data, was "sortedness-0.230710.0.tar", max compression
```

## Comparing `sortedness-0.230706.3.tar` & `sortedness-0.230710.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230706.3/LICENSE
--rw-r--r--   0        0        0     5535 2023-07-07 01:07:58.511167 sortedness-0.230706.3/README.md
--rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230706.3/build.py
--rw-r--r--   0        0        0     1328 2023-07-07 01:07:59.639168 sortedness-0.230706.3/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-02 18:43:33.326749 sortedness-0.230706.3/src/sortedness/__init__.py
--rw-r--r--   0        0        0     7224 2023-07-07 00:44:07.161305 sortedness-0.230706.3/src/sortedness/agnostic.py
--rw-r--r--   0        0        0     1281 2023-05-02 18:58:14.909747 sortedness-0.230706.3/src/sortedness/config.py
--rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230706.3/src/sortedness/evaluation/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-02 18:58:14.873747 sortedness-0.230706.3/src/sortedness/evaluation/plot.py
--rw-r--r--   0        0        0     5145 2023-05-02 18:58:14.889747 sortedness-0.230706.3/src/sortedness/global_.py
--rw-r--r--   0        0        0     3043 2023-07-07 00:44:07.169305 sortedness-0.230706.3/src/sortedness/gtau.py
--rw-r--r--   0        0        0    24912 2023-07-07 01:06:49.299076 sortedness-0.230706.3/src/sortedness/local.py
--rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230706.3/src/sortedness/matrices.py
--rw-r--r--   0        0        0     2983 2023-07-07 00:49:33.533727 sortedness-0.230706.3/src/sortedness/parallel.py
--rw-r--r--   0        0        0     8399 2023-07-07 00:56:13.866263 sortedness-0.230706.3/src/sortedness/rank.py
--rw-r--r--   0        0        0     4707 2023-05-02 18:58:14.909747 sortedness-0.230706.3/src/sortedness/trustworthiness.py
--rw-r--r--   0        0        0     3518 2023-07-07 00:28:29.856946 sortedness-0.230706.3/src/sortedness/wtau/__init__.py
--rw-r--r--   0        0        0  1267818 2023-07-07 00:57:29.546358 sortedness-0.230706.3/src/sortedness/wtau/wtau.c
--rwxr-xr-x   0        0        0  1348408 2023-05-30 20:09:00.000000 sortedness-0.230706.3/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0        0        0   334715 2023-07-07 00:57:29.570359 sortedness-0.230706.3/src/sortedness/wtau/wtau.html
--rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230706.3/src/sortedness/wtau/wtau.pyx
--rw-r--r--   0        0        0     6708 1970-01-01 00:00:00.000000 sortedness-0.230706.3/setup.py
--rw-r--r--   0        0        0     6140 1970-01-01 00:00:00.000000 sortedness-0.230706.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230710.0/LICENSE
+-rw-r--r--   0        0        0     5535 2023-07-11 02:49:51.038638 sortedness-0.230710.0/README.md
+-rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230710.0/build.py
+-rw-r--r--   0        0        0     1328 2023-07-11 02:50:49.082635 sortedness-0.230710.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-02 18:43:33.326749 sortedness-0.230710.0/src/sortedness/__init__.py
+-rw-r--r--   0        0        0     7224 2023-07-07 00:44:07.161305 sortedness-0.230710.0/src/sortedness/agnostic.py
+-rw-r--r--   0        0        0     1281 2023-05-02 18:58:14.909747 sortedness-0.230710.0/src/sortedness/config.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230710.0/src/sortedness/evaluation/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-02 18:58:14.873747 sortedness-0.230710.0/src/sortedness/evaluation/plot.py
+-rw-r--r--   0        0        0     5145 2023-05-02 18:58:14.889747 sortedness-0.230710.0/src/sortedness/global_.py
+-rw-r--r--   0        0        0     3043 2023-07-07 00:44:07.169305 sortedness-0.230710.0/src/sortedness/gtau.py
+-rw-r--r--   0        0        0    26230 2023-07-11 02:49:29.806640 sortedness-0.230710.0/src/sortedness/local.py
+-rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230710.0/src/sortedness/matrices.py
+-rw-r--r--   0        0        0     2983 2023-07-07 00:49:33.533727 sortedness-0.230710.0/src/sortedness/parallel.py
+-rw-r--r--   0        0        0     8399 2023-07-07 00:56:13.866263 sortedness-0.230710.0/src/sortedness/rank.py
+-rw-r--r--   0        0        0     4707 2023-05-02 18:58:14.909747 sortedness-0.230710.0/src/sortedness/trustworthiness.py
+-rw-r--r--   0        0        0     3518 2023-07-07 00:28:29.856946 sortedness-0.230710.0/src/sortedness/wtau/__init__.py
+-rw-r--r--   0        0        0  1267818 2023-07-07 01:08:20.579195 sortedness-0.230710.0/src/sortedness/wtau/wtau.c
+-rwxr-xr-x   0        0        0  1348408 2023-05-30 20:09:00.000000 sortedness-0.230710.0/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0   334715 2023-07-07 01:08:20.643195 sortedness-0.230710.0/src/sortedness/wtau/wtau.html
+-rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230710.0/src/sortedness/wtau/wtau.pyx
+-rw-r--r--   0        0        0     6708 1970-01-01 00:00:00.000000 sortedness-0.230710.0/setup.py
+-rw-r--r--   0        0        0     6140 1970-01-01 00:00:00.000000 sortedness-0.230710.0/PKG-INFO
```

### Comparing `sortedness-0.230706.3/LICENSE` & `sortedness-0.230710.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/README.md` & `sortedness-0.230710.0/README.md`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/build.py` & `sortedness-0.230710.0/build.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/pyproject.toml` & `sortedness-0.230710.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortedness"
-version = "0.230706.3"
+version = "0.230710.0"
 description = "Measures of projection quality"
 authors = ["davips <dpsabc@gmail.com>", "tacito <tacito.neves@gmail.com>"]
 license = "GPLv3"
 build = "build.py"  # For Cython. apt-get package needed: python3-numpy
 readme = 'README.md'
 packages = [
     { include = "sortedness", from = "src" }
```

### Comparing `sortedness-0.230706.3/src/sortedness/agnostic.py` & `sortedness-0.230710.0/src/sortedness/agnostic.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/config.py` & `sortedness-0.230710.0/src/sortedness/config.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/evaluation/plot.py` & `sortedness-0.230710.0/src/sortedness/evaluation/plot.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/global_.py` & `sortedness-0.230710.0/src/sortedness/global_.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/gtau.py` & `sortedness-0.230710.0/src/sortedness/gtau.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/local.py` & `sortedness-0.230710.0/src/sortedness/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     result = np.array(result, dtype=float)
     if return_pvalues:
         return np.array(list(zip(result, pvalues)))
     return result
 
 
-def pwsortedness(X, X_, parallel=True, parallel_n_trigger=200, batches=10, debug=False, dist=None, **parallel_kwargs):
+def pwsortedness(X, X_, i=None, parallel=True, parallel_n_trigger=200, batches=10, debug=False, dist=None, cython=False, **parallel_kwargs):
     """
     Local pairwise sortedness (Λ𝜏w) based on Sebastiano Vigna weighted Kendall's 𝜏
 
     Importance rankings are calculated internally based on proximity of each pair to the point of interest.
 
     # TODO?: add flag to break extremely rare cases of ties that persist after projection (implies a much slower algorithm)
         This probably doesn't make any difference on the result, except on categorical, pathological or toy datasets
@@ -286,29 +286,37 @@
 
     Parameters
     ----------
     X
         Original dataset
     X_
         Projected points
+    i
+        None:   calculate pwsortedness for all instances
+        `int`:  index of the instance of interest
     parallel
         None: Avoid high-memory parallelization
         True: Full parallelism
         False: No parallelism
     parallel_kwargs
         Any extra argument to be provided to pathos parallelization
     parallel_n_trigger
         Threshold to disable parallelization for small n values
     batches
         Parallel batch size
     debug
         Whether to print more info
     dist
         Provide distance matrices (D, D_) instead of points
-        X and X_ are ignored
+        X and X_ should be None
+    cython
+        Whether to:
+            (True) improve speed by ~2x; or,
+            (False) be more compatible/portable.
+
 
     Returns
     -------
         Numpy vector
 
     >>> import numpy as np
     >>> from functools import partial
@@ -334,69 +342,95 @@
     (0.730078995423, 0.774457348878, 0.837310352695)
     >>> r = pwsortedness(original, projected2[:, 1:])
     >>> min(r), round(mean(r), 12), max(r)
     (0.18672441995, 0.281712132364, 0.420214364305)
     >>> r = pwsortedness(original, projectedrnd)
     >>> min(r), round(mean(r), 12), max(r)
     (-0.198780473657, -0.064598420372, 0.147224384381)
+    >>> pwsortedness(original, projected1)[1]
+    0.730078995423
+    >>> pwsortedness(original, projected1, cython=True)[1]
+    0.730078995423
+    >>> pwsortedness(original, projected1, i=1)
+    0.730078995423
     """
     npoints = len(X) if X is not None else len(dist[0])  # pragma: no cover
     tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
+    pmap = mp.ProcessingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
     if debug:  # pragma: no cover
         print(1)
     thread = lambda M: -pdist(M, metric="sqeuclidean")
+
+    # if i is not None:
+    #     tmp, tmp_ = X[0], X_[0]
+    #     X[0], X_[0] = X[i], X_[i]
+    #     X[i], X_[i] = tmp, tmp_
+
     scores_X, scores_X_ = tmap(thread, [X, X_]) if X is not None else (-squareform(dist[0]), -squareform(dist[1]))
     if debug:  # pragma: no cover
         print(2)
-    D, D_ = tmap(squareform, [-scores_X, -scores_X_]) if dist is None else (dist[0], dist[1])
-    if debug:  # pragma: no cover
-        print(3)
-    n = len(D)
 
-    def makeM(E):
+    def makeM(E, single=False):
         n = len(E)
         m = (n ** 2 - n) // 2
-        M = np.zeros((m, n))
+        M = np.zeros((m, 1 if single else n))
         if debug:  # pragma: no cover
             print(4)
         c = 0
         for i in range(n - 1):  # a bit slow, but only a fraction of wtau (~5%)
             h = n - i - 1
             d = c + h
             M[c:d] = E[i] + E[i + 1:]
             c = d
         if debug:  # pragma: no cover
             print(5)
         del E
         gc.collect()
         return M.T
 
-    M = makeM(D)
-    if debug:  # pragma: no cover
-        print(6)
-    R = rank_alongrow(M, step=n // batches, parallel=parallel, **parallel_kwargs).T
-    del M
-    gc.collect()
-    if debug:  # pragma: no cover
-        print(7)
-    from sortedness.wtau import parwtau
-    res = np.round(parwtau(scores_X, scores_X_, npoints, R, parallel=parallel, **parallel_kwargs), 12)
-    del R
-    gc.collect()
-
-    # M_ = makeM(D_)
-    # if debug: print(6)
-    # R_ = rank_alongrow(M_, step=n // batches, parallel=parallel, **parallel_kwargs).T
-    # del M_
-    # gc.collect()
-    # if debug: print(7)
-    # r_ = np.round(parwtau(scores_X, scores_X_, npoints, parallel=parallel, **parallel_kwargs), 12)
-    # del R_
-    # gc.collect()
-    return res
+    D = squareform(-scores_X) if dist is None else dist[0]
+    if i is None:
+        if debug:  # pragma: no cover
+            print(3)
+        n = len(D)
+        M = makeM(D)
+        if debug:  # pragma: no cover
+            print(6)
+        R = rank_alongrow(M, step=n // batches, parallel=parallel, **parallel_kwargs).T
+        del M
+        gc.collect()
+        if debug:  # pragma: no cover
+            print(7)
+        if cython:
+            from sortedness.wtau import parwtau
+            res = np.round(parwtau(scores_X, scores_X_, npoints, R, parallel=parallel, **parallel_kwargs), 12)
+            del R
+            gc.collect()
+            return res
+        else:
+            def thread(r):
+                corr, pvalue = weightedtau(scores_X, scores_X_, rank=r)
+                return round(corr, 12), round(pvalue, 12)
+
+            result, pvalues = [], []
+            lst = (R[:, i] for i in range(len(X)))
+            for corrs, pvalue in pmap(thread, lst):
+                result.append(corrs)
+                pvalues.append(pvalue)
+            result = np.array(result, dtype=float)
+            return result
+
+    M = makeM(D[:, i:i + 1], single=True)
+    r = rankdata(M, axis=1, method="average")[0].astype(int) - 1
+    return round(weightedtau(scores_X, scores_X_, r)[0], 12)
+
+    # D = cdist(X, X[:1])
+    # M = makeM(D, single=True)
+    # r = rankdata(M[0], method="average").astype(int) - 1
+    # return round(weightedtau(scores_X, scores_X_, r)[0], 12)
 
 
 def rsortedness(X, X_, f=weightedtau, return_pvalues=False, parallel=True, parallel_n_trigger=500, parallel_kwargs=None, **kwargs):  # pragma: no cover
     """
     Reciprocal sortedness: consider the neighborhood relation the other way around
 
     Might be good to assess the effect of a projection on hubness, and also to serve as a loss function for a custom projection algorithm.
```

### Comparing `sortedness-0.230706.3/src/sortedness/matrices.py` & `sortedness-0.230710.0/src/sortedness/matrices.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/parallel.py` & `sortedness-0.230710.0/src/sortedness/parallel.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/rank.py` & `sortedness-0.230710.0/src/sortedness/rank.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/trustworthiness.py` & `sortedness-0.230710.0/src/sortedness/trustworthiness.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/wtau/__init__.py` & `sortedness-0.230710.0/src/sortedness/wtau/__init__.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/wtau/wtau.c` & `sortedness-0.230710.0/src/sortedness/wtau/wtau.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3",
             "-ffast-math",
             "-march=native",
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
-            "/tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sortedness.wtau.wtau",
         "sources": [
             "src/sortedness/wtau/wtau.pyx"
@@ -1136,177 +1136,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1337,42 +1337,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -10659,15 +10659,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_perm, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10676,29 +10676,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10709,15 +10709,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10726,29 +10726,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10759,15 +10759,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10776,29 +10776,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10809,15 +10809,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10826,29 +10826,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10859,15 +10859,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10876,29 +10876,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10909,89 +10909,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -10999,33 +10999,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -11033,96 +11033,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11138,15 +11138,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11154,53 +11154,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
@@ -11208,30 +11208,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11246,15 +11246,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11270,15 +11270,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11286,53 +11286,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
@@ -11340,30 +11340,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11378,15 +11378,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11402,15 +11402,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11418,53 +11418,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
@@ -11472,30 +11472,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11510,176 +11510,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":975
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":990
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1000
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25665,26 +25665,26 @@
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/tmppyy735sl/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 947, __pyx_L1_error)
```

### Comparing `sortedness-0.230706.3/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so` & `sortedness-0.230710.0/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/wtau/wtau.html` & `sortedness-0.230710.0/src/sortedness/wtau/wtau.html`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/src/sortedness/wtau/wtau.pyx` & `sortedness-0.230710.0/src/sortedness/wtau/wtau.pyx`

 * *Files identical despite different names*

### Comparing `sortedness-0.230706.3/setup.py` & `sortedness-0.230710.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['lange>=1.230203.1,<2.0.0', 'pathos>=0.3.0,<0.4.0']
 
 extras_require = \
 {':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'sortedness',
-    'version': '0.230706.3',
+    'version': '0.230710.0',
     'description': 'Measures of projection quality',
     'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n\n# sortedness\n\n`sortedness` is a measure of quality of data transformation, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n## Overview\nLocal variants return a value for each provided point. The global variant returns a single value for all points.\nAny local variant can be used as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant: `global_sortedness(X, X_)`.\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import sortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = sortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.432937128932 0.7813889452999166 0.944810120534\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.578096068617 -0.06328160775358334 0.396112816715\n"""\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = pwsortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.730078995423 0.7744573488776667 0.837310352695\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.198780473657 -0.0645984203715 0.147224384381\n"""\n```\n\n\n</p>\n</details>\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import global_pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print measurement result and p-value.\ns = global_pwsortedness(original, original)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected2)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected1)\nprint(list(s))\n"""\n[0.7715617715617715, 5.240847664048334e-20]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projectedrnd)\nprint(list(s))\n"""\n[-0.06107226107226107, 0.46847188611226276]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**\n\n\n\n\n\n## Grants\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['sortedness', 'sortedness.evaluation', 'sortedness.wtau']
 package_data = \ {'': ['*']} install_requires = \ ['lange>=1.230203.1,<2.0.0',
 'pathos>=0.3.0,<0.4.0'] extras_require = \ {':python_version >= "3.8" and
 python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']} setup_kwargs = { 'name':
-'sortedness', 'version': '0.230706.3', 'description': 'Measures of projection
+'sortedness', 'version': '0.230710.0', 'description': 'Measures of projection
 quality', 'long_description': '![test](https://github.com/sortedness/
 sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/
 sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/
 sortedness/sortedness)\n\n[github]\n\n![Python version](https://img.shields.io/
 badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/
 License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![API
 documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)]
```

### Comparing `sortedness-0.230706.3/PKG-INFO` & `sortedness-0.230710.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortedness
-Version: 0.230706.3
+Version: 0.230710.0
 Summary: Measures of projection quality
 License: GPLv3
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sortedness Version: 0.230706.3 Summary: Measures of
+Metadata-Version: 2.1 Name: sortedness Version: 0.230710.0 Summary: Measures of
 projection quality License: GPLv3 Author: davips Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lange (>=1.230203.1,<2.0.0) Requires-Dist: pathos
 (>=0.3.0,<0.4.0) Requires-Dist: scipy (>=1.10.1,<2.0.0) ; python_version >=
 "3.8" and python_version < "3.11" Description-Content-Type: text/markdown !
```

