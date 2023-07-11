# Comparing `tmp/codem-0.25.1.tar.gz` & `tmp/codem-0.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codem-0.25.1.tar", last modified: Mon May  8 20:56:26 2023, max compression
+gzip compressed data, was "codem-0.25.2.tar", last modified: Tue Jul 11 17:45:55 2023, max compression
```

## Comparing `codem-0.25.1.tar` & `codem-0.25.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 20:56:07.000000 codem-0.25.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-08 20:56:26.755257 codem-0.25.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-08 20:56:07.000000 codem-0.25.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-08 20:56:07.000000 codem-0.25.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:56:26.755257 codem-0.25.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.751257 codem-0.25.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.751257 codem-0.25.1/src/codem/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/lib/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29467 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    24882 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/dsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/icp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/vcd/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/vcd/meshing/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/meshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/meshing/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/vcd/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-08 20:56:08.000000 codem-0.25.1/tests/test_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.871037 codem-0.25.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 17:45:37.000000 codem-0.25.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-11 17:45:55.871037 codem-0.25.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-11 17:45:38.000000 codem-0.25.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-11 17:45:38.000000 codem-0.25.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:45:55.871037 codem-0.25.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.863037 codem-0.25.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/lib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32538 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24882 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/dsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/icp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/vcd/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/vcd/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/meshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/meshing/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/vcd/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.871037 codem-0.25.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-11 17:45:38.000000 codem-0.25.2/tests/test_registration.py
```

### Comparing `codem-0.25.1/LICENSE` & `codem-0.25.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codem-0.25.1/PKG-INFO` & `codem-0.25.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.1
+Version: 0.25.2
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
```

### Comparing `codem-0.25.1/pyproject.toml` & `codem-0.25.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -87,17 +87,19 @@
   "pyproj.crs",
   "pyproj.database",
   "pyproj.enums",
   "pyproj.transformer",
   "rasterio",
   "rasterio.coords",
   "rasterio.crs",
+  "rasterio.errors",
   "rasterio.enums",
   "rasterio.fill",
   "rasterio.transform",
+  "rasterio.warp",
   "rich",
   "rich.console",
   "rich.logging",
   "rich.progress",
   "scipy",
   "scipy.sparse",
   "scipy.spatial",
```

### Comparing `codem-0.25.1/readme.md` & `codem-0.25.2/readme.md`

 * *Files identical despite different names*

### Comparing `codem-0.25.1/src/codem/lib/log.py` & `codem-0.25.2/src/codem/lib/log.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.1/src/codem/main.py` & `codem-0.25.2/src/codem/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,15 +410,15 @@
     else:
         resolution = max(fnd_obj.native_resolution, aoi_obj.native_resolution)
     fnd_obj.resolution = aoi_obj.resolution = resolution
 
     # create DSM, but if doing tight-search do not resample
     resample = not config["TIGHT_SEARCH"]
     fnd_obj._create_dsm(resample=resample)
-    aoi_obj._create_dsm(resample=resample)
+    aoi_obj._create_dsm(resample=resample, fallback_crs=fnd_obj.crs)
     return fnd_obj, aoi_obj
 
 
 def coarse_registration(
     fnd_obj: GeoData, aoi_obj: GeoData, config: Dict[str, Any]
 ) -> DsmRegistration:
     dsm_reg = DsmRegistration(fnd_obj, aoi_obj, config)
```

### Comparing `codem-0.25.1/src/codem/preprocessing/preprocess.py` & `codem-0.25.2/src/codem/preprocessing/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,22 @@
 import codem.lib.resources as r
 import cv2
 import numpy as np
 import pdal
 import pyproj
 import rasterio.fill
 import rasterio.transform
+import rasterio.warp
 import trimesh
 from rasterio import windows
 from rasterio.coords import BoundingBox
 from rasterio.coords import disjoint_bounds
 from rasterio.crs import CRS
 from rasterio.enums import Resampling
+from rasterio.errors import CRSError
 from typing_extensions import TypedDict
 
 
 class RegistrationParameters(TypedDict):
     matrix: np.ndarray
     omega: np.float64
     phi: np.float64
