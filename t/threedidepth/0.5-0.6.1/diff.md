# Comparing `tmp/threedidepth-0.5.tar.gz` & `tmp/threedidepth-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/threedidepth-0.5.tar", last modified: Fri Jul  2 08:38:06 2021, max compression
+gzip compressed data, was "threedidepth-0.6.1.tar", last modified: Tue Jul 11 10:01:58 2023, max compression
```

## Comparing `threedidepth-0.5.tar` & `threedidepth-0.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2021-07-02 08:38:06.000000 threedidepth-0.5/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1507 2021-07-02 08:38:06.000000 threedidepth-0.5/LICENSE
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1610 2021-07-02 08:38:06.000000 threedidepth-0.5/README.rst
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      118 2021-07-02 08:38:06.000000 threedidepth-0.5/MANIFEST.in
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2021-07-02 08:38:06.000000 threedidepth-0.5/test/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     2159 2021-07-02 08:38:06.000000 threedidepth-0.5/test/test_morton.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    13714 2021-07-02 08:38:06.000000 threedidepth-0.5/test/test_calculate.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1847 2021-07-02 08:38:06.000000 threedidepth-0.5/test/test_commands.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       24 2021-07-02 08:38:06.000000 threedidepth-0.5/test/__init__.py
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2021-07-02 08:38:06.000000 threedidepth-0.5/src/
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    25088 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth/calculate.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     5403 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth/morton.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1717 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth/commands.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       24 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth/__init__.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1446 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth/fixes.py
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       69 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/entry_points.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)        1 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/dependency_links.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)        1 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/not-zip-safe
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      612 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/SOURCES.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     3896 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/PKG-INFO
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       13 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/top_level.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       71 2021-07-02 08:38:06.000000 threedidepth-0.5/src/threedidepth.egg-info/requires.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1737 2021-07-02 08:38:06.000000 threedidepth-0.5/setup.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      696 2021-07-02 08:38:06.000000 threedidepth-0.5/CHANGES.rst
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      303 2021-07-02 08:38:06.000000 threedidepth-0.5/docker-compose.yml
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      404 2021-07-02 08:38:06.000000 threedidepth-0.5/requirements.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     3896 2021-07-02 08:38:06.000000 threedidepth-0.5/PKG-INFO
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      229 2021-07-02 08:38:06.000000 threedidepth-0.5/setup.cfg
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1358 2021-07-02 08:38:06.000000 threedidepth-0.5/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:58.875739 threedidepth-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-11 10:01:48.000000 threedidepth-0.6.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-11 10:01:48.000000 threedidepth-0.6.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-11 10:01:48.000000 threedidepth-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 10:01:48.000000 threedidepth-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-11 10:01:58.875739 threedidepth-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-11 10:01:48.000000 threedidepth-0.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 10:01:48.000000 threedidepth-0.6.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-11 10:01:48.000000 threedidepth-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-11 10:01:58.875739 threedidepth-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-11 10:01:48.000000 threedidepth-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:58.871739 threedidepth-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:58.871739 threedidepth-0.6.1/src/threedidepth/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 10:01:48.000000 threedidepth-0.6.1/src/threedidepth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26347 2023-07-11 10:01:48.000000 threedidepth-0.6.1/src/threedidepth/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-11 10:01:48.000000 threedidepth-0.6.1/src/threedidepth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-11 10:01:48.000000 threedidepth-0.6.1/src/threedidepth/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-11 10:01:48.000000 threedidepth-0.6.1/src/threedidepth/morton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:58.871739 threedidepth-0.6.1/src/threedidepth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 10:01:58.000000 threedidepth-0.6.1/src/threedidepth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:58.875739 threedidepth-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 10:01:48.000000 threedidepth-0.6.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-07-11 10:01:48.000000 threedidepth-0.6.1/test/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-11 10:01:48.000000 threedidepth-0.6.1/test/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-11 10:01:48.000000 threedidepth-0.6.1/test/test_morton.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `threedidepth-0.5/LICENSE` & `threedidepth-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `threedidepth-0.5/test/test_morton.py` & `threedidepth-0.6.1/test/test_morton.py`

 * *Files identical despite different names*

### Comparing `threedidepth-0.5/test/test_calculate.py` & `threedidepth-0.6.1/test/test_calculate.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,21 +324,25 @@
 
     # prepare gridadmin uses
     admin.cells.get_nodgrid.return_value = nodgrid[tuple(map(slice, *indices))]
     admin.variable = "s1"
     if mode in (MODE_CONSTANT_S1):
         data = {"id": ids, "s1": s1}
         admin.nodes.subset().timeseries().only().data = data
