# Comparing `tmp/card91_python_package-0.0.1.tar.gz` & `tmp/card91_python_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "card91_python_package-0.0.1.tar", last modified: Mon Jul 10 12:16:20 2023, max compression
+gzip compressed data, was "card91_python_package-0.0.2.tar", last modified: Tue Jul 11 04:42:53 2023, max compression
```

## Comparing `card91_python_package-0.0.1.tar` & `card91_python_package-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-10 12:16:20.106182 card91_python_package-0.0.1/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      718 2023-07-10 12:16:20.102182 card91_python_package-0.0.1/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-10 12:16:20.102182 card91_python_package-0.0.1/card91_python_package/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       34 2023-07-10 12:07:47.000000 card91_python_package-0.0.1/card91_python_package/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       69 2023-07-10 11:30:50.000000 card91_python_package-0.0.1/card91_python_package/mysdk.py
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-10 12:16:20.102182 card91_python_package-0.0.1/card91_python_package.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      718 2023-07-10 12:16:20.000000 card91_python_package-0.0.1/card91_python_package.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      253 2023-07-10 12:16:20.000000 card91_python_package-0.0.1/card91_python_package.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-10 12:16:20.000000 card91_python_package-0.0.1/card91_python_package.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       22 2023-07-10 12:16:20.000000 card91_python_package-0.0.1/card91_python_package.egg-info/top_level.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-10 12:16:20.106182 card91_python_package-0.0.1/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      838 2023-07-10 12:16:16.000000 card91_python_package-0.0.1/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 04:42:53.811553 card91_python_package-0.0.2/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      718 2023-07-11 04:42:53.811553 card91_python_package-0.0.2/PKG-INFO
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 04:42:53.807553 card91_python_package-0.0.2/card91_python_package/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       67 2023-07-11 04:13:41.000000 card91_python_package-0.0.2/card91_python_package/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       69 2023-07-10 11:30:50.000000 card91_python_package-0.0.2/card91_python_package/mysdk.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 04:42:53.811553 card91_python_package-0.0.2/card91_python_package.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      718 2023-07-11 04:42:53.000000 card91_python_package-0.0.2/card91_python_package.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      253 2023-07-11 04:42:53.000000 card91_python_package-0.0.2/card91_python_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-11 04:42:53.000000 card91_python_package-0.0.2/card91_python_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       22 2023-07-11 04:42:53.000000 card91_python_package-0.0.2/card91_python_package.egg-info/top_level.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-11 04:42:53.811553 card91_python_package-0.0.2/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      838 2023-07-11 04:42:27.000000 card91_python_package-0.0.2/setup.py
```

### Comparing `card91_python_package-0.0.1/PKG-INFO` & `card91_python_package-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: card91_python_package
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package provides the wrapping of URLs for not exposing to clients
 Home-page: https://github.com/nk2909/Python-SDK.git
 Author: Nishant Kabariya
 Author-email: testurl@yopmail.com
 Keywords: python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `card91_python_package-0.0.1/card91_python_package.egg-info/PKG-INFO` & `card91_python_package-0.0.2/card91_python_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: card91-python-package
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package provides the wrapping of URLs for not exposing to clients
 Home-page: https://github.com/nk2909/Python-SDK.git
 Author: Nishant Kabariya
 Author-email: testurl@yopmail.com
 Keywords: python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `card91_python_package-0.0.1/setup.py` & `card91_python_package-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="card91_python_package",
-    version="0.0.1",
+    version="0.0.2",
     description="This package provides the wrapping of URLs for not exposing to clients",
     url="https://github.com/nk2909/Python-SDK.git",
     author="Nishant Kabariya",
     author_email="testurl@yopmail.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
```

