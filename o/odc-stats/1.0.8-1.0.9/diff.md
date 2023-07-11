# Comparing `tmp/odc-stats-1.0.8.tar.gz` & `tmp/odc-stats-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc-stats-1.0.8.tar", last modified: Mon Dec 20 03:37:02 2021, max compression
+gzip compressed data, was "odc-stats-1.0.9.tar", last modified: Wed Dec 22 01:07:36 2021, max compression
```

## Comparing `odc-stats-1.0.8.tar` & `odc-stats-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 03:37:02.919385 odc-stats-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-20 03:36:49.000000 odc-stats-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13662 2021-12-20 03:37:02.919385 odc-stats-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13271 2021-12-20 03:36:49.000000 odc-stats-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 03:37:02.907385 odc-stats-1.0.8/odc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 03:37:02.915385 odc-stats-1.0.8/odc/stats/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3748 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_cli_common.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_cli_generate_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_cli_generate_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_cli_publish_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6088 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     6714 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_cli_save_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_gjson.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_sqs.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_stac_fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_text.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    17934 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    22869 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 03:37:02.915385 odc-stats-1.0.8/odc/stats/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/fc_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     5947 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/gm.py
--rw-r--r--   0 runner    (1001) docker     (121)     7343 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/gm_ls_bitmask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/pq.py
--rw-r--r--   0 runner    (1001) docker     (121)     7731 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/pq_bitmask.py
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/tcw_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8224 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/plugins/wofs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11164 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/proc.py
--rw-r--r--   0 runner    (1001) docker     (121)    21019 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)    11510 2021-12-20 03:36:49.000000 odc-stats-1.0.8/odc/stats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 03:37:02.919385 odc-stats-1.0.8/odc_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13662 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-12-20 03:37:02.000000 odc-stats-1.0.8/odc_stats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-20 03:36:49.000000 odc-stats-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      944 2021-12-20 03:37:02.919385 odc-stats-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-20 03:36:49.000000 odc-stats-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 01:07:36.130791 odc-stats-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-22 01:07:25.000000 odc-stats-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    13662 2021-12-22 01:07:36.130791 odc-stats-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13271 2021-12-22 01:07:25.000000 odc-stats-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 01:07:36.118791 odc-stats-1.0.9/odc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 01:07:36.126791 odc-stats-1.0.9/odc/stats/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3748 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_cli_generate_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_cli_generate_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_cli_publish_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6088 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6722 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_cli_save_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3378 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_gjson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_stac_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17934 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23932 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 01:07:36.126791 odc-stats-1.0.9/odc/stats/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/fc_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5947 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/gm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7343 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/gm_ls_bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/pq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7731 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/pq_bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/tcw_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8224 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/plugins/wofs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11164 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/proc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21027 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11489 2021-12-22 01:07:25.000000 odc-stats-1.0.9/odc/stats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 01:07:36.130791 odc-stats-1.0.9/odc_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13662 2021-12-22 01:07:36.000000 odc-stats-1.0.9/odc_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-12-22 01:07:36.000000 odc-stats-1.0.9/odc_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-22 01:07:36.000000 odc-stats-1.0.9/odc_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-12-22 01:07:36.000000 odc-stats-1.0.9/odc_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-22 01:07:35.000000 odc-stats-1.0.9/odc_stats.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2021-12-22 01:07:36.000000 odc-stats-1.0.9/odc_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-12-22 01:07:36.000000 odc-stats-1.0.9/odc_stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-22 01:07:25.000000 odc-stats-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2021-12-22 01:07:36.130791 odc-stats-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-22 01:07:25.000000 odc-stats-1.0.9/setup.py
```

### Comparing `odc-stats-1.0.8/LICENSE` & `odc-stats-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/PKG-INFO` & `odc-stats-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-stats
-Version: 1.0.8
+Version: 1.0.9
 Summary: Statistical Product Generation Framework
 Home-page: https://github.com/opendatacube/odc-stats/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-stats-1.0.8/README.md` & `odc-stats-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_cli_common.py` & `odc-stats-1.0.9/odc/stats/_cli_common.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_cli_generate_cache.py` & `odc-stats-1.0.9/odc/stats/_cli_generate_cache.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_cli_generate_mosaic.py` & `odc-stats-1.0.9/odc/stats/_cli_generate_mosaic.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_cli_publish_tasks.py` & `odc-stats-1.0.9/odc/stats/_cli_publish_tasks.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_cli_run.py` & `odc-stats-1.0.9/odc/stats/_cli_run.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_cli_save_tasks.py` & `odc-stats-1.0.9/odc/stats/_cli_save_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import click
 import sys
 from ._cli_common import main, click_range2d
 from .utils import fuse_products, fuse_ds
