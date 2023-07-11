# Comparing `tmp/neuroshape-0.0.4.6.5.tar.gz` & `tmp/neuroshape-0.0.4.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.6.5.tar", last modified: Mon Jun 26 01:55:49 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.6.6.tar", last modified: Tue Jul 11 01:49:03 2023, max compression
```

## Comparing `neuroshape-0.0.4.6.5.tar` & `neuroshape-0.0.4.6.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:49.129194 neuroshape-0.0.4.6.5/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.6.5/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-26 01:55:49.128908 neuroshape-0.0.4.6.5/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.5/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.821233 neuroshape-0.0.4.6.5/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.6.5/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)    22913 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.5/neuroshape/eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.884516 neuroshape-0.0.4.6.5/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    15330 2023-06-21 07:38:08.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.907978 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5042 2023-06-19 01:29:34.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4137 2023-06-17 23:29:12.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.5/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:49.068850 neuroshape-0.0.4.6.5/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    11784 2023-06-21 03:32:59.000000 neuroshape-0.0.4.6.5/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.5/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    31133 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.5/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.5/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/zscore_avg_method.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.837562 neuroshape-0.0.4.6.5/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1383 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      670 2023-06-26 01:55:37.000000 neuroshape-0.0.4.6.5/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-26 01:55:49.129277 neuroshape-0.0.4.6.5/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-26 01:55:25.000000 neuroshape-0.0.4.6.5/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:49.109092 neuroshape-0.0.4.6.5/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.6.5/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.6.5/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.5/src/glmfit.c
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.211407 neuroshape-0.0.4.6.6/
+-rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.6.6/LICENSE
+-rw-r--r--   0 c3336955   (503) staff       (20)     6795 2023-07-11 01:49:03.210956 neuroshape-0.0.4.6.6/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.6/README.rst
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.183672 neuroshape-0.0.4.6.6/neuroshape/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    22407 2023-06-16 11:25:08.000000 neuroshape-0.0.4.6.6/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    22913 2023-07-04 03:05:38.000000 neuroshape-0.0.4.6.6/neuroshape/eigenmodes.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.196157 neuroshape-0.0.4.6.6/neuroshape/nulls/
+-rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    15998 2023-06-28 22:07:04.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/spins.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.199159 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5042 2023-06-19 22:07:48.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4137 2023-06-19 22:07:48.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/permutation.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.6/neuroshape/recon.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/stats.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.208435 neuroshape-0.0.4.6.6/neuroshape/utils/
+-rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.6.6/neuroshape/utils/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/check_map.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/checks.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/concavehull.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    11779 2023-06-28 11:45:24.000000 neuroshape-0.0.4.6.6/neuroshape/utils/eigen.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.6/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    32940 2023-06-28 10:54:36.000000 neuroshape-0.0.4.6.6/neuroshape/utils/geometry.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     2580 2023-07-01 22:04:11.000000 neuroshape-0.0.4.6.6/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.6/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-11 10:05:42.000000 neuroshape-0.0.4.6.6/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/tmpname.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/zscore_avg_method.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.190939 neuroshape-0.0.4.6.6/neuroshape.egg-info/
+-rw-r--r--   0 c3336955   (503) staff       (20)     6795 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     1383 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)      670 2023-07-11 01:48:59.000000 neuroshape-0.0.4.6.6/pyproject.toml
+-rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-07-11 01:49:03.211550 neuroshape-0.0.4.6.6/setup.cfg
+-rw-r--r--   0 c3336955   (503) staff       (20)     1048 2023-07-11 01:48:48.000000 neuroshape-0.0.4.6.6/setup.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.210321 neuroshape-0.0.4.6.6/src/
+-rw-r--r--   0 c3336955   (503) staff       (20)     5389 2023-06-16 11:25:08.000000 neuroshape-0.0.4.6.6/src/eta_squared.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.6.6/src/euler_threshold.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.6/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.6.5/LICENSE` & `neuroshape-0.0.4.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/README.rst` & `neuroshape-0.0.4.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.6.6/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.6.6/neuroshape/eigenmodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,15 +562,15 @@
         raise ImportWarning("Could not find cholmod library. using (slower) LU decomposition")
         cholmod = False
         
     fem = Solver(surface, use_cholmod=cholmod)
     evals, emodes = fem.eigs(k=num_modes)
     
     # standardize modes
