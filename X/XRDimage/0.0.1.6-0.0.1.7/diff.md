# Comparing `tmp/XRDimage-0.0.1.6.tar.gz` & `tmp/XRDimage-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XRDimage-0.0.1.6.tar", last modified: Tue Jul 11 18:20:44 2023, max compression
+gzip compressed data, was "XRDimage-0.0.1.7.tar", last modified: Tue Jul 11 19:06:34 2023, max compression
```

## Comparing `XRDimage-0.0.1.6.tar` & `XRDimage-0.0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1074 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/LICENSE
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1694 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/PKG-INFO
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      293 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/README.md
-drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/XRDimage/
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      191 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/__init__.py
--rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)      919 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/center_of_grav.py
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1171 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/dark_correction.py
--rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)     1992 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/ellipse_fitting.py
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     4433 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/find_center.py
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     2691 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/image_processing_function.py
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1968 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/image_registration.py
--rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)     5058 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/image_segmentation.py
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1497 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/mask.py
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     4395 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/temperature_independent.py
-drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/XRDimage.egg-info/
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1694 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/PKG-INFO
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      481 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/SOURCES.txt
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)        1 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/dependency_links.txt
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       59 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/requires.txt
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)        9 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/top_level.txt
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       96 2023-07-11 18:12:42.000000 XRDimage-0.0.1.6/pyproject.toml
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       38 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/setup.cfg
--rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     2136 2023-07-11 18:05:30.000000 XRDimage-0.0.1.6/setup.py
+drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 19:06:34.615771 XRDimage-0.0.1.7/
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1074 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/LICENSE
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1694 2023-07-11 19:06:34.615771 XRDimage-0.0.1.7/PKG-INFO
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      293 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/README.md
+drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 19:06:34.615771 XRDimage-0.0.1.7/XRDimage/
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      287 2023-07-11 19:04:10.000000 XRDimage-0.0.1.7/XRDimage/__init__.py
+-rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)      919 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/center_of_grav.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1171 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/dark_correction.py
+-rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)     1992 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/ellipse_fitting.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     4433 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/find_center.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     2695 2023-07-11 19:01:38.000000 XRDimage-0.0.1.7/XRDimage/image_processing_function.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1968 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/image_registration.py
+-rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)     5058 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/image_segmentation.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1497 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/mask.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     4395 2023-07-11 14:46:52.000000 XRDimage-0.0.1.7/XRDimage/temperature_independent.py
+drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 19:06:34.615771 XRDimage-0.0.1.7/XRDimage.egg-info/
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1694 2023-07-11 19:06:34.000000 XRDimage-0.0.1.7/XRDimage.egg-info/PKG-INFO
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      481 2023-07-11 19:06:34.000000 XRDimage-0.0.1.7/XRDimage.egg-info/SOURCES.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)        1 2023-07-11 19:06:34.000000 XRDimage-0.0.1.7/XRDimage.egg-info/dependency_links.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       59 2023-07-11 19:06:34.000000 XRDimage-0.0.1.7/XRDimage.egg-info/requires.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)        9 2023-07-11 19:06:34.000000 XRDimage-0.0.1.7/XRDimage.egg-info/top_level.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       96 2023-07-11 18:12:42.000000 XRDimage-0.0.1.7/pyproject.toml
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       38 2023-07-11 19:06:34.615771 XRDimage-0.0.1.7/setup.cfg
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     2136 2023-07-11 19:05:52.000000 XRDimage-0.0.1.7/setup.py
```

### Comparing `XRDimage-0.0.1.6/LICENSE` & `XRDimage-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/PKG-INFO` & `XRDimage-0.0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
```

### Comparing `XRDimage-0.0.1.6/XRDimage/center_of_grav.py` & `XRDimage-0.0.1.7/XRDimage/center_of_grav.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/dark_correction.py` & `XRDimage-0.0.1.7/XRDimage/dark_correction.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/ellipse_fitting.py` & `XRDimage-0.0.1.7/XRDimage/ellipse_fitting.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/find_center.py` & `XRDimage-0.0.1.7/XRDimage/find_center.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/image_processing_function.py` & `XRDimage-0.0.1.7/XRDimage/image_processing_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from PIL import Image
 import os
 from os.path import join, isfile, isdir
 import re
 import sys
 
 # relative imports
-from dark_correction import dark_correction
-from find_center import find_center
-from image_registration import register_image
-from temperature_independent import resize_image
+from .dark_correction import dark_correction
+from .find_center import find_center
+from .image_registration import register_image
+from .temperature_independent import resize_image
 
 def save_img(img, file_path):
     ''' 
     Save image as tiff file to specified file path.
 
     Authors:
         Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
```

### Comparing `XRDimage-0.0.1.6/XRDimage/image_registration.py` & `XRDimage-0.0.1.7/XRDimage/image_registration.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/image_segmentation.py` & `XRDimage-0.0.1.7/XRDimage/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/mask.py` & `XRDimage-0.0.1.7/XRDimage/mask.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage/temperature_independent.py` & `XRDimage-0.0.1.7/XRDimage/temperature_independent.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.6/XRDimage.egg-info/PKG-INFO` & `XRDimage-0.0.1.7/XRDimage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
```

### Comparing `XRDimage-0.0.1.6/setup.py` & `XRDimage-0.0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools 
 
 setuptools.setup(
       name='XRDimage',
-      version='0.0.1.6',
+      version='0.0.1.7',
       description='XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.',
       long_description="""
                   XRDImage is a Python3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH. 
                   X-Ray Diffraction (XRD) is a technique used to identify and quantify crystalline phases in a material. By obtaining diffraction patterns, 
                   XRD enables the identification of crystalline phases and orientation, determination of various structural properties such as lattice parameters, 
                   stain, grain size, epitaxy, phase composition, and preferred orientation. The analysis of diffraction patterns also allows for 
                   the identification of internal stress and defects in crystals, providing valuable insights into material performance in different environments.
```

