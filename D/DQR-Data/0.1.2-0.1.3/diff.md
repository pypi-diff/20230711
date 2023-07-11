# Comparing `tmp/DQR_Data-0.1.2.tar.gz` & `tmp/DQR_Data-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DQR_Data-0.1.2.tar", last modified: Tue Jul 11 14:40:20 2023, max compression
+gzip compressed data, was "DQR_Data-0.1.3.tar", last modified: Tue Jul 11 14:43:01 2023, max compression
```

## Comparing `DQR_Data-0.1.2.tar` & `DQR_Data-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 14:40:20.162459 DQR_Data-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-11 14:40:20.103057 DQR_Data-0.1.2/DQR_Data/
--rw-rw-rw-   0        0        0       34 2023-07-11 10:38:04.000000 DQR_Data-0.1.2/DQR_Data/__init__.py
--rw-rw-rw-   0        0        0      294 2023-07-11 10:38:04.000000 DQR_Data-0.1.2/DQR_Data/example.py
--rw-rw-rw-   0        0        0      548 2023-07-11 10:38:04.000000 DQR_Data-0.1.2/DQR_Data/main.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:40:20.161958 DQR_Data-0.1.2/DQR_Data.egg-info/
--rw-rw-rw-   0        0        0     5861 2023-07-11 14:40:19.000000 DQR_Data-0.1.2/DQR_Data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-11 14:40:19.000000 DQR_Data-0.1.2/DQR_Data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 14:40:19.000000 DQR_Data-0.1.2/DQR_Data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-11 14:40:19.000000 DQR_Data-0.1.2/DQR_Data.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 14:40:19.000000 DQR_Data-0.1.2/DQR_Data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5861 2023-07-11 14:40:20.162459 DQR_Data-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-07-11 14:40:20.169258 DQR_Data-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      775 2023-07-11 14:39:04.000000 DQR_Data-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:43:01.798662 DQR_Data-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-11 14:43:01.764225 DQR_Data-0.1.3/DQR_Data/
+-rw-rw-rw-   0        0        0       34 2023-07-11 10:38:04.000000 DQR_Data-0.1.3/DQR_Data/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-07-11 10:38:04.000000 DQR_Data-0.1.3/DQR_Data/example.py
+-rw-rw-rw-   0        0        0      548 2023-07-11 10:38:04.000000 DQR_Data-0.1.3/DQR_Data/main.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:43:01.796624 DQR_Data-0.1.3/DQR_Data.egg-info/
+-rw-rw-rw-   0        0        0      360 2023-07-11 14:43:01.000000 DQR_Data-0.1.3/DQR_Data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-11 14:43:01.000000 DQR_Data-0.1.3/DQR_Data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:43:01.000000 DQR_Data-0.1.3/DQR_Data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-11 14:43:01.000000 DQR_Data-0.1.3/DQR_Data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 14:43:01.000000 DQR_Data-0.1.3/DQR_Data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      360 2023-07-11 14:43:01.799162 DQR_Data-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-07-11 14:43:01.802470 DQR_Data-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-11 14:42:39.000000 DQR_Data-0.1.3/setup.py
```

### Comparing `DQR_Data-0.1.2/DQR_Data/main.py` & `DQR_Data-0.1.3/DQR_Data/main.py`

 * *Files identical despite different names*

### Comparing `DQR_Data-0.1.2/setup.py` & `DQR_Data-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 
 from setuptools import setup
-with open("Readme.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()  
+
 setup(
     name='DQR_Data',
-    version='0.1.2',
+    version='0.1.3',
     description='A python library for cryptocurrency trading for Binance and Deribit',
-    long_description=long_description,    
-    long_description_content_type="text/markdown",
     author='DAOQuantResearch',
     author_email='DQR-contact@proton.me',
     packages=['DQR_Data'],
     url="https://github.com/DAOQuantResearch/data_package/tree/release_v1",
     project_urls={
         'Source': 'https://github.com/DAOQuantResearch/data_package/tree/release_v1',
     },
```