-    emodes = (emodes - np.mean(emodes, axis=0))/np.std(emodes, axis=0)
+    emodes = (emodes - np.mean(emodes, axis=1))/np.std(emodes, axis=1)
     
     # remove the medial wall
     medial_wall = find_medial_wall(sdir, sid).reshape(-1,)
     emodes[medial_wall] = np.nan
     
     if not outevec:
         outevec = surf_file.replace(ext, '') + '_outevecs_' + str(num_modes) + '.txt'
```

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/eigensphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     eigen_decomposition,
     transform_to_spheroid,
     transform_to_ellipsoid,
     resample_spheroid,
     reconstruct_data,
     )
 
+import copy
+
 import numpy as np
 import nibabel as nib
 import matplotlib.pyplot as plt
 from nilearn import plotting
 from brainsmash.utils.dataio import is_string_like, dataio
 
 cmap = plt.get_cmap('viridis')
@@ -48,15 +50,16 @@
         
         A[:, j] = A[:, j] / np.linalg.norm(A[:, j])
         
     return A
 
 def eigenmode_resample(surface, data, evals, emodes, 
                        angles=None, decomp_method='matrix', 
-                       medial=None, resample=True):
+                       medial=None, randomize=False,
+                       resample=True):
     """
     Resample the hypersphere bounded by the eigengroups contained within `emodes`,
     and reconstruct the data using coefficients conditioned on the original data
     Based on the degenerate solutions of solving the Laplace-Beltrami operator 
     on the cortex. The power spectrum is perfectly retained (the square of the 
     eigenvalues).
     
@@ -199,61 +202,14 @@
     #     else:
     #         raise ValueError("Normalization type must be 'constant', 'number', 'volume', 'area'")
     if decomp_method is not None:
         if decomp_method in methods:
             method = decomp_method
         else:
             raise ValueError("Eigenmode decomposition method must be 'matrix' or 'regression'")
-            
-    # find eigengroups
-    groups = _get_eigengroups(emodes)
-    
-    # if not given angles
-    if angles is None:
-        angles = np.random.randn(len(groups) + 1) * np.pi
-    
-    # initialize the new modes
-    new_modes = np.zeros_like(emodes)
-    
-    m = 0 #index of angles
-    # resample the hypersphere (except for groups 1 and 2)
-    for idx in range(1, len(groups)):
-        group_modes = emodes[:, groups[idx]]
-        group_evals = evals[groups[idx]]
-        
-        if len(groups[idx]) == 3:
-            # do simple rotation
-            # initialize the points
-            p = group_modes / np.linalg.norm(group_modes)
-            p *= np.sin(angles[m])
-            
-            # ensure orthonormal
-            group_new_modes = gram_schmidt(p)
-             # get the index for the angles
-            new_modes[:, groups[idx]] = group_new_modes
-        
-        m += 1
-        # else, transform to spheroid and index the angles properly
-        group_new_modes = transform_to_spheroid(group_evals, group_modes)
-        group_spherical_modes = resample_spheroid(group_new_modes, angles[m])
-        
-        # ensure orthonormal
-        group_spherical_modes = gram_schmidt(group_spherical_modes)
-        
-        # transform back to ellipsoid
-        group_ellipsoid_modes = transform_to_ellipsoid(group_evals, group_spherical_modes)
-        
-        new_modes[:, groups[idx]] = group_ellipsoid_modes / np.linalg.norm(group_ellipsoid_modes)
-        
-    # find the coefficents of the modes to the data by solving the OLS
-    # decomposition, either through the normal equation solution or regression    
-    coeffs = eigen_decomposition(data, emodes, method=method)
-    
-    # matrix multiply the estimated coefficients by the new modes
-    surrogate_data = reconstruct_data(coeffs, new_modes)
     
     # mask out medial wall
     if medial is None:
         # get index of medial wall hopefully
         medial_wall = np.abs(data) == 0.0
         
     elif medial is False:
@@ -288,31 +244,92 @@
                 medial_wall = medial
         else:
             raise ValueError("Could not use provided medial wall array or "
                              "file, please check")
     
     medial_wall = medial_wall.astype(bool)
     
+    medial_mask = np.logical_not(medial_wall)
+    data_copy = copy.deepcopy(data) # deepcopy original data so it's not modified
+    data_copy = data_copy[medial_mask]
+    emodes_copy = copy.deepcopy(emodes)
+    emodes_copy = emodes_copy[medial_mask]
+    
+    # find eigengroups
+    groups = _get_eigengroups(emodes_copy)
+    
+    # if not given angles
+    if angles is None:
+        angles = np.random.randn(len(groups) + 1) * np.pi
+    
+    # initialize the new modes
+    new_modes = np.zeros_like(emodes_copy)
+    
+    m = 0 #index of angles
+    # resample the hypersphere (except for groups 1 and 2)
+    for idx in range(1, len(groups)):
+        group_modes = emodes_copy[:, groups[idx]]
+        group_evals = evals[groups[idx]]
+        
+        if len(groups[idx]) == 3:
+            # do simple rotation
+            # initialize the points
+            p = group_modes / np.sqrt(group_evals)
+            p *= np.cos(angles[m])
+            
+            # ensure orthonormal
+            group_new_modes = gram_schmidt(p)
+             # get the index for the angles
+            new_modes[:, groups[idx]] = group_new_modes
+        
+        m += 1
+        # else, transform to spheroid and index the angles properly
+        group_new_modes = transform_to_spheroid(group_evals, group_modes)
+        group_spherical_modes = resample_spheroid(group_new_modes, angles[m])
+        
+        # ensure orthonormal
+        group_spherical_modes = gram_schmidt(group_spherical_modes)
+        
+        # transform back to ellipsoid
+        group_ellipsoid_modes = transform_to_ellipsoid(group_evals, group_spherical_modes)
+        
+        new_modes[:, groups[idx]] = gram_schmidt(group_ellipsoid_modes) #/ np.linalg.norm(group_ellipsoid_modes)
+     
+    #new_modes = gram_schmidt(new_modes) #/ np.linalg.norm(new_modes)
+    # find the coefficents of the modes to the data by solving the OLS
+    # decomposition, either through the normal equation solution or regression    
+    coeffs = eigen_decomposition(data_copy, emodes_copy, method=method)
+    
+    # matrix multiply the estimated coefficients by the new modes
+    surrogate_data = np.zeros_like(data)
+    
+    if randomize is True:
+        for i in range(len(groups)):
+            coeffs[groups[i]] = np.random.permutation(coeffs[groups[i]])
+    
+    surrogate_data[medial_mask] = reconstruct_data(coeffs, new_modes)
+    
     # mask out medial wall from surrogate
-    surrogate_data[medial_wall] = 0.0
+    #surrogate_data[medial_wall] = 0.0
     
     if resample is True:
         mask = np.logical_not(medial_wall)
 
         # Mask the data and surrogate_data excluding the medial wall
         data_no_mwall = data[mask]
-        surr_no_mwall = surrogate_data[mask]
+        surr_no_mwall = copy.deepcopy(surrogate_data)
+        surr_no_mwall = surr_no_mwall[mask]
         
         # Get the rank ordered indices
-        data_ranks = np.argsort(data_no_mwall)
-        surr_ranks = np.argsort(surr_no_mwall)
+        data_ranks = data_no_mwall.argsort()[::-1]
+        surr_ranks = surr_no_mwall.argsort()[::-1]
         
         # Resample surr_no_mwall according to the rank ordering of data_no_mwall
         surr_no_mwall[surr_ranks] = data_no_mwall[data_ranks]
-        output_surr = np.copy(surrogate_data)
+        output_surr = np.zeros_like(surrogate_data)
         output_surr[mask] = surr_no_mwall
         surrogate_data = output_surr
     
     return surrogate_data
 
 
 def plot_data(surface, data, hemi='left', view='lateral', cmap='gray', show=True):
```

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.6.6/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/permutation.py` & `neuroshape-0.0.4.6.6/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/recon.py` & `neuroshape-0.0.4.6.6/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/stats.py` & `neuroshape-0.0.4.6.6/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/checks.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/eigen.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         
     _, M = eigenmodes.shape
     n = int(np.ceil(M * pv / 100))
     
     eigenmodes = eigenmodes[:,:n]
     coeffs = coeffs[:n].reshape(-1, 1)
     