+        admin.nodes.subset().only().data = data
     if mode in (MODE_LINEAR_S1):
-        data = {"coordinates": coordinates, "s1": s1}
+        data = {"id": ids, "coordinates": coordinates, "s1": s1}
         admin.nodes.subset().timeseries().only().data = data
+        admin.nodes.subset().only().data = data
     if mode in (MODE_LIZARD_S1):
         admin.nodes.subset().timeseries().only.side_effect = [
-            mock.Mock(data={"id": ids, "s1": s1}),
-            mock.Mock(data={"coordinates": coordinates, "s1": s1}),
+            mock.Mock(data={"id": ids, "coordinates": coordinates, "s1": s1})
+        ]
+        admin.nodes.subset().only.side_effect = [
+            mock.Mock(data={"id": ids, "coordinates": coordinates, "s1": s1})
         ]
 
     indexes = slice(7, 8)
     calculator_kwargs = {
         "result_admin": admin,
         "calculation_step": indexes.start,
         "dem_shape": nodgrid.shape,
@@ -363,27 +367,27 @@
             [2, 0, 6, 3],
             subset_name=SUBSET_2D_OPEN_WATER,
         )
     if mode in (MODE_LINEAR_S1):
         admin.nodes.subset.assert_called_with(SUBSET_2D_OPEN_WATER)
         admin.nodes.subset().timeseries.assert_called_with(indexes=indexes)
         admin.nodes.subset().timeseries().only.assert_called_with(
-            "s1", "coordinates",
+            "s1", "id",
         )
     if mode in (MODE_CONSTANT_S1):
         admin.nodes.subset.assert_called_with(SUBSET_2D_OPEN_WATER)
         admin.nodes.subset().timeseries.assert_called_with(indexes=indexes)
         admin.nodes.subset().timeseries().only.assert_called_with(
             "s1", "id",
         )
     if mode in (MODE_LIZARD_S1):
         admin.nodes.subset.assert_called_with(SUBSET_2D_OPEN_WATER)
         admin.nodes.subset().timeseries.assert_called_with(indexes=indexes)
         admin.nodes.subset().timeseries().only.assert_has_calls(
-            [mock.call("s1", "id"), mock.call("s1", "coordinates")]
+            [mock.call("s1", "id")]
         )
 
 
 @fixture
 def depthmock():
     import_path = (
         "threedidepth.calculate.BaseCalculator._depth_from_water_level"
```

### Comparing `threedidepth-0.5/test/test_commands.py` & `threedidepth-0.6.1/test/test_commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,27 +16,43 @@
         wd.assert_called_with(
             gridadmin_path="a",
             results_3di_path="b",
             dem_path="c",
             waterdepth_path="d",
             calculation_steps=None,
             mode=commands.MODE_LIZARD,
+            calculate_maximum_waterlevel=False,
             progress_func=None,
             netcdf=False
         )
         args.append("--constant")
         with mock.patch.object(sys, "argv", args):
             commands.threedidepth()
         wd.assert_called_with(
             gridadmin_path="a",
             results_3di_path="b",
             dem_path="c",
             waterdepth_path="d",
             calculation_steps=None,
             mode=commands.MODE_CONSTANT,
+            calculate_maximum_waterlevel=False,
+            progress_func=None,
+            netcdf=False
+        )
+        args.append("--maximum")
+        with mock.patch.object(sys, "argv", args):
+            commands.threedidepth()
+        wd.assert_called_with(
+            gridadmin_path="a",
+            results_3di_path="b",
+            dem_path="c",
+            waterdepth_path="d",
+            calculation_steps=None,
+            mode=commands.MODE_CONSTANT,
+            calculate_maximum_waterlevel=True,
             progress_func=None,
             netcdf=False
         )
 
 
 def test_command_with_multiple_steps(tmpdir):
     depth_path = tmpdir.join("waterdepth.tif")
@@ -48,10 +64,11 @@
         wd.assert_called_with(
             gridadmin_path="a",
             results_3di_path="b",
             dem_path="c",
             waterdepth_path="d",
             calculation_steps=[1, 2, 3],
             mode=commands.MODE_LIZARD,
+            calculate_maximum_waterlevel=False,
             progress_func=None,
             netcdf=False
         )
```

### Comparing `threedidepth-0.5/src/threedidepth/calculate.py` & `threedidepth-0.6.1/src/threedidepth/calculate.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from itertools import product
 from os import path
 
 from osgeo import gdal
 from osgeo import osr
 from scipy.interpolate import LinearNDInterpolator
-from scipy.spatial import qhull
+from scipy.spatial import Delaunay
 import h5netcdf.legacyapi as netCDF4
 import h5py
 import numpy as np
 
 from threedigrid.admin.gridresultadmin import GridH5ResultAdmin
 from threedigrid.admin.gridresultadmin import GridH5AggregateResultAdmin
 from threedigrid.admin.constants import SUBSET_2D_OPEN_WATER
@@ -40,18 +40,24 @@
 
     PIXEL_MAP = "pixel_map"
     LOOKUP_S1 = "lookup_s1"
     INTERPOLATOR = "interpolator"
     DELAUNAY = "delaunay"
 
     def __init__(
-        self, result_admin, calculation_step, dem_shape, dem_geo_transform,
+        self, result_admin, dem_shape, dem_geo_transform,
+        calculation_step=None, get_max_level=False
     ):
+        if calculation_step is None and not get_max_level:
+            raise ValueError(
+                "a calculation_step is required unless get_max_level is True"
+            )
         self.ra = result_admin
         self.calculation_step = calculation_step
+        self.get_max_level = get_max_level
         self.dem_shape = dem_shape
         self.dem_geo_transform = dem_geo_transform
 
     def __call__(self, indices, values, no_data_value):
         """Return result values array.
 
         Args:
@@ -80,77 +86,91 @@
         # paste positive depths only
         negative_1d = depth_1d <= 0
         depth_1d[negative_1d] = fillvalue
         depth[active] = depth_1d
 
         return depth
 
-    @property
-    def indexes(self):
-        return slice(self.calculation_step, self.calculation_step + 1)
+    @staticmethod
+    def indexes(calculation_step):
+        return slice(calculation_step, calculation_step + 1)
 
     @property
     def lookup_s1(self):
         """
         Return the lookup table to find waterlevel by cell id.
 
         Both cells outside any defined grid cell and cells in a grid cell that
         are currently not active ('no data') will return the NO_DATA_VALUE as
         defined in threedigrid.
         """
         try:
             return self.cache[self.LOOKUP_S1]
         except KeyError:
             nodes = self.ra.nodes.subset(SUBSET_2D_OPEN_WATER)
-            timeseries = nodes.timeseries(indexes=self.indexes)
-            data = timeseries.only(self.ra.variable, "id").data
+            if self.get_max_level:
+                # array van Ntimesteps * Nnodes
+                timeseries = nodes.timeseries(
+                    indexes=slice(0, self.ra.calculation_steps)
+                )
+                data = timeseries.only(self.ra.variable, "id").data
+                s1 = np.max(data[self.ra.variable], axis=0)
+            else:
+                timeseries = nodes.timeseries(
+                    indexes=self.indexes(self.calculation_step)
+                )
+                data = timeseries.only(self.ra.variable, "id").data
+                s1 = data[self.ra.variable][0]
             lookup_s1 = np.full((data["id"]).max() + 1, NO_DATA_VALUE)
-            lookup_s1[data["id"]] = data[self.ra.variable][0]
+            lookup_s1[data["id"]] = s1
             self.cache[self.LOOKUP_S1] = lookup_s1
         return lookup_s1
 
     @property
+    def coordinates(self):
+        nodes = self.ra.nodes.subset(SUBSET_2D_OPEN_WATER)
+        data = nodes.only("id", "coordinates").data
+        # transpose does:
+        # [[x1, x2, x3], [y1, y2, y3]] --> [[x1, y1], [x2, y2], [x3, y3]]
+        points = data["coordinates"].transpose()
+        ids = data["id"]
+        return points, ids
+
+    @property
     def interpolator(self):
         try:
             return self.cache[self.INTERPOLATOR]
         except KeyError:
-            nodes = self.ra.nodes.subset(SUBSET_2D_OPEN_WATER)
-            timeseries = nodes.timeseries(indexes=self.indexes)
-            data = timeseries.only(self.ra.variable, "coordinates").data
-            points = data["coordinates"].transpose()
-            values = data[self.ra.variable][0]
+            points, ids = self.coordinates
+            s1 = self.lookup_s1[ids]
             interpolator = LinearNDInterpolator(
-                points, values, fill_value=NO_DATA_VALUE
+                points, s1, fill_value=NO_DATA_VALUE
             )
             self.cache[self.INTERPOLATOR] = interpolator
             return interpolator
 
     @property
     def delaunay(self):
         """
-        Return a (delaunay, s1) tuple.
+        Return a (delaunay, ids) tuple.
 
-        `delaunay` is a qhull.Delaunay object, and `s1` is an array of
-        waterlevels for the corresponding delaunay vertices.
+        `delaunay` is a scipy.spatial.Delaunay object, and `ids` is an array of
+        ids for the corresponding simplices.
         """
         try:
             return self.cache[self.DELAUNAY]
         except KeyError:
-            nodes = self.ra.nodes.subset(SUBSET_2D_OPEN_WATER)
-            timeseries = nodes.timeseries(indexes=self.indexes)
-            data = timeseries.only(self.ra.variable, "coordinates").data
-            points = data["coordinates"].transpose()
-            s1 = data[self.ra.variable][0]
+            points, ids = self.coordinates
 
             # reorder a la lizard
-            points, s1 = morton.reorder(points, s1)
+            points, ids = morton.reorder(points, ids)
 
-            delaunay = qhull.Delaunay(points)
-            self.cache[self.DELAUNAY] = delaunay, s1
-            return delaunay, s1
+            delaunay = Delaunay(points)
+            self.cache[self.DELAUNAY] = delaunay, ids
+            return delaunay, ids
 
     def _get_nodgrid(self, indices):
         """Return node grid.
 
         Args:
             indices (tuple): ((i1, j1), (i2, j2)) subarray indices
         """
@@ -228,37 +248,38 @@
         used."""
         # start with the constant level result
         nodgrid = self._get_nodgrid(indices).ravel()
         level = self.lookup_s1[nodgrid]
 
         # determine result raster cell centers and in which triangle they are
         points = self._get_points(indices)
-        delaunay, s1 = self.delaunay
+        delaunay, ids = self.delaunay
+        s1 = self.lookup_s1[ids]
         simplices = delaunay.find_simplex(points)
 
         # determine which points will use interpolation
         in_gridcell = nodgrid != 0
         in_triangle = simplices != -1
         in_interpol = in_gridcell & in_triangle
         points = points[in_interpol]
 
         # get the nodes and the transform for the corresponding triangles
         transform = delaunay.transform[simplices[in_interpol]]
-        vertices = delaunay.vertices[simplices[in_interpol]]
+        simplices = delaunay.simplices[simplices[in_interpol]]
 
         # calculate weight, see print(spatial.Delaunay.transform.__doc__) and
         # Wikipedia about barycentric coordinates
-        weight = np.empty(vertices.shape)
+        weight = np.empty(simplices.shape)
         weight[:, :2] = np.sum(
             transform[:, :2] * (points - transform[:, 2])[:, np.newaxis], 2
         )
         weight[:, 2] = 1 - weight[:, 0] - weight[:, 1]
 
         # set weight to zero when for inactive nodes
-        nodelevel = s1[vertices]
+        nodelevel = s1[simplices]
         weight[nodelevel == NO_DATA_VALUE] = 0
 
         # determine the sum of weights per result cell
         weight_sum = weight.sum(axis=1)
 
         # further subselect points suitable for interpolation
         suitable = weight_sum > 0.5
@@ -438,28 +459,31 @@
 
     def __init__(
             self,
             source_path,
             target_path,
             result_admin,
             calculation_steps,
+            write_time_dimension=True,
             **kwargs
     ):
         kwargs["band_count"] = len(calculation_steps)
         super().__init__(source_path, target_path, **kwargs)
 
         self.ra = result_admin
         self.calculation_steps = calculation_steps
+        self.write_time_dimension = write_time_dimension
 
     def __enter__(self):
         """Open datasets"""
         self.source = gdal.Open(self.source_path, gdal.GA_ReadOnly)
         self.target = netCDF4.Dataset(self.target_path, "w")
         self._set_coords()
-        self._set_time()
+        if self.write_time_dimension:
+            self._set_time()
         self._set_meta_info()
         self._create_variable()
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Close datasets"""
@@ -531,15 +555,15 @@
             f"EPSG:{self.ra.epsg_code}"
         )  # for GDAL
 
     def _create_variable(self):
         water_depth = self.target.createVariable(
             "water_depth",
             "f4",
-            ("time", "y", "x",),
+            ("time", "y", "x",) if self.write_time_dimension else ("y", "x",),
             fill_value=-9999,
             zlib=True
         )
         water_depth.long_name = "water depth"
         water_depth.units = "m"
         water_depth.grid_mapping = "projected_coordinate_system"
 
@@ -559,15 +583,20 @@
                 indices=indices,
                 values=values,
                 no_data_value=no_data_value,
             )
 
             # write
             water_depth = self.target['water_depth']
-            water_depth[band, yoff:yoff + ysize, xoff:xoff + xsize] = result
+            if self.write_time_dimension:
+                water_depth[
+                    band, yoff:yoff + ysize, xoff:xoff + xsize
+                ] = result
+            else:
+                water_depth[yoff:yoff + ysize, xoff:xoff + xsize] = result
 
 
 class ProgressClass:
     """ Progress function and calculation step iterator in one.
 
     Args:
         calculation_steps (list(int)): Calculation steps
@@ -653,14 +682,15 @@
 
 def calculate_waterdepth(
     gridadmin_path,
     results_3di_path,
     dem_path,
     waterdepth_path,
     calculation_steps=None,
+    calculate_maximum_waterlevel=False,
     mode=MODE_LIZARD,
     progress_func=None,
     netcdf=False,
 ):
     """Calculate waterdepth and save it as GeoTIFF.
 
     Args:
@@ -677,14 +707,16 @@
         raise ValueError("Unknown mode: '%s'" % mode)
 
     result_admin = ResultAdmin(
         gridadmin_path=gridadmin_path, results_3di_path=results_3di_path,
     )
 
     # handle calculation step
+    if calculate_maximum_waterlevel:
+        calculation_steps = [0]
     max_calculation_step = result_admin.calculation_steps - 1
     if calculation_steps is None:
         calculation_steps = [max_calculation_step]
     else:
         assert min(calculation_steps) >= 0
         assert max(calculation_steps) <= max_calculation_step, (
             "Maximum calculation step is '%s'." % max_calculation_step
@@ -701,24 +733,29 @@
         "target_path": waterdepth_path,
         "progress_func": None if progress_func is None else progress_class,
     }
     if netcdf:
         converter_class = NetcdfConverter
         converter_kwargs['result_admin'] = result_admin
         converter_kwargs['calculation_steps'] = calculation_steps
+        converter_kwargs[
+            'write_time_dimension'
+        ] = not calculate_maximum_waterlevel
     else:
         converter_class = GeoTIFFConverter
         converter_kwargs['band_count'] = len(calculation_steps)
 
     with converter_class(**converter_kwargs) as converter:
         calculator_kwargs_except_step = {
             "result_admin": result_admin,
             "dem_geo_transform": converter.geo_transform,
             "dem_shape": (converter.raster_y_size, converter.raster_x_size),
+            "get_max_level": calculate_maximum_waterlevel
         }
+
         for band, calculation_step in progress_class:
             calculator_kwargs = {
                 "calculation_step": calculation_step,
                 **calculator_kwargs_except_step,
             }
 
             with CalculatorClass(**calculator_kwargs) as calculator:
```

### Comparing `threedidepth-0.5/src/threedidepth/morton.py` & `threedidepth-0.6.1/src/threedidepth/morton.py`

 * *Files identical despite different names*

### Comparing `threedidepth-0.5/src/threedidepth/commands.py` & `threedidepth-0.6.1/src/threedidepth/commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,22 +24,29 @@
         "dem_path", metavar="dem", help="path to bathymetry file"
     )
     parser.add_argument(
         "waterdepth_path",
         metavar="waterdepth",
         help="path to resulting geotiff"
     )
-    parser.add_argument(
+    calculation_type_group = parser.add_mutually_exclusive_group()
+    calculation_type_group.add_argument(
         "-s",
         "--steps",
         nargs="+",
         type=int,
         dest="calculation_steps",
         help="simulation result step(s)",
     )
+    calculation_type_group.add_argument(
+        "--maximum",
+        action="store_true",
+        dest="calculate_maximum_waterlevel",
+        help="calculate maximum waterlevel instead of waterlevel per timestep",
+    )
     parser.add_argument(
         "-c",
         "--constant",
         action="store_true",
         help="disable interpolation and use constant waterlevel per grid cell",
     )
     parser.add_argument(
```

### Comparing `threedidepth-0.5/src/threedidepth/fixes.py` & `threedidepth-0.6.1/src/threedidepth/fixes.py`

 * *Files identical despite different names*

### Comparing `threedidepth-0.5/src/threedidepth.egg-info/SOURCES.txt` & `threedidepth-0.6.1/src/threedidepth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `threedidepth-0.5/setup.py` & `threedidepth-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- encoding: utf-8 -*-
 from glob import glob
 from os.path import basename
 from os.path import splitext
 from setuptools import find_packages
 from setuptools import setup
 
-version = '0.5'
+version = '0.6.1'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('CHANGES.rst') as changes_file:
     changes = changes_file.read()
```

### Comparing `threedidepth-0.5/CHANGES.rst` & `threedidepth-0.6.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog of threedidepth
 =========================
 
 
+0.6.1 (2023-07-11)
+------------------
+
+- Add release action for automatic upload to GitHub and PyPI.
+
+
+0.6.0 (2023-07-10)
+------------------
+
+- Update dependency versions
+- Add support for calculating maximum waterlevel as well as per timestep.
+
+
 0.5 (2021-07-02)
 ----------------
 
 - Added support for result type 'aggregate'.
 
 - Got rid of NetCDF4 dependency by using h5netcdf.
```

### Comparing `threedidepth-0.5/Dockerfile` & `threedidepth-0.6.1/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM ubuntu:bionic
+FROM ubuntu:jammy
 
 LABEL maintainer="arjan.verkerk@nelen-schuurmans.nl"
 
 # Get rid of debconf messages like "unable to initialize frontend: Dialog".
 # https://github.com/docker/docker/issues/4032#issuecomment-192327844
 ARG DEBIAN_FRONTEND=noninteractive
 
@@ -11,14 +11,18 @@
 # for writing Dockerfiles". https://docs.docker.com/engine/userguide/↵
 # eng-image/dockerfile_best-practices/
 RUN apt-get update && apt-get install -y \
     git \
     locales \
     python3-pip \
     python3-gdal \
+    python3-dev \
+    libcairo2-dev \
+    pkg-config \
+    libgirepository1.0-dev \
     && rm -rf /var/lib/apt/lists/*
 
 RUN locale-gen en_US.UTF-8
 ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
 
 RUN pip3 install --upgrade pip virtualenv
```

