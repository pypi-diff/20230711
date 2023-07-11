# Comparing `tmp/lib-dt-computer-vision-0.0.7.tar.gz` & `tmp/lib-dt-computer-vision-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dt-computer-vision-0.0.7.tar", last modified: Fri Jun 10 15:26:54 2022, max compression
+gzip compressed data, was "lib-dt-computer-vision-0.1.0.tar", last modified: Tue Jul 11 20:36:09 2023, max compression
```

## Comparing `lib-dt-computer-vision-0.0.7.tar` & `lib-dt-computer-vision-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.781987 lib-dt-computer-vision-0.0.7/
--rw-r--r--   0     1000 root         (0)      577 2022-06-10 15:26:54.781987 lib-dt-computer-vision-0.0.7/PKG-INFO
--rw-r--r--   0     1000 root         (0)       38 2022-06-10 15:26:54.781987 lib-dt-computer-vision-0.0.7/setup.cfg
--rw-rw-r--   0     1000 root         (0)     2355 2022-03-03 21:47:00.000000 lib-dt-computer-vision-0.0.7/setup.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.773987 lib-dt-computer-vision-0.0.7/src/
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.773987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/
--rw-rw-r--   0     1000 root         (0)       22 2022-06-10 15:26:36.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/__init__.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.773987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/anti_instagram/
--rw-rw-r--   0     1000 root         (0)       42 2022-03-07 16:42:30.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/anti_instagram/__init__.py
--rw-rw-r--   0     1000 root         (0)     3477 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/anti_instagram/anti_instagram.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.777987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/
--rw-rw-r--   0     1000 root         (0)       80 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/__init__.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.777987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/
--rw-rw-r--   0     1000 root         (0)        0 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/__init__.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.777987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/
--rw-rw-r--   0     1000 root         (0)        0 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
--rw-rw-r--   0     1000 root         (0)      297 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/boards.py
--rw-rw-r--   0     1000 root         (0)     1763 2022-06-10 15:20:28.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
--rw-rw-r--   0     1000 root         (0)       51 2022-06-09 17:55:13.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
--rw-rw-r--   0     1000 root         (0)     2697 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
--rw-rw-r--   0     1000 root         (0)     1277 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
--rw-rw-r--   0     1000 root         (0)     5381 2022-06-09 17:39:59.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/types.py
--rw-rw-r--   0     1000 root         (0)     1804 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/utils.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.777987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/
--rw-rw-r--   0     1000 root         (0)       46 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/__init__.py
--rwxrwxr-x   0     1000 root         (0)     5254 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/ground_projector.py
--rwxrwxr-x   0     1000 root         (0)     5408 2022-03-21 19:42:50.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/rendering.py
--rw-rw-r--   0     1000 root         (0)       70 2022-03-08 16:08:00.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/types.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.781987 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/
--rw-rw-r--   0     1000 root         (0)      884 2022-03-03 22:48:11.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/__init__.py
--rw-rw-r--   0     1000 root         (0)    12570 2022-03-14 19:59:04.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/line_detector.py
--rw-rw-r--   0     1000 root         (0)     2586 2022-03-14 20:35:51.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/rendering.py
--rw-rw-r--   0     1000 root         (0)     4817 2022-03-21 19:42:50.000000 lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/types.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-06-10 15:26:54.781987 lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/
--rw-r--r--   0     1000 root         (0)      577 2022-06-10 15:26:54.000000 lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/PKG-INFO
--rw-r--r--   0     1000 root         (0)     1384 2022-06-10 15:26:54.000000 lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/SOURCES.txt
--rw-r--r--   0     1000 root         (0)        1 2022-06-10 15:26:54.000000 lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/dependency_links.txt
--rw-r--r--   0     1000 root         (0)       37 2022-06-10 15:26:54.000000 lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/requires.txt
--rw-r--r--   0     1000 root         (0)       19 2022-06-10 15:26:54.000000 lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      510 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2355 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.766722 lib-dt-computer-vision-0.1.0/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.766722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-07-11 20:33:46.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3477 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/anti_instagram.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       80 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/assets/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    18236 2023-07-11 05:49:30.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui.png
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      297 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/boards.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4705 2023-07-11 20:31:42.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       51 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2697 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6997 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5435 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/types.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1804 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       77 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/__init__.py
+-rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     5254 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/ground_projector.py
+-rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     8532 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       70 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      884 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12570 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/line_detector.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2586 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4817 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-11 20:36:09.770722 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      510 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       37 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       19 2023-07-11 20:36:09.000000 lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/top_level.txt
```

### Comparing `lib-dt-computer-vision-0.0.7/setup.py` & `lib-dt-computer-vision-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/anti_instagram/anti_instagram.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/anti_instagram/anti_instagram.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/types.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import cv2
 import numpy as np
 
 from .utils import invert_map, ensure_ndarray
 
 BGRImage = np.ndarray
