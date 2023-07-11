# Comparing `tmp/zensvi-0.6.8.tar.gz` & `tmp/zensvi-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.6.8.tar", max compression
+gzip compressed data, was "zensvi-0.6.9.tar", max compression
```

## Comparing `zensvi-0.6.8.tar` & `zensvi-0.6.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.8/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.8/README.md
--rwxr-xr-x   0        0        0      712 2023-07-11 08:27:17.516816 zensvi-0.6.8/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.8/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.8/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.8/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.8/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.8/src/zensvi/download/__init__.py
--rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.6.8/src/zensvi/download/mapillary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.6.8/src/zensvi/download/mapillary/config/.gitkeep
--rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.6.8/src/zensvi/download/mapillary/config/__init__.py
--rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.6.8/src/zensvi/download/mapillary/config/api/__init__.py
--rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.6.8/src/zensvi/download/mapillary/config/api/entities.py
--rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.6.8/src/zensvi/download/mapillary/config/api/general.py
--rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.6.8/src/zensvi/download/mapillary/config/api/vector_tiles.py
--rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.6.8/src/zensvi/download/mapillary/controller/__init__.py
--rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.6.8/src/zensvi/download/mapillary/controller/detection.py
--rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.6.8/src/zensvi/download/mapillary/controller/feature.py
--rw-r--r--   0        0        0    31634 2023-07-11 08:20:22.811895 zensvi-0.6.8/src/zensvi/download/mapillary/controller/image.py
--rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.6.8/src/zensvi/download/mapillary/controller/save.py
--rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.6.8/src/zensvi/download/mapillary/interface.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.6.8/src/zensvi/download/mapillary/models/.gitkeep
--rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.6.8/src/zensvi/download/mapillary/models/__init__.py
--rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.6.8/src/zensvi/download/mapillary/models/api/__init__.py
--rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.6.8/src/zensvi/download/mapillary/models/api/entities.py
--rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.6.8/src/zensvi/download/mapillary/models/api/general.py
--rw-r--r--   0        0        0    19294 2023-07-11 08:22:13.318683 zensvi-0.6.8/src/zensvi/download/mapillary/models/api/vector_tiles.py
--rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.6.8/src/zensvi/download/mapillary/models/client.py
--rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.6.8/src/zensvi/download/mapillary/models/config.py
--rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.6.8/src/zensvi/download/mapillary/models/exceptions.py
--rw-r--r--   0        0        0    14602 2023-07-11 08:21:05.329571 zensvi-0.6.8/src/zensvi/download/mapillary/models/geojson.py
--rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.6.8/src/zensvi/download/mapillary/models/logger.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.6.8/src/zensvi/download/mapillary/utils/.gitkeep
--rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.6.8/src/zensvi/download/mapillary/utils/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.6.8/src/zensvi/download/mapillary/utils/auth.py
--rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.6.8/src/zensvi/download/mapillary/utils/extract.py
--rw-r--r--   0        0        0    16138 2023-07-11 08:22:32.866063 zensvi-0.6.8/src/zensvi/download/mapillary/utils/filter.py
--rw-r--r--   0        0        0    26693 2023-07-11 08:26:13.918807 zensvi-0.6.8/src/zensvi/download/mapillary/utils/format.py
--rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.6.8/src/zensvi/download/mapillary/utils/time.py
--rw-r--r--   0        0        0     9976 2023-07-11 08:22:46.586975 zensvi-0.6.8/src/zensvi/download/mapillary/utils/verify.py
--rwxr-xr-x   0        0        0    46157 2023-07-11 08:17:09.841741 zensvi-0.6.8/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.8/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.8/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.8/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.8/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.8/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-23 05:30:15.378713 zensvi-0.6.8/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.8/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.8/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.8/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.8/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 zensvi-0.6.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.9/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.9/README.md
+-rwxr-xr-x   0        0        0     1400 2023-07-11 09:05:50.294362 zensvi-0.6.9/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.9/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.9/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.9/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.9/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.9/src/zensvi/download/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.6.9/src/zensvi/download/mapillary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.6.9/src/zensvi/download/mapillary/config/.gitkeep
+-rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.6.9/src/zensvi/download/mapillary/config/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/__init__.py
+-rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/entities.py
+-rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/general.py
+-rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/vector_tiles.py
+-rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.6.9/src/zensvi/download/mapillary/controller/__init__.py
+-rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.6.9/src/zensvi/download/mapillary/controller/detection.py
+-rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.6.9/src/zensvi/download/mapillary/controller/feature.py
+-rw-r--r--   0        0        0    31634 2023-07-11 08:20:22.811895 zensvi-0.6.9/src/zensvi/download/mapillary/controller/image.py
+-rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.6.9/src/zensvi/download/mapillary/controller/save.py
+-rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.6.9/src/zensvi/download/mapillary/interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.6.9/src/zensvi/download/mapillary/models/.gitkeep
+-rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.6.9/src/zensvi/download/mapillary/models/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/__init__.py
+-rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/entities.py
+-rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/general.py
+-rw-r--r--   0        0        0    19294 2023-07-11 08:22:13.318683 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.6.9/src/zensvi/download/mapillary/models/client.py
+-rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.6.9/src/zensvi/download/mapillary/models/config.py
+-rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.6.9/src/zensvi/download/mapillary/models/exceptions.py
+-rw-r--r--   0        0        0    14602 2023-07-11 08:21:05.329571 zensvi-0.6.9/src/zensvi/download/mapillary/models/geojson.py
+-rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.6.9/src/zensvi/download/mapillary/models/logger.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.6.9/src/zensvi/download/mapillary/utils/.gitkeep
+-rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.6.9/src/zensvi/download/mapillary/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.6.9/src/zensvi/download/mapillary/utils/auth.py
+-rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.6.9/src/zensvi/download/mapillary/utils/extract.py
+-rw-r--r--   0        0        0    16138 2023-07-11 08:22:32.866063 zensvi-0.6.9/src/zensvi/download/mapillary/utils/filter.py
+-rw-r--r--   0        0        0    26693 2023-07-11 08:26:13.918807 zensvi-0.6.9/src/zensvi/download/mapillary/utils/format.py
+-rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.6.9/src/zensvi/download/mapillary/utils/time.py
+-rw-r--r--   0        0        0     9976 2023-07-11 08:22:46.586975 zensvi-0.6.9/src/zensvi/download/mapillary/utils/verify.py
+-rwxr-xr-x   0        0        0    46157 2023-07-11 08:17:09.841741 zensvi-0.6.9/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.9/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.9/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.9/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.9/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.9/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-23 05:30:15.378713 zensvi-0.6.9/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.9/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.9/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.9/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.9/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 zensvi-0.6.9/PKG-INFO
```

### Comparing `zensvi-0.6.8/LICENSE` & `zensvi-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/README.md` & `zensvi-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/pyproject.toml` & `zensvi-0.6.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,65 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.6.8"
+version = "0.6.9"
 description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 Pillow = ">=8.3.2,<9.6"
 geopandas = ">=0.10.0"
 geopy = "^2.2.0"