-    new_data = np.matmul(eigenmodes, coeffs)
+    new_data = coeffs.T @ eigenmodes.T
     
     return new_data.squeeze()
     
 
 def reconstruct_surface(surface, eigenmodes, n=100, normalize='area', norm_factor=1, method='matrix'):
     """
     Reconstruct a surface of `n_vertices` given a set of eigenmodes
@@ -311,25 +311,25 @@
 
 def resample_spheroid(spheroid_eigenmodes, angle):
     """
     Resample the N-D hypersphere generated by the N orthogonal unit modes
 
     """
     # ensure the eigenmodes are normalized on the unit hypersphere
-    spheroid_eigenmodes = spheroid_eigenmodes / np.linalg.norm(spheroid_eigenmodes, axis=0)
+    spheroid_eigenmodes = spheroid_eigenmodes #/ np.linalg.norm(spheroid_eigenmodes, axis=0)
     
     # length of group to determine evenness or oddness of dimensions
     #dims = spheroid_eigenmodes.shape[0]
     
     # initialize the new points p
     p = spheroid_eigenmodes
     
     # compute the coordinates for the new points
     for i in range(1, spheroid_eigenmodes.shape[1]):
-        p[:, i] *= np.sin(angle)
+        p[:, i] *= np.cos(angle)
     
     # Compute the coordinates for new points p
     # print("Computing the coordinates for each dimension, multiplying by single angle per group")
     # if dims % 2 == 0: # EVEN
     #     p *= np.cos(angle)
     # else: #dims % 2 == 1 ODD
     #     p *= np.sin(angle)
```

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/geometry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from nipype.interfaces.freesurfer import MRIMarchingCubes
-from lapy import TriaMesh
+from lapy import TriaMesh, TriaIO, Solver
 import warnings
 from collections import OrderedDict
 import scipy.optimize as optimize
 import subprocess
 import os
 import nibabel as nib
 from neuromaps.transforms import mni152_to_fsaverage
 from nilearn import image
 import numpy as np
 from neuromaps.datasets.atlases import fetch_mni152
 from ants import image_read, registration, apply_transforms
 from scipy.spatial import Delaunay, KDTree
+from brainspace import mesh
 
 """
 Helper utilities for geometry and registration
 
     - Runs mri_mc from Freesurfer to create 2d surface
     - Projects 2d surface using gmsh
     - Writes out geometry in tetrahedral format, triangular format, or in Freesurfer binary