@@ -308,15 +310,17 @@
             (array["NormalX"], array["NormalY"], array["NormalZ"])
         ).T
         self.normal_vectors = filtered_normals
 
     def _calculate_resolution(self) -> None:
         raise NotImplementedError
 
-    def _create_dsm(self, resample: bool = True) -> None:
+    def _create_dsm(
+        self, resample: bool = True, fallback_crs: Optional[CRS] = None
+    ) -> None:
         raise NotImplementedError
 
     def prep(self) -> None:
         """
         Prepares data for registration.
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
@@ -351,15 +355,17 @@
     """
 
     def __init__(self, config: dict, fnd: bool) -> None:
         super().__init__(config, fnd)
         self.type = "dsm"
         self._calculate_resolution()
 
-    def _create_dsm(self, resample: bool = True) -> None:
+    def _create_dsm(
+        self, resample: bool = True, fallback_crs: Optional[CRS] = None
+    ) -> None:
         """
         Resamples the DSM to the registration pipeline resolution and applies
         a scale factor to convert to meters.
         """
 
         with rasterio.open(self.file) as data:
             resample_factor = (
@@ -404,14 +410,45 @@
                 if self.window is None:
                     self.transform = data.transform
                 else:
                     self.transform = data.window_transform(self.window)
             self.nodata = data.nodata
             self.crs = data.crs
 
+            if all(
+                (
+                    not self.fnd,  # the dataset is the compliment
+                    (
+                        self.crs is not None
+                        and not self.crs.is_projected  # the CRS is not projected
+                    ),
+                ),
+            ):
+                # handle the case where compliment has a non-projected CRS
+                transform, width, height = rasterio.warp.calculate_default_transform(
+                    CRS.from_epsg("4326"),
+                    fallback_crs,
+                    self.dsm.shape[0],
+                    self.dsm.shape[1],
+                    *data.bounds,
+                )
+                dsm = np.zeros((width, height), dtype=self.dsm.dtype)
+                _, transform = rasterio.warp.reproject(
+                    source=rasterio.band(data, 1),
+                    destination=dsm,
+                    dst_transform=transform,
+                    dst_crs=fallback_crs,
+                    dst_nodata=data.nodata,
+                    resampling=Resampling.cubic,
+                )
+
+                self.transform = transform
+                self.crs = fallback_crs
+                self.dsm = dsm
+
             # Scale the elevation values into meters
             mask = (self._get_nodata_mask(self.dsm)).astype(bool)
             if np.can_cast(self.units_factor, self.dsm.dtype, casting="same_kind"):
                 self.dsm[mask] *= self.units_factor
             elif isinstance(self.units_factor, float):
                 if self.units_factor.is_integer():
                     self.dsm[mask] *= int(self.units_factor)
@@ -442,14 +479,15 @@
             elif "AREA_OR_POINT" in tags and tags["AREA_OR_POINT"] == "Point":
                 self.area_or_point = "Point"
             else:
                 self.area_or_point = "Area"
                 self.logger.debug(
                     f"'AREA_OR_POINT' not supplied in {tag}-{self.type.upper()} - defaulting to 'Area'"
                 )
+
         if self.nodata is None:
             self.logger.info(f"{tag}-{self.type.upper()} does not have a nodata value.")
         if self.transform == rasterio.Affine.identity():
             self.logger.warning(f"{tag}-{self.type.upper()} has an identity transform.")
 
     def _calculate_resolution(self) -> None:
         """
@@ -477,14 +515,48 @@
             tag = ["AOI", "Foundation"][int(self.fnd)]
             if data.crs is None:
                 self.logger.warning(
                     f"Linear unit for {tag}-{self.type.upper()} not detected -> "
                     "meters assumed"
                 )
                 self.native_resolution = abs(T.a)
+                self.units = "m"
+            elif not data.crs.is_valid:
+                self.logger.warning(
+                    f"CRS {data.crs.to_wkt()} is not valid, assuming linear units "
+                    "are meters."
+                )
+                self.native_resolution = abs(T.a)
+                self.units = "m"
+            elif not data.crs.is_projected:
+                self.logger.info("CRS is not projected, converting to meters")
+
+                # determine appropriate UTM CRSs
+                utm_crs_list = pyproj.database.query_utm_crs_info(
+                    datum_name="WGS 84",
+                    area_of_interest=pyproj.aoi.AreaOfInterest(
+                        west_lon_degree=T.c,
+                        south_lat_degree=T.f,
+                        east_lon_degree=T.c,
+                        north_lat_degree=T.f,
+                    ),
+                )
+                best_guess_crs = CRS.from_epsg(utm_crs_list[0].code)
+
+                # transform from GCS to UTM for resolution purposes
+                T, _, _ = rasterio.warp.calculate_default_transform(
+                    CRS.from_epsg("4326"),
+                    best_guess_crs,
+                    data.width,
+                    data.height,
+                    *data.bounds,
+                )
+                self.native_resolution = abs(T.a)
+                self.crs = best_guess_crs
+                self.units = "m"
             else:
                 self.logger.info(
                     f"Linear unit for {tag}-{self.type.upper()} detected as "
                     f"{data.crs.linear_units}"
                 )
                 self.units_factor = data.crs.linear_units_factor[1]
                 self.units = data.crs.linear_units
@@ -501,15 +573,17 @@
     """
 
     def __init__(self, config: dict, fnd: bool) -> None:
         super().__init__(config, fnd)
         self.type = "pcloud"
         self._calculate_resolution()
 
-    def _create_dsm(self, resample: bool = True) -> None:
+    def _create_dsm(
+        self, resample: bool = True, fallback_crs: Optional[CRS] = None
+    ) -> None:
         """
         Converts the point cloud to meters and rasters it to a DSM.
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
         self.logger.info(
             f"Extracting DSM from {tag}-{self.type.upper()} with resolution of: {self.resolution} meters"
         )
@@ -543,59 +617,66 @@
         os.close(file_handle)
         os.remove(tmp_file)
 
     def _calculate_resolution(self) -> None:
         """
         Calculates point cloud average point spacing.
         """
-        pdal_pipeline = [
-            self.file,
-            {"type": "filters.hexbin", "edge_size": 25, "threshold": 1},
-        ]
-        pipeline = pdal.Pipeline(json.dumps(pdal_pipeline))
+        tag = ["AOI", "Foundation"][int(self.fnd)]
+
+        pipeline = pdal.Reader(self.file)
+        pipeline |= pdal.Filter.hexbin(edge_size=25, threshold=1)
         pipeline.execute()
 
-        tag = ["AOI", "Foundation"][int(self.fnd)]
         metadata = pipeline.metadata["metadata"]
         reader_metadata = [val for key, val in metadata.items() if "readers" in key]
-        if reader_metadata[0]["srs"]["horizontal"] == "":
+        try:
+            crs = CRS.from_string(reader_metadata[0]["srs"]["horizontal"])
+        except (CRSError, IndexError, KeyError):
+            crs = None
+        if crs is None:
             self.logger.warning(
                 f"Linear unit for {tag}-{self.type.upper()} not detected --> meters assumed"
             )
-            spacing = metadata["filters.hexbin"]["avg_pt_spacing"]
+            self.units_factor = 1.0
+            self.units = "m"
+        elif not crs.is_projected:
+            self.logger.warning(
+                f"Coordinate system for {tag}-{self.type.upper()} not projected --> meters assumed"
+            )
+            self.units_factor = 1.0
+            self.units = "m"
         else:
-            crs = CRS.from_string(reader_metadata[0]["srs"]["horizontal"])
             self.logger.info(
                 f"Linear unit for {tag}-{self.type.upper()} detected as {crs.linear_units}."
             )
-            spacing = (
-                crs.linear_units_factor[1]
-                * metadata["filters.hexbin"]["avg_pt_spacing"]
-            )
             self.units_factor = crs.linear_units_factor[1]
             self.units = crs.linear_units
-
+        self.native_resolution = (
+            self.units_factor * metadata["filters.hexbin"]["avg_pt_spacing"]
+        )
         self.logger.info(
-            f"Calculated native resolution for {tag}-{self.type.upper()} as: {spacing:.1f} meters"
+            f"Calculated native resolution for {tag}-{self.type.upper()} as: "
+            f"{self.native_resolution :.1f} meters"
         )
 
-        self.native_resolution = spacing
-
 
 class Mesh(GeoData):
     """
     A class for storing and preparing Mesh data.
     """
 
     def __init__(self, config: dict, fnd: bool) -> None:
         super().__init__(config, fnd)
         self.type = "mesh"
         self._calculate_resolution()
 
-    def _create_dsm(self, resample: bool = True) -> None:
+    def _create_dsm(
+        self, resample: bool = True, fallback_crs: Optional[CRS] = None
+    ) -> None:
         """
         Converts mesh vertices to meters and rasters them to a DSM.
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
         self.logger.info(
             f"Extracting DSM from {tag}-{self.type.upper()} with resolution of: {self.resolution} meters"
         )
```

### Comparing `codem-0.25.1/src/codem/registration/apply.py` & `codem-0.25.2/src/codem/registration/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         self.logger = logging.getLogger(__name__)
         self.fnd_crs = fnd_obj.crs
         self.fnd_units_factor = fnd_obj.units_factor
         self.fnd_units = fnd_obj.units
         self.aoi_file = aoi_obj.file
         self.aoi_nodata = aoi_obj.nodata
         self.aoi_resolution = aoi_obj.native_resolution
+        self.aoi_crs = aoi_obj.crs
         self.aoi_units_factor = aoi_obj.units_factor
         self.aoi_type = aoi_obj.type
         self.aoi_area_or_point = aoi_obj.area_or_point
         self.registration_transform = registration_parameters["matrix"]
         self.registration_rmse = registration_parameters["rmse_3d"]
         self.residual_vectors = residual_vectors
         self.residual_origins = residual_origins
@@ -125,22 +126,17 @@
         if self.aoi_type == "mesh":
             return aoi_to_fnd_array
         else:
             aoi_to_fnd_array = np.reshape(aoi_to_fnd_array, (1, 16))
             aoi_to_fnd_string = [
                 " ".join(item) for item in aoi_to_fnd_array.astype(str)
             ][0]
-            if self.fnd_crs is not None:
-                registration_transformation = pdal.Filter.transformation(
-                    matrix=aoi_to_fnd_string, override_srs=self.fnd_crs.to_string()
-                )
-            else:
-                registration_transformation = pdal.Filter.transforamtion(
-                    matrix=aoi_to_fnd_string
-                )
+            registration_transformation = pdal.Filter.transformation(
+                matrix=aoi_to_fnd_string
+            )
             return registration_transformation
 
     def apply(self) -> None:
         """
         Call the appropriate registration function depending on data type
         """
         if os.path.splitext(self.aoi_file)[-1] in r.dsm_filetypes:
@@ -157,24 +153,30 @@
         generally used to express 2D information. Instead, we apply the solved
         3D transformation to the 2.5D data and "re-raster" it.
         """
         input_name = os.path.basename(self.aoi_file)
         root, ext = os.path.splitext(input_name)
         output_name = f"{root}_registered{ext}"
         output_path = os.path.join(self.config["OUTPUT_DIR"], output_name)
-
         # construct pdal pipeline
-        pipeline = pdal.Reader.gdal(filename=self.aoi_file, header="Z")
+        pipeline = pdal.Reader.gdal(
+            filename=self.aoi_file,
+            header="Z",
+        )
 
         # no nodata is present, filter based on its limits
         if self.aoi_nodata is not None:
             pipeline |= pdal.Filter.range(
                 limits=f"Z![{self.aoi_nodata}:{self.aoi_nodata}]"
             )
 
+        # handle the case where the AOI underwent a CRS change
+        if self.aoi_crs is not None:  # if statement to satisfy mypy
+            pipeline |= pdal.Filter.reprojection(out_srs=self.aoi_crs.to_wkt())
+
         # insert the transform filter to register the AOI
         registration_task = self.get_registration_transformation()
         if isinstance(registration_task, pdal.pipeline.Filter):
             pipeline |= registration_task
         else:
             raise ValueError(
                 f"get_registration_transformation returned {type(registration_task)} "
@@ -334,15 +336,19 @@
 
     def _apply_pointcloud(self) -> None:
         """
         Applies the registration transformation to a point cloud file.
         """
         pipeline = pdal.Reader(self.aoi_file)
         pipeline |= self.get_registration_transformation()
-        pipeline |= pdal.Writer.las(filename=self.out_name)
+
+        writer_kwargs = {"filename": self.out_name}
+        if self.fnd_crs is not None:
+            writer_kwargs["a_srs"] = self.fnd_crs.to_wkt()
+        pipeline |= pdal.Writer.las(**writer_kwargs)
 
         pipeline.execute()
         self.logger.info(
             f"Registration has been applied to AOI-PCLOUD and saved to: {self.out_name}"
         )
 
         if self.config["ICP_SAVE_RESIDUALS"]:
```

### Comparing `codem-0.25.1/src/codem/registration/dsm.py` & `codem-0.25.2/src/codem/registration/dsm.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.1/src/codem/registration/icp.py` & `codem-0.25.2/src/codem/registration/icp.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.1/src/codem.egg-info/PKG-INFO` & `codem-0.25.2/src/codem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.1
+Version: 0.25.2
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
```

### Comparing `codem-0.25.1/src/codem.egg-info/SOURCES.txt` & `codem-0.25.2/src/codem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codem-0.25.1/src/vcd/main.py` & `codem-0.25.2/src/vcd/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,17 +71,20 @@
     AFTER: str
     SPACING: float = 0.43
     GROUNDHEIGHT: float = 1.0
     RESOLUTION: float = 2.0
     VERBOSE: bool = False
     MIN_POINTS: int = 30
     CLUSTER_TOLERANCE: float = 2.0
-    CULL_CLUSTER_IDS: Tuple[int, ...] = (-1, 0, 1)
+    CULL_CLUSTER_IDS: Tuple[int, ...] = (-1, 0)
+    CLASS_LABELS: Tuple[int, ...] = (2, 6)
     OUTPUT_DIR: Optional[str] = None
     COLORMAP: str = "RdBu"
+    TRUST_LABELS: bool = False
+    COMPUTE_HAG: bool = False
 
     def __post_init__(self) -> None:
         # set output directory
         if self.OUTPUT_DIR is None:
             current_time = time.localtime(time.time())
             timestamp = "%d-%02d-%02d_%02d-%02d-%02d" % (
                 current_time.tm_year,
@@ -163,15 +166,21 @@
         default=VcdRunConfig.CLUSTER_TOLERANCE,
         help="Cluster tolerance used by pdal.Filter.cluster",
     )
     ap.add_argument(
         "--cull_cluster_ids",
         type=str,
         default=",".join(map(str, VcdRunConfig.CULL_CLUSTER_IDS)),
-        help="Coma separated list of cluster IDs to cull when producing the meshes",
+        help="Comma separated list of cluster IDs to cull when producing the meshes",
+    )
+    ap.add_argument(
+        "--class_labels",
+        type=str,
+        default=",".join(map(str, VcdRunConfig.CLASS_LABELS)),
+        help="Comma separated list of classification labels to use when producing the meshes",
     )
     ap.add_argument(
         "-v", "--verbose", action="count", default=0, help="turn on verbose logging"
     )
     ap.add_argument(
         "--colormap",
         type=str,
@@ -179,14 +188,31 @@
         help=(
             "Colormap to apply to generated output files where supported.  Name has "
             "to align with a matplotlib named colormap.  See "
             "https://matplotlib.org/stable/tutorials/colors/colormaps.html#diverging "
             "for list of options."
         ),
     )
+    ap.add_argument(
+        "--trust_labels",
+        action="store_true",
+        help=(
+            "Trusts existing classification labels in the removal of vegetation/noise, "
+            "otherwise return information is used to approximate vegetation/noise "
+            "detection."
+        ),
+    )
+    ap.add_argument(
+        "--compute_hag",
+        action="store_true",
+        help=(
+            "Compute height above ground between after scan (non-ground) and before "
+            "scan (ground), otherwise compute to nearest neighbor from after to before."
+        ),
+    )
     args = ap.parse_args()
     return args
 
 
 def create_config(args: argparse.Namespace) -> Dict[str, Any]:
     config = VcdRunConfig(
         os.fsdecode(os.path.abspath(args.before)),
@@ -194,14 +220,17 @@
         SPACING=float(args.spacing_override),
         VERBOSE=args.verbose,
         GROUNDHEIGHT=float(args.ground_height),
         RESOLUTION=float(args.resolution),
         MIN_POINTS=int(args.min_points),
         CLUSTER_TOLERANCE=float(args.cluster_tolerance),
         CULL_CLUSTER_IDS=tuple(map(int, args.cull_cluster_ids.split(","))),
+        CLASS_LABELS=tuple(map(int, args.class_labels.split(","))),
+        TRUST_LABELS=args.trust_labels,
+        COMPUTE_HAG=args.compute_hag,
     )
     return dataclasses.asdict(config)
 
 
 def run_console(
     config: VCDParameters, logger: logging.Logger, console: Console
 ) -> None:
@@ -257,16 +286,15 @@
         progress.advance(registration, 15)
         console.print("══════════ Rasterizing products ", justify="center")
         v.rasterize()
         progress.advance(registration, 15)
         console.print("══════════ Meshing products ", justify="center")
 
         m = Mesh(v)
-        m.write("non-ground", m.cluster(v.ng_clusters))
-        m.write("ground", m.cluster(v.ground_clusters))
+        m.write("cluster", m.cluster(v.clusters))
 
         v.save()
         progress.advance(registration, 10)
 
 
 def main() -> None:
     args = get_args()
```

### Comparing `codem-0.25.1/src/vcd/meshing/mesh.py` & `codem-0.25.2/src/vcd/meshing/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
                 if len(arr):
                     cluster_id = arr[0][dimension]
                     print(
                         f"Not enough points to cluster {cluster_id}. We have {len(arr)} and need 5"
                     )
                 else:
                     print("Cluster has no points!")
+                continue
 
             x = arr["X"]
             y = arr["Y"]
             z = arr["Z"]
             cluster_id = arr[0][dimension]
             classification = arr[0]["Classification"]
             status = np.average(arr["dZ3d"])
```

### Comparing `codem-0.25.1/src/vcd/preprocessing/preprocess.py` & `codem-0.25.2/src/vcd/preprocessing/preprocess.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     RESOLUTION: np.float64
     OUTPUT_DIR: str
     BEFORE: str
     AFTER: str
     MIN_POINTS: int
     CLUSTER_TOLERANCE: float
     CULL_CLUSTER_IDS: Tuple[int, ...]
+    CLASS_LABELS: Tuple[int, ...]
     COLORMAP: str
+    TRUST_LABELS: bool
+    COMPUTE_HAG: bool
     log: Log
 
 
 class Product(NamedTuple):
     df: pd.DataFrame
     z_name: str
     description: str = ""
@@ -149,82 +152,107 @@
             self.logger.logger.info(f"Loaded {self.filename}")
 
         filters = _get_utm(filters)
 
         self.crs = filters.crs
         self.utm = filters.utm
 
-        filters |= pdal.Filter.range(limits="Classification![7:7]")
-        filters |= pdal.Filter.range(limits="Classification![18:)")
-        filters |= pdal.Filter.range(limits="Classification![9:9]")
-        filters |= pdal.Filter.returns(groups="only")
-        filters |= pdal.Filter.elm(cell=20.0)
-        filters |= pdal.Filter.outlier(where="Classification!=7")
-        filters |= pdal.Filter.range(limits="Classification![7:7]")
-        filters |= pdal.Filter.assign(assignment="Classification[:]=1")
-        filters |= pdal.Filter.smrf()
+        # Do not (fully) trust original classifications -- original workflow.
+        if not self.config["TRUST_LABELS"]:
+            filters |= pdal.Filter.range(limits="Classification![7:7]")
+            filters |= pdal.Filter.range(limits="Classification![18:)")
+            filters |= pdal.Filter.range(limits="Classification![9:9]")
+            filters |= pdal.Filter.returns(groups="only")
+            filters |= pdal.Filter.elm(cell=20.0)
+            filters |= pdal.Filter.outlier(where="Classification!=7")
+            filters |= pdal.Filter.range(limits="Classification![7:7]")
+            filters |= pdal.Filter.assign(assignment="Classification[:]=1")
+            filters |= pdal.Filter.smrf()
+
+        else:
+            filters |= pdal.Filter.returns(groups="only")
+        
         filters.execute()
         self.pipeline = filters
         return filters
 
 
 class VCD:
     def __init__(self, before: PointCloud, after: PointCloud) -> None:
         self.before = before
         self.after = after
         self.products: List[Product] = []
         self.gh = before.config["GROUNDHEIGHT"]
         self.resolution = before.config["RESOLUTION"]
+        self.trust_labels = before.config["TRUST_LABELS"]
+        self.compute_hag = before.config["COMPUTE_HAG"]
 
     def compute_indexes(self) -> None:
         after = self.after.df
         before = self.before.df
 
-        tree3d = cKDTree(before[["X", "Y", "Z"]])
-        d3d, i3d = tree3d.query(after[["X", "Y", "Z"]], k=1)
+        # Compute height as delta Z between nearest point in before cloud from the after cloud -- original workflow.
+        if not self.before.config["COMPUTE_HAG"]:
+            tree3d = cKDTree(before[["X", "Y", "Z"]])
+            _, i3d = tree3d.query(after[["X", "Y", "Z"]], k=1)
+            after["dZ3d"] = after.Z - before.iloc[i3d].Z.values
+        
+        # Compute height as HAG, treating after as non-ground and before as ground -- new workflow.
+        else:
+            # Assing after non-ground, before ground.
+            after["TempClassification"] = 1
+            before["TempClassification"] = 2
+
+            # Merge clouds.
+            allpoints = pd.concat([after, before])
+
+            # Stash original classifications, then compute HAG using TempClassification. Pop the original classifications.
+            pipeline = pdal.Pipeline(dataframes=[allpoints])
+            pipeline |= pdal.Filter.ferry(dimensions="TempClassification=>Classification")
+            pipeline |= pdal.Filter.hag_delaunay()
+            pipeline.execute()
 
-        after["dX3d"] = after.X - before.iloc[i3d].X.values
-        after["dY3d"] = after.Y - before.iloc[i3d].Y.values
-        after["dZ3d"] = after.Z - before.iloc[i3d].Z.values
+            # Assign HAG as dZ3d and d3 in keeping with the original approach.
+            result = pipeline.get_dataframe(0)
+            after["dZ3d"] = result["HeightAboveGround"]
 
-        after["d3"] = d3d
 
     def cluster(self) -> None:
         after = self.after.df
         gh = self.gh
 
-        array = after[(after.Classification != 2) & (after.d3 > gh)].to_records()
-        self.ng_clusters = pdal.Filter.cluster(
-            min_points=self.after.config["MIN_POINTS"],
-            tolerance=self.after.config["CLUSTER_TOLERANCE"],
-        ).pipeline(array)
-        self.ng_clusters.execute()
-        ng_cluster_df = pd.DataFrame(self.ng_clusters.arrays[0])
+        thresholdFilter = pdal.Filter.range(limits="dZ3d![-{gh}:{gh}]".format(gh=gh))
 
-        p = self.make_product(
-            ng_cluster_df.X,
-            ng_cluster_df.Y,
-            ng_cluster_df.ClusterID,
-            description=f"Non-ground clusters greater than {gh:.2f} height",
-        )
-        self.products.append(p)
+        conditions = [f"Classification=={id}" for id in self.after.config["CLASS_LABELS"]]
+        expression = " || ".join(conditions)
+        rangeFilter = pdal.Filter.expression(expression=expression)
 
-        array = after[(after.Classification == 2) & (after.d3 > gh)].to_records()
-        self.ground_clusters = pdal.Filter.cluster(
+        clusterFilter = pdal.Filter.cluster(
             min_points=self.after.config["MIN_POINTS"],
             tolerance=self.after.config["CLUSTER_TOLERANCE"],
-        ).pipeline(array)
-        self.ground_clusters.execute()
-        ground_cluster_df = pd.DataFrame(self.ground_clusters.arrays[0])
+        )
+
+        conditions = [f"ClusterID!={id}" for id in self.after.config["CULL_CLUSTER_IDS"]]
+        expression = " && ".join(conditions)
+        clusterIdFilter = pdal.Filter.expression(expression=expression)
+
+        array = after.to_records()
+        self.clusters = pdal.Pipeline([thresholdFilter, rangeFilter, clusterFilter, clusterIdFilter], [array])
+        self.clusters.execute()
+        cluster_df = pd.DataFrame(self.clusters.arrays[0])
+
+        # Encode the size of each cluster as a new dimension for analysis.
+        cluster_df['ClusterSize'] = cluster_df.groupby(['ClusterID'])['ClusterID'].transform('count')
+        self.cluster_sizes = cluster_df["ClusterSize"].to_numpy()
 
         p = self.make_product(
-            ground_cluster_df.X,
-            ground_cluster_df.Y,
-            ground_cluster_df.ClusterID,
-            description=f"Ground clusters greater than {gh:.2f} height",
+            cluster_df.X,
+            cluster_df.Y,
+            cluster_df.ClusterID,
+            description=f"Clusters greater than +/-{gh:.2f} height",
         )
         self.products.append(p)
 
     def make_products(self) -> None:
         after = self.after.df
         p = self.make_product(
             after.X, after.Y, after.dZ3d, description="Before minus after"
@@ -286,56 +314,43 @@
         return None
 
     def save(self, format: str = ".las") -> None:
         with contextlib.suppress(FileExistsError):
             os.mkdir(os.path.join(self.before.config["OUTPUT_DIR"], "points"))
 
         # Determine Colormap
-        flex_max = min(
-            clusters.arrays[0]["dZ3d"].min()
-            for clusters in (self.ng_clusters, self.ground_clusters)
-        )
+        flex_max = self.clusters.arrays[0]["dZ3d"].min()
 
-        new_max = max(
-            clusters.arrays[0]["dZ3d"].max()
-            for clusters in (self.ng_clusters, self.ground_clusters)
-        )
+        new_max = self.clusters.arrays[0]["dZ3d"].max()
 
         divnorm = colors.TwoSlopeNorm(vmin=flex_max, vcenter=0, vmax=new_max)
         # we are only writing the first point-clouds
         colormap = plt.colormaps[self.before.config["COLORMAP"]]
 
         # write point cloud output
-        for output in ("ground", "new_ground"):
-            if output == "ground":
-                path = "gnd-clusters"
-                array = self.ground_clusters.arrays[0]
-            elif output == "new_ground":
-                path = "ng-clusters"
-                array = self.ng_clusters.arrays[0]
-            else:
-                raise RuntimeError("How did you even get here?")
-
-            filename = os.path.join(
-                self.before.config["OUTPUT_DIR"], "points", f"{path}{format}"
-            )
+        path = "clusters"
+        array = self.clusters.arrays[0]
+        sizes = self.cluster_sizes
+        filename = os.path.join(
+            self.before.config["OUTPUT_DIR"], "points", f"{path}{format}"
+        )
 
-            # convert colors from [0. 1] floats to [0, 65535] per LAS spec
-            rgb = np.array(
-                [
-                    colors.to_rgba_array(colormap(divnorm(array["dZ3d"])))
-                    * np.iinfo(np.uint16).max
-                ],
-                dtype=np.uint16,
-            )[0, :, :-1]
+        # convert colors from [0. 1] floats to [0, 65535] per LAS spec
+        rgb = np.array(
+            [
+                colors.to_rgba_array(colormap(divnorm(array["dZ3d"])))
+                * np.iinfo(np.uint16).max
+            ],
+            dtype=np.uint16,
+        )[0, :, :-1]
 
-            array = rfn.append_fields(
-                array, ["Red", "Green", "Blue"], [rgb[:, 0], rgb[:, 1], rgb[:, 2]]
-            )
+        array = rfn.append_fields(
+            array, ["Red", "Green", "Blue", "ClusterSize"], [rgb[:, 0], rgb[:, 1], rgb[:, 2], sizes]
+        )
 
-            crs = self.after.crs
-            pipeline = pdal.Writer.las(
-                filename=filename,
-                extra_dims="all",
-                a_srs=crs.to_string() if crs is not None else crs,
-            ).pipeline(array)
-            pipeline.execute()
+        crs = self.after.crs
+        pipeline = pdal.Writer.las(
+            filename=filename,
+            extra_dims="all",
+            a_srs=crs.to_string() if crs is not None else crs,
+        ).pipeline(array)
+        pipeline.execute()
```

### Comparing `codem-0.25.1/tests/test_registration.py` & `codem-0.25.2/tests/test_registration.py`

 * *Files identical despite different names*

