# Comparing `tmp/rfit-0.3.20230711.tar.gz` & `tmp/rfit-0.3.20230712.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfit-0.3.20230711.tar", last modified: Tue Jul 11 13:52:20 2023, max compression
+gzip compressed data, was "rfit-0.3.20230712.tar", last modified: Tue Jul 11 14:31:30 2023, max compression
```

## Comparing `rfit-0.3.20230711.tar` & `rfit-0.3.20230712.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.279638 rfit-0.3.20230711/
--rw-r--r--   0 elo        (503) staff       (20)     1065 2022-06-01 20:20:03.000000 rfit-0.3.20230711/LICENSE
--rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 13:52:20.279779 rfit-0.3.20230711/PKG-INFO
--rw-r--r--   0 elo        (503) staff       (20)      346 2023-07-11 13:51:01.000000 rfit-0.3.20230711/README.md
--rw-r--r--   0 elo        (503) staff       (20)       84 2022-06-01 20:20:03.000000 rfit-0.3.20230711/pyproject.toml
--rw-r--r--   0 elo        (503) staff       (20)      697 2023-07-11 13:52:20.280427 rfit-0.3.20230711/setup.cfg
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.272077 rfit-0.3.20230711/src/
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.274872 rfit-0.3.20230711/src/rfit/
--rw-r--r--   0 elo        (503) staff       (20)      363 2022-06-01 20:20:03.000000 rfit-0.3.20230711/src/rfit/__init__.py
--rw-r--r--   0 elo        (503) staff       (20)     2225 2023-07-11 13:40:13.000000 rfit-0.3.20230711/src/rfit/api.py
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.279055 rfit-0.3.20230711/src/rfit/learn/
--rw-r--r--   0 elo        (503) staff       (20)      304 2022-06-01 20:20:03.000000 rfit-0.3.20230711/src/rfit/learn/__init__.py
--rwxr-xr-x   0 elo        (503) staff       (20)     4749 2022-06-01 20:20:03.000000 rfit-0.3.20230711/src/rfit/learn/boundary_plots.py
--rwxr-xr-x   0 elo        (503) staff       (20)     1412 2023-07-11 13:42:41.000000 rfit-0.3.20230711/src/rfit/learn/helper.py
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 13:52:20.277379 rfit-0.3.20230711/src/rfit.egg-info/
--rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/PKG-INFO
--rw-r--r--   0 elo        (503) staff       (20)      323 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/SOURCES.txt
--rw-r--r--   0 elo        (503) staff       (20)        1 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/dependency_links.txt
--rw-r--r--   0 elo        (503) staff       (20)       33 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/requires.txt
--rw-r--r--   0 elo        (503) staff       (20)        5 2023-07-11 13:52:20.000000 rfit-0.3.20230711/src/rfit.egg-info/top_level.txt
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.338324 rfit-0.3.20230712/
+-rw-r--r--   0 elo        (503) staff       (20)     1065 2023-07-11 14:19:49.000000 rfit-0.3.20230712/LICENSE
+-rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 14:31:30.338467 rfit-0.3.20230712/PKG-INFO
+-rw-r--r--   0 elo        (503) staff       (20)      346 2023-07-11 14:30:33.000000 rfit-0.3.20230712/README.md
+-rw-r--r--   0 elo        (503) staff       (20)       84 2023-07-11 14:19:49.000000 rfit-0.3.20230712/pyproject.toml
+-rw-r--r--   0 elo        (503) staff       (20)      697 2023-07-11 14:31:30.339106 rfit-0.3.20230712/setup.cfg
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.331164 rfit-0.3.20230712/src/
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.334062 rfit-0.3.20230712/src/rfit/
+-rw-r--r--   0 elo        (503) staff       (20)      363 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/__init__.py
+-rw-r--r--   0 elo        (503) staff       (20)     2225 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/api.py
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.337710 rfit-0.3.20230712/src/rfit/learn/
+-rw-r--r--   0 elo        (503) staff       (20)      304 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/learn/__init__.py
+-rwxr-xr-x   0 elo        (503) staff       (20)     4749 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/learn/boundary_plots.py
+-rwxr-xr-x   0 elo        (503) staff       (20)     1432 2023-07-11 14:29:18.000000 rfit-0.3.20230712/src/rfit/learn/helper.py
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.336462 rfit-0.3.20230712/src/rfit.egg-info/
+-rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/PKG-INFO
+-rw-r--r--   0 elo        (503) staff       (20)      323 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/SOURCES.txt
+-rw-r--r--   0 elo        (503) staff       (20)        1 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/dependency_links.txt
+-rw-r--r--   0 elo        (503) staff       (20)       33 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/requires.txt
+-rw-r--r--   0 elo        (503) staff       (20)        5 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/top_level.txt
```

### Comparing `rfit-0.3.20230711/LICENSE` & `rfit-0.3.20230712/LICENSE`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230711/PKG-INFO` & `rfit-0.3.20230712/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rfit
-Version: 0.3.20230711
+Version: 0.3.20230712
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
 
-Last updated: 2023-07-11
+Last updated: 2023-07-12
 
 This package (rfit - regression.fit) is for use at The George Washington University Data Science program. There are some useful and convenient functions we use in our python classes. 
 
 One of them is dfapi, which connects to the api.regression.fit endpoint, to load dataframes used in our classes.
```

### Comparing `rfit-0.3.20230711/setup.cfg` & `rfit-0.3.20230712/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rfit
-version = 0.3.20230711
+version = 0.3.20230712
 author = Edwin Lo
 author_email = elo@regression.fit
 description = GWU Data Science python class helper functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/physicsland/rfitapi
 project_urls =
```

### Comparing `rfit-0.3.20230711/src/rfit/api.py` & `rfit-0.3.20230712/src/rfit/api.py`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230711/src/rfit/learn/boundary_plots.py` & `rfit-0.3.20230712/src/rfit/learn/boundary_plots.py`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230711/src/rfit/learn/helper.py` & `rfit-0.3.20230712/src/rfit/learn/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
       valCnt (bool): value_count option, defaults to False
   Return: None
   """
   cnt = 1
   print('\ndataframe Basic Check function -')
   
   if (chkNull):
-    print(f'Null values: {dframe.isnull().sum().sort_values(ascending=False)}')
+    print(f'\n{cnt}: Null values:')
     cnt+=1
+    print( dframe.isnull().sum().sort_values(ascending=False) )
   
   if (info):
     try:
       print(f'\n{cnt}: info(): ')
       cnt+=1
       print(dframe.info())
     except: pass
```

### Comparing `rfit-0.3.20230711/src/rfit.egg-info/PKG-INFO` & `rfit-0.3.20230712/src/rfit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rfit
-Version: 0.3.20230711
+Version: 0.3.20230712
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
 
-Last updated: 2023-07-11
+Last updated: 2023-07-12
 
 This package (rfit - regression.fit) is for use at The George Washington University Data Science program. There are some useful and convenient functions we use in our python classes. 
 
 One of them is dfapi, which connects to the api.regression.fit endpoint, to load dataframes used in our classes.
```

