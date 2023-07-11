# Comparing `tmp/XRDimage-0.0.1.5.tar.gz` & `tmp/XRDimage-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XRDimage-0.0.1.5.tar", last modified: Tue Jul 11 03:59:29 2023, max compression
+gzip compressed data, was "XRDimage-0.0.1.6.tar", last modified: Tue Jul 11 18:20:44 2023, max compression
```

## Comparing `XRDimage-0.0.1.5.tar` & `XRDimage-0.0.1.6.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-11 03:59:29.060829 XRDimage-0.0.1.5/
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)        6 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/.keep
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1074 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/LICENSE
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)     1713 2023-07-11 03:59:29.055722 XRDimage-0.0.1.5/PKG-INFO
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      293 2023-07-10 19:47:45.000000 XRDimage-0.0.1.5/README.md
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-11 03:59:28.951195 XRDimage-0.0.1.5/XRDimage/
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      191 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/XRDimage/__init__.py
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      919 2023-07-10 15:28:37.000000 XRDimage-0.0.1.5/XRDimage/center_of_grav.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1171 2023-07-10 15:28:26.000000 XRDimage-0.0.1.5/XRDimage/dark_correction.py
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1992 2023-07-10 15:28:21.000000 XRDimage-0.0.1.5/XRDimage/ellipse_fitting.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4433 2023-07-10 15:28:10.000000 XRDimage-0.0.1.5/XRDimage/find_center.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     2691 2023-07-10 15:26:50.000000 XRDimage-0.0.1.5/XRDimage/image_processing_function.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1968 2023-07-10 15:26:55.000000 XRDimage-0.0.1.5/XRDimage/image_registration.py
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     5058 2023-07-10 19:42:29.000000 XRDimage-0.0.1.5/XRDimage/image_segmentation.py
--rw-r--r--   0 ewf22    (1167172) rxf131   (10097)    39510 2023-07-10 18:50:14.000000 XRDimage-0.0.1.5/XRDimage/kdSimulationScript.m
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1497 2023-07-10 15:25:53.000000 XRDimage-0.0.1.5/XRDimage/mask.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4395 2023-07-10 15:13:42.000000 XRDimage-0.0.1.5/XRDimage/temperature_independent.py
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-11 03:59:29.039535 XRDimage-0.0.1.5/XRDimage.egg-info/
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1713 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/PKG-INFO
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)      546 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/SOURCES.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/dependency_links.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)       59 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/requires.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-11 03:59:28.000000 XRDimage-0.0.1.5/XRDimage.egg-info/top_level.txt
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)       29 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/XRDimageDescription.txt
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)       87 2023-07-11 03:43:34.000000 XRDimage-0.0.1.5/pyproject.toml
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       38 2023-07-11 03:59:29.064128 XRDimage-0.0.1.5/setup.cfg
--rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2112 2023-07-11 03:56:19.000000 XRDimage-0.0.1.5/setup.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      626 2023-07-03 15:13:51.000000 XRDimage-0.0.1.5/test
+drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1074 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/LICENSE
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1694 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/PKG-INFO
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      293 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/README.md
+drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/XRDimage/
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      191 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/__init__.py
+-rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)      919 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/center_of_grav.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1171 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/dark_correction.py
+-rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)     1992 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/ellipse_fitting.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     4433 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/find_center.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     2691 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/image_processing_function.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1968 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/image_registration.py
+-rwxrwxr-x   0 weiqi     (1000) weiqi     (1000)     5058 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/image_segmentation.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1497 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/mask.py
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     4395 2023-07-11 14:46:52.000000 XRDimage-0.0.1.6/XRDimage/temperature_independent.py
+drwxrwxr-x   0 weiqi     (1000) weiqi     (1000)        0 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/XRDimage.egg-info/
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     1694 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/PKG-INFO
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)      481 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/SOURCES.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)        1 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/dependency_links.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       59 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/requires.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)        9 2023-07-11 18:20:44.000000 XRDimage-0.0.1.6/XRDimage.egg-info/top_level.txt
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       96 2023-07-11 18:12:42.000000 XRDimage-0.0.1.6/pyproject.toml
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)       38 2023-07-11 18:20:44.604625 XRDimage-0.0.1.6/setup.cfg
+-rw-rw-r--   0 weiqi     (1000) weiqi     (1000)     2136 2023-07-11 18:05:30.000000 XRDimage-0.0.1.6/setup.py
```

### Comparing `XRDimage-0.0.1.5/LICENSE` & `XRDimage-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/PKG-INFO` & `XRDimage-0.0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
-Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
 
 
                   XRDImage is a Python3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH. 
                   X-Ray Diffraction (XRD) is a technique used to identify and quantify crystalline phases in a material. By obtaining diffraction patterns, 
                   XRD enables the identification of crystalline phases and orientation, determination of various structural properties such as lattice parameters, 
                   stain, grain size, epitaxy, phase composition, and preferred orientation. The analysis of diffraction patterns also allows for 
                   the identification of internal stress and defects in crystals, providing valuable insights into material performance in different environments.
 
                   Due to the nature of XRD Imaging techniques, most XRD images may not turn out perfect out of the lab. In XRDImage, 
                   we have created an image processing pipeline with multitudes of functions to pre-process XRD Images.
                    
