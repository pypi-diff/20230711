# Comparing `tmp/metget-0.2.1.tar.gz` & `tmp/metget-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.2.1.tar", last modified: Tue Jul 11 02:36:58 2023, max compression
+gzip compressed data, was "metget-0.2.2.tar", last modified: Tue Jul 11 21:11:14 2023, max compression
```

## Comparing `metget-0.2.1.tar` & `metget-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.616305 metget-0.2.1/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.1/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11376 2023-07-11 02:36:58.615259 metget-0.2.1/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    10454 2023-07-11 02:36:15.000000 metget-0.2.1/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 02:36:26.000000 metget-0.2.1/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 02:36:58.616367 metget-0.2.1/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.609552 metget-0.2.1/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.611260 metget-0.2.1/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11376 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      573 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 02:36:58.000000 metget-0.2.1/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.614153 metget-0.2.1/src/metget_client/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 02:36:26.000000 metget-0.2.1/src/metget_client/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    19700 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)     9948 2023-07-10 15:42:48.000000 metget-0.2.1/src/metget_client/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.1/src/metget_client/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.1/src/metget_client/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.1/src/metget_client/spinnerlogger.py
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 02:36:58.614332 metget-0.2.1/test/
--rw-r--r--   0 zcobell    (502) staff       (20)    44282 2023-07-11 02:36:15.000000 metget-0.2.1/test/test_status.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.099548 metget-0.2.2/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.2/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11524 2023-07-11 21:11:14.099351 metget-0.2.2/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    10602 2023-07-11 21:08:59.000000 metget-0.2.2/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 21:10:34.000000 metget-0.2.2/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 21:11:14.099598 metget-0.2.2/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.094238 metget-0.2.2/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.095873 metget-0.2.2/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11524 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 21:11:14.000000 metget-0.2.2/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.098259 metget-0.2.2/src/metget_client/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 21:10:34.000000 metget-0.2.2/src/metget_client/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    20020 2023-07-11 21:08:59.000000 metget-0.2.2/src/metget_client/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10008 2023-07-11 21:08:59.000000 metget-0.2.2/src/metget_client/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.2/src/metget_client/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.2/src/metget_client/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.2/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:11:14.099039 metget-0.2.2/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_cli.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     7352 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2632 2023-07-11 21:08:59.000000 metget-0.2.2/test/test_track.py
```

### Comparing `metget-0.2.1/LICENSE.md` & `metget-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.1/PKG-INFO` & `metget-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.1
+Version: 0.2.2
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
@@ -23,14 +23,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
 ![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/master/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
 
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
@@ -135,15 +136,15 @@
 $ metget build --domain hwrf-mawar02w 0.15 -90 20 -85 25 \
                --domain gfs 0.25 -100 10 -80 30 \
                --start "2023-06-01 00:00" \
                --end "2023-06-03 00:00" \ 
                --timestep 3600 \
                --backfill \
                --format owi-ascii \
-               --output metget_hwrf_data \
+               --output metget_hwrf_data
 ```
 
 #### Example 5 - Get the status of the GFS model runs
 This example demonstrates the ability for the system to provide information about what data is currently available
 
 ```bash
 $ metget status gfs --format pretty
```

### Comparing `metget-0.2.1/README.md` & `metget-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
 ![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/master/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
 
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
@@ -113,15 +114,15 @@
 $ metget build --domain hwrf-mawar02w 0.15 -90 20 -85 25 \
                --domain gfs 0.25 -100 10 -80 30 \
                --start "2023-06-01 00:00" \
                --end "2023-06-03 00:00" \ 
                --timestep 3600 \
                --backfill \
                --format owi-ascii \
-               --output metget_hwrf_data \
+               --output metget_hwrf_data
 ```
 
 #### Example 5 - Get the status of the GFS model runs
 This example demonstrates the ability for the system to provide information about what data is currently available
 
 ```bash
 $ metget status gfs --format pretty
```

### Comparing `metget-0.2.1/pyproject.toml` & `metget-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.2.1"
+version = "0.2.2"
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
-current_version = "0.2.1"
+current_version = "0.2.2"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.2.1/src/metget.egg-info/PKG-INFO` & `metget-0.2.2/src/metget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.1
+Version: 0.2.2
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
@@ -23,14 +23,15 @@
 ![MetGet Logo](https://raw.githubusercontent.com/waterinstitute/metget/main/static/img/MetGet_logo_blue.png)
 MetGet is an application which allows users to query, format, and blend meteorological data from various sources
 to be used in hydrodynamic modeling applications.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/metget.svg)](https://badge.fury.io/py/metget)
 ![Testing](https://github.com/waterinstitute/metget/actions/workflows/pytest.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/waterinstitute/MetGet/branch/master/graph/badge.svg?token=I36RIBPFMD)](https://codecov.io/gh/waterinstitute/MetGet)
 
 ## Development Partners
 
 MetGet is developed by [The Water Institute](https://thewaterinstitute.org) and has been funded by the 
 University of North Carolina at Chapel Hill [Coastal Resilience Center of Excellence](https://www.coastalresiliencecenter.org).
 
 ![The Water Institute](https://thewaterinstitute.org/images/01-Primary_Logo_Final.png)
@@ -135,15 +136,15 @@
 $ metget build --domain hwrf-mawar02w 0.15 -90 20 -85 25 \
                --domain gfs 0.25 -100 10 -80 30 \
                --start "2023-06-01 00:00" \
                --end "2023-06-03 00:00" \ 
                --timestep 3600 \
                --backfill \
                --format owi-ascii \
-               --output metget_hwrf_data \
+               --output metget_hwrf_data
 ```
 
 #### Example 5 - Get the status of the GFS model runs
 This example demonstrates the ability for the system to provide information about what data is currently available
 
 ```bash
 $ metget status gfs --format pretty
```

### Comparing `metget-0.2.1/src/metget.egg-info/SOURCES.txt` & `metget-0.2.2/src/metget.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,12 @@
 src/metget_client/metget_client.py
 src/metget_client/metget_credits.py
 src/metget_client/metget_data.py
 src/metget_client/metget_environment.py
 src/metget_client/metget_status.py
 src/metget_client/metget_track.py
 src/metget_client/spinnerlogger.py
-test/test_status.py
+test/test_build.py
+test/test_cli.py
+test/test_credits.py
+test/test_status.py
+test/test_track.py
```

### Comparing `metget-0.2.1/src/metget_client/metget_build.py` & `metget-0.2.2/src/metget_client/metget_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,18 +265,24 @@
             "data_type": kwargs.get("data_type", "wind_pressure"),
             "time_step": kwargs.get("time_step", 3600),
             "domains": kwargs.get("domains"),
             "compression": kwargs.get("compression", False),
             "epsg": kwargs.get("epsg", 4326),
             "filename": kwargs.get("filename", "metget_data"),
         }
+
         if kwargs.get("strict", False):
             request_data["strict"] = True
+        else:
+            request_data["strict"] = False
+
         if kwargs.get("dry_run", False):
             request_data["dry_run"] = True
+        else:
+            request_data["dry_run"] = False
 
         if kwargs.get("save_json_request", False):
             with open("request.json", "w") as f:
                 f.write(json.dumps(request_data, indent=2))
 
         return request_data
 
@@ -442,14 +448,20 @@
         """
         response = None
 
         if self.__metget_api_version == 1:
             response = self.__check_metget_status_v1(data_id)
         elif self.__metget_api_version == 2:
             response = self.__check_metget_status_v2(data_id)
+        else:
+            raise RuntimeError(
+                "Invalid MetGet API version. Must be 1 or 2. Got {:d}".format(
+                    self.__metget_api_version
+                )
+            )
         json_response = json.loads(response)
         status = json_response["body"]["status"]
         data_url = json_response["body"]["destination"]
         return data_url, status
 
     def __check_metget_status_v1(self, data_id: str) -> str:
         """
```

### Comparing `metget-0.2.1/src/metget_client/metget_client.py` & `metget-0.2.2/src/metget_client/metget_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,12 +303,15 @@
     subparsers = p.add_subparsers(help="Sub-command help")
     initialize_build_cli(subparsers)
     initialize_status_cli(subparsers)
     initialize_track_cli(subparsers)
     initialize_credits_cli(subparsers)
 
     args = p.parse_args()
-    args.func(args)
+    if "func" in args:
+        args.func(args)
+    else:
+        p.print_help()
 
 
 if __name__ == "__main__":
     metget_client_cli()
```

### Comparing `metget-0.2.1/src/metget_client/metget_credits.py` & `metget-0.2.2/src/metget_client/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.1/src/metget_client/metget_data.py` & `metget-0.2.2/src/metget_client/metget_data.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.1/src/metget_client/metget_environment.py` & `metget-0.2.2/src/metget_client/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.1/src/metget_client/metget_status.py` & `metget-0.2.2/src/metget_client/metget_status.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.1/src/metget_client/metget_track.py` & `metget-0.2.2/src/metget_client/metget_track.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.1/src/metget_client/spinnerlogger.py` & `metget-0.2.2/src/metget_client/spinnerlogger.py`

 * *Files identical despite different names*

