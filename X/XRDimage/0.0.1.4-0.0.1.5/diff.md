# Comparing `tmp/XRDimage-0.0.1.4.tar.gz` & `tmp/XRDimage-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XRDimage-0.0.1.4.tar", last modified: Mon Jul 10 20:33:56 2023, max compression
+gzip compressed data, was "XRDimage-0.0.1.5.tar", last modified: Tue Jul 11 03:59:29 2023, max compression
```

## Comparing `XRDimage-0.0.1.4.tar` & `XRDimage-0.0.1.5.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-10 20:33:56.213852 XRDimage-0.0.1.4/
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)        6 2023-07-03 15:13:51.000000 XRDimage-0.0.1.4/.keep
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1074 2023-07-03 15:13:51.000000 XRDimage-0.0.1.4/LICENSE
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)     1713 2023-07-10 20:33:56.210844 XRDimage-0.0.1.4/PKG-INFO
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      293 2023-07-10 19:47:45.000000 XRDimage-0.0.1.4/README.md
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-10 20:33:56.163851 XRDimage-0.0.1.4/XRDimage/
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      191 2023-07-03 15:13:51.000000 XRDimage-0.0.1.4/XRDimage/__init__.py
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      919 2023-07-10 15:28:37.000000 XRDimage-0.0.1.4/XRDimage/center_of_grav.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1171 2023-07-10 15:28:26.000000 XRDimage-0.0.1.4/XRDimage/dark_correction.py
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1992 2023-07-10 15:28:21.000000 XRDimage-0.0.1.4/XRDimage/ellipse_fitting.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4433 2023-07-10 15:28:10.000000 XRDimage-0.0.1.4/XRDimage/find_center.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     2691 2023-07-10 15:26:50.000000 XRDimage-0.0.1.4/XRDimage/image_processing_function.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1968 2023-07-10 15:26:55.000000 XRDimage-0.0.1.4/XRDimage/image_registration.py
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     5058 2023-07-10 19:42:29.000000 XRDimage-0.0.1.4/XRDimage/image_segmentation.py
--rw-r--r--   0 ewf22    (1167172) rxf131   (10097)    39510 2023-07-10 18:50:14.000000 XRDimage-0.0.1.4/XRDimage/kdSimulationScript.m
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1497 2023-07-10 15:25:53.000000 XRDimage-0.0.1.4/XRDimage/mask.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4395 2023-07-10 15:13:42.000000 XRDimage-0.0.1.4/XRDimage/temperature_independent.py
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-10 20:33:56.202928 XRDimage-0.0.1.4/XRDimage.egg-info/
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1713 2023-07-10 20:33:55.000000 XRDimage-0.0.1.4/XRDimage.egg-info/PKG-INFO
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)      560 2023-07-10 20:33:55.000000 XRDimage-0.0.1.4/XRDimage.egg-info/SOURCES.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-10 20:33:55.000000 XRDimage-0.0.1.4/XRDimage.egg-info/dependency_links.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)       59 2023-07-10 20:33:55.000000 XRDimage-0.0.1.4/XRDimage.egg-info/requires.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-10 20:33:55.000000 XRDimage-0.0.1.4/XRDimage.egg-info/top_level.txt
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)       29 2023-07-03 15:13:51.000000 XRDimage-0.0.1.4/XRDimageDescription.txt
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      109 2023-07-10 19:47:33.000000 XRDimage-0.0.1.4/pyproject.toml
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       38 2023-07-10 20:33:56.218014 XRDimage-0.0.1.4/setup.cfg
--rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2112 2023-07-10 20:33:42.000000 XRDimage-0.0.1.4/setup.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      626 2023-07-03 15:13:51.000000 XRDimage-0.0.1.4/test
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       23 2023-07-10 20:19:12.000000 XRDimage-0.0.1.4/testImport.py
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-11 03:59:29.060829 XRDimage-0.0.1.5/
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)        6 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/.keep
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1074 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/LICENSE
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)     1713 2023-07-11 03:59:29.055722 XRDimage-0.0.1.5/PKG-INFO
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)      293 2023-07-10 19:47:45.000000 XRDimage-0.0.1.5/README.md
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-11 03:59:28.951195 XRDimage-0.0.1.5/XRDimage/
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)      191 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/XRDimage/__init__.py
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      919 2023-07-10 15:28:37.000000 XRDimage-0.0.1.5/XRDimage/center_of_grav.py
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1171 2023-07-10 15:28:26.000000 XRDimage-0.0.1.5/XRDimage/dark_correction.py
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1992 2023-07-10 15:28:21.000000 XRDimage-0.0.1.5/XRDimage/ellipse_fitting.py
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4433 2023-07-10 15:28:10.000000 XRDimage-0.0.1.5/XRDimage/find_center.py
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     2691 2023-07-10 15:26:50.000000 XRDimage-0.0.1.5/XRDimage/image_processing_function.py
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1968 2023-07-10 15:26:55.000000 XRDimage-0.0.1.5/XRDimage/image_registration.py
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     5058 2023-07-10 19:42:29.000000 XRDimage-0.0.1.5/XRDimage/image_segmentation.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)    39510 2023-07-10 18:50:14.000000 XRDimage-0.0.1.5/XRDimage/kdSimulationScript.m
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1497 2023-07-10 15:25:53.000000 XRDimage-0.0.1.5/XRDimage/mask.py
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4395 2023-07-10 15:13:42.000000 XRDimage-0.0.1.5/XRDimage/temperature_independent.py
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-11 03:59:29.039535 XRDimage-0.0.1.5/XRDimage.egg-info/
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1713 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/PKG-INFO
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)      546 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/SOURCES.txt
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/dependency_links.txt
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)       59 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/requires.txt
+-rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/top_level.txt
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)       29 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/XRDimageDescription.txt
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)       87 2023-07-11 03:43:34.000000 XRDimage-0.0.1.5/pyproject.toml
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       38 2023-07-11 03:59:29.064128 XRDimage-0.0.1.5/setup.cfg
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2112 2023-07-11 03:56:19.000000 XRDimage-0.0.1.5/setup.py
+-rw-rw----   0 ewf22    (1167172) rxf131   (10097)      626 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/test
```

### Comparing `XRDimage-0.0.1.4/LICENSE` & `XRDimage-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/PKG-INFO` & `XRDimage-0.0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
```

### Comparing `XRDimage-0.0.1.4/XRDimage/center_of_grav.py` & `XRDimage-0.0.1.5/XRDimage/center_of_grav.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/dark_correction.py` & `XRDimage-0.0.1.5/XRDimage/dark_correction.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/ellipse_fitting.py` & `XRDimage-0.0.1.5/XRDimage/ellipse_fitting.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/find_center.py` & `XRDimage-0.0.1.5/XRDimage/find_center.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/image_processing_function.py` & `XRDimage-0.0.1.5/XRDimage/image_processing_function.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/image_registration.py` & `XRDimage-0.0.1.5/XRDimage/image_registration.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/image_segmentation.py` & `XRDimage-0.0.1.5/XRDimage/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/kdSimulationScript.m` & `XRDimage-0.0.1.5/XRDimage/kdSimulationScript.m`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/mask.py` & `XRDimage-0.0.1.5/XRDimage/mask.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage/temperature_independent.py` & `XRDimage-0.0.1.5/XRDimage/temperature_independent.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.4/XRDimage.egg-info/PKG-INFO` & `XRDimage-0.0.1.5/XRDimage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
```

