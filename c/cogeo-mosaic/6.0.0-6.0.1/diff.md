# Comparing `tmp/cogeo_mosaic-6.0.0.tar.gz` & `tmp/cogeo_mosaic-6.0.1.tar.gz`

## Comparing `cogeo_mosaic-6.0.0.tar` & `cogeo_mosaic-6.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/CHANGES.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/README.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/cache.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/errors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/logger.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/models.py
--rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/mosaic.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/utils.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/az.py
--rw-r--r--   0        0        0    13571 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/base.py
--rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/dynamodb.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/file.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/gs.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/memory.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/s3.py
--rw-r--r--   0        0        0    14051 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/sqlite.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/stac.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/utils.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/web.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/scripts/__init__.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/scripts/cli.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/LICENSE
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/pyproject.toml
--rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/CHANGES.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/cache.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/errors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/logger.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/models.py
+-rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/mosaic.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/utils.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/az.py
+-rw-r--r--   0        0        0    13571 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/base.py
+-rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/dynamodb.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/file.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/gs.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/memory.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/s3.py
+-rw-r--r--   0        0        0    14051 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/sqlite.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/stac.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/utils.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/backends/web.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/scripts/__init__.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/cogeo_mosaic/scripts/cli.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/LICENSE
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0    17282 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.1/PKG-INFO
```

### Comparing `cogeo_mosaic-6.0.0/CHANGES.md` & `cogeo_mosaic-6.0.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+## 6.0.1 (2023-07-11)
+
+* fix `HttpBackend` post_init method
+
 ## 6.0.0 (2023-07-10)
 
 * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0` requirements
 
 * replace `supermercado` with [`supermorecado`](https://github.com/developmentseed/supermorecado) to burn geometries as tiles for different TMS
 
 * update MosaicJSON models to `0.0.3` specification (adds `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and `layers` attributes)
```

### Comparing `cogeo_mosaic-6.0.0/CONTRIBUTING.md` & `cogeo_mosaic-6.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/README.md` & `cogeo_mosaic-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/cache.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/cache.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/errors.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/errors.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/mosaic.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/mosaic.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/utils.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/utils.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/__init__.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/az.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/az.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/base.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/base.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/dynamodb.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/file.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/file.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/gs.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/gs.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/memory.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/memory.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/s3.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/s3.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/sqlite.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/stac.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/stac.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/utils.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/utils.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/web.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/backends/web.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,25 +21,18 @@
 
 @attr.s
 class HttpBackend(BaseBackend):
     """Http/Https Backend Adapter"""
 
     # Because the HttpBackend is a Read-Only backend, there is no need for
     # mosaic_def to be in the init method.
-    mosaic_def: MosaicJSON = attr.ib(init=False)
+    mosaic_def: MosaicJSON = attr.ib(init=False, default=None)
 
     _backend_name = "HTTP"
 
-    def __attrs_post_init__(self):
-        """Post Init."""
-        self.mosaic_def = self._read()
-        self.minzoom = self.mosaic_def.minzoom
-        self.maxzoom = self.mosaic_def.maxzoom
-        self.bounds = self.mosaic_def.bounds
-
     @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get mosaicjson document."""
         try:
```

### Comparing `cogeo_mosaic-6.0.0/cogeo_mosaic/scripts/cli.py` & `cogeo_mosaic-6.0.1/cogeo_mosaic/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/.gitignore` & `cogeo_mosaic-6.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/LICENSE` & `cogeo_mosaic-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/pyproject.toml` & `cogeo_mosaic-6.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-6.0.0/PKG-INFO` & `cogeo_mosaic-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogeo-mosaic
-Version: 6.0.0
+Version: 6.0.1
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
 
 
+## 6.0.1 (2023-07-11)
+
+* fix `HttpBackend` post_init method
+
 ## 6.0.0 (2023-07-10)
 
 * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0` requirements
 
 * replace `supermercado` with [`supermorecado`](https://github.com/developmentseed/supermorecado) to burn geometries as tiles for different TMS
 
 * update MosaicJSON models to `0.0.3` specification (adds `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and `layers` attributes)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cogeo-mosaic Version: 6.0.0 Summary: CLI and
+Metadata-Version: 2.1 Name: cogeo-mosaic Version: 6.0.1 Summary: CLI and
 Backends to work with MosaicJSON. Project-URL: Homepage, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Documentation, https://
 developmentseed.org/cogeo-mosaic/ Project-URL: Issues, https://github.com/
 developmentseed/cogeo-mosaic/issues Project-URL: Source, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Changelog, https://
 developmentseed.org/cogeo-mosaic/release-notes/ Author-email: Vincent Sarago
 developmentseed.com> License: MIT License Copyright (c) 2019 Development Seed
@@ -57,18 +57,19 @@
 developmentseed/titiler): A lightweight Cloud Optimized GeoTIFF dynamic tile
 server (COG, STAC and MosaicJSON). ## Contribution & Development See
 [CONTRIBUTING.md](https://github.com/developmentseed/cogeo-mosaic/blob/master/
 CONTRIBUTING.md) ## License See [LICENSE](https://github.com/developmentseed/
 cogeo-mosaic/blob/master/LICENSE) ## Authors Created by [Development Seed](
 developmentseed.org>) See [contributors](https://github.com/developmentseed/
 cogeo-mosaic/graphs/contributors) for a listing of individual contributors. ##
-Changelog ## 6.0.0 (2023-07-10) * update `morecantile>=4.1,<5.0` and `rio-
-tiler>=5.0,<6.0` requirements * replace `supermercado` with [`supermorecado`]
-(https://github.com/developmentseed/supermorecado) to burn geometries as tiles
-for different TMS * update MosaicJSON models to `0.0.3` specification (adds
+Changelog ## 6.0.1 (2023-07-11) * fix `HttpBackend` post_init method ## 6.0.0
+(2023-07-10) * update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0`
+requirements * replace `supermercado` with [`supermorecado`](https://
+github.com/developmentseed/supermorecado) to burn geometries as tiles for
+different TMS * update MosaicJSON models to `0.0.3` specification (adds
 `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and
 `layers` attributes) * allow Mosaic creation using other TileMatrixSet (default
 is still `WebMercatorQuad`) * add `tms` support to MosaicBackend to read tile
 in other TMS than the mosaic TileMatrixSet ```python # Before # Mosaic and
 output Tile in WebMercatorQuad with MosaicBackend("mosaic.json") as mosaic:
 img, _ = mosaic.tile(0, 0, 0) # Now # Mosaic in WebMercatorQuad (default),
 output tile in WGS84 WGS1984Quad = morecantile.tms.get("WGS1984Quad") with
```

