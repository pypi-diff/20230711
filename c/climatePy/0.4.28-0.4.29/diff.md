# Comparing `tmp/climatePy-0.4.28.tar.gz` & `tmp/climatePy-0.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.28.tar", last modified: Tue Jul 11 15:10:37 2023, max compression
+gzip compressed data, was "climatePy-0.4.29.tar", last modified: Tue Jul 11 19:37:08 2023, max compression
```

## Comparing `climatePy-0.4.28.tar` & `climatePy-0.4.29.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.185566 climatePy-0.4.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 15:10:33.000000 climatePy-0.4.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 15:10:37.185566 climatePy-0.4.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-11 15:10:33.000000 climatePy-0.4.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.137565 climatePy-0.4.28/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59297 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.137565 climatePy-0.4.28/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.137565 climatePy-0.4.28/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:10:37.185566 climatePy-0.4.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 15:10:35.000000 climatePy-0.4.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.185566 climatePy-0.4.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:33.000000 climatePy-0.4.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 15:10:33.000000 climatePy-0.4.28/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 15:10:33.000000 climatePy-0.4.28/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.620567 climatePy-0.4.29/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 19:37:04.000000 climatePy-0.4.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 19:37:08.620567 climatePy-0.4.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-11 19:37:04.000000 climatePy-0.4.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.564567 climatePy-0.4.29/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60892 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.568568 climatePy-0.4.29/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.568568 climatePy-0.4.29/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:37:08.620567 climatePy-0.4.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 19:37:06.000000 climatePy-0.4.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.620567 climatePy-0.4.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:04.000000 climatePy-0.4.29/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 19:37:04.000000 climatePy-0.4.29/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 19:37:04.000000 climatePy-0.4.29/tests/test_utils.py
```

### Comparing `climatePy-0.4.28/LICENSE` & `climatePy-0.4.29/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/PKG-INFO` & `climatePy-0.4.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.28
+Version: 0.4.29
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.28/README.md` & `climatePy-0.4.29/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/climatePy/__init__.py` & `climatePy-0.4.29/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/climatePy/_climatepy_filter.py` & `climatePy-0.4.29/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/climatePy/_dap.py` & `climatePy-0.4.29/climatePy/_dap.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,16 +285,55 @@
         grid        = None,
         start       = None,
         end         = None,
         toptobottom = False,
         dopar       = True,
         verbose     = False
         ):
+
+        """Get Data (Data Access Protocol)
+
+        This function provides a consistent data access protocol (DAP) to a wide
+        range of local and remote resources including VRT, TDS, NetCDF.
+        
+        Define and get data from a DAP resource.
+        
+        Parameters:
+        - URL: str, optional
+            Local file path or URL.
+        - catalog: object, optional
+            Subset of open.dap catalog.
+        - AOI: object, optional
+            List containing an extent() and crs.
+        - startDate: object, optional
+            For non "dated" items, start can be called by index.
+        - endDate: object, optional
+            For non "dated" items, end can be called by index.
+        - varname: object, optional
+            Variable name.
+        - grid: object, optional
+            A list containing an extent() and crs.
+        - start: object, optional
+            For non "dated" items, start can be called by index.
+        - end: object, optional
+            For non "dated" items, end can be called by index.
+        - toptobottom: bool, optional
+            Should data be inverse?
+        - dopar: bool, if True, parallelize the download of the data 
+        - verbose: bool, optional
+            Should dap_summary be printed?
+        
+        Details:
+        Wraps dap_get and dap_crop into one.
+        If AOI is None, no spatial crop is executed.
+        If startDate and endDate are None, no temporal crop is executed.
+        If only endDate is None, it defaults to the startDate.
         
-        """Get data from a DAP server"""
+        Returns: dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+        """
     
 
         if not isinstance(toptobottom, bool):
 
             # print("Checking if all toptobottom values are Nan...")
 
             # convert to float to check for nan
