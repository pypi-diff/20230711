# Comparing `tmp/rfit-0.2.20230120.tar.gz` & `tmp/rfit-0.3.20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfit-0.2.20230120.tar", last modified: Sat Jan 21 03:31:04 2023, max compression
+gzip compressed data, was "rfit-0.3.20230711.tar", last modified: Tue Jul 11 13:52:20 2023, max compression
```

## Comparing `rfit-0.2.20230120.tar` & `rfit-0.3.20230711.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-01-21 03:31:04.239675 rfit-0.2.20230120/
--rw-r--r--   0 elo        (503) staff       (20)     1065 2022-06-01 20:20:03.000000 rfit-0.2.20230120/LICENSE
--rw-r--r--   0 elo        (503) staff       (20)      861 2023-01-21 03:31:04.239825 rfit-0.2.20230120/PKG-INFO
--rw-r--r--   0 elo        (503) staff       (20)      346 2022-06-01 20:20:03.000000 rfit-0.2.20230120/README.md
--rw-r--r--   0 elo        (503) staff       (20)       84 2022-06-01 20:20:03.000000 rfit-0.2.20230120/pyproject.toml
--rw-r--r--   0 elo        (503) staff       (20)      714 2023-01-21 03:31:04.240588 rfit-0.2.20230120/setup.cfg
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-01-21 03:31:04.232915 rfit-0.2.20230120/src/
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-01-21 03:31:04.236251 rfit-0.2.20230120/src/rfit/
--rw-r--r--   0 elo        (503) staff       (20)      363 2022-06-01 20:20:03.000000 rfit-0.2.20230120/src/rfit/__init__.py
--rw-r--r--   0 elo        (503) staff       (20)     2231 2023-01-21 03:16:28.000000 rfit-0.2.20230120/src/rfit/api.py
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-01-21 03:31:04.239370 rfit-0.2.20230120/src/rfit/learn/
--rw-r--r--   0 elo        (503) staff       (20)      304 2022-06-01 20:20:03.000000 rfit-0.2.20230120/src/rfit/learn/__init__.py
--rwxr-xr-x   0 elo        (503) staff       (20)     4749 2022-06-01 20:20:03.000000 rfit-0.2.20230120/src/rfit/learn/boundary_plots.py
--rwxr-xr-x   0 elo        (503) staff       (20)     2453 2022-06-01 20:20:03.000000 rfit-0.2.20230120/src/rfit/learn/helper.py
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-01-21 03:31:04.238264 rfit-0.2.20230120/src/rfit.egg-info/
--rw-r--r--   0 elo        (503) staff       (20)      861 2023-01-21 03:31:04.000000 rfit-0.2.20230120/src/rfit.egg-info/PKG-INFO
--rw-r--r--   0 elo        (503) staff       (20)      323 2023-01-21 03:31:04.000000 rfit-0.2.20230120/src/rfit.egg-info/SOURCES.txt
--rw-r--r--   0 elo        (503) staff       (20)        1 2023-01-21 03:31:04.000000 rfit-0.2.20230120/src/rfit.egg-info/dependency_links.txt
--rw-r--r--   0 elo        (503) staff       (20)       49 2023-01-21 03:31:04.000000 rfit-0.2.20230120/src/rfit.egg-info/requires.txt
--rw-r--r--   0 elo        (503) staff       (20)        5 2023-01-21 03:31:04.000000 rfit-0.2.20230120/src/rfit.egg-info/top_level.txt
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.279638 rfit-0.3.20230711/
+-rw-r--r--   0 elo        (503) staff       (20)     1065 2022-06-01 20:20:03.000000 rfit-0.3.20230711/LICENSE
+-rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 13:52:20.279779 rfit-0.3.20230711/PKG-INFO
+-rw-r--r--   0 elo        (503) staff       (20)      346 2023-07-11 13:51:01.000000 rfit-0.3.20230711/README.md
+-rw-r--r--   0 elo        (503) staff       (20)       84 2022-06-01 20:20:03.000000 rfit-0.3.20230711/pyproject.toml
+-rw-r--r--   0 elo        (503) staff       (20)      697 2023-07-11 13:52:20.280427 rfit-0.3.20230711/setup.cfg
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.272077 rfit-0.3.20230711/src/
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.274872 rfit-0.3.20230711/src/rfit/
+-rw-r--r--   0 elo        (503) staff       (20)      363 2022-06-01 20:20:03.000000 rfit-0.3.20230711/src/rfit/__init__.py
+-rw-r--r--   0 elo        (503) staff       (20)     2225 2023-07-11 13:40:13.000000 rfit-0.3.20230711/src/rfit/api.py
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.279055 rfit-0.3.20230711/src/rfit/learn/
+-rw-r--r--   0 elo        (503) staff       (20)      304 2022-06-01 20:20:03.000000 rfit-0.3.20230711/src/rfit/learn/__init__.py
+-rwxr-xr-x   0 elo        (503) staff       (20)     4749 2022-06-01 20:20:03.000000 rfit-0.3.20230711/src/rfit/learn/boundary_plots.py
+-rwxr-xr-x   0 elo        (503) staff       (20)     1412 2023-07-11 13:42:41.000000 rfit-0.3.20230711/src/rfit/learn/helper.py
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.277379 rfit-0.3.20230711/src/rfit.egg-info/
+-rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/PKG-INFO
+-rw-r--r--   0 elo        (503) staff       (20)      323 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/SOURCES.txt
+-rw-r--r--   0 elo        (503) staff       (20)        1 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/dependency_links.txt
+-rw-r--r--   0 elo        (503) staff       (20)       33 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/requires.txt
+-rw-r--r--   0 elo        (503) staff       (20)        5 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/top_level.txt
```

### Comparing `rfit-0.2.20230120/LICENSE` & `rfit-0.3.20230711/LICENSE`

 * *Files identical despite different names*

### Comparing `rfit-0.2.20230120/PKG-INFO` & `rfit-0.3.20230711/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rfit
-Version: 0.2.20230120
+Version: 0.3.20230711
 Summary: GWU Data Science python class helper functions
 Home-page: https://github.com/physicsland/rfitapi
 Author: Edwin Lo
 Author-email: elo@regression.fit
 Project-URL: Bug Tracker, https://github.com/physicsland/rfitapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Regression.fit api
 
