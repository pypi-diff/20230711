# Comparing `tmp/vulcan-annotation-2.6.1.tar.gz` & `tmp/vulcan-annotation-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-annotation-2.6.1.tar", last modified: Tue Jul 11 13:19:19 2023, max compression
+gzip compressed data, was "vulcan-annotation-2.6.2.tar", last modified: Tue Jul 11 13:20:57 2023, max compression
```

## Comparing `vulcan-annotation-2.6.1.tar` & `vulcan-annotation-2.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 13:19:19.321672 vulcan-annotation-2.6.1/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-16 05:10:40.000000 vulcan-annotation-2.6.1/LICENSE
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      806 2023-07-11 13:19:19.321672 vulcan-annotation-2.6.1/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      328 2023-07-11 12:57:40.000000 vulcan-annotation-2.6.1/README.md
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-11 13:19:19.321672 vulcan-annotation-2.6.1/setup.cfg
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      843 2023-07-11 13:19:06.000000 vulcan-annotation-2.6.1/setup.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 13:19:19.321672 vulcan-annotation-2.6.1/vulcan_annotation/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       33 2023-07-11 13:18:59.000000 vulcan-annotation-2.6.1/vulcan_annotation/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     4288 2023-07-11 13:03:11.000000 vulcan-annotation-2.6.1/vulcan_annotation/annotation.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 13:19:19.321672 vulcan-annotation-2.6.1/vulcan_annotation.egg-info/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      806 2023-07-11 13:19:19.000000 vulcan-annotation-2.6.1/vulcan_annotation.egg-info/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      292 2023-07-11 13:19:19.000000 vulcan-annotation-2.6.1/vulcan_annotation.egg-info/SOURCES.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-11 13:19:19.000000 vulcan-annotation-2.6.1/vulcan_annotation.egg-info/dependency_links.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       10 2023-07-11 13:19:19.000000 vulcan-annotation-2.6.1/vulcan_annotation.egg-info/requires.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       18 2023-07-11 13:19:19.000000 vulcan-annotation-2.6.1/vulcan_annotation.egg-info/top_level.txt
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 13:20:57.430375 vulcan-annotation-2.6.2/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-16 05:10:40.000000 vulcan-annotation-2.6.2/LICENSE
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      806 2023-07-11 13:20:57.430375 vulcan-annotation-2.6.2/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      328 2023-07-11 12:57:40.000000 vulcan-annotation-2.6.2/README.md
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-11 13:20:57.430375 vulcan-annotation-2.6.2/setup.cfg
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      843 2023-07-11 13:20:43.000000 vulcan-annotation-2.6.2/setup.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 13:20:57.430375 vulcan-annotation-2.6.2/vulcan_annotation/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       34 2023-07-11 13:20:33.000000 vulcan-annotation-2.6.2/vulcan_annotation/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     4288 2023-07-11 13:03:11.000000 vulcan-annotation-2.6.2/vulcan_annotation/annotation.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 13:20:57.430375 vulcan-annotation-2.6.2/vulcan_annotation.egg-info/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      806 2023-07-11 13:20:57.000000 vulcan-annotation-2.6.2/vulcan_annotation.egg-info/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      292 2023-07-11 13:20:57.000000 vulcan-annotation-2.6.2/vulcan_annotation.egg-info/SOURCES.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-11 13:20:57.000000 vulcan-annotation-2.6.2/vulcan_annotation.egg-info/dependency_links.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       10 2023-07-11 13:20:57.000000 vulcan-annotation-2.6.2/vulcan_annotation.egg-info/requires.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       18 2023-07-11 13:20:57.000000 vulcan-annotation-2.6.2/vulcan_annotation.egg-info/top_level.txt
```

### Comparing `vulcan-annotation-2.6.1/LICENSE` & `vulcan-annotation-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-annotation-2.6.1/PKG-INFO` & `vulcan-annotation-2.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-annotation
-Version: 2.6.1
+Version: 2.6.2
 Summary: Vulcan annotation for structured data.
 Home-page: https://github.com/vulcan-coalition/vulcan_annotation
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-annotation-2.6.1/setup.py` & `vulcan-annotation-2.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vulcan-annotation",
-    version="2.6.1",
+    version="2.6.2",
     author="Chatavut Viriyasuthee",
     author_email="chatavut@lab.ai",
     description="Vulcan annotation for structured data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vulcan-coalition/vulcan_annotation",
     packages=["vulcan_annotation"],
```

### Comparing `vulcan-annotation-2.6.1/vulcan_annotation/annotation.py` & `vulcan-annotation-2.6.2/vulcan_annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `vulcan-annotation-2.6.1/vulcan_annotation.egg-info/PKG-INFO` & `vulcan-annotation-2.6.2/vulcan_annotation.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-annotation
-Version: 2.6.1
+Version: 2.6.2
 Summary: Vulcan annotation for structured data.
 Home-page: https://github.com/vulcan-coalition/vulcan_annotation
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

