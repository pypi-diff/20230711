# Comparing `tmp/lib-dt-computer-vision-0.1.0.tar.gz` & `tmp/lib-dt-computer-vision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dt-computer-vision-0.1.0.tar", last modified: Tue Jul 11 20:36:09 2023, max compression
+gzip compressed data, was "lib-dt-computer-vision-0.1.1.tar", last modified: Tue Jul 11 21:06:43 2023, max compression
```

## Comparing `lib-dt-computer-vision-0.1.0.tar` & `lib-dt-computer-vision-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      510 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2355 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.766722 lib-dt-computer-vision-0.1.0/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.766722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-07-11 20:33:46.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3477 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/anti_instagram.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       80 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/assets/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    18236 2023-07-11 05:49:30.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui.png
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      297 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/boards.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4705 2023-07-11 20:31:42.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       51 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2697 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6997 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5435 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/types.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1804 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       77 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/__init__.py
--rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     5254 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/ground_projector.py
--rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     8532 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/rendering.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       70 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      884 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12570 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/line_detector.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2586 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/rendering.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4817 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      510 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       37 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       19 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.360695 lib-dt-computer-vision-0.1.1/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      510 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-07-11 21:06:43.360695 lib-dt-computer-vision-0.1.1/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2386 2023-07-11 21:06:19.000000 lib-dt-computer-vision-0.1.1/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-07-11 21:06:38.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/anti_instagram/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/anti_instagram/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3477 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/anti_instagram/anti_instagram.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       80 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/assets/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    18236 2023-07-11 05:49:30.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui.png
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      297 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/boards.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4705 2023-07-11 20:31:42.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       51 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2697 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6997 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5435 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/types.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1804 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       77 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/__init__.py
+-rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     5254 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/ground_projector.py
+-rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     8532 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       70 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      884 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12570 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/line_detector.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2586 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4817 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 21:06:43.356695 lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      510 2023-07-11 21:06:43.000000 lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-07-11 21:06:43.000000 lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-07-11 21:06:43.000000 lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       37 2023-07-11 21:06:43.000000 lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       19 2023-07-11 21:06:43.000000 lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/top_level.txt
```

### Comparing `lib-dt-computer-vision-0.1.0/setup.py` & `lib-dt-computer-vision-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,10 +70,11 @@
     author=maintainer,
     author_email=maintainer_email,
     url=library_webpage,
     tests_require=tests_require,
     install_requires=install_requires,
     package_dir={"": "src"},
     packages=find_packages("./src"),
+    include_package_data=True,
     long_description=description,
     version=version,
 )
```

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/anti_instagram.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/anti_instagram/anti_instagram.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui.png` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui.png`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/types.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/types.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/utils.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/camera/utils.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/ground_projector.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/ground_projector.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/rendering.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/ground_projection/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/__init__.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/line_detector.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/line_detector.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/rendering.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/types.py` & `lib-dt-computer-vision-0.1.1/src/dt_computer_vision/line_detection/types.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/SOURCES.txt` & `lib-dt-computer-vision-0.1.1/src/lib_dt_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

