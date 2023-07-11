# Comparing `tmp/zensvi-0.6.3.tar.gz` & `tmp/zensvi-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.6.3.tar", max compression
+gzip compressed data, was "zensvi-0.6.4.tar", max compression
```

## Comparing `zensvi-0.6.3.tar` & `zensvi-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,52 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.3/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.3/README.md
--rwxr-xr-x   0        0        0      730 2023-06-18 04:34:24.479287 zensvi-0.6.3/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.3/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.3/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.3/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.3/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.3/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.000000 zensvi-0.6.3/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.3/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.3/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.3/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.3/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.3/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.000000 zensvi-0.6.3/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.3/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.3/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.3/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.3/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 zensvi-0.6.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.4/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.4/README.md
+-rwxr-xr-x   0        0        0      711 2023-07-11 06:35:05.908717 zensvi-0.6.4/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.4/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.4/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.4/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.4/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.4/src/zensvi/download/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-11 06:32:32.162593 zensvi-0.6.4/src/zensvi/download/mapillary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 06:24:53.511744 zensvi-0.6.4/src/zensvi/download/mapillary/config/.gitkeep
+-rw-r--r--   0        0        0     1110 2023-07-11 06:24:53.511867 zensvi-0.6.4/src/zensvi/download/mapillary/config/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-11 06:24:53.511973 zensvi-0.6.4/src/zensvi/download/mapillary/config/api/__init__.py
+-rw-r--r--   0        0        0    25264 2023-07-11 06:29:42.794455 zensvi-0.6.4/src/zensvi/download/mapillary/config/api/entities.py
+-rw-r--r--   0        0        0     1917 2023-07-11 06:24:53.512174 zensvi-0.6.4/src/zensvi/download/mapillary/config/api/general.py
+-rw-r--r--   0        0        0     8163 2023-07-11 06:24:53.512230 zensvi-0.6.4/src/zensvi/download/mapillary/config/api/vector_tiles.py
+-rw-r--r--   0        0        0      481 2023-07-11 06:24:53.512345 zensvi-0.6.4/src/zensvi/download/mapillary/controller/__init__.py
+-rw-r--r--   0        0        0     2249 2023-07-11 06:24:53.512421 zensvi-0.6.4/src/zensvi/download/mapillary/controller/detection.py
+-rw-r--r--   0        0        0     4679 2023-07-11 06:24:53.512508 zensvi-0.6.4/src/zensvi/download/mapillary/controller/feature.py
+-rw-r--r--   0        0        0    31458 2023-07-11 06:24:53.512658 zensvi-0.6.4/src/zensvi/download/mapillary/controller/image.py
+-rw-r--r--   0        0        0     4856 2023-07-11 06:24:53.512748 zensvi-0.6.4/src/zensvi/download/mapillary/controller/save.py
+-rw-r--r--   0        0        0    34865 2023-07-11 06:32:18.108423 zensvi-0.6.4/src/zensvi/download/mapillary/interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 06:24:53.512961 zensvi-0.6.4/src/zensvi/download/mapillary/models/.gitkeep
+-rw-r--r--   0        0        0      520 2023-07-11 06:24:53.513032 zensvi-0.6.4/src/zensvi/download/mapillary/models/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 06:24:53.513119 zensvi-0.6.4/src/zensvi/download/mapillary/models/api/__init__.py
+-rw-r--r--   0        0        0     8104 2023-07-11 06:24:53.513199 zensvi-0.6.4/src/zensvi/download/mapillary/models/api/entities.py
+-rw-r--r--   0        0        0    14355 2023-07-11 06:24:53.513259 zensvi-0.6.4/src/zensvi/download/mapillary/models/api/general.py
+-rw-r--r--   0        0        0    19230 2023-07-11 06:24:53.513364 zensvi-0.6.4/src/zensvi/download/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0        0        0     8257 2023-07-11 06:24:53.513428 zensvi-0.6.4/src/zensvi/download/mapillary/models/client.py
+-rw-r--r--   0        0        0     1398 2023-07-11 06:28:48.079302 zensvi-0.6.4/src/zensvi/download/mapillary/models/config.py
+-rw-r--r--   0        0        0    10328 2023-07-11 06:24:53.513573 zensvi-0.6.4/src/zensvi/download/mapillary/models/exceptions.py
+-rw-r--r--   0        0        0    14586 2023-07-11 06:24:53.513657 zensvi-0.6.4/src/zensvi/download/mapillary/models/geojson.py
+-rw-r--r--   0        0        0     2496 2023-07-11 06:24:53.513728 zensvi-0.6.4/src/zensvi/download/mapillary/models/logger.py
+-rw-r--r--   0        0        0        0 2023-07-11 06:24:53.513791 zensvi-0.6.4/src/zensvi/download/mapillary/utils/.gitkeep
+-rw-r--r--   0        0        0      511 2023-07-11 06:24:53.513859 zensvi-0.6.4/src/zensvi/download/mapillary/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2023-07-11 06:24:53.513925 zensvi-0.6.4/src/zensvi/download/mapillary/utils/auth.py
+-rw-r--r--   0        0        0     1750 2023-07-11 06:24:53.513994 zensvi-0.6.4/src/zensvi/download/mapillary/utils/extract.py
+-rw-r--r--   0        0        0    16122 2023-07-11 06:24:53.514092 zensvi-0.6.4/src/zensvi/download/mapillary/utils/filter.py
+-rw-r--r--   0        0        0    26677 2023-07-11 06:24:53.514229 zensvi-0.6.4/src/zensvi/download/mapillary/utils/format.py
+-rw-r--r--   0        0        0     1723 2023-07-11 06:24:53.514307 zensvi-0.6.4/src/zensvi/download/mapillary/utils/time.py
+-rw-r--r--   0        0        0     9928 2023-07-11 06:24:53.514400 zensvi-0.6.4/src/zensvi/download/mapillary/utils/verify.py
+-rwxr-xr-x   0        0        0    46141 2023-07-11 06:25:33.087778 zensvi-0.6.4/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.4/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.4/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.4/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.4/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.4/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-23 05:30:15.378713 zensvi-0.6.4/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.4/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.4/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.4/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.4/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 zensvi-0.6.4/PKG-INFO
```

### Comparing `zensvi-0.6.3/LICENSE` & `zensvi-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/README.md` & `zensvi-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/pyproject.toml` & `zensvi-0.6.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.6.3"
+version = "0.6.4"
 description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -19,14 +19,13 @@
 setuptools = "^64.0.3"
 Shapely=">=1.8.1"
 torch = "^2.0.0"
 tqdm = "^4.0.0"
 transformers = "^4.10.2"
 scipy = "1.7.3"
 networkx="^3.1"
