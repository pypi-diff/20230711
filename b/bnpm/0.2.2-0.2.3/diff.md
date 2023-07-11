# Comparing `tmp/bnpm-0.2.2.tar.gz` & `tmp/bnpm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnpm-0.2.2.tar", last modified: Tue Jul 11 19:39:44 2023, max compression
+gzip compressed data, was "bnpm-0.2.3.tar", last modified: Tue Jul 11 20:03:18 2023, max compression
```

## Comparing `bnpm-0.2.2.tar` & `bnpm-0.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.435567 bnpm-0.2.2/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 19:39:44.435679 bnpm-0.2.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.433843 bnpm-0.2.2/bnpm/
--rwxrwxrwx   0 root         (0) root         (0)      907 2023-07-11 19:38:00.000000 bnpm-0.2.2/bnpm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.2/bnpm/ca2p_preprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.2/bnpm/classification.py
--rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.2/bnpm/clustering.py
--rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.2/bnpm/container_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.2/bnpm/cross_validation.py
--rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.2/bnpm/cupy_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.2/bnpm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.2/bnpm/dtw.py
--rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.2/bnpm/email_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.2/bnpm/featurization.py
--rwxrwxrwx   0 root         (0) root         (0)    23399 2023-06-29 05:55:34.000000 bnpm-0.2.2/bnpm/file_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    11769 2023-06-10 18:47:53.000000 bnpm-0.2.2/bnpm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.2/bnpm/image_processing.py
--rwxrwxrwx   0 root         (0) root         (0)    23809 2023-07-11 01:29:59.000000 bnpm-0.2.2/bnpm/indexing.py
--rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.2/bnpm/linear_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.2/bnpm/math_functions.py
--rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.2/bnpm/misc.py
--rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.2/bnpm/optimization.py
--rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.2/bnpm/other_peoples_code.py
--rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.2/bnpm/parallel_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.2/bnpm/path_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    40543 2023-07-11 00:22:09.000000 bnpm-0.2.2/bnpm/plotting_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.2/bnpm/resource_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)    34760 2023-07-11 19:35:57.000000 bnpm-0.2.2/bnpm/server.py
--rwxrwxrwx   0 root         (0) root         (0)    31408 2023-07-11 01:31:23.000000 bnpm-0.2.2/bnpm/similarity.py
--rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.2/bnpm/spectral.py
--rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.2/bnpm/stats.py
--rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.2/bnpm/timeSeries.py
--rwxrwxrwx   0 root         (0) root         (0)    23576 2023-07-06 21:06:01.000000 bnpm-0.2.2/bnpm/torch_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.2/bnpm/video.py
--rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.2/bnpm/welford_moving.py
--rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.2/bnpm/welford_moving_2D.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.435101 bnpm-0.2.2/bnpm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-11 19:39:44.000000 bnpm-0.2.2/bnpm.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 19:39:44.435350 bnpm-0.2.2/demos/
--rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.2.2/demos/slurmDispatcher.py
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-11 19:39:44.436046 bnpm-0.2.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-10 00:46:32.000000 bnpm-0.2.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 20:03:18.531739 bnpm-0.2.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-07-11 20:02:02.000000 bnpm-0.2.3/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 20:03:18.531867 bnpm-0.2.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 20:03:18.530067 bnpm-0.2.3/bnpm/
+-rwxrwxrwx   0 root         (0) root         (0)      907 2023-07-11 20:02:50.000000 bnpm-0.2.3/bnpm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.3/bnpm/ca2p_preprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.3/bnpm/classification.py
+-rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.3/bnpm/clustering.py
+-rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.3/bnpm/container_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.3/bnpm/cross_validation.py
+-rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.3/bnpm/cupy_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.3/bnpm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.3/bnpm/dtw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.3/bnpm/email_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.3/bnpm/featurization.py
+-rwxrwxrwx   0 root         (0) root         (0)    23399 2023-06-29 05:55:34.000000 bnpm-0.2.3/bnpm/file_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    11769 2023-06-10 18:47:53.000000 bnpm-0.2.3/bnpm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.3/bnpm/image_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)    23809 2023-07-11 01:29:59.000000 bnpm-0.2.3/bnpm/indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.3/bnpm/linear_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.3/bnpm/math_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.3/bnpm/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.3/bnpm/optimization.py
+-rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.3/bnpm/other_peoples_code.py
+-rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.3/bnpm/parallel_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.3/bnpm/path_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    40543 2023-07-11 00:22:09.000000 bnpm-0.2.3/bnpm/plotting_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.3/bnpm/resource_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)    34760 2023-07-11 19:35:57.000000 bnpm-0.2.3/bnpm/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    31408 2023-07-11 01:31:23.000000 bnpm-0.2.3/bnpm/similarity.py
+-rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.3/bnpm/spectral.py
+-rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.3/bnpm/stats.py
+-rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.3/bnpm/timeSeries.py
+-rwxrwxrwx   0 root         (0) root         (0)    23576 2023-07-06 21:06:01.000000 bnpm-0.2.3/bnpm/torch_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.3/bnpm/video.py
+-rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.3/bnpm/welford_moving.py
+-rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.3/bnpm/welford_moving_2D.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 20:03:18.531503 bnpm-0.2.3/bnpm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      899 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      349 2023-06-10 00:46:32.000000 bnpm-0.2.3/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-11 20:03:18.532257 bnpm-0.2.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-11 20:02:35.000000 bnpm-0.2.3/setup.py
```

### Comparing `bnpm-0.2.2/LICENSE` & `bnpm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/PKG-INFO` & `bnpm-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
```

### Comparing `bnpm-0.2.2/README.md` & `bnpm-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/__init__.py` & `bnpm-0.2.3/bnpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             'torch_helpers',
             'video',
         ]
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
```

### Comparing `bnpm-0.2.2/bnpm/ca2p_preprocessing.py` & `bnpm-0.2.3/bnpm/ca2p_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/classification.py` & `bnpm-0.2.3/bnpm/classification.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/clustering.py` & `bnpm-0.2.3/bnpm/clustering.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/container_helpers.py` & `bnpm-0.2.3/bnpm/container_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/cross_validation.py` & `bnpm-0.2.3/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/cupy_helpers.py` & `bnpm-0.2.3/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/decomposition.py` & `bnpm-0.2.3/bnpm/decomposition.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/dtw.py` & `bnpm-0.2.3/bnpm/dtw.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/email_helpers.py` & `bnpm-0.2.3/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/featurization.py` & `bnpm-0.2.3/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/file_helpers.py` & `bnpm-0.2.3/bnpm/file_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/h5_handling.py` & `bnpm-0.2.3/bnpm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/image_processing.py` & `bnpm-0.2.3/bnpm/image_processing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/indexing.py` & `bnpm-0.2.3/bnpm/indexing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/linear_regression.py` & `bnpm-0.2.3/bnpm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/math_functions.py` & `bnpm-0.2.3/bnpm/math_functions.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/misc.py` & `bnpm-0.2.3/bnpm/misc.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/optimization.py` & `bnpm-0.2.3/bnpm/optimization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/other_peoples_code.py` & `bnpm-0.2.3/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/parallel_helpers.py` & `bnpm-0.2.3/bnpm/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/path_helpers.py` & `bnpm-0.2.3/bnpm/path_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/plotting_helpers.py` & `bnpm-0.2.3/bnpm/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/resource_tracking.py` & `bnpm-0.2.3/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/server.py` & `bnpm-0.2.3/bnpm/server.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/similarity.py` & `bnpm-0.2.3/bnpm/similarity.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/spectral.py` & `bnpm-0.2.3/bnpm/spectral.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/stats.py` & `bnpm-0.2.3/bnpm/stats.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/timeSeries.py` & `bnpm-0.2.3/bnpm/timeSeries.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/torch_helpers.py` & `bnpm-0.2.3/bnpm/torch_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/video.py` & `bnpm-0.2.3/bnpm/video.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/welford_moving.py` & `bnpm-0.2.3/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm/welford_moving_2D.py` & `bnpm-0.2.3/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.2/bnpm.egg-info/PKG-INFO` & `bnpm-0.2.3/bnpm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
```

### Comparing `bnpm-0.2.2/bnpm.egg-info/SOURCES.txt` & `bnpm-0.2.3/bnpm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 bnpm/__init__.py
 bnpm/ca2p_preprocessing.py
 bnpm/classification.py
 bnpm/clustering.py
 bnpm/container_helpers.py
@@ -35,9 +37,8 @@
 bnpm/video.py
 bnpm/welford_moving.py
 bnpm/welford_moving_2D.py
 bnpm.egg-info/PKG-INFO
 bnpm.egg-info/SOURCES.txt
 bnpm.egg-info/dependency_links.txt
 bnpm.egg-info/requires.txt
-bnpm.egg-info/top_level.txt
-demos/slurmDispatcher.py
+bnpm.egg-info/top_level.txt
```

### Comparing `bnpm-0.2.2/setup.py` & `bnpm-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,20 @@
 
 
 setup(
     name='bnpm',
     version=version,
     author='Richard Hakim',
     keywords=['data analysis', 'machine learning', 'neuroscience'],
-    packages=['bnpm'],
     license='LICENSE',
     description='A library of useful modules for data analysis.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
+    url='https://github.com/RichieHakim/basic_neural_processing_modules',
+
+    packages=['bnpm'],
+
     install_requires=deps_core,
     extras_require={
         'advanced': deps_advanced,
     },
-    url='https://github.com/RichieHakim/basic_neural_processing_modules',
 )
```