### Comparing `XRDimage-0.0.1.4/XRDimage.egg-info/SOURCES.txt` & `XRDimage-0.0.1.5/XRDimage.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .keep
 LICENSE
 README.md
 XRDimageDescription.txt
 pyproject.toml
 setup.py
 test
-testImport.py
 XRDimage/__init__.py
 XRDimage/center_of_grav.py
 XRDimage/dark_correction.py
 XRDimage/ellipse_fitting.py
 XRDimage/find_center.py
 XRDimage/image_processing_function.py
 XRDimage/image_registration.py
```

### Comparing `XRDimage-0.0.1.4/setup.py` & `XRDimage-0.0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='XRDimage',
-      version='0.0.1.4',
+      version='0.0.1.5',
       description='XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.',
       long_description="""
                   XRDImage is a Python3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH. 
                   X-Ray Diffraction (XRD) is a technique used to identify and quantify crystalline phases in a material. By obtaining diffraction patterns, 
                   XRD enables the identification of crystalline phases and orientation, determination of various structural properties such as lattice parameters, 
                   stain, grain size, epitaxy, phase composition, and preferred orientation. The analysis of diffraction patterns also allows for 
                   the identification of internal stress and defects in crystals, providing valuable insights into material performance in different environments.
```

### Comparing `XRDimage-0.0.1.4/test` & `XRDimage-0.0.1.5/test`

 * *Files identical despite different names*