@@ -276,119 +277,151 @@
 
     cmd = "sed 's/double/float/g;s/UNSTRUCTURED_GRID/POLYDATA/g;s/CELLS/POLYGONS/g;/CELL_TYPES/,$d' " + tria_file + " > " + tria_file + "'_fixed'"
     os.system(cmd)
     os.system('mv -f ' + tria_file + '_fixed ' + tria_file)
     
     return tria_file
 
-# def mesh_and_remove_medial_wall(nifti_input_filename, fs_dir=None, mesh_type='tria'):
-#     """
-#     Generates a mesh and removes the medial wall when given a FreeSurfer subject directory
-#     Requires recon-all to have been completed and for the names of the
-#     outputs to not have been modified. If `fs_dir` is NoneType or
-#     the annotation files cannot be found, then a naive implementation
-#     of FSL fast is performed to remove the medial wall from the vertices
-#     of the nifti input.
-#     """
-    
-#     if mesh_type not in ['tria', 'tetra']:
-#         raise ValueError("mesh type must be triangular or tetrahedral")
-        
-#     nifti_input_file_head, nifti_input_file_tail = os.path.split(nifti_input_filename)
-#     nifti_input_file_main, nifti_input_file_ext = os.path.splitext(nifti_input_file_tail)
-    
-#     # check if nifti is in MNI152 space
-#     img = image.load_img(nifti_input_filename)
+def create_temp_surface(surface_input, surface_output_filename):
+    """Write surface to a new vtk file.
+
+    Parameters
+    ----------
+    surface_input : brainspace compatible object
+        Loaded vtk object corresponding to a surface triangular mesh
+    surface_output_filename : str
+        Filename of surface to be saved
+    """
+
+    f = open(surface_output_filename, 'w')
+    f.write('# vtk DataFile Version 2.0\n')
+    f.write(surface_output_filename + '\n')
+    f.write('ASCII\n')
+    f.write('DATASET POLYDATA\n')
+    f.write('POINTS ' + str(np.shape(surface_input.Points)[0]) + ' float\n')
+    for i in range(np.shape(surface_input.Points)[0]):
+        f.write(' '.join(map(str, np.array(surface_input.Points[i, :]))))
+        f.write('\n')
+    f.write('\n')
+    f.write('POLYGONS ' + str(np.shape(surface_input.polys2D)[0]) + ' ' + str(4* np.shape(surface_input.polys2D)[0]) + '\n')
+    for i in range(np.shape(surface_input.polys2D)[0]):
+        f.write(' '.join(map(str, np.append(3, np.array(surface_input.polys2D[i, :])))))
+        f.write('\n')
+    f.close()
+
+def get_indices(surface_original, surface_new):
+    """Extract indices of vertices of the two surfaces that match.
+
+    Parameters
+    ----------
+    surface_original : brainspace compatible object
+        Loaded vtk object corresponding to a surface triangular mesh
+    surface_new : brainspace compatible object
+        Loaded vtk object corresponding to a surface triangular mesh
+
+    Returns
+    ------
+    indices : array
+        indices of vertices
+    """
+
+    indices = np.zeros([np.shape(surface_new.Points)[0],1])
+    for i in range(np.shape(surface_new.Points)[0]):
+        indices[i] = np.where(np.all(np.equal(surface_new.Points[i,:],surface_original.Points), axis=1))[0][0]
+    indices = indices.astype(int)
     
