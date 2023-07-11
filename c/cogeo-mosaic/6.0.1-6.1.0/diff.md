# Comparing `tmp/cogeo_mosaic-6.0.1.tar.gz` & `tmp/cogeo_mosaic-6.1.0.tar.gz`

## Comparing `cogeo_mosaic-6.0.1.tar` & `cogeo_mosaic-6.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/CHANGES.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/README.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/cache.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/errors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/logger.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/models.py
--rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/mosaic.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/utils.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/az.py
--rw-r--r--   0        0        0    13571 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/base.py
--rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/dynamodb.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/file.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/gs.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/memory.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/s3.py
--rw-r--r--   0        0        0    14051 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/sqlite.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/stac.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/utils.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/web.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/scripts/__init__.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/scripts/cli.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/LICENSE
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/pyproject.toml
--rw-r--r--   0        0        0    17282 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/CHANGES.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/cache.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/errors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/logger.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/models.py
+-rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/mosaic.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/utils.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/az.py
+-rw-r--r--   0        0        0    13654 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/base.py
+-rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/dynamodb.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/file.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/gs.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/memory.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/s3.py
+-rw-r--r--   0        0        0    14051 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/sqlite.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/stac.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/utils.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/backends/web.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/scripts/__init__.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/cogeo_mosaic/scripts/cli.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/LICENSE
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0    17363 2020-02-02 00:00:00.000000 cogeo_mosaic-6.1.0/PKG-INFO
```

### Comparing `cogeo_mosaic-6.0.1/CHANGES.md` & `cogeo_mosaic-6.1.0/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+## 6.1.0 (2023-07-11)
+
+* add `tilematrixset` in `MosaicBackend.info()` response
+
 ## 6.0.1 (2023-07-11)
 
 * fix `HttpBackend` post_init method
 
 ## 6.0.0 (2023-07-10)
 
 * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0` requirements
```

### Comparing `cogeo_mosaic-6.0.1/CONTRIBUTING.md` & `cogeo_mosaic-6.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/README.md` & `cogeo_mosaic-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/cache.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/cache.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/errors.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/errors.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/mosaic.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/mosaic.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/utils.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/utils.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/__init__.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/az.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/az.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/base.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,14 +336,15 @@
         return Info(
             bounds=self.geographic_bounds,
             center=self.center,
             maxzoom=self.maxzoom,
             minzoom=self.minzoom,
             name=self.mosaic_def.name if self.mosaic_def.name else "mosaic",
             quadkeys=[] if not quadkeys else self._quadkeys,
+            tilematrixset=repr(self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS),
         )
 
     @property
     def center(self):
         """Return center from the mosaic definition."""
         return (
             (self.bounds[0] + self.bounds[2]) / 2,
```

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/dynamodb.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/file.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/file.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/gs.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/gs.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/memory.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/memory.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/s3.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/s3.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/sqlite.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/stac.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/stac.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/utils.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/utils.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/web.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/backends/web.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/cogeo_mosaic/scripts/cli.py` & `cogeo_mosaic-6.1.0/cogeo_mosaic/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/.gitignore` & `cogeo_mosaic-6.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/LICENSE` & `cogeo_mosaic-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/pyproject.toml` & `cogeo_mosaic-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.1/PKG-INFO` & `cogeo_mosaic-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogeo-mosaic
-Version: 6.0.1
+Version: 6.1.0
 Summary: CLI and Backends to work with MosaicJSON.
 Project-URL: Homepage, https://github.com/developmentseed/cogeo-mosaic
 Project-URL: Documentation, https://developmentseed.org/cogeo-mosaic/
 Project-URL: Issues, https://github.com/developmentseed/cogeo-mosaic/issues
 Project-URL: Source, https://github.com/developmentseed/cogeo-mosaic
 Project-URL: Changelog, https://developmentseed.org/cogeo-mosaic/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
@@ -142,14 +142,18 @@
 Created by [Development Seed](<http://developmentseed.org>)
 
 See [contributors](https://github.com/developmentseed/cogeo-mosaic/graphs/contributors) for a listing of individual contributors.
 
 ## Changelog
 
 
+## 6.1.0 (2023-07-11)
+
+* add `tilematrixset` in `MosaicBackend.info()` response
+
 ## 6.0.1 (2023-07-11)
 
 * fix `HttpBackend` post_init method
 
 ## 6.0.0 (2023-07-10)
 
 * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0` requirements
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cogeo-mosaic Version: 6.0.1 Summary: CLI and
+Metadata-Version: 2.1 Name: cogeo-mosaic Version: 6.1.0 Summary: CLI and
 Backends to work with MosaicJSON. Project-URL: Homepage, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Documentation, https://
 developmentseed.org/cogeo-mosaic/ Project-URL: Issues, https://github.com/
 developmentseed/cogeo-mosaic/issues Project-URL: Source, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Changelog, https://
 developmentseed.org/cogeo-mosaic/release-notes/ Author-email: Vincent Sarago
 developmentseed.com> License: MIT License Copyright (c) 2019 Development Seed
@@ -57,15 +57,16 @@
 developmentseed/titiler): A lightweight Cloud Optimized GeoTIFF dynamic tile
 server (COG, STAC and MosaicJSON). ## Contribution & Development See
 [CONTRIBUTING.md](https://github.com/developmentseed/cogeo-mosaic/blob/master/
 CONTRIBUTING.md) ## License See [LICENSE](https://github.com/developmentseed/
 cogeo-mosaic/blob/master/LICENSE) ## Authors Created by [Development Seed](
 developmentseed.org>) See [contributors](https://github.com/developmentseed/
 cogeo-mosaic/graphs/contributors) for a listing of individual contributors. ##
-Changelog ## 6.0.1 (2023-07-11) * fix `HttpBackend` post_init method ## 6.0.0
+Changelog ## 6.1.0 (2023-07-11) * add `tilematrixset` in `MosaicBackend.info()`
+response ## 6.0.1 (2023-07-11) * fix `HttpBackend` post_init method ## 6.0.0
 (2023-07-10) * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0`
 requirements * replace `supermercado` with [`supermorecado`](https://
 github.com/developmentseed/supermorecado) to burn geometries as tiles for
 different TMS * update MosaicJSON models to `0.0.3` specification (adds
 `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and
 `layers` attributes) * allow Mosaic creation using other TileMatrixSet (default
 is still `WebMercatorQuad`) * add `tms` support to MosaicBackend to read tile
```