-mapillary="1.0.11"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zensvi-0.6.3/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.6.4/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/download/streetview_downloader.py` & `zensvi-0.6.4/src/zensvi/download/streetview_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
 import csv
 import glob
 import shutil
 import numpy as np
 import osmnx as ox
 from abc import ABC, abstractmethod
-import mapillary.interface as mly
 from shapely import wkt
 from PIL import Image
 
+import zensvi.download.mapillary.interface as mly
 from zensvi.download.utils.imtool import ImageTool
 from zensvi.download.utils.get_pids import panoids
 from zensvi.download.utils.geoprocess import GeoProcessor
 from zensvi.download.utils.helpers import standardize_column_names, create_buffer_gdf
 
 # set logging level to warning
 import logging
@@ -328,17 +328,18 @@
             # Save the results of retried rows as another checkpoint
             if len(results) > 0:
                 pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_retry.csv', index=False)
                 # Merge the retry checkpoint into the final dataframe
                 retry_df = pd.read_csv(f'{dir_cache_pids}/checkpoint_retry.csv')
                 results_df = pd.concat([results_df, retry_df], ignore_index=True)
 
-        # now save results_df as a new cache after dropping lat_lon_id and drop duplicates in panoid
+        # now save results_df as a new cache after dropping lat_lon_id
         results_df = results_df.drop(columns='lat_lon_id')
-        results_df = results_df.drop_duplicates(subset='panoid')
+        # drop duplicates in panoid and id_columns
+        results_df = results_df.drop_duplicates(subset=['panoid'] + id_columns)
         results_df.to_csv(self.cache_pids_raw, index=False)
 
         # delete the cache directory
         if dir_cache_pids.exists():
             shutil.rmtree(dir_cache_pids)
         return results_df
 
@@ -677,15 +678,15 @@
         
         if checkpoints == [] and failed_rows == []:
             print("There is no panorama ID to download")
             return
 
         # now save results_df as a new cache after dropping lat_lon_id and drop duplicates in panoid
         results_df = results_df.drop(columns='lat_lon_id')
-        results_df = results_df.drop_duplicates(subset='id')
+        results_df = results_df.drop_duplicates(subset=['id'] + id_columns)
         results_df.to_csv(self.cache_pids_raw, index=False)
 
         # delete the cache directory
         if dir_cache_pids.exists():
             shutil.rmtree(dir_cache_pids)
         return results_df
```

### Comparing `zensvi-0.6.3/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.6.4/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.6.4/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/download/utils/get_pids.py` & `zensvi-0.6.4/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/download/utils/helpers.py` & `zensvi-0.6.4/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/download/utils/imtool.py` & `zensvi-0.6.4/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/download/utils/proxies.csv` & `zensvi-0.6.4/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/src/zensvi/transform/transform_image.py` & `zensvi-0.6.4/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.3/PKG-INFO` & `zensvi-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.6.3
+Version: 0.6.4
 Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=8.3.2,<9.6)
 Requires-Dist: Shapely (>=1.8.1)
 Requires-Dist: geopandas (>=0.10.0)
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
-Requires-Dist: mapillary (==1.0.11)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.16.5,<1.23.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: scipy (==1.7.3)
```