-#     if _check_mni(nifti_input_filename) is False:
-#         # keep original affine and mask image to return MNI152
-#         # registered image
-#         img_affine = img.affine
-#         img_mni = native_to_mni152(nifti_input_filename)
-#         img_mni_filename = nifti_input_file_head + '_mni152' + nifti_input_file_ext
-#         print("Saving MNI152-registered input to {}".format(img_mni_filename))
-#         nib.save(img_mni, img_mni_filename)
-        
-#     # if fs_dir is None:
-#     #     print("FreeSurfer subject directory not given, using FSL fast")
-#     #     new_vertices = _remove_medial_wall_no_fs(nifti_input_filename)
-#     #     return new_vertices
-       
-#     # register nifti to FreeSurfer average space
-#     img_fs = mni152_to_fsaverage(img_mni)
-    
-#     # prepare transformation
-#     lh, rh = img_fs
-#     lh_verts = lh.darrays[0].data.reshape(-1,3)
-#     rh_verts = rh.darrays[0].data.reshape(-1,3)
-    
-#     # combine the hemispheres into one image
-#     verts = np.vstack((lh_verts, rh_verts))
-    
-#     xx, yy, zz = verts.T
-
-#     points = np.zeros([xx.shape[0],4])
-#     points[:,0] = xx
-#     points[:,1] = yy
-#     points[:,2] = zz
-#     points[:,3] = 1
-
-#     # calculate transformation matrix
-#     T = get_tkrvox2ras(img.shape, img.header.get_zooms())
-
-#     # apply transformation
-#     points2 = np.matmul(T, np.transpose(points))
-    
-#     #img_fs_filename = nifti_input_file_head + '_fsaverage' + 
-
-#     # generate mesh
-#     tria_file = make_tria_file(img_fs)    
-    
-#     # find pial surfaces and annotation files
-#     lh_pial = fs_dir + '/surf/lh.pial'
-#     rh_pial = fs_dir + '/surf/rh.pial'
-    
-#     try:
-#         # Load the lh and rh pial surface
-#         lh_pial = read_geometry(lh_pial)
-#         rh_pial = read_geometry(rh_pial)    
-        
-#         # Load the lh and rh annotation
-#         lh_labels, _, lh_names = read_annot(fs_dir + '/label/lh.aparc.annot')
-#         rh_labels, _, rh_names = read_annot(fs_dir + '/label/rh.aparc.annot')
-        
-#         # Find the medial wall
-#         lh_medial_wall_label = np.where(lh_names == b'unknown')[0]
-#         lh_medial_wall_vertices = np.where(lh_labels == lh_medial_wall_label)[0]
-        
-#         # mask out medial wall vertices
-        
-#         # fix shape of data structure
-        
-#         return new_vertices
-        
-#     except:
-#     #     # do FSL fast implementation
-#     #     new_vertices = _remove_medial_wall_no_fs(nifti_input_filename)
-#         return new_vertices
-        
+    return indices
 
