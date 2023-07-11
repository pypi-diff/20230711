# Comparing `tmp/climatePy-0.4.25.tar.gz` & `tmp/climatePy-0.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.25.tar", last modified: Mon Jul 10 21:24:10 2023, max compression
+gzip compressed data, was "climatePy-0.4.26.tar", last modified: Tue Jul 11 15:00:53 2023, max compression
```

## Comparing `climatePy-0.4.25.tar` & `climatePy-0.4.26.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.049995 climatePy-0.4.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 21:24:07.000000 climatePy-0.4.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:24:10.049995 climatePy-0.4.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 21:24:07.000000 climatePy-0.4.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.009995 climatePy-0.4.25/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.009995 climatePy-0.4.25/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.009995 climatePy-0.4.25/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 21:24:10.000000 climatePy-0.4.25/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:24:10.049995 climatePy-0.4.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 21:24:09.000000 climatePy-0.4.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.049995 climatePy-0.4.25/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:07.000000 climatePy-0.4.25/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-10 21:24:07.000000 climatePy-0.4.25/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-10 21:24:07.000000 climatePy-0.4.25/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.368823 climatePy-0.4.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 15:00:50.000000 climatePy-0.4.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-11 15:00:53.368823 climatePy-0.4.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 15:00:50.000000 climatePy-0.4.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.320822 climatePy-0.4.26/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59297 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.324822 climatePy-0.4.26/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.324822 climatePy-0.4.26/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:00:53.368823 climatePy-0.4.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 15:00:52.000000 climatePy-0.4.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.368823 climatePy-0.4.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:50.000000 climatePy-0.4.26/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 15:00:50.000000 climatePy-0.4.26/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 15:00:50.000000 climatePy-0.4.26/tests/test_utils.py
```

### Comparing `climatePy-0.4.25/LICENSE` & `climatePy-0.4.26/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.25/PKG-INFO` & `climatePy-0.4.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.25
+Version: 0.4.26
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.25/README.md` & `climatePy-0.4.26/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.25/climatePy/__init__.py` & `climatePy-0.4.26/climatePy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     return data
 
 from ._climatepy_filter import climatepy_filter
 from ._dap import dap, dap_crop, dap_get
 from ._shortcuts import getTerraClim, getTerraClimNormals, getGridMET, getMACA, \
     get3DEP, getLOCA, getPRISM, getPolaris, \
     getBCCA, getLivneh, getLivneh_fluxes, getISRIC_soils, getDaymet, \
-    getVIC, getNASADEM, getWorldClim, getCHIRPS, getLCMAP, getNLDAS
+    getVIC, getNASADEM, getWorldClim, getCHIRPS, getLCMAP, getNLDAS, getGLDAS, getMODIS
+from ._netrc_utils import writeDodsrc, writeNetrc, getNetrcPath, getDodsrcPath, checkNetrc, checkDodsrc
 
 __all__ = [
+    'params',
     'climatepy_filter',
     'dap',
     'dap_crop',
     'dap_get',
     'getTerraClim',
     'getTerraClimNormals', 
     'getGridMET', 
@@ -41,15 +43,22 @@
     'getDaymet',
     'getVIC', 
     'getNASADEM', 
     'getWorldClim', 
     'getCHIRPS', 
     'getLCMAP',
     'getNLDAS',
-    'params'
+    'getGLDAS',
+    'getMODIS',
+    'writeDodsrc',
+    'writeNetrc',
+    'getNetrcPath',
+    'getDodsrcPath',
+    'checkNetrc',
+    'checkDodsrc'
 ]
 
 ##############################
 # # Old method
 # import pandas as pd
 # import pkg_resources
```

### Comparing `climatePy-0.4.25/climatePy/_climatepy_filter.py` & `climatePy-0.4.26/climatePy/_climatepy_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,23 +292,23 @@
         if scenario is not None:
             if isinstance(scenario, str):
                 catalog = catalog[catalog['scenario'].str.contains(scenario)]
             elif isinstance(scenario, list):
                 catalog = catalog[catalog['scenario'].str.contains('|'.join(scenario))]
 
     # # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