+RGBImage = np.ndarray
 HSVImage = np.ndarray
 
 
 @dataclasses.dataclass
 class Point:
     """
     A generic 2D point.
@@ -18,15 +19,15 @@
     x: float
     y: float
 
     def as_array(self) -> np.ndarray:
         return np.array([self.x, self.y])
 
     def __repr__(self):
-        return f"P({self.x}, {self.y})"
+        return f"P({round(self.x, 4)}, {round(self.y, 4)})"
 
 
 class Pixel(Point):
 
     def as_integers(self) -> np.ndarray:
         return np.array([int(self.x), int(self.y)], dtype=int)
 
@@ -76,15 +77,15 @@
         dst = cv2.undistortPoints(src,
                                   self.camera.K,
                                   self.camera.D,
                                   R=self.camera.R,
                                   P=self.camera.P)
         return Pixel(*dst[0, 0])
 
-    def rectify(self, image: BGRImage, interpolation=cv2.INTER_NEAREST):
+    def rectify(self, image: BGRImage, interpolation=cv2.INTER_NEAREST) -> BGRImage:
         """
         Undistorts an image.
         While cv2.INTER_NEAREST is faster, use cv2.INTER_CUBIC for higher quality.
         """
         if not self._rectify_inited:
             self._init_rectify_maps()
         # rectify distorted image
```

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/camera/utils.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/camera/utils.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/ground_projector.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/ground_projector.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/ground_projection/rendering.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/ground_projection/rendering.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,173 +1,249 @@
 #!/usr/bin/env python3
 
-from typing import Optional, Dict, List, Tuple
+from typing import Optional, Dict, List, Tuple, Union
 
 import cv2
 import numpy as np
 
 from dt_computer_vision.ground_projection.types import GroundPoint
 
 Color = Tuple[int, int, int]
 Segment = Tuple[GroundPoint, GroundPoint]
 
-grid_size = 6
+GRID_SIZE: int = 4
+# resolution of each cell in meters
+RESOLUTION: float = 0.1
+# how often (number of cells) do we draw a tick with the value
+TICKS_EVERY: int = 2
 # everything here is calibrated for a 1000x1000 image
-scale = 1000
-s_segment_thickness = 10
-s_padding = 80
-s_grid_thickness = 3
-s_font_size = 3
-s_font_thickness = 3
-
-
-def draw_grid_image(size: Tuple[int, int]):
+SCALE: int = 1000
+S_SEGMENT_THICKNESS: int = 10
+S_PADDING: int = 80
+S_GRID_THICKNESS: int = 3
+S_FONT_SIZE: int = 3
+S_FONT_THICKNESS: int = 3
+
+
+def draw_grid_image(
+        size: Tuple[int, int],
+        # default values
+        grid_size: Union[int, Tuple[int, int]] = GRID_SIZE,
+        scale: int = SCALE,
+        s_padding: int = S_PADDING,
+        s_grid_thickness: int = S_GRID_THICKNESS,
+        s_font_size: int = S_FONT_SIZE,
+        s_font_thickness: int = S_FONT_THICKNESS,
+        ticks_every: Union[int, Tuple[int, int]] = TICKS_EVERY,
+        resolution: Union[float, Tuple[float, float]] = RESOLUTION,
+        start_y: float = 0.0
+):
     """
     Generates a grid image with distances from the robot's origin.
 