+def calc_eig(tria, num_modes):
+    """Calculate the eigenvalues and eigenmodes of a surface.
 
-# def _remove_medial_wall_no_fs(nifti_input_filename):
-#     """
-#     Remove the medial wall using FSL fast and masking out the subcortex
-#     """
+    Parameters
+    ----------
+    tria : lapy compatible object
+        Loaded vtk object corresponding to a surface triangular mesh
+    num_modes : int
+        Number of eigenmodes to be calculated
+
+    Returns
+    ------
+    evals : array (num_modes x 1)
+        Eigenvalues
+    emodes : array (number of surface points x num_modes)
+        Eigenmodes
+    """
     
+    fem = Solver(tria, use_cholmod=True)
+    evals, emodes = fem.eigs(k=num_modes)
     
+    return evals, emodes
     
-#     return new_vertices
+def calc_surface_eigenmodes(surface_input_filename, mask_input_filename, save_cut, num_modes):
+    """Main function to calculate the eigenmodes of a cortical surface with application of a mask (e.g., to remove the medial wall).
 
-#def compute_geodesic_distances(vertices, ):
-    
-    
+    Parameters
+    ----------
+    surface_input_filename : str
+        Filename of input surface
+    mask_input_filename : str
+        Filename of mask to be applied on the surface (e.g., cortex without medial wall, values = 1 for mask and 0 elsewhere)
+    output_eval_filename : str  
+        Filename of text file where the output eigenvalues will be stored
+    output_emode_filename : str  
+        Filename of text file where the output eigenmodes will be stored
+    save_cut : boolean 
+        Boolean to decide if the new surface with mask applied will be saved to a new surface file
+    num_modes : int
+        Number of eigenmodes to be calculated          
+    """
+
+    # load surface (as a brainspace object)
+    surface_orig = mesh.mesh_io.read_surface(surface_input_filename)
+    
+    # load mask
+    # can be any ROI (even whole cortex)
+    mask_input_file_main, mask_input_file_ext = os.path.splitext(mask_input_filename)
+    if mask_input_file_ext == '.txt':
+        mask = np.loadtxt(mask_input_filename, delimiter=',')
+    elif mask_input_file_ext == '.gii':
+        mask = nib.load(mask_input_filename).darrays[0].data
+    
+    # create temporary suface based on mask
+    surface_cut = mesh.mesh_operations.mask_points(surface_orig, mask)
+
+    if save_cut == 1:
+        # old method: save vtk of surface_cut and open via lapy TriaIO 
+        # The writing phase of this process is very slow especially for large surfaces
+        temp_cut_filename='temp_cut.gii'
+        temp_cut = nib.GiftiImage()
+        temp_cut.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray(surface_cut.GetPoints().astype('float32')))
+        temp_cut.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray(mesh.mesh_elements.get_cells(surface_cut).astype('int32')))
+        nib.save(temp_cut, temp_cut_filename)
+        # load surface (as a lapy object)
+        vertices, faces = temp_cut.agg_data()
+        tria = TriaMesh(vertices, faces)
+    else:
+        # new method: replace v and t of surface_orig with v and t of surface_cut
+        # faster version without the need to write the vtk file
+        # load surface (as a lapy object)
+        tria = TriaIO.import_vtk(surface_input_filename)
+        tria.v = surface_cut.Points
+        tria.t = np.reshape(surface_cut.Polygons, [surface_cut.n_cells, 4])[:,1:4]
+
+    # calculate eigenvalues and eigenmodes
+    evals, emodes = calc_eig(tria, num_modes)
+    
+    # get indices of vertices of surface_orig that match surface_cut
+    indices = get_indices(surface_orig, surface_cut)
+    
+    # reshape emodes to match vertices of original surface
+    emodes_reshaped = np.zeros([surface_orig.n_points,np.shape(emodes)[1]])
+    for mode in range(np.shape(emodes)[1]):
+        emodes_reshaped[indices,mode] = np.expand_dims(emodes[:,mode], axis=1)
+        
+    return evals, emodes_reshaped
     
 
 def nearest_neighbor(P, X, radius=None):
     """
     Find the one-nearest neighbors of vertices in points `P` on another 
     surface `X` using Delaunay triangulation and KDTree query.
