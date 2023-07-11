# Comparing `tmp/climatePy-0.4.26.tar.gz` & `tmp/climatePy-0.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.26.tar", last modified: Tue Jul 11 15:00:53 2023, max compression
+gzip compressed data, was "climatePy-0.4.27.tar", last modified: Tue Jul 11 15:07:27 2023, max compression
```

## Comparing `climatePy-0.4.26.tar` & `climatePy-0.4.27.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.368823 climatePy-0.4.26/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 15:00:50.000000 climatePy-0.4.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-11 15:00:53.368823 climatePy-0.4.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 15:00:50.000000 climatePy-0.4.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.320822 climatePy-0.4.26/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59297 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.324822 climatePy-0.4.26/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 15:00:50.000000 climatePy-0.4.26/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.324822 climatePy-0.4.26/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:00:53.000000 climatePy-0.4.26/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:00:53.368823 climatePy-0.4.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 15:00:52.000000 climatePy-0.4.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:53.368823 climatePy-0.4.26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:00:50.000000 climatePy-0.4.26/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 15:00:50.000000 climatePy-0.4.26/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 15:00:50.000000 climatePy-0.4.26/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.325904 climatePy-0.4.27/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 15:07:21.000000 climatePy-0.4.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-11 15:07:27.321903 climatePy-0.4.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-11 15:07:21.000000 climatePy-0.4.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.265901 climatePy-0.4.27/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59297 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.269901 climatePy-0.4.27/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 15:07:21.000000 climatePy-0.4.27/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.269901 climatePy-0.4.27/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:07:27.000000 climatePy-0.4.27/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:07:27.325904 climatePy-0.4.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 15:07:25.000000 climatePy-0.4.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:27.321903 climatePy-0.4.27/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:07:21.000000 climatePy-0.4.27/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 15:07:21.000000 climatePy-0.4.27/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 15:07:21.000000 climatePy-0.4.27/tests/test_utils.py
```

### Comparing `climatePy-0.4.26/LICENSE` & `climatePy-0.4.27/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/PKG-INFO` & `climatePy-0.4.27/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.26
+Version: 0.4.27
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [**climatePy**](https://github.com/LynkerIntel/climatePy)
+# [**climatePy**](https://github.com/anguswg-ucsb/climatePy)
 
 <!-- badges: start -->
 
 [![stage](https://img.shields.io/badge/stage-dev-orange)](#)
 [![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
 [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
@@ -32,22 +32,23 @@
 
 2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
 
 3. A set of shortcuts that implement these methods for a core set of selected catalog elements
 
 <br>
 
----
+## Links
 
+- [climatePy (Lynker intel)](https://github.com/LynkerIntel/climatePy)
 - [climatePy PyPI](https://pypi.org/project/climatePy/)
-- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
+- [**climateR/climatePy slideshow**](https://mikejohnson51.github.io/climateR-intro/#1)
 
----
+<br>
 
-## Table of Contents (Optional)
+## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Credits](#credits)
 - [License](#license)
 - [How to Contribute](#how-to-contribute)
```

### Comparing `climatePy-0.4.26/README.md` & `climatePy-0.4.27/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# [**climatePy**](https://github.com/LynkerIntel/climatePy)
+# [**climatePy**](https://github.com/anguswg-ucsb/climatePy)
 
 <!-- badges: start -->
 
 [![stage](https://img.shields.io/badge/stage-dev-orange)](#)
 [![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
 [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
@@ -20,22 +20,23 @@
 
 2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
 
 3. A set of shortcuts that implement these methods for a core set of selected catalog elements
 
 <br>
 
----
+## Links
 
+- [climatePy (Lynker intel)](https://github.com/LynkerIntel/climatePy)
 - [climatePy PyPI](https://pypi.org/project/climatePy/)
-- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
+- [**climateR/climatePy slideshow**](https://mikejohnson51.github.io/climateR-intro/#1)
 
----
+<br>
 
-## Table of Contents (Optional)
+## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Credits](#credits)
 - [License](#license)
 - [How to Contribute](#how-to-contribute)
```

### Comparing `climatePy-0.4.26/climatePy/__init__.py` & `climatePy-0.4.27/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy/_climatepy_filter.py` & `climatePy-0.4.27/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy/_dap.py` & `climatePy-0.4.27/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy/_netrc_utils.py` & `climatePy-0.4.27/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy/_shortcuts.py` & `climatePy-0.4.27/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy/_utils.py` & `climatePy-0.4.27/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy/data/catalog.csv` & `climatePy-0.4.27/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.27/climatePy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.26
+Version: 0.4.27
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [**climatePy**](https://github.com/LynkerIntel/climatePy)
+# [**climatePy**](https://github.com/anguswg-ucsb/climatePy)
 
 <!-- badges: start -->
 
 [![stage](https://img.shields.io/badge/stage-dev-orange)](#)
 [![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
 [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
@@ -32,22 +32,23 @@
 
 2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
 
 3. A set of shortcuts that implement these methods for a core set of selected catalog elements
 
 <br>
 
----
+## Links
 
+- [climatePy (Lynker intel)](https://github.com/LynkerIntel/climatePy)
 - [climatePy PyPI](https://pypi.org/project/climatePy/)
-- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
+- [**climateR/climatePy slideshow**](https://mikejohnson51.github.io/climateR-intro/#1)
 
----
+<br>
 
-## Table of Contents (Optional)
+## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Credits](#credits)
 - [License](#license)
 - [How to Contribute](#how-to-contribute)
```

### Comparing `climatePy-0.4.26/setup.py` & `climatePy-0.4.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.26',
+    version='0.4.27',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.26/tests/test_shortcuts.py` & `climatePy-0.4.27/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.26/tests/test_utils.py` & `climatePy-0.4.27/tests/test_utils.py`

 * *Files identical despite different names*