-
```

### Comparing `XRDimage-0.0.1.5/XRDimage/center_of_grav.py` & `XRDimage-0.0.1.6/XRDimage/center_of_grav.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/dark_correction.py` & `XRDimage-0.0.1.6/XRDimage/dark_correction.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/ellipse_fitting.py` & `XRDimage-0.0.1.6/XRDimage/ellipse_fitting.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/find_center.py` & `XRDimage-0.0.1.6/XRDimage/find_center.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/image_processing_function.py` & `XRDimage-0.0.1.6/XRDimage/image_processing_function.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/image_registration.py` & `XRDimage-0.0.1.6/XRDimage/image_registration.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/image_segmentation.py` & `XRDimage-0.0.1.6/XRDimage/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/mask.py` & `XRDimage-0.0.1.6/XRDimage/mask.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage/temperature_independent.py` & `XRDimage-0.0.1.6/XRDimage/temperature_independent.py`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.1.5/XRDimage.egg-info/PKG-INFO` & `XRDimage-0.0.1.6/XRDimage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
-Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
 
 
                   XRDImage is a Python3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH. 
                   X-Ray Diffraction (XRD) is a technique used to identify and quantify crystalline phases in a material. By obtaining diffraction patterns, 
                   XRD enables the identification of crystalline phases and orientation, determination of various structural properties such as lattice parameters, 
                   stain, grain size, epitaxy, phase composition, and preferred orientation. The analysis of diffraction patterns also allows for 
                   the identification of internal stress and defects in crystals, providing valuable insights into material performance in different environments.
 
                   Due to the nature of XRD Imaging techniques, most XRD images may not turn out perfect out of the lab. In XRDImage, 
                   we have created an image processing pipeline with multitudes of functions to pre-process XRD Images.
                    
-
```

### Comparing `XRDimage-0.0.1.5/setup.py` & `XRDimage-0.0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from setuptools import setup
+import setuptools 
 
-
-setup(name='XRDimage',
-      version='0.0.1.5',
+setuptools.setup(
+      name='XRDimage',
+      version='0.0.1.6',
       description='XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.',
       long_description="""
                   XRDImage is a Python3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH. 
                   X-Ray Diffraction (XRD) is a technique used to identify and quantify crystalline phases in a material. By obtaining diffraction patterns, 
                   XRD enables the identification of crystalline phases and orientation, determination of various structural properties such as lattice parameters, 
                   stain, grain size, epitaxy, phase composition, and preferred orientation. The analysis of diffraction patterns also allows for 
                   the identification of internal stress and defects in crystals, providing valuable insights into material performance in different environments.
@@ -14,16 +14,16 @@
                   Due to the nature of XRD Imaging techniques, most XRD images may not turn out perfect out of the lab. In XRDImage, 
                   we have created an image processing pipeline with multitudes of functions to pre-process XRD Images.
                    """,
       url='http://engineering.case.edu/centers/sdle/',
       author='Weiqi Yue, Ethan Fang, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French',
       author_email='wxy215@case.edu, pkt19@case.edu, roger.french@case.edu',
       license='MIT License',
-      packages=[''],
-      package_dir={'XRDimage': './XRDimage'},
+      packages=setuptools.find_packages(),
+      #package_dir={'XRDimage': './XRDimage'},
 #      package_data={'XRDimage': ['data','files/data/FullSizeModules/*','files/tutorials/*','files/data/out','README.rst']},
       python_requires='>=3.8',
       install_requires=['numpy', 'Pillow', 'opencv-python', 'matplotlib', 'imageio', 'scikit-learn'],
 #      include_package_data=True,
       project_urls={"Documentation":"https://xrdimage-doc.readthedocs.io/en/latest/","Bugtracker": "https://bitbucket.org/cwrusdle/xrd-image/src/main/"},
-      )
+)
```