-from odc.index import ordered_dss, dataset_count
+from odc.dscache.tools import ordered_dss, dataset_count
 from itertools import groupby
 
 
 @main.command("save-tasks")
 @click.option(
     "--grid",
     type=str,
```

### Comparing `odc-stats-1.0.8/odc/stats/_gjson.py` & `odc-stats-1.0.9/odc/stats/_gjson.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 import toolz
 from typing import Tuple, Dict, Any
 from datetime import timedelta
 
 from datacube.model import GridSpec
 from datacube.utils.geometry import polygon_from_transform, Geometry
-from odc.index import solar_offset
+from odc.dscache.tools import solar_offset
 from .model import TileIdx_xy, TileIdx_txy
 
 
 def gs_bounds(gs: GridSpec, tiles: Tuple[Tuple[int, int], Tuple[int, int]]) -> Geometry:
     """
     Compute Polygon for a selection of tiles.
 
@@ -35,15 +35,15 @@
 
 
 def compute_grid_info(
     cells: Dict[TileIdx_xy, Any], resolution: float = math.inf, title_width: int = 0
 ) -> Dict[TileIdx_xy, Any]:
     """
     Compute geojson feature for every cell in ``cells``.
-    Where ``cells`` is produced by ``odc.index.bin_dataset_stream``
+    Where ``cells`` is produced by ``bin_dataset_stream``
     """
     if title_width == 0:
         nmax = max([max(abs(ix), abs(iy)) for ix, iy in cells])
         # title_width is the number of digits in the index
         title_width = len(str(nmax))
 
     grid_info = {}
```

### Comparing `odc-stats-1.0.8/odc/stats/_sqs.py` & `odc-stats-1.0.9/odc/stats/_sqs.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_stac_fetch.py` & `odc-stats-1.0.9/odc/stats/_stac_fetch.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/_text.py` & `odc-stats-1.0.9/odc/stats/_text.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/io.py` & `odc-stats-1.0.9/odc/stats/io.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/model.py` & `odc-stats-1.0.9/odc/stats/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import math
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta, timezone
-from typing import Any, Dict, List, Optional, Tuple, Union
-from uuid import UUID
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from uuid import UUID, uuid5
 from pathlib import Path
 
 import pandas as pd
 import pystac
 import xarray as xr
 from datacube.model import Dataset
 from datacube.utils.dates import normalise_dt
 from datacube.utils.geometry import GeoBox
-from odc.index import odc_uuid
 from ._text import split_and_check
 from pystac.extensions.projection import ProjectionExtension
 from toolz import dicttoolz
 from rasterio.crs import CRS
 import warnings
 
 from eodatasets3.assemble import DatasetAssembler, serialise
@@ -28,14 +27,46 @@
 TileIdx_xy = Tuple[int, int]
 TileIdx_txy = Tuple[str, int, int]
 TileIdx = Union[TileIdx_txy, TileIdx_xy]
 
 default_href_prefix = "https://collections.dea.ga.gov.au/product"
 EXT_TIFF = "tif"  # because "consistency"
 
+# Some random UUID to be ODC namespace
+ODC_NS = UUID("6f34c6f4-13d6-43c0-8e4e-42b6c13203af")
+
+
+def odc_uuid(
+    algorithm: str,
+    algorithm_version: str,
+    sources: Sequence[UUID],
+    deployment_id: str = "",
+    **other_tags,
+) -> UUID:
+    """
+    Generate deterministic UUID for a derived Dataset.
+
+    :param algorithm: Name of the algorithm
+    :param algorithm_version: Version string of the algorithm
+    :param sources: Sequence of input Dataset UUIDs
+    :param deployment_id: Some sort of identifier for installation that performs
+                          the run, for example Docker image hash, or dea module version on NCI.
+    :param **other_tags: Any other identifiers necessary to uniquely identify dataset
+    """
+    tags = [f"{k}={str(v)}" for k, v in other_tags.items()]
+
+    stringified_sources = (
+        [str(algorithm), str(algorithm_version), str(deployment_id)]
+        + sorted(tags)
+        + [str(u) for u in sorted(sources)]
+    )
+
+    srcs_hashes = "\n".join(s.lower() for s in stringified_sources)
+    return uuid5(ODC_NS, srcs_hashes)
+
 
 def format_datetime(dt: datetime, with_tz=True, timespec="microseconds") -> str:
     dt = normalise_dt(dt)
     dt = dt.isoformat(timespec=timespec)
     if with_tz:
         dt = dt + "Z"
     return dt
@@ -652,8 +683,8 @@
     # Renew work token when this close to deadline (seconds)
     renew_safety_margin: int = 30
 
     # How often future is checked for timeout/sqs renew
     future_poll_interval: float = 5
 
     def __post_init__(self):
-        self.cog_opts = dicttoolz.merge(self.default_cog_settings(), self.cog_opts)
+        self.cog_opts = dicttoolz.merge(self.default_cog_settings(), self.cog_opts)
```

### Comparing `odc-stats-1.0.8/odc/stats/plugins/_base.py` & `odc-stats-1.0.9/odc/stats/plugins/_base.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/_registry.py` & `odc-stats-1.0.9/odc/stats/plugins/_registry.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/fc_percentiles.py` & `odc-stats-1.0.9/odc/stats/plugins/fc_percentiles.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,55 +43,89 @@
         4. Calculate the clear wet pixels
         5. Drop the WOfS band
         """
 
         water = xx.water & 0b1110_1111
         xx = xx.drop_vars(["water"])
 
+        # Pick out the dry pixels
+        dry = water == 0
+
+        # Pick out the pixels that have an unmixing error of less than 30
         unmixing_error_lt_30 = xx.ue < 30
         xx = xx.drop_vars(["ue"])
 
-        dry = water == 0
-        dry_and_ue_lt_30 = dry & unmixing_error_lt_30
+        # Sum the bands and pick out only pixels that sum to less than 120
+        # Also clips to 0-100
+        sum_bands = None
+        for band in xx.data_vars.keys():
+            attributes = xx[band].attrs
+            mask = xx[band] == NODATA
+            band_data = keep_good_only(xx[band], ~mask, nodata=0)
+            if sum_bands is None:
+                sum_bands = band_data
+            else:
+                sum_bands = sum_bands + band_data
+
+            # Note: clipping to 0-100
+            clipped = np.clip(xx[band], 0, 100)
+            # Set masked values back to 255
+            xx[band] = clipped.where(~mask, NODATA)
+            xx[band].attrs = attributes
+
+        # Note: hard limit of 120 for the sum of values.
+        sum_lt_120 = sum_bands < 120
+
+        valid = dry & unmixing_error_lt_30 & sum_lt_120
+
+        xx = keep_good_only(xx, valid, nodata=NODATA)
 
-        xx = keep_good_only(xx, dry_and_ue_lt_30, nodata=NODATA)
         xx["wet"] = water == 128
+        xx["valid"] = valid
 
         return xx
 
     def fuser(self, xx):
         wet = xx["wet"]
-        xx = _xr_fuse(xx.drop_vars(["wet"]), partial(_fuse_mean_np, nodata=NODATA), "")
+        valid = xx["valid"]
 
-        band, *bands = xx.data_vars.keys()
-        all_bands_invalid = xx[band] == NODATA
-        for band in bands:
-            all_bands_invalid &= xx[band] == NODATA
+        xx = _xr_fuse(xx.drop_vars(["wet", "valid"]), partial(_fuse_mean_np, nodata=NODATA), "")
+
+        # Not sure why we're doing this... alex leith, 2021-12
+        # band, *bands = xx.data_vars.keys()
+        # all_bands_nodata = xx[band] == NODATA
+        # for band in bands:
+        #     all_bands_nodata &= xx[band] == NODATA
+
+        # This used to have "& all_bands_nodata"
+        xx["wet"] = _xr_fuse(wet, _fuse_or_np, wet.name)
+        xx["valid"] = _xr_fuse(valid, _fuse_or_np, valid.name)
 
-        xx["wet"] = _xr_fuse(wet, _fuse_or_np, wet.name) & all_bands_invalid
         return xx
 
     def reduce(self, xx: xr.Dataset) -> xr.Dataset:
         # (!all_bands_valid) & is_ever_wet => 0
         # (!all_bands_valid) & (!is_ever_wet) => 1
         # all_bands_valid => 2
 
         wet = xx["wet"]
-        xx = xx.drop_vars(["wet"])
+        valid = xx["valid"]
+        xx = xx.drop_vars(["wet", "valid"])
 
         yy = xr_quantile_bands(xx, [0.1, 0.5, 0.9], nodata=NODATA)
         is_ever_wet = _or_fuser(wet).squeeze(wet.dims[0], drop=True)
 
         band, *bands = yy.data_vars.keys()
         all_bands_valid = yy[band] != NODATA
         for band in bands:
             all_bands_valid &= yy[band] != NODATA
 
         all_bands_valid = all_bands_valid.astype(np.uint8)
         is_ever_wet = is_ever_wet.astype(np.uint8)
         yy["qa"] = 1 + all_bands_valid - is_ever_wet * (1 - all_bands_valid)
-        yy["count_valid"] = all_bands_valid
+
+        yy["count_valid"] = valid.sum(axis=0, dtype="int16")
 
         return yy
 
 
 register("fc-percentiles", StatsFCP)
```

### Comparing `odc-stats-1.0.8/odc/stats/plugins/gm.py` & `odc-stats-1.0.9/odc/stats/plugins/gm.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/gm_ls_bitmask.py` & `odc-stats-1.0.9/odc/stats/plugins/gm_ls_bitmask.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/pq.py` & `odc-stats-1.0.9/odc/stats/plugins/pq.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/pq_bitmask.py` & `odc-stats-1.0.9/odc/stats/plugins/pq_bitmask.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/tcw_percentiles.py` & `odc-stats-1.0.9/odc/stats/plugins/tcw_percentiles.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/plugins/wofs.py` & `odc-stats-1.0.9/odc/stats/plugins/wofs.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/proc.py` & `odc-stats-1.0.9/odc/stats/proc.py`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/odc/stats/tasks.py` & `odc-stats-1.0.9/odc/stats/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from odc.dscache import DatasetCache
 from datacube import Datacube
 from datacube.model import Dataset, GridSpec
 from datacube.utils.geometry import Geometry
 from datacube.utils.documents import transform_object_tree
 from datacube.utils.dates import normalise_dt
 
-from odc.index import chopped_dss, bin_dataset_stream, dataset_count, all_datasets
+from odc.dscache.tools import chopped_dss, bin_dataset_stream, dataset_count, all_datasets
 from odc.dscache.tools.tiling import parse_gridspec_with_name
 from odc.dscache.tools.profiling import ds_stream_test_func
 from ._text import split_and_check
 
 from odc.aws import s3_download, s3_url_parse
 from itertools import chain
```

### Comparing `odc-stats-1.0.8/odc/stats/utils.py` & `odc-stats-1.0.9/odc/stats/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import toolz
 from typing import Dict, Tuple, List, Any, Callable, Optional
 from collections import namedtuple
 from datetime import datetime
-from .model import DateTimeRange
-from odc.index import odc_uuid
+from .model import DateTimeRange, odc_uuid
 from datacube.storage import measurement_paths
 from datacube.model import Dataset, DatasetType
 from datacube.index.eo3 import prep_eo3
 
 
 CompressedDataset = namedtuple("CompressedDataset", ["id", "time"])
 Cell = Any
```

### Comparing `odc-stats-1.0.8/odc_stats.egg-info/PKG-INFO` & `odc-stats-1.0.9/odc_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-stats
-Version: 1.0.8
+Version: 1.0.9
 Summary: Statistical Product Generation Framework
 Home-page: https://github.com/opendatacube/odc-stats/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-stats-1.0.8/odc_stats.egg-info/SOURCES.txt` & `odc-stats-1.0.9/odc_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odc-stats-1.0.8/setup.cfg` & `odc-stats-1.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 	click
 	dask
 	datacube
 	distributed
 	numpy
 	odc-cloud[ASYNC]
 	odc_algo
-	odc_dscache
-	odc_stac
+	odc_dscache>=0.2.2
 	pandas
 	pystac>=1.1.0
 	eodatasets3>=0.22.0
 	toolz
 	tqdm
 	xarray
```

