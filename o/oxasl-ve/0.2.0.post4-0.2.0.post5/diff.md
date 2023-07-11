# Comparing `tmp/oxasl-ve-0.2.0.post4.tar.gz` & `tmp/oxasl-ve-0.2.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oxasl-ve-0.2.0.post4.tar", last modified: Tue Jul 11 10:44:14 2023, max compression
+gzip compressed data, was "dist/oxasl-ve-0.2.0.post5.tar", last modified: Tue Jul 11 12:08:57 2023, max compression
```

## Comparing `oxasl-ve-0.2.0.post4.tar` & `oxasl-ve-0.2.0.post5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 10:44:14.000000 oxasl-ve-0.2.0.post4/
--rw-r--r--   0 martin    (1000) martin    (1000)    10174 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post4/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       33 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post4/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     1001 2023-07-11 10:44:14.000000 oxasl-ve-0.2.0.post4/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      356 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post4/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 10:44:14.000000 oxasl-ve-0.2.0.post4/oxasl_ve/
--rw-r--r--   0 martin    (1000) martin    (1000)      632 2023-07-11 10:41:35.000000 oxasl-ve-0.2.0.post4/oxasl_ve/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)       77 2023-07-11 10:44:13.000000 oxasl-ve-0.2.0.post4/oxasl_ve/_version.py
--rw-r--r--   0 martin    (1000) martin    (1000)    22539 2023-07-11 10:42:56.000000 oxasl-ve-0.2.0.post4/oxasl_ve/api.py
--rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post4/oxasl_ve/modmat_default.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1845 2022-11-25 12:32:00.000000 oxasl-ve-0.2.0.post4/oxasl_ve/veaslc_cli_wrapper.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 10:44:14.000000 oxasl-ve-0.2.0.post4/oxasl_ve/wrappers/
--rw-r--r--   0 martin    (1000) martin    (1000)       49 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post4/oxasl_ve/wrappers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1006 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post4/oxasl_ve/wrappers/veaslc.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 10:44:14.000000 oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     1001 2023-07-11 10:44:13.000000 oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-11 10:44:13.000000 oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-11 10:44:13.000000 oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       24 2023-07-11 10:44:13.000000 oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-11 10:44:13.000000 oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       25 2023-07-11 10:41:35.000000 oxasl-ve-0.2.0.post4/requirements.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-11 10:44:14.000000 oxasl-ve-0.2.0.post4/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     3768 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post4/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/
+-rw-r--r--   0 martin    (1000) martin    (1000)    10174 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post5/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)       33 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     1001 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      356 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/oxasl_ve/
+-rw-r--r--   0 martin    (1000) martin    (1000)      632 2023-07-11 12:08:12.000000 oxasl-ve-0.2.0.post5/oxasl_ve/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)       77 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve/_version.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    22544 2023-07-11 12:08:29.000000 oxasl-ve-0.2.0.post5/oxasl_ve/api.py
+-rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/oxasl_ve/modmat_default.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1845 2023-07-11 12:08:12.000000 oxasl-ve-0.2.0.post5/oxasl_ve/veaslc_cli_wrapper.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/
+-rw-r--r--   0 martin    (1000) martin    (1000)       49 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1006 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/veaslc.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1001 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       24 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       25 2023-07-11 12:03:38.000000 oxasl-ve-0.2.0.post5/requirements.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)     3768 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post5/setup.py
```

### Comparing `oxasl-ve-0.2.0.post4/LICENSE` & `oxasl-ve-0.2.0.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post4/PKG-INFO` & `oxasl-ve-0.2.0.post5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.0.post4
+Version: 0.2.0.post5
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `oxasl-ve-0.2.0.post4/oxasl_ve/__init__.py` & `oxasl-ve-0.2.0.post5/oxasl_ve/__init__.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post4/oxasl_ve/api.py` & `oxasl-ve-0.2.0.post5/oxasl_ve/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
                 _combine_vessels_weighted(wsp, num_vessels, basil_output, method=wsp.ifnone("arrival_combine", "weightedperf"))
 
     #report = Report("Combined output for all vessels")
     #oxford_asl.output_report(wsp.output.all_vessels.native, report=report)
     #wsp.report.add("all_vessels", report)
     wsp.basildirs.append("")
 
-def run(wsp):
+def model_ve(wsp):
     """
     Do vessel decoding and modelling on vessel-encoded ASL data
 
     :param wsp: Workspace object
 
     Required workspace attributes
     -----------------------------
```

### Comparing `oxasl-ve-0.2.0.post4/oxasl_ve/modmat_default.py` & `oxasl-ve-0.2.0.post5/oxasl_ve/modmat_default.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post4/oxasl_ve/veaslc_cli_wrapper.py` & `oxasl-ve-0.2.0.post5/oxasl_ve/veaslc_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post4/oxasl_ve/wrappers/veaslc.py` & `oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/veaslc.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post4/oxasl_ve.egg-info/PKG-INFO` & `oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.0.post4
+Version: 0.2.0.post5
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `oxasl-ve-0.2.0.post4/setup.py` & `oxasl-ve-0.2.0.post5/setup.py`

 * *Files identical despite different names*

