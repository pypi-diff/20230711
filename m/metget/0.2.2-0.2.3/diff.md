# Comparing `tmp/metget-0.2.2.tar.gz` & `tmp/metget-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.2.2.tar", last modified: Tue Jul 11 21:11:14 2023, max compression
+gzip compressed data, was "metget-0.2.3.tar", last modified: Tue Jul 11 21:15:22 2023, max compression
```

## Comparing `metget-0.2.2.tar` & `metget-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.099548 metget-0.2.2/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.2/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11524 2023-07-11 21:11:14.099351 metget-0.2.2/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    10602 2023-07-11 21:08:59.000000 metget-0.2.2/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 21:10:34.000000 metget-0.2.2/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 21:11:14.099598 metget-0.2.2/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.094238 metget-0.2.2/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.095873 metget-0.2.2/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11524 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.098259 metget-0.2.2/src/metget_client/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 21:10:34.000000 metget-0.2.2/src/metget_client/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    20020 2023-07-11 21:08:59.000000 metget-0.2.2/src/metget_client/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)    10008 2023-07-11 21:08:59.000000 metget-0.2.2/src/metget_client/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.2/src/metget_client/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.2/src/metget_client/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/spinnerlogger.py
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.099039 metget-0.2.2/test/
--rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_cli.py
--rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     7352 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2632 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_track.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.161990 metget-0.2.3/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.3/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:15:22.161841 metget-0.2.3/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.3/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 21:14:04.000000 metget-0.2.3/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 21:15:22.162027 metget-0.2.3/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.157220 metget-0.2.3/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.158694 metget-0.2.3/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.160921 metget-0.2.3/src/metget_client/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 21:14:04.000000 metget-0.2.3/src/metget_client/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    20020 2023-07-11 21:08:59.000000 metget-0.2.3/src/metget_client/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10008 2023-07-11 21:08:59.000000 metget-0.2.3/src/metget_client/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.3/src/metget_client/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.3/src/metget_client/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.161649 metget-0.2.3/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_cli.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     7352 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2632 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_track.py
```

### Comparing `metget-0.2.2/LICENSE.md` & `metget-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/PKG-INFO` & `metget-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.2
+Version: 0.2.3
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
@@ -23,15 +23,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
 ![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
-[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/master/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
+[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/main/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
 
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
```

### Comparing `metget-0.2.2/README.md` & `metget-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
 ![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
-[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/master/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
+[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/main/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
 
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
```

### Comparing `metget-0.2.2/pyproject.toml` & `metget-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.2.2"
+version = "0.2.3"
 description = "A client package for interaction with a MetGet server instance"
 authors = [
     { name = "Zach Cobell", email = "zcobell@thewaterinstitute.org" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.8"
@@ -40,15 +40,15 @@
 [tool.setuptools.dynamic]
 version = { attr = "metget_client.__version__" }
 
 [project.scripts]
 metget = "metget_client:metget_client_cli"
 
 [tool.bumpver]
-current_version = "0.2.2"
+current_version = "0.2.3"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.2.2/src/metget.egg-info/PKG-INFO` & `metget-0.2.3/src/metget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.2
+Version: 0.2.3
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
@@ -23,15 +23,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
 ![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
-[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/master/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
+[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/main/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
 
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
```

### Comparing `metget-0.2.2/src/metget.egg-info/SOURCES.txt` & `metget-0.2.3/src/metget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_build.py` & `metget-0.2.3/src/metget_client/metget_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_client.py` & `metget-0.2.3/src/metget_client/metget_client.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_credits.py` & `metget-0.2.3/src/metget_client/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_data.py` & `metget-0.2.3/src/metget_client/metget_data.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_environment.py` & `metget-0.2.3/src/metget_client/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_status.py` & `metget-0.2.3/src/metget_client/metget_status.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/metget_track.py` & `metget-0.2.3/src/metget_client/metget_track.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/src/metget_client/spinnerlogger.py` & `metget-0.2.3/src/metget_client/spinnerlogger.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/test/test_build.py` & `metget-0.2.3/test/test_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/test/test_credits.py` & `metget-0.2.3/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/test/test_status.py` & `metget-0.2.3/test/test_status.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.2/test/test_track.py` & `metget-0.2.3/test/test_track.py`

 * *Files identical despite different names*

