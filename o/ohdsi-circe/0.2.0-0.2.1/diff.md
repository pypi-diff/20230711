# Comparing `tmp/ohdsi-circe-0.2.0.tar.gz` & `tmp/ohdsi-circe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-circe-0.2.0.tar", last modified: Wed Jun 14 08:26:50 2023, max compression
+gzip compressed data, was "ohdsi-circe-0.2.1.tar", last modified: Tue Jul 11 14:30:33 2023, max compression
```

## Comparing `ohdsi-circe-0.2.0.tar` & `ohdsi-circe-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.141492 ohdsi-circe-0.2.0/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.141492 ohdsi-circe-0.2.0/ohdsi/circe/
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.141492 ohdsi-circe-0.2.0/ohdsi/circe/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSetList.json
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/data/simpleCohort.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi/circe/
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi/circe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSetList.json
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/data/simpleCohort.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/setup.py
```

### Comparing `ohdsi-circe-0.2.0/PKG-INFO` & `ohdsi-circe-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-circe
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
```

### Comparing `ohdsi-circe-0.2.0/ohdsi/circe/__init__.py` & `ohdsi-circe-0.2.1/ohdsi/circe/__init__.py`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSet.json` & `ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSet.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSetList.json` & `ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSetList.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.0/ohdsi/circe/data/simpleCohort.json` & `ohdsi-circe-0.2.1/ohdsi/circe/data/simpleCohort.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.0/ohdsi_circe.egg-info/PKG-INFO` & `ohdsi-circe-0.2.1/ohdsi_circe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-circe
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
```

### Comparing `ohdsi-circe-0.2.0/setup.py` & `ohdsi-circe-0.2.1/setup.py`

 * *Files identical despite different names*

