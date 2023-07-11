# Comparing `tmp/metget-0.2.0.tar.gz` & `tmp/metget-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.2.0.tar", last modified: Mon Jul 10 23:03:43 2023, max compression
+gzip compressed data, was "metget-0.2.1.tar", last modified: Tue Jul 11 02:36:58 2023, max compression
```

## Comparing `metget-0.2.0.tar` & `metget-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-10 23:03:43.249775 metget-0.2.0/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.0/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11087 2023-07-10 23:03:43.249609 metget-0.2.0/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    10165 2023-07-10 18:50:25.000000 metget-0.2.0/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-10 23:03:02.000000 metget-0.2.0/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-10 23:03:43.249816 metget-0.2.0/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-10 23:03:43.245722 metget-0.2.0/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-10 23:03:43.247106 metget-0.2.0/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11087 2023-07-10 23:03:43.000000 metget-0.2.0/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      553 2023-07-10 23:03:43.000000 metget-0.2.0/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-10 23:03:43.000000 metget-0.2.0/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-10 23:03:43.000000 metget-0.2.0/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-10 23:03:43.000000 metget-0.2.0/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-10 23:03:43.000000 metget-0.2.0/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-10 23:03:43.249405 metget-0.2.0/src/metget_client/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-10 23:03:02.000000 metget-0.2.0/src/metget_client/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    19700 2023-07-08 15:58:57.000000 metget-0.2.0/src/metget_client/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)     9948 2023-07-10 15:42:48.000000 metget-0.2.0/src/metget_client/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.0/src/metget_client/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.0/src/metget_client/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.0/src/metget_client/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    17220 2023-07-08 15:58:57.000000 metget-0.2.0/src/metget_client/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.0/src/metget_client/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.0/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.616305 metget-0.2.1/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.1/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11376 2023-07-11 02:36:58.615259 metget-0.2.1/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    10454 2023-07-11 02:36:15.000000 metget-0.2.1/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 02:36:26.000000 metget-0.2.1/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 02:36:58.616367 metget-0.2.1/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.609552 metget-0.2.1/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.611260 metget-0.2.1/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11376 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      573 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.614153 metget-0.2.1/src/metget_client/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 02:36:26.000000 metget-0.2.1/src/metget_client/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    19700 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     9948 2023-07-10 15:42:48.000000 metget-0.2.1/src/metget_client/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.1/src/metget_client/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.1/src/metget_client/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.614332 metget-0.2.1/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    44282 2023-07-11 02:36:15.000000 metget-0.2.1/test/test_status.py
```

### Comparing `metget-0.2.0/LICENSE.md` & `metget-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/PKG-INFO` & `metget-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.0
+Version: 0.2.1
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
@@ -17,18 +17,21 @@
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
-
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
+![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
+
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
```

### Comparing `metget-0.2.0/README.md` & `metget-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
-
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
+![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
+
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
```

### Comparing `metget-0.2.0/pyproject.toml` & `metget-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.2.0"
+version = "0.2.1"
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
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.2.0/src/metget.egg-info/PKG-INFO` & `metget-0.2.1/src/metget.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.0
+Version: 0.2.1
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
@@ -17,18 +17,21 @@
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
-
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
+![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
+
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
```

### Comparing `metget-0.2.0/src/metget.egg-info/SOURCES.txt` & `metget-0.2.1/src/metget.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 src/metget_client/metget_build.py
 src/metget_client/metget_client.py
 src/metget_client/metget_credits.py
 src/metget_client/metget_data.py
 src/metget_client/metget_environment.py
 src/metget_client/metget_status.py
 src/metget_client/metget_track.py
-src/metget_client/spinnerlogger.py
+src/metget_client/spinnerlogger.py
+test/test_status.py
```

### Comparing `metget-0.2.0/src/metget_client/metget_build.py` & `metget-0.2.1/src/metget_client/metget_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/src/metget_client/metget_client.py` & `metget-0.2.1/src/metget_client/metget_client.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/src/metget_client/metget_credits.py` & `metget-0.2.1/src/metget_client/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/src/metget_client/metget_data.py` & `metget-0.2.1/src/metget_client/metget_data.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/src/metget_client/metget_environment.py` & `metget-0.2.1/src/metget_client/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/src/metget_client/metget_status.py` & `metget-0.2.1/src/metget_client/metget_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         from datetime import datetime
 
         if self.__args.start:
             url += "&start={:s}".format(self.__args.start.strftime("%Y-%m-%d"))
             if not self.__args.end:
                 url += "&end={:s}".format(datetime.utcnow().strftime("%Y-%m-%d"))
             else:
-                url += "&end={:s}".format(self.__args.end)
+                url += "&end={:s}".format(self.__args.end.strftime("%Y-%m-%d"))
         return url
 
     def __status_track(self, model: str) -> None:
         """
         This method is used to get the status of the track data (NHC)
 
         Args:
```

### Comparing `metget-0.2.0/src/metget_client/metget_track.py` & `metget-0.2.1/src/metget_client/metget_track.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.0/src/metget_client/spinnerlogger.py` & `metget-0.2.1/src/metget_client/spinnerlogger.py`

 * *Files identical despite different names*