```

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/meshtransforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from scipy.interpolate import griddata
 import numpy as np
 from ..utils.concavehull import ConcaveHull
 from shapely.geometry import Point
 
-def grid(x, vertices, tol=20, spacing=0.5, ch=None):
+def grid(x, vertices, tol=20, spacing=1.0, ch=None):
     """
-    Interpolates surface onto grid for wavelet transform
+    Interpolates surface onto grid
     
     Parameters
     ----------
     x : (N,) np.ndarray
         Data values at each surface vertex
     vertices : (N,3) np.ndarray
         Vertices of gifti object
-    sf : float
-        Shrink factor, default 0.7
+    tol : float
+        Tolerance for calculation of concave hull, default 20
     spacing : float
-        Target grid spacing in mm, default 0.5
+        Target grid spacing in mm, default 1.0
     
     Returns
     -------
     interpolated_data : (N,M) np.ndarray
         Interpolated data on the grid 'xi'
     gridX : (N,) np.ndarray
         Interpolated x coordinates of vertices on the grid
@@ -35,18 +35,17 @@
     c = x
     x = vertices[:, 0]
     y = vertices[:, 1]
     gridX, gridY = np.mgrid[min(x):max(x):spacing, min(y):max(y):spacing]
     
     unbounded_data = griddata((x, y), c, (gridX, gridY), method='nearest', fill_value=0)
     
-    # if not ch:
-    #     ch = ConcaveHull()
-    #     ch.loadpoints(vertices[:, :2])
-    #     ch.calculatehull(tol=tol)
+    ch = ConcaveHull()
+    ch.loadpoints(vertices[:, :2])
+    ch.calculatehull(tol=tol)
     
     bounded_data = np.zeros(unbounded_data.shape)*np.nan
     for i in np.arange(len(unbounded_data)):
         for j in np.arange(len(unbounded_data[i])):
             if ch.boundary.contains(Point(gridX[i,j], gridY[i,j])):
                 bounded_data[i,j] = unbounded_data[i,j]
             else:
@@ -59,15 +58,15 @@
 def mesh(interpolated_data, vertices, gridX, gridY):
     """
     Backprojects grid from 'grid()' to surface
     
     Parameters
     ----------
     interpolated_data : (N,M) np.ndarray
-        Output from 'grid()', interpolated grid to perform wavelet transforms
+        Output from 'grid()', interpolated grid
     vertices : (N,3) np.ndarray
         Vertices of gifti object
     gridX : (N,N) np.ndarray
         Interpolated X coordinates
     gridY : (N,N) np.ndarray
         Interpolated Y coordinates
```

### Comparing `neuroshape-0.0.4.6.5/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.6.6/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.6.6/neuroshape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/pyproject.toml` & `neuroshape-0.0.4.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "setuptools>=42",
     "wheel",
 ]
 
 
 [project]
 name = "neuroshape"
-version = "0.0.4.6.5"
+version = "0.0.4.6.6"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.6.5/setup.py` & `neuroshape-0.0.4.6.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #                   include_dirs=[numpy.get_include()])
 
 #euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
 #                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.6.5',
+      version='0.0.4.6.6',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages())
       #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.6.5/src/eta_squared.c` & `neuroshape-0.0.4.6.6/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/src/euler_threshold.c` & `neuroshape-0.0.4.6.6/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.5/src/glmfit.c` & `neuroshape-0.0.4.6.6/src/glmfit.c`

 * *Files identical despite different names*