+    Args:
+        size (:obj:`tuple`): Size of the image to draw
+
+        grid_size (:obj:`int`): Number of cells to draw
+        scale (:obj:`int`): Scale of the image
+        s_padding (:obj:`int`): Padding of the grid
+        s_grid_thickness (:obj:`dict`): Grid lines thickness
+        s_font_size (:obj:`np.ndarray`): Font size
+        s_font_thickness (:obj:`int`): Font thickness
+
     Returns:
         :obj:`numpy array`: an OpenCV image
 
     """
+    # if grid_size is an integer, it means that the grid is square
+    grid_size = grid_size if isinstance(grid_size, tuple) else (grid_size, grid_size)
+
+    # if resolution is an integer, it means that the grid is linear
+    resolution = resolution if isinstance(resolution, tuple) else (resolution, resolution)
+
+    # if ticks_every is an integer, it means that we use the same value on both x and y
+    ticks_every = ticks_every if isinstance(ticks_every, tuple) else (ticks_every, ticks_every)
+
+    # unpack
+    resolution_x, resolution_y = resolution
+    ticks_every_x, ticks_every_y = ticks_every
+
+    # image is square
     size_x, size_y = size
 
     s = max(size_x, size_y) / scale
     padding = int(s_padding * s)
     grid_thickness = max(1, int(s_grid_thickness * s))
     font_size = s_font_size * s
     font_thickness = max(1, int(s_font_thickness * s))
 
-    half_grid_size = int(grid_size / 2)
-    cell_size_x = int((size_x - 3 * padding) / grid_size)
-    cell_size_y = int((size_y - 3 * padding) / grid_size)
-    origin_x, origin_y = 2 * padding + int(grid_size / 2) * cell_size_x, size_y - 2 * padding
+    grid_size_x, grid_size_y = grid_size
+
+    half_grid_size_horizontal = int(grid_size_x / 2)
+    cell_size_x = int((size_x - 3 * padding) / grid_size_x)
+    cell_size_y = int((size_y - 3 * padding) / grid_size_y)
+    origin_x, origin_y = 2 * padding + half_grid_size_horizontal * cell_size_x, size_y - 2 * padding
 
     # initialize gray image
     grid_image = np.ones((size_y, size_x, 3), np.uint8) * 128
 
     # draw vertical lines of the grid
-    for col in range(grid_size + 1):
+    for col in range(grid_size_x + 1):
         col_x = col * cell_size_x
         cv2.line(
             grid_image,
             pt1=(2 * padding + col_x, padding),
             pt2=(2 * padding + col_x, origin_y),
             color=(255, 255, 0),
             thickness=grid_thickness
         )
 
     h_text_centering_offset = int(size_x / 20)
     v_text_centering_offset = int(size_y / 200)
 
-    # draw the horizontal coordinates
-    for i in range(0, half_grid_size+1, 2):
+    # write the horizontal coordinates
+    for i in range(0, half_grid_size_horizontal+1, ticks_every_x):
         for v in {i, i * -1}:
-            text = f"{v * 10}cm"
+            text = f"{v * int(resolution_x * 100)}cm"
             text = " " * max(0, 4 - len(text)) + text
             cv2.putText(
                 grid_image,
                 text,
                 (origin_x + v * cell_size_x - h_text_centering_offset,
                  origin_y + h_text_centering_offset),
                 cv2.FONT_HERSHEY_PLAIN,
                 font_size,
                 (255, 255, 255),
                 font_thickness,
             )
 
     # draw horizontal lines of the grid
-    for row in range(grid_size + 1):
+    for row in range(grid_size_y + 1):
         row_y = row * cell_size_y
         cv2.line(
             grid_image,
             pt1=(2 * padding, padding + row_y),
             pt2=(size_x - padding, padding + row_y),
             color=(255, 255, 0),
             thickness=grid_thickness
         )
 
-    # draw the vertical coordinates
-    for i in range(0, grid_size + 1, 2):
+    # write the vertical coordinates
+    for i in range(0, grid_size_y + 1, ticks_every_y):
         cv2.putText(
             grid_image,
-            f"{i * 10}cm",
+            f"{int(start_y * 100) + i * int(resolution_y * 100)}cm",
             (10, origin_y - i * cell_size_y + v_text_centering_offset),
             cv2.FONT_HERSHEY_PLAIN,
             font_size,
             (255, 255, 255),
             font_thickness
         )
 
     # draw central vertical line
-    col_x = half_grid_size * cell_size_x
+    col_x = half_grid_size_horizontal * cell_size_x
     cv2.line(
         grid_image,
         pt1=(2 * padding + col_x, padding),
         pt2=(2 * padding + col_x, origin_y),
         color=(255, 0, 0),
         thickness=grid_thickness
     )
 
     # draw wheel's axis
-    cv2.line(
-        grid_image,
-        pt1=(2 * padding, origin_y),
-        pt2=(2 * padding + grid_size * cell_size_x, origin_y),
-        color=(255, 0, 0),
-        thickness=grid_thickness
-    )
+    if start_y == 0.0:
+        cv2.line(
+            grid_image,
+            pt1=(2 * padding, origin_y),
+            pt2=(2 * padding + grid_size_x * cell_size_x, origin_y),
+            color=(255, 0, 0),
+            thickness=grid_thickness
+        )
 
     return grid_image
 
 
-def debug_image(segments: Dict[Color, List[Segment]], size: Tuple[int, int],
-                background_image: Optional[np.ndarray] = None):
+def debug_image(
+        segments: Dict[Color, List[Segment]],
+        size: Tuple[int, int],
+        background_image: Optional[np.ndarray] = None,
+        # default values
+        grid_size: Union[int, Tuple[int, int]] = GRID_SIZE,
+        scale: int = SCALE,
+        s_segment_thickness: int = S_SEGMENT_THICKNESS,
+        s_padding: int = S_PADDING,
+        resolution: Union[float, Tuple[float, float]] = RESOLUTION,
+        start_y: float = 0.0
+):
     """
     Generates a debug image with all the projected segments plotted with respect to the
     robot's origin.
 
     Args:
         segments (:obj:`dict`): Line segments in the ground plane relative to robot's origin
