# Comparing `tmp/pheno-utils-0.3.1.tar.gz` & `tmp/pheno-utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.1.tar", last modified: Tue Jul 11 09:56:07 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.2.tar", last modified: Tue Jul 11 10:28:50 2023, max compression
```

## Comparing `pheno-utils-0.3.1.tar` & `pheno-utils-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:56:07.493607 pheno-utils-0.3.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1431 2023-07-11 09:56:07.492757 pheno-utils-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-21 16:13:16.000000 pheno-utils-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:56:07.450851 pheno-utils-0.3.1/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16963 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7754 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    19887 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13210 2023-07-11 09:55:28.000000 pheno-utils-0.3.1/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:56:07.487103 pheno-utils-0.3.1/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1431 2023-07-11 09:56:07.000000 pheno-utils-0.3.1/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-11 09:56:07.000000 pheno-utils-0.3.1/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 09:56:07.000000 pheno-utils-0.3.1/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-11 09:56:07.000000 pheno-utils-0.3.1/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.1/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-11 09:56:07.000000 pheno-utils-0.3.1/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 09:56:07.000000 pheno-utils-0.3.1/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-11 09:54:47.000000 pheno-utils-0.3.1/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 09:56:07.494103 pheno-utils-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:28:50.069188 pheno-utils-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-11 10:28:50.068168 pheno-utils-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-11 10:26:59.000000 pheno-utils-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:28:50.035898 pheno-utils-0.3.2/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16963 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7754 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    19887 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-07-11 10:28:05.000000 pheno-utils-0.3.2/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:28:50.064704 pheno-utils-0.3.2/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-11 10:28:49.000000 pheno-utils-0.3.2/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-11 10:28:49.000000 pheno-utils-0.3.2/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 10:28:49.000000 pheno-utils-0.3.2/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-11 10:28:49.000000 pheno-utils-0.3.2/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.2/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-11 10:28:49.000000 pheno-utils-0.3.2/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 10:28:49.000000 pheno-utils-0.3.2/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-11 10:28:01.000000 pheno-utils-0.3.2/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 10:28:50.072962 pheno-utils-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.2/setup.py
```

### Comparing `pheno-utils-0.3.1/LICENSE` & `pheno-utils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/PKG-INFO` & `pheno-utils-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.1
-Summary: Pheno data utils - A dynamic Python package developed by Pheno.AI, for handling our medical datasets. It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
+Version: 0.3.2
+Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pheno-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-Viz functions, loaders, mergers.
-
-WORK IN PROGRESS
+pheno-utils is a dynamic Python package developed by Pheno.AI, for handling our medical datasets. 
+It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
 
 ## Install
 
 ``` sh
 pip install pheno_utils
 ```
```

### Comparing `pheno-utils-0.3.1/pheno_utils/_modidx.py` & `pheno-utils-0.3.2/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.2/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.2/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/basic_plots.py` & `pheno-utils-0.3.2/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.2/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.2/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.2/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/config.py` & `pheno-utils-0.3.2/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/dates_plots.py` & `pheno-utils-0.3.2/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.2/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/meta_loader.py` & `pheno-utils-0.3.2/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.2/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.2/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.2/pheno_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.1
-Summary: Pheno data utils - A dynamic Python package developed by Pheno.AI, for handling our medical datasets. It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
+Version: 0.3.2
+Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pheno-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-Viz functions, loaders, mergers.
-
-WORK IN PROGRESS
+pheno-utils is a dynamic Python package developed by Pheno.AI, for handling our medical datasets. 
+It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
 
 ## Install
 
 ``` sh
 pip install pheno_utils
 ```
```

### Comparing `pheno-utils-0.3.1/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.2/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.1/settings.ini` & `pheno-utils-0.3.2/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.3.1
+version = 0.3.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
@@ -27,15 +27,15 @@
 title = %(lib_name)s
 
 ### PyPI ###
 audience = Developers
 author = hrossman
 author_email = hagairossman@gmail.com
 copyright = 2023 onwards, %(author)s
-description = Pheno data utils - A dynamic Python package developed by Pheno.AI, for handling our medical datasets. It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
+description = Pheno data utils - viz, loaders, mergers
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = hrossman
 
 ### Optional ###
 requirements = fastcore pandas==1.5.2 numpy scipy fastparquet matplotlib seaborn scikit-learn pyCompare tsmoothie smart_open neurokit2 "dask[dataframe]"
```

### Comparing `pheno-utils-0.3.1/setup.py` & `pheno-utils-0.3.2/setup.py`

 * *Files identical despite different names*