-Last updated: 2022-06-01
+Last updated: 2023-07-11
 
 This package (rfit - regression.fit) is for use at The George Washington University Data Science program. There are some useful and convenient functions we use in our python classes. 
 
 One of them is dfapi, which connects to the api.regression.fit endpoint, to load dataframes used in our classes.
```

### Comparing `rfit-0.2.20230120/setup.cfg` & `rfit-0.3.20230711/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rfit
-version = 0.2.20230120
+version = 0.3.20230711
 author = Edwin Lo
 author_email = elo@regression.fit
 description = GWU Data Science python class helper functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/physicsland/rfitapi
 project_urls = 
@@ -19,15 +19,14 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
 	matplotlib
 	pandas
-	mysql-connector
 	requests
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `rfit-0.2.20230120/src/rfit/api.py` & `rfit-0.3.20230711/src/rfit/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # __all__ = ('dfapi')
 import pandas as pd
 import numpy as np
 import requests
 
 def dfapi(tbname, ind_col_name = ""):
-  """ 
+  """
   call to api endpoint on regression.fit database to access datasets
-  :param str tbname: table name that exist on the server 
-  :param str ind_col_name: optional, name of index column 
-  :return: pandas.Dataframe
+  Args:
+      tbname (str): name of data table
+      ind_col_name (str or int): numeric id of column or column name
+  Return: pandas.Dataframe
   """
-  
   df = None # set a global variable to store the dataframe
   apikey = 'K35wHcKuwXuhHTaz7zY42rCje'
   parameters = {"apikey": apikey, 'table': tbname }
   heads = { "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:60.0) Gecko/20100101 Firefox/60.0" } # server has ModSecurity check if it is a browser request. 
   js = {'error': 'Initialize' }
 
   try:
```

### Comparing `rfit-0.2.20230120/src/rfit/learn/boundary_plots.py` & `rfit-0.3.20230711/src/rfit/learn/boundary_plots.py`

 * *Files identical despite different names*

### Comparing `rfit-0.2.20230120/src/rfit.egg-info/PKG-INFO` & `rfit-0.3.20230711/src/rfit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rfit
-Version: 0.2.20230120
+Version: 0.3.20230711
 Summary: GWU Data Science python class helper functions
 Home-page: https://github.com/physicsland/rfitapi
 Author: Edwin Lo
 Author-email: elo@regression.fit
 Project-URL: Bug Tracker, https://github.com/physicsland/rfitapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Regression.fit api
 
-Last updated: 2022-06-01
+Last updated: 2023-07-11
 
 This package (rfit - regression.fit) is for use at The George Washington University Data Science program. There are some useful and convenient functions we use in our python classes. 
 
 One of them is dfapi, which connects to the api.regression.fit endpoint, to load dataframes used in our classes.
```

