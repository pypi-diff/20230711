# Comparing `tmp/idbadapter-1.6.tar.gz` & `tmp/idbadapter-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.6.tar", last modified: Tue Jul 11 12:54:46 2023, max compression
+gzip compressed data, was "idbadapter-1.7.tar", last modified: Tue Jul 11 13:07:02 2023, max compression
```

## Comparing `idbadapter-1.6.tar` & `idbadapter-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:54:46.211832 idbadapter-1.6/
--rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.6/LICENSE
--rw-rw-rw-   0        0        0      695 2023-07-11 12:54:46.212832 idbadapter-1.6/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 12:54:46.183736 idbadapter-1.6/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.6/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    11984 2023-07-06 12:00:25.000000 idbadapter-1.6/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:54:46.210829 idbadapter-1.6/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 12:54:46.215842 idbadapter-1.6/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-07-11 12:54:42.000000 idbadapter-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:07:02.060124 idbadapter-1.7/
+-rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.7/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-07-11 13:07:02.060124 idbadapter-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 13:07:02.029022 idbadapter-1.7/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.7/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    11984 2023-07-06 12:00:25.000000 idbadapter-1.7/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:07:02.054106 idbadapter-1.7/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:07:02.062131 idbadapter-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-11 13:06:56.000000 idbadapter-1.7/setup.py
```

### Comparing `idbadapter-1.6/LICENSE` & `idbadapter-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.6/PKG-INFO` & `idbadapter-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.6
+Version: 1.7
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.6/idbadapter/schedule_loader.py` & `idbadapter-1.7/idbadapter/schedule_loader.py`

 * *Files identical despite different names*

### Comparing `idbadapter-1.6/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.7/idbadapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.6
+Version: 1.7
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.6/setup.py` & `idbadapter-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.6'
+version = '1.7'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.6',
+      version='1.7',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

