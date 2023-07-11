# Comparing `tmp/reprocess_wfc3-0.2.1.tar.gz` & `tmp/reprocess_wfc3-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprocess_wfc3-0.2.1.tar", last modified: Sun Nov 20 12:40:20 2022, max compression
+gzip compressed data, was "reprocess_wfc3-0.2.2.tar", last modified: Tue Jul 11 12:41:23 2023, max compression
```

## Comparing `reprocess_wfc3-0.2.1.tar` & `reprocess_wfc3-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2022-11-20 12:40:20.175737 reprocess_wfc3-0.2.1/
--rw-r--r--   0 gbrammer   (501) wheel        (0)     1157 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.1/.gitignore
--rw-r--r--   0 gbrammer   (501) wheel        (0)     1069 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.1/LICENSE
--rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2022-11-20 12:40:20.175608 reprocess_wfc3-0.2.1/PKG-INFO
--rw-r--r--   0 gbrammer   (501) wheel        (0)      366 2021-04-22 09:35:10.000000 reprocess_wfc3-0.2.1/README.md
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2022-11-20 12:40:20.174719 reprocess_wfc3-0.2.1/reprocess_wfc3/
--rw-r--r--   0 gbrammer   (501) wheel        (0)      144 2019-05-07 05:46:19.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/__init__.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)    12959 2022-01-03 10:31:57.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/anomalies.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)    29189 2022-01-05 09:57:26.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/reprocess_wfc3.py
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2022-11-20 12:40:20.175439 reprocess_wfc3-0.2.1/reprocess_wfc3/tests/
--rw-r--r--   0 gbrammer   (501) wheel        (0)        0 2019-05-07 05:47:38.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/tests/__init__.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)      326 2019-05-07 05:53:24.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/tests/test_basic.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)     4657 2022-01-12 11:51:09.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/utils.py
--rw-r--r--   0 gbrammer   (501) wheel        (0)       25 2022-11-20 12:40:20.000000 reprocess_wfc3-0.2.1/reprocess_wfc3/version.py
-drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2022-11-20 12:40:20.175228 reprocess_wfc3-0.2.1/reprocess_wfc3.egg-info/
--rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2022-11-20 12:40:20.000000 reprocess_wfc3-0.2.1/reprocess_wfc3.egg-info/PKG-INFO
--rw-r--r--   0 gbrammer   (501) wheel        (0)      395 2022-11-20 12:40:20.000000 reprocess_wfc3-0.2.1/reprocess_wfc3.egg-info/SOURCES.txt
--rw-r--r--   0 gbrammer   (501) wheel        (0)        1 2022-11-20 12:40:20.000000 reprocess_wfc3-0.2.1/reprocess_wfc3.egg-info/dependency_links.txt
--rw-r--r--   0 gbrammer   (501) wheel        (0)       15 2022-11-20 12:40:20.000000 reprocess_wfc3-0.2.1/reprocess_wfc3.egg-info/top_level.txt
--rw-r--r--   0 gbrammer   (501) wheel        (0)       38 2022-11-20 12:40:20.175772 reprocess_wfc3-0.2.1/setup.cfg
--rw-r--r--   0 gbrammer   (501) wheel        (0)      655 2021-04-22 08:59:48.000000 reprocess_wfc3-0.2.1/setup.py
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.903876 reprocess_wfc3-0.2.2/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)     1157 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.2/.gitignore
+-rw-r--r--   0 gbrammer   (501) wheel        (0)     1069 2019-03-18 10:39:43.000000 reprocess_wfc3-0.2.2/LICENSE
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2023-07-11 12:41:23.903757 reprocess_wfc3-0.2.2/PKG-INFO
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      366 2021-04-22 09:35:10.000000 reprocess_wfc3-0.2.2/README.md
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.902757 reprocess_wfc3-0.2.2/reprocess_wfc3/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      144 2019-05-07 05:46:19.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/__init__.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)    12959 2022-01-03 10:31:57.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/anomalies.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)    29191 2023-07-11 12:35:19.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/reprocess_wfc3.py
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.903474 reprocess_wfc3-0.2.2/reprocess_wfc3/tests/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)        0 2019-05-07 05:47:38.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/tests/__init__.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      326 2019-05-07 05:53:24.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/tests/test_basic.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)     4657 2022-01-12 11:51:09.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/utils.py
+-rw-r--r--   0 gbrammer   (501) wheel        (0)       25 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3/version.py
+drwxr-xr-x   0 gbrammer   (501) wheel        (0)        0 2023-07-11 12:41:23.903265 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      242 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/PKG-INFO
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      395 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/SOURCES.txt
+-rw-r--r--   0 gbrammer   (501) wheel        (0)        1 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/dependency_links.txt
+-rw-r--r--   0 gbrammer   (501) wheel        (0)       15 2023-07-11 12:41:23.000000 reprocess_wfc3-0.2.2/reprocess_wfc3.egg-info/top_level.txt
+-rw-r--r--   0 gbrammer   (501) wheel        (0)       38 2023-07-11 12:41:23.903916 reprocess_wfc3-0.2.2/setup.cfg
+-rw-r--r--   0 gbrammer   (501) wheel        (0)      702 2023-07-11 12:40:26.000000 reprocess_wfc3-0.2.2/setup.py
```

### Comparing `reprocess_wfc3-0.2.1/.gitignore` & `reprocess_wfc3-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.1/LICENSE` & `reprocess_wfc3-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.1/reprocess_wfc3/anomalies.py` & `reprocess_wfc3-0.2.2/reprocess_wfc3/anomalies.py`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.1/reprocess_wfc3/reprocess_wfc3.py` & `reprocess_wfc3-0.2.2/reprocess_wfc3/reprocess_wfc3.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         flat = 1
                 
     NSAMP = ima[0].header['NSAMP']
     sh = ima['SCI',1].shape
     
     cube = np.zeros((NSAMP, sh[0], sh[1]))
     if 'ima' in ima.filename():
-        dq = np.zeros((NSAMP, sh[0], sh[1]), dtype=np.int)
+        dq = np.zeros((NSAMP, sh[0], sh[1]), dtype=np.int32)
     else:
         dq = 0
     
     if get_err:
         cube_err = cube*0
         
     times = np.zeros(NSAMP)
```

### Comparing `reprocess_wfc3-0.2.1/reprocess_wfc3/utils.py` & `reprocess_wfc3-0.2.2/reprocess_wfc3/utils.py`

 * *Files identical despite different names*

### Comparing `reprocess_wfc3-0.2.1/setup.py` & `reprocess_wfc3-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #from distutils.core import setup
 from setuptools import setup
 
 #version = '0.1' # 
 #version = '0.2' # - change trail detection thresholds
-version = '0.2.1' # - error checking on fetch_calibs and calwf3
+# version = '0.2.1' # - error checking on fetch_calibs and calwf3
+version = '0.2.2' # - numpy bug, python>=3.9
 
 version_str = """# 
 __version__ = "{0}"\n""".format(version)
 
 fp = open('reprocess_wfc3/version.py','w')
 fp.write(version_str)
 fp.close()
```

