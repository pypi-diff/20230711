# Comparing `tmp/idbadapter-1.5.tar.gz` & `tmp/idbadapter-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.5.tar", last modified: Wed Jun  7 15:10:51 2023, max compression
+gzip compressed data, was "idbadapter-1.6.tar", last modified: Tue Jul 11 12:54:46 2023, max compression
```

## Comparing `idbadapter-1.5.tar` & `idbadapter-1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:10:51.049651 idbadapter-1.5/
--rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.5/LICENSE
--rw-rw-rw-   0        0        0      695 2023-06-07 15:10:51.049651 idbadapter-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 15:10:51.025650 idbadapter-1.5/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.5/idbadapter/__init__.py
--rw-rw-rw-   0        0        0     7801 2023-06-07 14:57:59.000000 idbadapter-1.5/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:10:51.047680 idbadapter-1.5/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 15:10:51.051647 idbadapter-1.5/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-07 15:08:05.000000 idbadapter-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:54:46.211832 idbadapter-1.6/
+-rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.6/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-07-11 12:54:46.212832 idbadapter-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 12:54:46.183736 idbadapter-1.6/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.6/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    11984 2023-07-06 12:00:25.000000 idbadapter-1.6/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:54:46.210829 idbadapter-1.6/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-11 12:54:46.000000 idbadapter-1.6/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:54:46.215842 idbadapter-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-11 12:54:42.000000 idbadapter-1.6/setup.py
```

### Comparing `idbadapter-1.5/LICENSE` & `idbadapter-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.5/PKG-INFO` & `idbadapter-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.5
+Version: 1.6
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.5/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.6/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.5
+Version: 1.6
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.5/setup.py` & `idbadapter-1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.3'
+version = '1.6'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.5',
+      version='1.6',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