-        size (:obj:`tuple`): Image of the image to draw
+        size (:obj:`tuple`): Size of the image to draw
         background_image (:obj:`np.ndarray`): Optional background image
 
+        grid_size (:obj:`int`): Number of cells to draw
+        scale (:obj:`int`): Scale of the image
+        s_segment_thickness (:obj:`int`): Thickness of the segments drawn
+        s_padding (:obj:`int`): Padding of the grid
+
     Returns:
         :obj:`numpy array`: an OpenCV image
 
     """
+    background_image = background_image if background_image is not None else draw_grid_image(
+        size,
+        grid_size=grid_size,
+        scale=scale,
+        s_padding=s_padding,
+        resolution=resolution,
+        start_y=start_y,
+    )
+
+    # if grid_size is an integer, it means that the grid is square
+    grid_size = grid_size if isinstance(grid_size, tuple) else (grid_size, grid_size)
+
+    # if resolution is an integer, it means that the grid is linear
+    resolution = resolution if isinstance(resolution, tuple) else (resolution, resolution)
+
+    # unpack
+    resolution_x, resolution_y = resolution
+
+    grid_size_x, grid_size_y = grid_size
     size_x, size_y = size
 
     s = max(size_x, size_y) / scale
     segment_thickness = max(1, int(s_segment_thickness * s))
     padding = int(s_padding * s)
 
-    half_grid_size = int(grid_size / 2)
-    cell_size_x = int((size_x - 3 * padding) / grid_size)
-    cell_size_y = int((size_y - 3 * padding) / grid_size)
-    origin_x, origin_y = 2 * padding + int(grid_size / 2) * cell_size_x, size_y - 2 * padding
+    half_grid_size_horizontal = int(grid_size_x / 2)
+    cell_size_x = int((size_x - 3 * padding) / grid_size_x)
+    cell_size_y = int((size_y - 3 * padding) / grid_size_y)
+    origin_x, origin_y = 2 * padding + half_grid_size_horizontal * cell_size_x, size_y - 2 * padding
 
-    background_image = background_image if background_image is not None else draw_grid_image(size)
     image = background_image.copy()
     # plot every segment if both ends are in the scope of the image (within 50cm from the origin)
     for color, lines in segments.items():
         for start, end in lines:
             # only draw segments that are within the grid
-            if np.any(np.abs([start.y, end.y]) > (half_grid_size / 10)):
+            if np.any(np.abs([start.y, end.y]) > (half_grid_size_horizontal * resolution_x)):
                 continue
-            if np.any(np.abs([start.x, end.x]) > (grid_size / 10)):
+            if np.any(np.abs([start.x, end.x]) > (grid_size_y * resolution_y)):
                 continue
             # draw segment
             cv2.line(
                 image,
                 pt1=(
-                    origin_x + int(-(start.y * 10) * cell_size_x),
-                    origin_y - int((start.x * 10) * cell_size_y)
+                    origin_x + int((-start.y / resolution_x) * cell_size_x),
+                    origin_y - int(((start.x - start_y) / resolution_y) * cell_size_y)
                 ),
                 pt2=(
-                    origin_x + int(-(end.y * 10) * cell_size_x),
-                    origin_y - int((end.x * 10) * cell_size_y)
+                    origin_x + int((-end.y / resolution_x) * cell_size_x),
+                    origin_y - int(((end.x - start_y) / resolution_y) * cell_size_y)
                 ),
                 color=color,
                 thickness=segment_thickness,
             )
     # ---
     return image
```

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/__init__.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/line_detector.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/line_detector.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/rendering.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/dt_computer_vision/line_detection/types.py` & `lib-dt-computer-vision-0.1.0/src/dt_computer_vision/line_detection/types.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.0.7/src/lib_dt_computer_vision.egg-info/SOURCES.txt` & `lib-dt-computer-vision-0.1.0/src/lib_dt_computer_vision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/dt_computer_vision/camera/calibration/__init__.py
 src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
 src/dt_computer_vision/camera/calibration/extrinsics/boards.py
 src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
 src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
 src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
 src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
+src/dt_computer_vision/camera/calibration/extrinsics/assets/gui.png
 src/dt_computer_vision/ground_projection/__init__.py
 src/dt_computer_vision/ground_projection/ground_projector.py
 src/dt_computer_vision/ground_projection/rendering.py
 src/dt_computer_vision/ground_projection/types.py
 src/dt_computer_vision/line_detection/__init__.py
 src/dt_computer_vision/line_detection/line_detector.py
 src/dt_computer_vision/line_detection/rendering.py
```

