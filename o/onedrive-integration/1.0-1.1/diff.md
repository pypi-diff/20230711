# Comparing `tmp/onedrive-integration-1.0.tar.gz` & `tmp/onedrive-integration-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedrive-integration-1.0.tar", last modified: Tue Jul 11 00:39:33 2023, max compression
+gzip compressed data, was "onedrive-integration-1.1.tar", last modified: Tue Jul 11 00:41:02 2023, max compression
```

## Comparing `onedrive-integration-1.0.tar` & `onedrive-integration-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 00:39:33.338674 onedrive-integration-1.0/
--rw-r--r--   0 william2399   (501) staff       (20)      485 2023-07-11 00:39:33.338249 onedrive-integration-1.0/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)      303 2023-07-11 00:39:16.000000 onedrive-integration-1.0/README.md
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 00:39:33.330337 onedrive-integration-1.0/onedrive-integration/
--rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedrive-integration-1.0/onedrive-integration/__init__.py
--rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 00:16:53.000000 onedrive-integration-1.0/onedrive-integration/ms_graph.py
--rw-r--r--   0 william2399   (501) staff       (20)     2375 2023-07-10 21:54:31.000000 onedrive-integration-1.0/onedrive-integration/onedrive_api.py
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 00:39:33.337531 onedrive-integration-1.0/onedrive_integration.egg-info/
--rw-r--r--   0 william2399   (501) staff       (20)      485 2023-07-11 00:39:33.000000 onedrive-integration-1.0/onedrive_integration.egg-info/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)      340 2023-07-11 00:39:33.000000 onedrive-integration-1.0/onedrive_integration.egg-info/SOURCES.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 00:39:33.000000 onedrive-integration-1.0/onedrive_integration.egg-info/dependency_links.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 00:39:33.000000 onedrive-integration-1.0/onedrive_integration.egg-info/not-zip-safe
--rw-r--r--   0 william2399   (501) staff       (20)       21 2023-07-11 00:39:33.000000 onedrive-integration-1.0/onedrive_integration.egg-info/top_level.txt
--rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 00:39:33.338818 onedrive-integration-1.0/setup.cfg
--rw-r--r--   0 william2399   (501) staff       (20)      518 2023-07-11 00:39:27.000000 onedrive-integration-1.0/setup.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 00:41:02.788207 onedrive-integration-1.1/
+-rw-r--r--   0 william2399   (501) staff       (20)      485 2023-07-11 00:41:02.787685 onedrive-integration-1.1/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)      303 2023-07-11 00:40:51.000000 onedrive-integration-1.1/README.md
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 00:41:02.778945 onedrive-integration-1.1/onedrive-integration/
+-rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedrive-integration-1.1/onedrive-integration/__init__.py
+-rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 00:16:53.000000 onedrive-integration-1.1/onedrive-integration/ms_graph.py
+-rw-r--r--   0 william2399   (501) staff       (20)     2375 2023-07-10 21:54:31.000000 onedrive-integration-1.1/onedrive-integration/onedrive_api.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 00:41:02.787005 onedrive-integration-1.1/onedrive_integration.egg-info/
+-rw-r--r--   0 william2399   (501) staff       (20)      485 2023-07-11 00:41:02.000000 onedrive-integration-1.1/onedrive_integration.egg-info/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)      340 2023-07-11 00:41:02.000000 onedrive-integration-1.1/onedrive_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 00:41:02.000000 onedrive-integration-1.1/onedrive_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 00:39:33.000000 onedrive-integration-1.1/onedrive_integration.egg-info/not-zip-safe
+-rw-r--r--   0 william2399   (501) staff       (20)       21 2023-07-11 00:41:02.000000 onedrive-integration-1.1/onedrive_integration.egg-info/top_level.txt
+-rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 00:41:02.788362 onedrive-integration-1.1/setup.cfg
+-rw-r--r--   0 william2399   (501) staff       (20)      518 2023-07-11 00:40:57.000000 onedrive-integration-1.1/setup.py
```

### Comparing `onedrive-integration-1.0/onedrive-integration/ms_graph.py` & `onedrive-integration-1.1/onedrive-integration/ms_graph.py`

 * *Files identical despite different names*

### Comparing `onedrive-integration-1.0/onedrive-integration/onedrive_api.py` & `onedrive-integration-1.1/onedrive-integration/onedrive_api.py`

 * *Files identical despite different names*

### Comparing `onedrive-integration-1.0/setup.py` & `onedrive-integration-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Read contents of README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
       name='onedrive-integration',
-      version='1.0',
+      version='1.1',
       long_description=long_description,
       long_description_content_type='text/markdown',
       description='Package for OneDrive File Management',
       author='William Guo',
       license='MIT',
       packages=['onedrive-integration'],
       zip_safe=False
```

