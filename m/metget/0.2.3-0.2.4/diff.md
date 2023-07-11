# Comparing `tmp/metget-0.2.3.tar.gz` & `tmp/metget-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.2.3.tar", last modified: Tue Jul 11 21:15:22 2023, max compression
+gzip compressed data, was "metget-0.2.4.tar", last modified: Tue Jul 11 21:34:31 2023, max compression
```

## Comparing `metget-0.2.3.tar` & `metget-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.161990 metget-0.2.3/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.3/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:15:22.161841 metget-0.2.3/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.3/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 21:14:04.000000 metget-0.2.3/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 21:15:22.162027 metget-0.2.3/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.157220 metget-0.2.3/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.158694 metget-0.2.3/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 21:15:22.000000 metget-0.2.3/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.160921 metget-0.2.3/src/metget_client/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 21:14:04.000000 metget-0.2.3/src/metget_client/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    20020 2023-07-11 21:08:59.000000 metget-0.2.3/src/metget_client/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)    10008 2023-07-11 21:08:59.000000 metget-0.2.3/src/metget_client/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.3/src/metget_client/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.3/src/metget_client/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.3/src/metget_client/spinnerlogger.py
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:15:22.161649 metget-0.2.3/test/
--rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_cli.py
--rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     7352 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2632 2023-07-11 21:08:59.000000 metget-0.2.3/test/test_track.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.566354 metget-0.2.4/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.4/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:34:31.564894 metget-0.2.4/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.4/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 21:34:02.000000 metget-0.2.4/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 21:34:31.566412 metget-0.2.4/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.559345 metget-0.2.4/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.560871 metget-0.2.4/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.563703 metget-0.2.4/src/metget_client/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 21:34:02.000000 metget-0.2.4/src/metget_client/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    19413 2023-07-11 21:17:13.000000 metget-0.2.4/src/metget_client/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10010 2023-07-11 21:30:40.000000 metget-0.2.4/src/metget_client/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.4/src/metget_client/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.4/src/metget_client/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.564684 metget-0.2.4/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_cli.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     8940 2023-07-11 21:28:48.000000 metget-0.2.4/test/test_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2632 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_track.py
```

### Comparing `metget-0.2.3/LICENSE.md` & `metget-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/PKG-INFO` & `metget-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.3
+Version: 0.2.4
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.2.3/README.md` & `metget-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/pyproject.toml` & `metget-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.2.3"
+version = "0.2.4"
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
-current_version = "0.2.3"
+current_version = "0.2.4"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.2.3/src/metget.egg-info/PKG-INFO` & `metget-0.2.4/src/metget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.3
+Version: 0.2.4
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.2.3/src/metget.egg-info/SOURCES.txt` & `metget-0.2.4/src/metget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/src/metget_client/metget_build.py` & `metget-0.2.4/src/metget_client/metget_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,33 +49,14 @@
             metget_api_version (int): MetGet API version
         """
         self.__metget_api_server = metget_api_server
         self.__metget_api_key = metget_api_key
         self.__metget_api_version = metget_api_version
 
     @staticmethod
-    def valid_datetime_type(arg_datetime_str: str) -> datetime:
-        """
-        Checks if the given datetime string is valid
-
-        Args:
-            arg_datetime_str (str): Datetime string to check
-
-        Returns:
-            datetime: Datetime object if valid
-        """
-        try:
-            return datetime.strptime(arg_datetime_str, "%Y-%m-%d %H:%M")
-        except ValueError:
-            msg = "Given DateTime ({0}) not valid! Expected format: 'YYYY-MM-DD HH:mm'".format(
-                arg_datetime_str
-            )
-            raise argparse.ArgumentTypeError(msg)
-
-    @staticmethod
     def parse_domain_data(domain_list: list, level: int, tau: int) -> dict:
         """
         Parses the domain data from the given list and returns a dictionary
 
         Args:
             domain_list (list): List of domain data
             level (int): Level of the domain
```

### Comparing `metget-0.2.3/src/metget_client/metget_client.py` & `metget-0.2.4/src/metget_client/metget_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     status.add_argument(
         "--ensemble-member",
         help="Ensemble member to request data for",
         type=str,
         metavar="s",
     )
     status.add_argument(
-        "--format", help="Output format (json, pretty)", metavar="f", default="json"
+        "--format", help="Output format (json, pretty)", metavar="f", default="pretty"
     )
 
 
 def initialize_track_cli(subparsers) -> None:
     """
     This method is used to initialize the track subparser
```

### Comparing `metget-0.2.3/src/metget_client/metget_credits.py` & `metget-0.2.4/src/metget_client/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/src/metget_client/metget_data.py` & `metget-0.2.4/src/metget_client/metget_data.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/src/metget_client/metget_environment.py` & `metget-0.2.4/src/metget_client/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/src/metget_client/metget_status.py` & `metget-0.2.4/src/metget_client/metget_status.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/src/metget_client/metget_track.py` & `metget-0.2.4/src/metget_client/metget_track.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/src/metget_client/spinnerlogger.py` & `metget-0.2.4/src/metget_client/spinnerlogger.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/test/test_build.py` & `metget-0.2.4/test/test_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/test/test_credits.py` & `metget-0.2.4/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.3/test/test_status.py` & `metget-0.2.4/test/test_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -264,7 +264,67 @@
             json=GEFS_STATUS_JSON,
         )
         s = MetGetStatus(args)
         s.get_status()
         out, err = capfd.readouterr()
         assert out == GEFS_STATUS_TEXT
 
+
+def test_status_ctcx(capfd) -> None:
+    """
+    Tests the status command for the COAMPS-CTCX model
+    Args:
+        capfd:
+
+    Returns:
+        None
+    """
+    from datetime import datetime
+    import json
+
+    args = argparse.Namespace()
+    args.model = "ctcx"
+    args.start = datetime(2022, 9, 26)
+    args.end = datetime(2022, 9, 30)
+    args.format = "json"
+    args.storm = None
+    args.endpoint = METGET_DMY_ENDPOINT
+    args.apikey = METGET_DMY_APIKEY
+    args.api_version = METGET_API_VERSION
+
+    with requests_mock.Mocker() as m:
+        m.get(
+            METGET_DMY_ENDPOINT
+            + "/status?"
+            + urlencode(
+                {
+                    "model": "ctcx",
+                    "start": "2022-09-26",
+                    "end": "2022-09-30",
+                }
+            ),
+            json=COAMPS_CTCX_STATUS_JSON,
+        )
+        s = MetGetStatus(args)
+        s.get_status()
+        out, err = capfd.readouterr()
+        out = out.replace("'", '"')
+        assert json.loads(out) == COAMPS_CTCX_STATUS_JSON["body"]
+
+    args.format = "pretty"
+    with requests_mock.Mocker() as m:
+        m.get(
+            METGET_DMY_ENDPOINT
+            + "/status?"
+            + urlencode(
+                {
+                    "model": "ctcx",
+                    "start": "2022-09-26",
+                    "end": "2022-09-30",
+                }
+            ),
+            json=COAMPS_CTCX_STATUS_JSON,
+        )
+        s = MetGetStatus(args)
+        s.get_status()
+        out, err = capfd.readouterr()
+        assert out == COAMPS_CTCX_STATUS_TEXT
```

### Comparing `metget-0.2.3/test/test_track.py` & `metget-0.2.4/test/test_track.py`

 * *Files identical despite different names*