-numpy = ">=1.16.5,<1.23.0"
+numpy = "^1.21.0"
 opencv_python = "^4.5.3"
 osmnx = "^1.1.1"
 pandas = "^1.3.3"
 requests = "^2.25.1"
 setuptools = ">=64.0.3"
 Shapely=">=1.8.1"
 torch = "^2.0.0"
-tqdm = "^4.0.0"
+tqdm = "^4.61.1"
 transformers = "^4.10.2"
-scipy = ">=1.7"
+scipy = "^1.7"
 networkx="^3.1"
+attrs = "^21.2.0"
+bleach = "^3.3.0"
+certifi = "^2021.5.30"
+chardet = "^4.0.0"
+click = "^8.0.1"
+click-plugins = "^1.1.1"
+cligj = "^0.7.2"
+coverage = "^5.5"
+docutils = "^0.17.1"
+future = "^0.18.2"
+hypothesis = "^6.14.0"
+idna = "^2.10"
+iniconfig = "^1.1.1"
+mapbox-vector-tile = "^1.2.1"
+mercantile = "^1.2.1"
+munch = "^2.5.0"
+pkginfo = "^1.7.0"
+pluggy = "^0.13.1"
+protobuf = "^3.17.3"
+psutil = "^5.8.0"
+py = "^1.10.0"
+pyparsing = "^2.4.7"
+requests-toolbelt = "^0.9.1"
+six = "^1.16.0"
+sortedcontainers = "^2.4.0"
+twine = "^1.13.0"
+urllib3 = "^1.26.5"
+vt2geojson = "^0.2.1"
+webencodings = "^0.5.1"
+Pygments = "^2.9.0"
+haversine = "^2.3.1"
+python-dotenv = "^0.19.0"
+turfpy = "^0.0.7"
+geojson = "^2.5.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zensvi-0.6.8/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.6.9/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/__init__.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/config/__init__.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/config/api/entities.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/config/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/config/api/general.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/config/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/config/api/vector_tiles.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/config/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/controller/detection.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/controller/detection.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/controller/feature.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/controller/feature.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/controller/image.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/controller/image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/controller/save.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/controller/save.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/interface.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/interface.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/__init__.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/api/entities.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/api/general.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/api/vector_tiles.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/client.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/client.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/config.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/config.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/exceptions.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/geojson.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/geojson.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/models/logger.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/models/logger.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/utils/auth.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/utils/auth.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/utils/extract.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/utils/extract.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/utils/filter.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/utils/filter.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/utils/format.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/utils/format.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/utils/time.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/utils/time.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/mapillary/utils/verify.py` & `zensvi-0.6.9/src/zensvi/download/mapillary/utils/verify.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/streetview_downloader.py` & `zensvi-0.6.9/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.6.9/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.6.9/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/utils/get_pids.py` & `zensvi-0.6.9/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/utils/helpers.py` & `zensvi-0.6.9/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/utils/imtool.py` & `zensvi-0.6.9/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/download/utils/proxies.csv` & `zensvi-0.6.9/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.8/src/zensvi/transform/transform_image.py` & `zensvi-0.6.9/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

