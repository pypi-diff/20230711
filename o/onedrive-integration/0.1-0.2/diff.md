# Comparing `tmp/onedrive_integration-0.1.tar.gz` & `tmp/onedrive_integration-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedrive_integration-0.1.tar", last modified: Mon Jul 10 23:13:58 2023, max compression
+gzip compressed data, was "onedrive_integration-0.2.tar", last modified: Mon Jul 10 23:29:51 2023, max compression
```

## Comparing `onedrive_integration-0.1.tar` & `onedrive_integration-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-10 23:13:58.195038 onedrive_integration-0.1/
--rw-r--r--   0 william2399   (501) staff       (20)      116 2023-07-10 23:13:58.194615 onedrive_integration-0.1/PKG-INFO
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-10 23:13:58.177178 onedrive_integration-0.1/onedrive_integration/
--rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedrive_integration-0.1/onedrive_integration/__init__.py
--rw-r--r--   0 william2399   (501) staff       (20)     1625 2023-07-06 03:10:57.000000 onedrive_integration-0.1/onedrive_integration/ms_graph.py
--rw-r--r--   0 william2399   (501) staff       (20)     2375 2023-07-10 21:54:31.000000 onedrive_integration-0.1/onedrive_integration/onedrive_api.py
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-10 23:13:58.193912 onedrive_integration-0.1/onedrive_integration.egg-info/
--rw-r--r--   0 william2399   (501) staff       (20)      116 2023-07-10 23:13:57.000000 onedrive_integration-0.1/onedrive_integration.egg-info/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)      330 2023-07-10 23:13:57.000000 onedrive_integration-0.1/onedrive_integration.egg-info/SOURCES.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-10 23:13:57.000000 onedrive_integration-0.1/onedrive_integration.egg-info/dependency_links.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-10 21:38:22.000000 onedrive_integration-0.1/onedrive_integration.egg-info/not-zip-safe
--rw-r--r--   0 william2399   (501) staff       (20)       21 2023-07-10 23:13:57.000000 onedrive_integration-0.1/onedrive_integration.egg-info/top_level.txt
--rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-10 23:13:58.195196 onedrive_integration-0.1/setup.cfg
--rw-r--r--   0 william2399   (501) staff       (20)      222 2023-07-10 21:38:17.000000 onedrive_integration-0.1/setup.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-10 23:29:51.959409 onedrive_integration-0.2/
+-rw-r--r--   0 william2399   (501) staff       (20)      141 2023-07-10 23:29:51.959016 onedrive_integration-0.2/PKG-INFO
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-10 23:29:51.949243 onedrive_integration-0.2/onedrive_integration/
+-rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedrive_integration-0.2/onedrive_integration/__init__.py
+-rw-r--r--   0 william2399   (501) staff       (20)     1625 2023-07-06 03:10:57.000000 onedrive_integration-0.2/onedrive_integration/ms_graph.py
+-rw-r--r--   0 william2399   (501) staff       (20)     2375 2023-07-10 21:54:31.000000 onedrive_integration-0.2/onedrive_integration/onedrive_api.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-10 23:29:51.958402 onedrive_integration-0.2/onedrive_integration.egg-info/
+-rw-r--r--   0 william2399   (501) staff       (20)      141 2023-07-10 23:29:51.000000 onedrive_integration-0.2/onedrive_integration.egg-info/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)      330 2023-07-10 23:29:51.000000 onedrive_integration-0.2/onedrive_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-10 23:29:51.000000 onedrive_integration-0.2/onedrive_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-10 21:38:22.000000 onedrive_integration-0.2/onedrive_integration.egg-info/not-zip-safe
+-rw-r--r--   0 william2399   (501) staff       (20)       21 2023-07-10 23:29:51.000000 onedrive_integration-0.2/onedrive_integration.egg-info/top_level.txt
+-rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-10 23:29:51.959569 onedrive_integration-0.2/setup.cfg
+-rw-r--r--   0 william2399   (501) staff       (20)      263 2023-07-10 23:29:48.000000 onedrive_integration-0.2/setup.py
```

### Comparing `onedrive_integration-0.1/onedrive_integration/ms_graph.py` & `onedrive_integration-0.2/onedrive_integration/ms_graph.py`

 * *Files identical despite different names*

### Comparing `onedrive_integration-0.1/onedrive_integration/onedrive_api.py` & `onedrive_integration-0.2/onedrive_integration/onedrive_api.py`

 * *Files identical despite different names*