-    # if isinstance(AOI, (shapely.geometry.point.Point, 
-    #         shapely.geometry.multipoint.MultiPoint,
-    #         shapely.geometry.linestring.LineString, 
-    #         shapely.geometry.multilinestring.MultiLineString, 
-    #         shapely.geometry.polygon.Polygon, 
-    #         shapely.geometry.multipolygon.MultiPolygon)):
+    if isinstance(AOI, (shapely.geometry.point.Point, 
+            shapely.geometry.multipoint.MultiPoint,
+            shapely.geometry.linestring.LineString, 
+            shapely.geometry.multilinestring.MultiLineString, 
+            shapely.geometry.polygon.Polygon, 
+            shapely.geometry.multipolygon.MultiPolygon)):
         
-    #     # convert shapely geometry to geopandas dataframe
-    #     AOI = shapely_to_gpd(AOI)
+        # convert shapely geometry to geopandas dataframe
+        AOI = shapely_to_gpd(AOI)
 
     # 5. AOI filter
     if AOI is not None:
         catalog = find_intersects(
             catalog = catalog,
             AOI     = AOI
             )
```

### Comparing `climatePy-0.4.25/climatePy/_dap.py` & `climatePy-0.4.26/climatePy/_dap.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,29 +375,29 @@
             dap_data = dap_crop(
                 URL       = URL,
                 catalog   = catalog,
                 AOI       = AOI,
                 startDate = startDate,
                 endDate   = endDate,
                 varname   = varname,
-                verbose   = verbose
+                verbose   = False
                 )
             
             # if dopar:
             #     if verbose:
             #         print("Getting DAP data in parallel")
             # else:
             #     if verbose:
             #         print("Getting DAP data in serial")
 
             # get dap data
             dap_data = dap_get(
                 dap_data = dap_data,
                 dopar    = dopar,
-                verbose  = verbose
+                verbose  = False
                 )
             
             return dap_data
         
 def match_args(func, *args, **kwargs):
 
     """Match default arguments for a function.
@@ -532,15 +532,16 @@
     ymax = dap_row['Yn'] + 0.5 * resy
 
     # expand dimensions of 'var' if it's a 2D array
     if var.ndim == 2:
         var = np.expand_dims(var, axis=-1)
     
     # check if size of first dimension of 'var' is equals number of rows in 'dap'
-    if var.shape[2] != dap_row["nrows"]:
+    if var.shape[2] != dap_row["nrows"] or dap_row["nrows"] == dap_row["ncols"]:
+    # if var.shape[2] != dap_row["nrows"]:
         # transpose the first two dimensions of 'var' if not in correct order
         var = var.transpose(dap_row["Y_name"], dap_row["X_name"], dap_row["T_name"])
         # var2 = var.transpose(dap_row["T_name"], dap_row["X_name"],  dap_row["Y_name"])
     
     # Create the DataArray with the CRS included
     r = xr.DataArray(
         var,
```

### Comparing `climatePy-0.4.25/climatePy/_netrc_utils.py` & `climatePy-0.4.26/climatePy/_netrc_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,43 +78,62 @@
     with open(dodsrcFile, 'r') as f:
         lines = f.readlines()
         lines = [re.sub("http.*//", "", line) for line in lines]
     
     return any(netrcFile in line for line in lines)
 
 def writeDodsrc(
-        netrcFile  = getNetrcPath(),
-        dodsrcFile = getDodsrcPath(), 
-        overwrite  = False
+        netrcFile  = None,
+        dodsrcFile = ".dodsrc"
         ):
     
-    if (checkDodsrc(dodsrcFile, netrcFile) and not overwrite):
-        raise ValueError(f"{dodsrcFile} already exists. Set `overwrite=True` if you'd like to overwrite.")
+    if not netrcFile:
+        netrcFile = getNetrcPath()
+
+    # if not dodsrcFile:
+    #     dodsrcFile = getDodsrcPath()
+
+    # if (checkDodsrc(dodsrcFile, netrcFile) and not overwrite):
+    #     raise ValueError(f"{dodsrcFile} already exists. Set `overwrite=True` if you'd like to overwrite.")
     
     dir = os.path.dirname(dodsrcFile)
-    
+
+    # string = f'USE_CACHE=0\n\
+    #     MAX_CACHE_SIZE=20\n\
+    #     MAX_CACHED_OBJ=5\n\
+    #     IGNORE_EXPIRES=0\n\
+    #     CACHE_ROOT={dir}/.dods_cache/\n\
+    #     DEFAULT_EXPIRES=86400\n\
+    #     ALWAYS_VALIDATE=0\n\
+    #     DEFLATE=0\n\
+    #     VALIDATE_SSL=1\n\
+    #     HTTP.COOKIEJAR={dir}/.cookies\n\
+    #     HTTP.NETRC={netrcFile}'
+
     string = f'USE_CACHE=0\n\
         MAX_CACHE_SIZE=20\n\
         MAX_CACHED_OBJ=5\n\
         IGNORE_EXPIRES=0\n\
-        CACHE_ROOT={dir}/.dods_cache/\n\
         DEFAULT_EXPIRES=86400\n\
         ALWAYS_VALIDATE=0\n\
         DEFLATE=0\n\
         VALIDATE_SSL=1\n\
-        HTTP.COOKIEJAR={dir}/.cookies\n\
+        HTTP.COOKIEJAR={dir}/.urs_cookies\n\
         HTTP.NETRC={netrcFile}'
     
     # create a dodsrc file
     with open(os.path.expanduser(dodsrcFile), 'w') as f:
         f.write(string)
         
     # set the owner-only permission
     os.chmod(dodsrcFile, 0o600)
 
+
+    return dodsrcFile
+
 def check_rc_files(
         dodsrcFile = getDodsrcPath(), 
         netrcFile  = getNetrcPath()
         ):
     
     if not checkDodsrc(dodsrcFile, netrcFile):
         if checkNetrc(netrcFile):
```

### Comparing `climatePy-0.4.25/climatePy/_shortcuts.py` & `climatePy-0.4.26/climatePy/_shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Data manipulation tools
 import pandas as pd
 import geopandas as gpd
 import xarray as xr
 import shapely
 from shapely.geometry import Point
 
+#  os lib
+import os
+
 # import climatePy modules
 from . import _utils as utils
 from . import _dap as dap
 from . import _climatepy_filter as climatepy_filter
+from . import _netrc_utils as netrc_utils
 
 # import climatePy._utils as utils
 # from climatePy import params
 # from climatePy import _dap as dap
 # from climatePy import _climatepy_filter as climatepy_filter
 
 # warnings lib
@@ -195,57 +199,126 @@
     
     return dap_data
 
 # --------------------
 # ---- getGLDAS  ----
 # --------------------
 
-# TODO: ADD GLDAS and need check_rc_files() function 
-# def getGLDAS(
-#         AOI       = None,
-#         varname   = None,
-#         startDate = None, 
-#         endDate   = None, 
-#         model     = None,
-#         verbose   = False
-#         ):
-    
-#     """Get GLDAS Data for an Area of Interest
-
-#     Args:
-#         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-#         varname (list): Variable name(s) to download.
-#         startDate (str): Start date in the form "YYYY-MM-DD"
-#         endDate (str): End date in the form "YYYY-MM-DD"
-#         model (str): Model to download.
-#         verbose (bool): Print verbose output
-
-#     Returns:
-#         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-#     """
-
-#     # get matching arguments for climatepy_filter function
-#     dap_meta = dap.climatepy_dap(
-#         AOI       = AOI, 
-#         id        = "GLDAS", 
-#         varname   = varname, 
-#         startDate = startDate, 
-#         endDate   = endDate,
-#         verbose   = verbose
-#         )
-    
-#     # dap_meta['dopar'] = dopar
-
-#     # need to provide dap_meta dictionary object directly as input
-#     dap_data = dap.dap(
-#         **dap_meta
-#         )
+# TODO: Fix netrc and dodsrc file creation process to work with earthdata credentials
+def getGLDAS(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        model     = None,
+        verbose   = False
+        ):
     
