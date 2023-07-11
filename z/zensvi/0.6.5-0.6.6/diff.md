# Comparing `tmp/zensvi-0.6.5.tar.gz` & `tmp/zensvi-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.6.5.tar", max compression
+gzip compressed data, was "zensvi-0.6.6.tar", max compression
```

## Comparing `zensvi-0.6.5.tar` & `zensvi-0.6.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.5/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.5/README.md
--rwxr-xr-x   0        0        0      711 2023-07-11 07:04:06.780508 zensvi-0.6.5/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.5/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.5/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.5/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.5/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.5/src/zensvi/download/__init__.py
--rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.6.5/src/zensvi/download/mapillary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.6.5/src/zensvi/download/mapillary/config/.gitkeep
--rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.6.5/src/zensvi/download/mapillary/config/__init__.py
--rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.6.5/src/zensvi/download/mapillary/config/api/__init__.py
--rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.6.5/src/zensvi/download/mapillary/config/api/entities.py
--rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.6.5/src/zensvi/download/mapillary/config/api/general.py
--rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.6.5/src/zensvi/download/mapillary/config/api/vector_tiles.py
--rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.6.5/src/zensvi/download/mapillary/controller/__init__.py
--rw-r--r--   0        0        0     2249 2023-07-11 07:03:47.658965 zensvi-0.6.5/src/zensvi/download/mapillary/controller/detection.py
--rw-r--r--   0        0        0     4679 2023-07-11 07:03:47.659262 zensvi-0.6.5/src/zensvi/download/mapillary/controller/feature.py
--rw-r--r--   0        0        0    31458 2023-07-11 07:03:47.659689 zensvi-0.6.5/src/zensvi/download/mapillary/controller/image.py
--rw-r--r--   0        0        0     4856 2023-07-11 07:03:47.660128 zensvi-0.6.5/src/zensvi/download/mapillary/controller/save.py
--rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.6.5/src/zensvi/download/mapillary/interface.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.6.5/src/zensvi/download/mapillary/models/.gitkeep
--rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.6.5/src/zensvi/download/mapillary/models/__init__.py
--rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.6.5/src/zensvi/download/mapillary/models/api/__init__.py
--rw-r--r--   0        0        0     8104 2023-07-11 07:03:47.661263 zensvi-0.6.5/src/zensvi/download/mapillary/models/api/entities.py
--rw-r--r--   0        0        0    14355 2023-07-11 07:03:47.661600 zensvi-0.6.5/src/zensvi/download/mapillary/models/api/general.py
--rw-r--r--   0        0        0    19230 2023-07-11 07:03:47.662091 zensvi-0.6.5/src/zensvi/download/mapillary/models/api/vector_tiles.py
--rw-r--r--   0        0        0     8257 2023-07-11 07:03:47.662498 zensvi-0.6.5/src/zensvi/download/mapillary/models/client.py
--rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.6.5/src/zensvi/download/mapillary/models/config.py
--rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.6.5/src/zensvi/download/mapillary/models/exceptions.py
--rw-r--r--   0        0        0    14586 2023-07-11 07:03:47.663455 zensvi-0.6.5/src/zensvi/download/mapillary/models/geojson.py
--rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.6.5/src/zensvi/download/mapillary/models/logger.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.6.5/src/zensvi/download/mapillary/utils/.gitkeep
--rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.6.5/src/zensvi/download/mapillary/utils/__init__.py
--rw-r--r--   0        0        0     1742 2023-07-11 07:03:47.664086 zensvi-0.6.5/src/zensvi/download/mapillary/utils/auth.py
--rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.6.5/src/zensvi/download/mapillary/utils/extract.py
--rw-r--r--   0        0        0    16122 2023-07-11 07:03:47.664681 zensvi-0.6.5/src/zensvi/download/mapillary/utils/filter.py
--rw-r--r--   0        0        0    26677 2023-07-11 07:03:47.665003 zensvi-0.6.5/src/zensvi/download/mapillary/utils/format.py
--rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.6.5/src/zensvi/download/mapillary/utils/time.py
--rw-r--r--   0        0        0     9928 2023-07-11 07:03:47.665403 zensvi-0.6.5/src/zensvi/download/mapillary/utils/verify.py
--rwxr-xr-x   0        0        0    46141 2023-07-11 07:03:47.665933 zensvi-0.6.5/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.5/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.5/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.5/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.5/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.5/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-23 05:30:15.378713 zensvi-0.6.5/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.5/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.5/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.5/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.5/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 zensvi-0.6.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.6/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.6/README.md
+-rwxr-xr-x   0        0        0      712 2023-07-11 07:06:43.466849 zensvi-0.6.6/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.6/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.6/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.6/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.6/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.6/src/zensvi/download/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.6.6/src/zensvi/download/mapillary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.6.6/src/zensvi/download/mapillary/config/.gitkeep
+-rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.6.6/src/zensvi/download/mapillary/config/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.6.6/src/zensvi/download/mapillary/config/api/__init__.py
+-rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.6.6/src/zensvi/download/mapillary/config/api/entities.py
+-rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.6.6/src/zensvi/download/mapillary/config/api/general.py
+-rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.6.6/src/zensvi/download/mapillary/config/api/vector_tiles.py
+-rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.6.6/src/zensvi/download/mapillary/controller/__init__.py
+-rw-r--r--   0        0        0     2249 2023-07-11 07:03:47.658965 zensvi-0.6.6/src/zensvi/download/mapillary/controller/detection.py
+-rw-r--r--   0        0        0     4679 2023-07-11 07:03:47.659262 zensvi-0.6.6/src/zensvi/download/mapillary/controller/feature.py
+-rw-r--r--   0        0        0    31458 2023-07-11 07:03:47.659689 zensvi-0.6.6/src/zensvi/download/mapillary/controller/image.py
+-rw-r--r--   0        0        0     4856 2023-07-11 07:03:47.660128 zensvi-0.6.6/src/zensvi/download/mapillary/controller/save.py
+-rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.6.6/src/zensvi/download/mapillary/interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.6.6/src/zensvi/download/mapillary/models/.gitkeep
+-rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.6.6/src/zensvi/download/mapillary/models/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.6.6/src/zensvi/download/mapillary/models/api/__init__.py
+-rw-r--r--   0        0        0     8104 2023-07-11 07:03:47.661263 zensvi-0.6.6/src/zensvi/download/mapillary/models/api/entities.py
+-rw-r--r--   0        0        0    14355 2023-07-11 07:03:47.661600 zensvi-0.6.6/src/zensvi/download/mapillary/models/api/general.py
+-rw-r--r--   0        0        0    19230 2023-07-11 07:03:47.662091 zensvi-0.6.6/src/zensvi/download/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0        0        0     8257 2023-07-11 07:03:47.662498 zensvi-0.6.6/src/zensvi/download/mapillary/models/client.py
+-rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.6.6/src/zensvi/download/mapillary/models/config.py
+-rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.6.6/src/zensvi/download/mapillary/models/exceptions.py
+-rw-r--r--   0        0        0    14586 2023-07-11 07:03:47.663455 zensvi-0.6.6/src/zensvi/download/mapillary/models/geojson.py
+-rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.6.6/src/zensvi/download/mapillary/models/logger.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.6.6/src/zensvi/download/mapillary/utils/.gitkeep
+-rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.6.6/src/zensvi/download/mapillary/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2023-07-11 07:03:47.664086 zensvi-0.6.6/src/zensvi/download/mapillary/utils/auth.py
+-rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.6.6/src/zensvi/download/mapillary/utils/extract.py
+-rw-r--r--   0        0        0    16122 2023-07-11 07:03:47.664681 zensvi-0.6.6/src/zensvi/download/mapillary/utils/filter.py
+-rw-r--r--   0        0        0    26677 2023-07-11 07:03:47.665003 zensvi-0.6.6/src/zensvi/download/mapillary/utils/format.py
+-rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.6.6/src/zensvi/download/mapillary/utils/time.py
+-rw-r--r--   0        0        0     9928 2023-07-11 07:03:47.665403 zensvi-0.6.6/src/zensvi/download/mapillary/utils/verify.py
+-rwxr-xr-x   0        0        0    46141 2023-07-11 07:03:47.665933 zensvi-0.6.6/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.6/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.6/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.6/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.6/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.6/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-23 05:30:15.378713 zensvi-0.6.6/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.6/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.6/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.6/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.6/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 zensvi-0.6.6/PKG-INFO
```

### Comparing `zensvi-0.6.5/LICENSE` & `zensvi-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/README.md` & `zensvi-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.6.6/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/__init__.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/config/__init__.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/config/api/entities.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/config/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/config/api/general.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/config/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/config/api/vector_tiles.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/config/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/controller/detection.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/controller/detection.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/controller/feature.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/controller/feature.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/controller/image.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/controller/image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/controller/save.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/controller/save.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/interface.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/interface.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/__init__.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/api/entities.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/api/general.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/api/vector_tiles.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/client.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/client.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/config.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/config.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/exceptions.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/geojson.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/geojson.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/models/logger.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/models/logger.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/utils/auth.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/utils/auth.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/utils/extract.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/utils/extract.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/utils/filter.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/utils/filter.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/utils/format.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/utils/format.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/utils/time.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/utils/time.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/mapillary/utils/verify.py` & `zensvi-0.6.6/src/zensvi/download/mapillary/utils/verify.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/streetview_downloader.py` & `zensvi-0.6.6/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.6.6/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.6.6/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/utils/get_pids.py` & `zensvi-0.6.6/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/utils/helpers.py` & `zensvi-0.6.6/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/utils/imtool.py` & `zensvi-0.6.6/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/download/utils/proxies.csv` & `zensvi-0.6.6/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/src/zensvi/transform/transform_image.py` & `zensvi-0.6.6/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.5/PKG-INFO` & `zensvi-0.6.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.6.5
+Version: 0.6.6
 Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.16.5,<1.23.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: scipy (>=1.7)
-Requires-Dist: setuptools (>=64.0.3,<65.0.0)
+Requires-Dist: setuptools (>=64.0.3)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Requires-Dist: transformers (>=4.10.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # ZenSVI
```

