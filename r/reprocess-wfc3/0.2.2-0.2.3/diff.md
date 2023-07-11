# Comparing `tmp/reprocess_wfc3-0.2.2.tar.gz` & `tmp/reprocess_wfc3-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprocess_wfc3-0.2.2.tar", last modified: Tue Jul 11 12:41:23 2023, max compression
+gzip compressed data, was "reprocess_wfc3-0.2.3.tar", last modified: Tue Jul 11 12:45:10 2023, max compression
```

## Comparing `reprocess_wfc3-0.2.2.tar` & `reprocess_wfc3-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.903876 reprocess_wfc3-0.2.2/
--rw-r--r--   0 gbrammer   (501) wheel        (0)     1157 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.2/.gitignore
--rw-r--r--   0 gbrammer   (501) wheel        (0)     1069 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.2/LICENSE
--rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2023-07-11 12:41:23.903757 reprocess_wfc3-0.2.2/PKG-INFO
--rw-r--r--   0 gbrammer   (501) wheel        (0)      366 2021-04-22 09:35:10.000000 reprocess_wfc3-0.2.2/README.md
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.902757 reprocess_wfc3-0.2.2/reprocess_wfc3/
--rw-r--r--   0 gbrammer   (501) wheel        (0)      144 2019-05-07 05:46:19.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/__init__.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)    12959 2022-01-03 10:31:57.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/anomalies.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)    29191 2023-07-11 12:35:19.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/reprocess_wfc3.py
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.903474 reprocess_wfc3-0.2.2/reprocess_wfc3/tests/
--rw-r--r--   0 gbrammer   (501) wheel        (0)        0 2019-05-07 05:47:38.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/tests/__init__.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)      326 2019-05-07 05:53:24.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/tests/test_basic.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)     4657 2022-01-12 11:51:09.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/utils.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)       25 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/version.py
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.903265 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/
--rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/PKG-INFO
--rw-r--r--   0 gbrammer   (501) wheel        (0)      395 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/SOURCES.txt
--rw-r--r--   0 gbrammer   (501) wheel        (0)        1 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/dependency_links.txt
--rw-r--r--   0 gbrammer   (501) wheel        (0)       15 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/top_level.txt
--rw-r--r--   0 gbrammer   (501) wheel        (0)       38 2023-07-11 12:41:23.903916 reprocess_wfc3-0.2.2/setup.cfg
--rw-r--r--   0 gbrammer   (501) wheel        (0)      702 2023-07-11 12:40:26.000000 reprocess_wfc3-0.2.2/setup.py
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:45:10.929557 reprocess_wfc3-0.2.3/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)     1157 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.3/.gitignore
+-rw-r--r--   0 gbrammer   (501) wheel        (0)     1069 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.3/LICENSE
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2023-07-11 12:45:10.929426 reprocess_wfc3-0.2.3/PKG-INFO
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      366 2021-04-22 09:35:10.000000 reprocess_wfc3-0.2.3/README.md
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:45:10.928348 reprocess_wfc3-0.2.3/reprocess_wfc3/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      144 2019-05-07 05:46:19.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/__init__.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)    12959 2022-01-03 10:31:57.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/anomalies.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)    29191 2023-07-11 12:35:19.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/reprocess_wfc3.py
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:45:10.929138 reprocess_wfc3-0.2.3/reprocess_wfc3/tests/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)        0 2019-05-07 05:47:38.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/tests/__init__.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      326 2019-05-07 05:53:24.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/tests/test_basic.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)     4657 2022-01-12 11:51:09.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/utils.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)       25 2023-07-11 12:45:10.000000 reprocess_wfc3-0.2.3/reprocess_wfc3/version.py
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:45:10.928879 reprocess_wfc3-0.2.3/reprocess_wfc3.egg-info/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2023-07-11 12:45:10.000000 reprocess_wfc3-0.2.3/reprocess_wfc3.egg-info/PKG-INFO
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      395 2023-07-11 12:45:10.000000 reprocess_wfc3-0.2.3/reprocess_wfc3.egg-info/SOURCES.txt
+-rw-r--r--   0 gbrammer   (501) wheel        (0)        1 2023-07-11 12:45:10.000000 reprocess_wfc3-0.2.3/reprocess_wfc3.egg-info/dependency_links.txt
+-rw-r--r--   0 gbrammer   (501) wheel        (0)       15 2023-07-11 12:45:10.000000 reprocess_wfc3-0.2.3/reprocess_wfc3.egg-info/top_level.txt
+-rw-r--r--   0 gbrammer   (501) wheel        (0)       38 2023-07-11 12:45:10.929597 reprocess_wfc3-0.2.3/setup.cfg
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      753 2023-07-11 12:44:31.000000 reprocess_wfc3-0.2.3/setup.py
```

### Comparing `reprocess_wfc3-0.2.2/.gitignore` & `reprocess_wfc3-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.2/LICENSE` & `reprocess_wfc3-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.2/reprocess_wfc3/anomalies.py` & `reprocess_wfc3-0.2.3/reprocess_wfc3/anomalies.py`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.2/reprocess_wfc3/reprocess_wfc3.py` & `reprocess_wfc3-0.2.3/reprocess_wfc3/reprocess_wfc3.py`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.2/reprocess_wfc3/utils.py` & `reprocess_wfc3-0.2.3/reprocess_wfc3/utils.py`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.2/setup.py` & `reprocess_wfc3-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #from distutils.core import setup
 from setuptools import setup
 
 #version = '0.1' # 
 #version = '0.2' # - change trail detection thresholds
 # version = '0.2.1' # - error checking on fetch_calibs and calwf3
-version = '0.2.2' # - numpy bug, python>=3.9
+# version = '0.2.2' # - numpy bug, python>=3.9
+version = '0.2.3' # - actually increment version
 
 version_str = """# 
 __version__ = "{0}"\n""".format(version)
 
 fp = open('reprocess_wfc3/version.py','w')
 fp.write(version_str)
 fp.close()
```