-#     return dap_data
+    """Get GLDAS Data for an Area of Interest
 
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        model (str): Model to download.
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+
+    if not netrc_utils.checkNetrc():
+
+        raise Exception("netrc file not found. Please run writeNetrc() with earth data credentials..")
+    
+    else:
+
+        x = netrc_utils.writeDodsrc()
+
+        # get matching arguments for climatepy_filter function
+        dap_meta = dap.climatepy_dap(
+            AOI       = AOI, 
+            id        = "GLDAS", 
+            varname   = varname, 
+            startDate = startDate, 
+            endDate   = endDate,
+            verbose   = verbose
+            )
+        
+        # dap_meta['dopar'] = dopar
+
+        # need to provide dap_meta dictionary object directly as input
+        dap_data = dap.dap(
+            **dap_meta
+            )
+        
+        # remove dodsrc file
+        os.unlink(x)
+
+        return dap_data
+    
+# --------------------
+# ---- getMODIS  ----
+# --------------------
+
+
+def getMODIS(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        model     = None,
+        verbose   = False
+        ):
+    
+    """Get MODIS Data for an Area of Interest
+
+    Args:
+        AOI (geopandas dataframe, shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        model (str): Model to download.
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+    
+    if not netrc_utils.checkNetrc():
+
+        raise Exception("netrc file not found. Please run writeNetrc() with earth data credentials..")
+    
+    else:
+
+        x = netrc_utils.writeDodsrc()
+
+        # get matching arguments for climatepy_filter function
+        dap_meta = dap.climatepy_dap(
+            AOI       = AOI, 
+            id        = "MODIS", 
+            varname   = varname, 
+            startDate = startDate, 
+            endDate   = endDate,
+            verbose   = verbose
+            )
+        
+        # dap_meta['dopar'] = dopar
+
+        # need to provide dap_meta dictionary object directly as input
+        dap_data = dap.dap(
+            **dap_meta
+            )
+        
+        # remove dodsrc file
+        os.unlink(x)
+
+        return dap_data
+    
 # -------------------
 # ---- getDaymet ----
 # -------------------
 
 def getDaymet(
         AOI       = None,
         varname   = None,
@@ -573,32 +646,42 @@
         endDate (str): End date in the form "YYYY-MM-DD"
         model (str): Model name. Default is None.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
+    if not netrc_utils.checkNetrc():
 
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "NLDAS", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        model     = model,
-        verbose   = verbose
-        )
+        raise Exception("netrc file not found. Please run writeNetrc() with earth data credentials..")
     
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
+    else:
+
+        x = netrc_utils.writeDodsrc()
+
+        # get matching arguments for climatepy_filter function
+        dap_meta = dap.climatepy_dap(
+            AOI       = AOI,
+            id        = "NLDAS", 
+            varname   = varname, 
+            startDate = startDate, 
+            endDate   = endDate,
+            model     = model,
+            verbose   = verbose
+            )
+        
+        # need to provide dap_meta dictionary object directly as input
+        dap_data = dap.dap(
+            **dap_meta
+            )
+        
+        # unlink Dodsrc file
+        os.unlink(x)
     
-    return dap_data
+        return dap_data
 
 # -----------------
 # ---- getMACA ---- 
 # -----------------
 
 def getMACA(
         AOI       = None,
```

### Comparing `climatePy-0.4.25/climatePy/_utils.py` & `climatePy-0.4.26/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.25/climatePy/data/catalog.csv` & `climatePy-0.4.26/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.25/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.26/climatePy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.25
+Version: 0.4.26
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.25/setup.py` & `climatePy-0.4.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.25',
+    version='0.4.26',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.25/tests/test_shortcuts.py` & `climatePy-0.4.26/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.25/tests/test_utils.py` & `climatePy-0.4.26/tests/test_utils.py`

 * *Files identical despite different names*