```

### Comparing `climatePy-0.4.28/climatePy/_netrc_utils.py` & `climatePy-0.4.29/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/climatePy/_shortcuts.py` & `climatePy-0.4.29/climatePy/_shortcuts.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,27 +35,29 @@
 # ----------------------
 
 def getTerraClim(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get Terra Climate Normals for an Area of Interest
 
     These layers from TerraClimate were creating using climatically aided interpolation of monthly anomalies from the CRU Ts4.0 
     and Japanese 55-year Reanalysis (JRA-55) datasets with WorldClim v2.0 climatologies.
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to be extracted
         startDate (str): Start date for data extraction in YYYY-MM-DD format
         endDate (str): End date for data extraction in YYYY-MM-DD format
+        dopar (bool): Use parallel processing
         verbose (bool): Print out additional information
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
     # get matching arguments for climatepy_filter function
     dap_meta = dap.climatepy_dap(
@@ -63,15 +65,17 @@
         AOI       = AOI, 
         id        = "terraclim", 
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
     # dap_data = dap(
         **dap_meta
         )
     
     return dap_data
@@ -86,27 +90,29 @@
 # -----------------------------
 
 def getTerraClimNormals(
         AOI       = None,
         varname   = None,
         month     = [i for i in range(1, 13)],
         scenario  = '19812010', 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get Terra Climate Normals for an Area of Interest
 
     These layers from TerraClimate were creating using climatically aided interpolation of monthly anomalies 
     from the CRU Ts4.0 and Japanese 55-year Reanalysis (JRA-55) datasets with WorldClim v2.0 climatologies.
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to be extracted
         month (int, list): Month(s) to extract data for
         scenario (str): Scenario to extract data for
+        dopar (bool): Use parallel processing
         verbose (bool): Print out additional information
     
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
 
     """
 
@@ -142,42 +148,45 @@
     # call dap
     dap_data = dap.dap(
         catalog   = raw, 
         AOI       = AOI, 
         startDate = min(dates).strftime("%Y-%m-%d"),
         endDate   = max(dates).strftime("%Y-%m-%d"), 
         varname   = varname,
+        dopar     = dopar,
         verbose   = verbose
         )
 
     return dap_data
 
 # --------------------
 # ---- getGridMET ----
 # --------------------
 
 def getGridMET(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get GridMet Climate Data for an Area of Interest
 
     gridMET is a dataset of daily high-spatial resolution (~4-km, 1/24th degree) surface meteorological data 
     covering the contiguous US from 1979-yesterday. These data are updated daily.
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (list): Variable name(s) to download. Options include:
             ['pr', 'rmin', 'rmax', 'srad', 'sph', 'swe', 'tmmn', 'tmmx', 'vs', 'vpd', 'ws']
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
 
     # get matching arguments for climatepy_filter function
@@ -186,15 +195,15 @@
         id        = "gridmet", 
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
     
-    # dap_meta['dopar'] = dopar
+    dap_meta['dopar'] = dopar
 
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
@@ -206,25 +215,27 @@
 # TODO: Fix netrc and dodsrc file creation process to work with earthdata credentials
 def getGLDAS(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         model     = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get GLDAS Data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         model (str): Model to download.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
 
     if not netrc_utils.checkNetrc():
@@ -241,15 +252,15 @@
             id        = "GLDAS", 
             varname   = varname, 
             startDate = startDate, 
             endDate   = endDate,
             verbose   = verbose
             )
         
-        # dap_meta['dopar'] = dopar
+        dap_meta['dopar'] = dopar
 
         # need to provide dap_meta dictionary object directly as input
         dap_data = dap.dap(
             **dap_meta
             )
         
         # remove dodsrc file
@@ -264,25 +275,27 @@
 
 def getMODIS(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         model     = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get MODIS Data for an Area of Interest
 
     Args:
         AOI (geopandas dataframe, shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         model (str): Model to download.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
     
     if not netrc_utils.checkNetrc():
@@ -299,15 +312,15 @@
             id        = "MODIS", 
             varname   = varname, 
             startDate = startDate, 
             endDate   = endDate,
             verbose   = verbose
             )
         
-        # dap_meta['dopar'] = dopar
+        dap_meta['dopar'] = dopar
 
         # need to provide dap_meta dictionary object directly as input
         dap_data = dap.dap(
             **dap_meta
             )
         
         # remove dodsrc file
@@ -320,14 +333,15 @@
 # -------------------
 
 def getDaymet(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get Daymet Climate Data for an Area of Interest
 
     This dataset provides Daymet Version 4 model output data as gridded estimates of daily weather parameters for North America.
     Daymet output variables include the following parameters: minimum temperature, maximum temperature, precipitation, shortwave radiation,
@@ -338,14 +352,15 @@
     Conic projection for North America and are in a netCDF file format compliant with Climate and Forecast (CF) metadata conventions.
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (list): Variable name(s) to download. Options include:	
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
 
     """
 
@@ -354,15 +369,17 @@
         AOI       = AOI, 
         id        = "daymet4", 
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -374,14 +391,15 @@
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None,
         model     = 'CCSM4',
         scenario  = 'rcp45', 
         ensemble  = None,  
+        dopar     = True,
         verbose   = False
         ):
     
     """Get BCCA data for an Area of Interest
 
     This dataset provides BCCA model output data as gridded estimates of daily weather parameters for North America.
 
@@ -389,14 +407,15 @@
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download. Options include:
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         model (str): Model name. Default is 'CCSM4'.
         scenario (str): Scenario name. Default is 'rcp45'.
         ensemble (str): Ensemble name. Default is None.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
 
     """
     # get matching arguments for climatepy_filter function
@@ -407,15 +426,17 @@
         model     = model,
         scenario  = scenario, 
         ensemble  = ensemble, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -424,26 +445,28 @@
 # ------------------
 def getPRISM(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         timeRes   = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get PRISM data for an Area of Interest
         Currently only monthly data is available.
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         timeRes (str): time resolution of data to be downloaded. Options are "daily" or "monthly". Default is "monthly"
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
 
     """
 
@@ -463,14 +486,16 @@
             id        = "prism_monthly",
             # id        = "prism_" + timeRes, 
             varname   = varname, 
             startDate = startDate, 
             endDate   = endDate,
             verbose   = verbose
             )
+        
+        dap_meta['dopar'] = dopar
 
         # need to provide dap_meta dictionary object directly as input
         dap_data = dap.dap(
             **dap_meta
             )
         
         return dap_data
@@ -494,27 +519,29 @@
 
 def getLivneh(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         timeRes   = "daily",
+        dopar     = True,
         verbose   = False
         ):
     
     """Get Livneh Climate Data for an Area of Interest
 
     This dataset provides Livneh model output data as gridded estimates of daily weather parameters for North America.
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         timeRes (str): Time resolution. Options include: "daily" or "monthly". Default is "daily".
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
 
     if timeRes == "daily":
@@ -533,15 +560,17 @@
             AOI       = AOI,
             id        = "Livneh_monthly", 
             varname   = varname, 
             startDate = startDate, 
             endDate   = endDate,
             verbose   = verbose
             )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -550,26 +579,28 @@
 # --------------------------
 
 def getLivneh_fluxes(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get Livneh Fluxes Climate Data for an Area of Interest
 
     This dataset provides Livneh model output data as gridded estimates of daily weather parameters for North America.
     
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
     
     # get matching arguments for climatepy_filter function
@@ -578,14 +609,16 @@
         id        = "Livneh_fluxes", 
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -596,31 +629,48 @@
 def getVIC(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         model     = 'ccsm4', 
         scenario  = 'rcp45',
+        dopar     = True,
         verbose   = False
         ):
     
-    """Get VIC Climate Data for an Area of Interest"""
+    """Get VIC Climate Data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        model (str): Climate model. Options include: 'ccsm4', 'cnrm_cm5', 'gfdl_cm3', 'hadgem2_es', 'ipsl_cm5a_lr', 'miroc_esm', 'mri_cgcm3', 'noresm1_m'
+        scenario (str): Climate scenario. Options include: 'rcp45', 'rcp85'
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
 
     # get matching arguments for climatepy_filter function
     dap_meta = dap.climatepy_dap(
         AOI       = AOI,
         id        = "bcsd_vic", 
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         model     = model,
         scenario  = scenario,
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -630,25 +680,27 @@
 
 def getNLDAS(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         model     = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get NLDAS Climate Data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         model (str): Model name. Default is None.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """
     if not netrc_utils.checkNetrc():
 
@@ -665,14 +717,16 @@
             varname   = varname, 
             startDate = startDate, 
             endDate   = endDate,
             model     = model,
             verbose   = verbose
             )
         
+        dap_meta['dopar'] = dopar
+        
         # need to provide dap_meta dictionary object directly as input
         dap_data = dap.dap(
             **dap_meta
             )
         
         # unlink Dodsrc file
         os.unlink(x)
@@ -687,14 +741,15 @@
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         timeRes   = 'day',
         model     = 'CCSM4', 
         scenario  = 'rcp45', 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get MACA Climate Data for an Area of Interest
 
     Multivariate Adaptive Constructed Analogs (MACA) is a statistical method for downscaling Global Climate Models
     (GCMs) from their native coarse resolution to a higher spatial resolution that captures reflects 
@@ -704,14 +759,15 @@
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         timeRes (str): Time resolution. Either "mmonth" or "day". Default is 'day'.
         model (str): Model name. Default is 'CCSM4'.
         scenario (str): Scenario name. Default is 'rcp45'.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
 
     """
     
@@ -726,15 +782,17 @@
         varname   = varname, 
         model     = model,
         scenario  = scenario, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -745,27 +803,29 @@
 # TODO: too much data is extracted when function is called, need to look into what is going on here with the dap function
 # TODO: currently crashes my computer, even when I try to run on a small AOI and for a short time period
 def getCHIRPS(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get CHIRPS data for an Area of Interest
 
     CHIRPS is a global dataset of daily precipitation estimates, with a spatial resolution of 0.05 degrees (~5 km).
     Currently only monthly data is available.
 
     Args:
         AOI (geopandas dataframe, shapely geometry): Area of Interest polygon to extract data for.
         varname (str): variable name to extract (e.g. tmin).
         startDate (str): start date of data to be downloaded (YYYY-MM-DD). Default is None.
         endDate (str): end date of data to be downloaded (YYYY-MM-DD). Default is None.
+        dopar (bool): use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): print verbose output. Default is False.
     """
 
     timeRes = "monthly"
 
     # make sure timeRes is capitalized correctly
     timeRes = " ".join(word.capitalize() for word in timeRes.split())
@@ -786,15 +846,17 @@
         AOI       = AOI, 
         id        = "chirps20Global" + timeRes + "P05", 
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -805,14 +867,15 @@
 def getLOCA(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
         model     = 'CCSM4',
         scenario  = 'rcp45',
+        dopar     = True,
         verbose   = False
         ):
     
     """Get LOCA Climate Data for an Area of Interest
 
     LOCA is a statistical downscaling technique that uses past history to add improved fine-scale detail to global climate models.
 
@@ -824,14 +887,15 @@
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
         model (str): Model name. Default is 'CCSM4'.
         scenario (str): Scenario name. Default is 'rcp45'.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
 
     """
 
@@ -842,29 +906,32 @@
         varname   = varname, 
         startDate = startDate, 
         endDate   = endDate,
         model     = model,
         scenario  = scenario,
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
 # --------------------
 # ---- getPolaris ----
 # --------------------
 
 def getPolaris(
         AOI       = None,
         varname   = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get Polaris Climate Data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
@@ -879,15 +946,17 @@
     # get matching arguments for climatepy_filter function
     dap_meta = dap.climatepy_dap(
         AOI       = AOI, 
         id        = "polaris", 
         varname   = varname, 
         verbose   = verbose
         )
-
+    
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -897,24 +966,26 @@
 
 # TODO this function throws an error on the first call and succeeds on the second call (temp file issue?) 
 def getWorldClim(
         AOI       = None,
         varname   = None,
         date 	  = None,
         res       = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get WorldClim data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         date (str): date in the form "YYYY-MM-DD"
         res (str): Resolution of data to download. One of: "10m", "5m", "2.5m", "30s". Default is "10m".
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """	
 
     if res is None:
@@ -929,14 +1000,16 @@
         id        = "wc2.1_" + res,
         varname   = varname,
         startDate = date,
         endDate   = date,
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -944,60 +1017,64 @@
 # ---- getISRIC_soils ----
 # ------------------------
 # getSoilGrids vs getISRIC_soils
 
 def getISRIC_soils(
         AOI       = None,
         varname   = None,
-        date 	  = None,
-        res       = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get ISRIC Soil Grids data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """	
 
     # get matching arguments for climatepy_filter function
     dap_meta = dap.climatepy_dap(
         AOI       = AOI,
         id        = "ISRIC Soil Grids",
         varname   = varname,
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
 # -----------------
 # ---- get3DEP ----
 # -----------------
 
 def get3DEP(
         AOI       = None,
         res       = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get USGS Digatal Elevation Model (DEM) data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         res (str): Resolution of data to download. One of: "10m", "30m". Default is "30m".
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """	
 
     if res is None:
@@ -1012,48 +1089,54 @@
         AOI       = AOI,
         id        = "USGS 3DEP",
         asset     = res + " CONUS DEM",
         varname   = "elevation",
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+    
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
 # --------------------
 # ---- getNASADEM ----
 # --------------------
 
 def getNASADEM(
         AOI       = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get NASA Digatal Elevation Model (DEM) data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """	
 
     # get matching arguments for climatepy_filter function
     dap_meta = dap.climatepy_dap(
         AOI       = AOI,
         id        = "NASADEM",
         varname   = "elevation",
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -1063,25 +1146,27 @@
 
 def AquaGoesSSTAnom(
         AOI       = None,
         varname   = None,
         startDate = None,
         endDate   = None,
         units     = None,
+        dopar     = True,
         verbose   = False
         ):
     
     """Get SST anomolies from AquaGoesSSTAnomC data for an Area of Interest
 
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in "YYYY-MM-DD" format.
         endDate (str): End date in "YYYY-MM-DD" format.
         units: temperature units to return data in "C" or "F". Default is "C".
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """	
 
     if units == None:
@@ -1096,14 +1181,16 @@
         id        = "aquaGoesSSTAnom" + units,
         varname   = varname,
         startDate = startDate,
         endDate   = endDate,
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
 
@@ -1113,24 +1200,26 @@
 # ------------------
 
 def getLCMAP(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        dopar     = True,
         verbose   = False
         ):
     
     """Get LCMAP data for an Area of Interest
     
     Args:
         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
         varname (str, list): Variable name(s) to download.
         startDate (str): Start date in the form "YYYY-MM-DD"
         endDate (str): End date in the form "YYYY-MM-DD"
+        dopar (bool): Use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): Print verbose output. Default is False.
 
     Returns:
         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
     """	
 
     # get matching arguments for climatepy_filter function
@@ -1139,13 +1228,15 @@
         id        = "LCMAP",
         varname   = varname,
         startDate = startDate,
         endDate   = endDate,
         verbose   = verbose
         )
     
+    dap_meta['dopar'] = dopar
+
     # need to provide dap_meta dictionary object directly as input
     dap_data = dap.dap(
         **dap_meta
         )
     
     return dap_data
```

### Comparing `climatePy-0.4.28/climatePy/_utils.py` & `climatePy-0.4.29/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/climatePy/data/catalog.csv` & `climatePy-0.4.29/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.29/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.28
+Version: 0.4.29
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.28/setup.py` & `climatePy-0.4.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.28',
+    version='0.4.29',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.28/tests/test_shortcuts.py` & `climatePy-0.4.29/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.28/tests/test_utils.py` & `climatePy-0.4.29/tests/test_utils.py`

 * *Files identical despite different names*

