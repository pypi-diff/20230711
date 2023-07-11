# Comparing `tmp/climatePy-0.4.27.tar.gz` & `tmp/climatePy-0.4.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.27.tar", last modified: Tue Jul 11 15:07:27 2023, max compression
+gzip compressed data, was "climatePy-0.4.28.tar", last modified: Tue Jul 11 15:10:37 2023, max compression
```

## Comparing `climatePy-0.4.27.tar` & `climatePy-0.4.28.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.325904 climatePy-0.4.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 15:07:21.000000 climatePy-0.4.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-11 15:07:27.321903 climatePy-0.4.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-11 15:07:21.000000 climatePy-0.4.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.265901 climatePy-0.4.27/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59297 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.269901 climatePy-0.4.27/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.269901 climatePy-0.4.27/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:07:27.325904 climatePy-0.4.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 15:07:25.000000 climatePy-0.4.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.321903 climatePy-0.4.27/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:21.000000 climatePy-0.4.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 15:07:21.000000 climatePy-0.4.27/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 15:07:21.000000 climatePy-0.4.27/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.185566 climatePy-0.4.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 15:10:33.000000 climatePy-0.4.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 15:10:37.185566 climatePy-0.4.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-11 15:10:33.000000 climatePy-0.4.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.137565 climatePy-0.4.28/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59297 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.137565 climatePy-0.4.28/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 15:10:33.000000 climatePy-0.4.28/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.137565 climatePy-0.4.28/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:10:37.000000 climatePy-0.4.28/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:10:37.185566 climatePy-0.4.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 15:10:35.000000 climatePy-0.4.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:37.185566 climatePy-0.4.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:10:33.000000 climatePy-0.4.28/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 15:10:33.000000 climatePy-0.4.28/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 15:10:33.000000 climatePy-0.4.28/tests/test_utils.py
```

### Comparing `climatePy-0.4.27/LICENSE` & `climatePy-0.4.28/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/PKG-INFO` & `climatePy-0.4.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.27
+Version: 0.4.28
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -57,29 +57,29 @@
 ## Installation
 
 `climatePy` can be downloaded from PyPI via `pip` like so:
 
 ``` 
 pip install climatePy
 ```
-**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
+**Note:** climatePy is still in **development**
 
 <br>
 
 ## Usage
 
 ### Loading climate catalog
 
 ```python
+import climatePy
 import geopandas as gpd
 import matplotlib.pyplot as plt
-from climatePy import params
 
 # load climate catalog
-catalog = params()
+catalog = climatePy.params()
 
 # load example AOI data
 AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
 ```
 <br>
 
 ### Using `climatepy_filter()`:
@@ -108,15 +108,15 @@
 
 ### Getting climate data in AOI
 
 Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
 
 ```python
 # collect raw meta data
-prcp = shortcuts.getTerraClim(
+prcp = climatePy.getTerraClim(
     AOI       = AOI,
     varname   = "ppt",
     startDate = "2018-01-01",
     endDate   = "2018-01-01"
     )
 ```
 ![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
@@ -126,15 +126,15 @@
 
 ### Get data within a date range
 
 We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
 
 ```python
 # collect raw meta data
-prcp = shortcuts.getTerraClim(
+prcp = climatePy.getTerraClim(
     AOI       = AOI,
     varname   = "ppt",
     startDate = "2018-01-01",
     endDate   = "2018-12-01"
     )
 ```
 ![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
```

### Comparing `climatePy-0.4.27/README.md` & `climatePy-0.4.28/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,29 @@
 ## Installation
 
 `climatePy` can be downloaded from PyPI via `pip` like so:
 
 ``` 
 pip install climatePy
 ```
-**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
+**Note:** climatePy is still in **development**
 
 <br>
 
 ## Usage
 
 ### Loading climate catalog
 
 ```python
+import climatePy
 import geopandas as gpd
 import matplotlib.pyplot as plt
-from climatePy import params
 
 # load climate catalog
-catalog = params()
+catalog = climatePy.params()
 
 # load example AOI data
 AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
 ```
 <br>
 
 ### Using `climatepy_filter()`:
@@ -96,15 +96,15 @@
 
 ### Getting climate data in AOI
 
 Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
 
 ```python
 # collect raw meta data
-prcp = shortcuts.getTerraClim(
+prcp = climatePy.getTerraClim(
     AOI       = AOI,
     varname   = "ppt",
     startDate = "2018-01-01",
     endDate   = "2018-01-01"
     )
 ```
 ![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
@@ -114,15 +114,15 @@
 
 ### Get data within a date range
 
 We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
 
 ```python
 # collect raw meta data
-prcp = shortcuts.getTerraClim(
+prcp = climatePy.getTerraClim(
     AOI       = AOI,
     varname   = "ppt",
     startDate = "2018-01-01",
     endDate   = "2018-12-01"
     )
 ```
 ![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
```

### Comparing `climatePy-0.4.27/climatePy/__init__.py` & `climatePy-0.4.28/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy/_climatepy_filter.py` & `climatePy-0.4.28/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy/_dap.py` & `climatePy-0.4.28/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy/_netrc_utils.py` & `climatePy-0.4.28/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy/_shortcuts.py` & `climatePy-0.4.28/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy/_utils.py` & `climatePy-0.4.28/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy/data/catalog.csv` & `climatePy-0.4.28/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.28/climatePy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.27
+Version: 0.4.28
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -57,29 +57,29 @@
 ## Installation
 
 `climatePy` can be downloaded from PyPI via `pip` like so:
 
 ``` 
 pip install climatePy
 ```
-**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
+**Note:** climatePy is still in **development**
 
 <br>
 
 ## Usage
 
 ### Loading climate catalog
 
 ```python
+import climatePy
 import geopandas as gpd
 import matplotlib.pyplot as plt
-from climatePy import params
 
 # load climate catalog
-catalog = params()
+catalog = climatePy.params()
 
 # load example AOI data
 AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
 ```
 <br>
 
 ### Using `climatepy_filter()`:
@@ -108,15 +108,15 @@
 
 ### Getting climate data in AOI
 
 Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
 
 ```python
 # collect raw meta data
-prcp = shortcuts.getTerraClim(
+prcp = climatePy.getTerraClim(
     AOI       = AOI,
     varname   = "ppt",
     startDate = "2018-01-01",
     endDate   = "2018-01-01"
     )
 ```
 ![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
@@ -126,15 +126,15 @@
 
 ### Get data within a date range
 
 We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
 
 ```python
 # collect raw meta data
-prcp = shortcuts.getTerraClim(
+prcp = climatePy.getTerraClim(
     AOI       = AOI,
     varname   = "ppt",
     startDate = "2018-01-01",
     endDate   = "2018-12-01"
     )
 ```
 ![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
```

### Comparing `climatePy-0.4.27/setup.py` & `climatePy-0.4.28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.27',
+    version='0.4.28',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.27/tests/test_shortcuts.py` & `climatePy-0.4.28/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.27/tests/test_utils.py` & `climatePy-0.4.28/tests/test_utils.py`

 * *Files identical despite different names*

