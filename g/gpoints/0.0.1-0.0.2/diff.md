# Comparing `tmp/gpoints-0.0.1.tar.gz` & `tmp/gpoints-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpoints-0.0.1.tar", last modified: Tue Jul 11 21:09:50 2023, max compression
+gzip compressed data, was "gpoints-0.0.2.tar", last modified: Tue Jul 11 21:40:46 2023, max compression
```

## Comparing `gpoints-0.0.1.tar` & `gpoints-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 21:09:50.191054 gpoints-0.0.1/
--rw-rw-rw-   0        0        0      676 2023-07-11 21:09:50.175416 gpoints-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 21:09:50.159786 gpoints-0.0.1/gpoints/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 gpoints-0.0.1/gpoints/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-07-11 21:09:00.000000 gpoints-0.0.1/gpoints/graph_points.py
-drwxrwxrwx   0        0        0        0 2023-07-11 21:09:50.175416 gpoints-0.0.1/gpoints.egg-info/
--rw-rw-rw-   0        0        0      676 2023-07-11 21:09:50.000000 gpoints-0.0.1/gpoints.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-07-11 21:09:50.000000 gpoints-0.0.1/gpoints.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 21:09:50.000000 gpoints-0.0.1/gpoints.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 21:09:50.000000 gpoints-0.0.1/gpoints.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 21:09:50.191054 gpoints-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-07-11 21:08:40.000000 gpoints-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 21:40:46.556581 gpoints-0.0.2/
+-rw-rw-rw-   0        0        0      665 2023-07-11 21:40:46.556581 gpoints-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 21:40:46.516997 gpoints-0.0.2/gpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 gpoints-0.0.2/gpoints/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-07-11 21:09:00.000000 gpoints-0.0.2/gpoints/graph_points.py
+drwxrwxrwx   0        0        0        0 2023-07-11 21:40:46.556581 gpoints-0.0.2/gpoints.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-07-11 21:40:46.000000 gpoints-0.0.2/gpoints.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-07-11 21:40:46.000000 gpoints-0.0.2/gpoints.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 21:40:46.000000 gpoints-0.0.2/gpoints.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 21:40:46.000000 gpoints-0.0.2/gpoints.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 21:40:46.556581 gpoints-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-11 21:39:54.000000 gpoints-0.0.2/setup.py
```

### Comparing `gpoints-0.0.1/PKG-INFO` & `gpoints-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gpoints
-Version: 0.0.1
+Version: 0.0.2
 Summary: From graph Image as input, get corresponding points
 Author: Ujjawal Kumar (India)
 Author-email: <kumarujjawal3621@gmail.com>
-Keywords: python,video,stream,video stream,camera stream,sockets
+Keywords: python,points,stock price,Image,numpy array
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `gpoints-0.0.1/gpoints/graph_points.py` & `gpoints-0.0.2/gpoints/graph_points.py`

 * *Files identical despite different names*

### Comparing `gpoints-0.0.1/gpoints.egg-info/PKG-INFO` & `gpoints-0.0.2/gpoints.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gpoints
-Version: 0.0.1
+Version: 0.0.2
 Summary: From graph Image as input, get corresponding points
 Author: Ujjawal Kumar (India)
 Author-email: <kumarujjawal3621@gmail.com>
-Keywords: python,video,stream,video stream,camera stream,sockets
+Keywords: python,points,stock price,Image,numpy array
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `gpoints-0.0.1/setup.py` & `gpoints-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'From graph Image as input, get corresponding points'
 LONG_DESCRIPTION = '4 argumnents: 1.Path to image 2.Range of horizontal value 3.Range of vertical value 4. 0/1'
 # Setting up
 
 setup(
     name="gpoints",
     version=VERSION,
     author="Ujjawal Kumar (India)",
     author_email="<kumarujjawal3621@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
+    keywords=['python', 'points', 'stock price', 'Image', 'numpy array'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

