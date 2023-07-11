# Comparing `tmp/dummy_url_wrapper-0.0.1.tar.gz` & `tmp/dummy_url_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dummy_url_wrapper-0.0.1.tar", last modified: Tue Jul 11 08:21:32 2023, max compression
+gzip compressed data, was "dummy_url_wrapper-0.0.2.tar", last modified: Tue Jul 11 12:03:34 2023, max compression
```

## Comparing `dummy_url_wrapper-0.0.1.tar` & `dummy_url_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 08:21:32.151238 dummy_url_wrapper-0.0.1/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-11 08:21:32.151238 dummy_url_wrapper-0.0.1/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 08:21:32.151238 dummy_url_wrapper-0.0.1/dummy_url_wrapper/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       67 2023-07-11 04:13:41.000000 dummy_url_wrapper-0.0.1/dummy_url_wrapper/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      746 2023-07-11 08:20:33.000000 dummy_url_wrapper-0.0.1/dummy_url_wrapper/mysdk.py
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 08:21:32.151238 dummy_url_wrapper-0.0.1/dummy_url_wrapper.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-11 08:21:32.000000 dummy_url_wrapper-0.0.1/dummy_url_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      229 2023-07-11 08:21:32.000000 dummy_url_wrapper-0.0.1/dummy_url_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-11 08:21:32.000000 dummy_url_wrapper-0.0.1/dummy_url_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-11 08:21:32.000000 dummy_url_wrapper-0.0.1/dummy_url_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-11 08:21:32.151238 dummy_url_wrapper-0.0.1/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      834 2023-07-11 07:02:40.000000 dummy_url_wrapper-0.0.1/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 12:03:34.192074 dummy_url_wrapper-0.0.2/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-11 12:03:34.192074 dummy_url_wrapper-0.0.2/PKG-INFO
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 12:03:34.192074 dummy_url_wrapper-0.0.2/dummy_url_wrapper/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       67 2023-07-11 04:13:41.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      746 2023-07-11 08:20:33.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper/mysdk.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 12:03:34.192074 dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-11 12:03:34.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-11 12:03:34.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-11 12:03:34.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       23 2023-07-11 12:03:34.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-11 12:03:34.000000 dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-11 12:03:34.192074 dummy_url_wrapper-0.0.2/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      886 2023-07-11 12:03:17.000000 dummy_url_wrapper-0.0.2/setup.py
```

### Comparing `dummy_url_wrapper-0.0.1/PKG-INFO` & `dummy_url_wrapper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy_url_wrapper
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

### Comparing `dummy_url_wrapper-0.0.1/dummy_url_wrapper/mysdk.py` & `dummy_url_wrapper-0.0.2/dummy_url_wrapper/mysdk.py`

 * *Files identical despite different names*

### Comparing `dummy_url_wrapper-0.0.1/dummy_url_wrapper.egg-info/PKG-INFO` & `dummy_url_wrapper-0.0.2/dummy_url_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy-url-wrapper
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

### Comparing `dummy_url_wrapper-0.0.1/setup.py` & `dummy_url_wrapper-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dummy_url_wrapper",
-    version="0.0.1",
+    version="0.0.2",
     description="This package provides the wrapping of URLs for not exposing to clients",
     url="https://github.com/nk2909/Python-SDK.git",
     author="Nishant Kabariya",
     author_email="testurl@yopmail.com",
+    install_requires=["python-dotenv", "requests"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
```

