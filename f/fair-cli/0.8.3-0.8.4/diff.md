# Comparing `tmp/fair_cli-0.8.3.tar.gz` & `tmp/fair_cli-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.8.3.tar", max compression
+gzip compressed data, was "fair_cli-0.8.4.tar", max compression
```

## Comparing `fair_cli-0.8.3.tar` & `fair_cli-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.3/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-07-11 16:34:34.113172 fair_cli-0.8.3/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.3/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.3/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.3/fair/__init__.py
--rw-r--r--   0        0        0    21730 2023-07-11 16:34:34.113408 fair_cli-0.8.3/fair/cli.py
--rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.8.3/fair/common.py
--rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.8.3/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.3/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.3/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.3/fair/files.txt
--rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.8.3/fair/history.py
--rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.3/fair/identifiers.py
--rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.8.3/fair/logging.py
--rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.3/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.3/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.3/fair/registry/file_formats.json
--rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.8.3/fair/registry/file_types.py
--rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.8.3/fair/registry/requests.py
--rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.8.3/fair/registry/server.py
--rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.8.3/fair/registry/storage.py
--rw-r--r--   0        0        0    41199 2023-07-11 14:54:18.135858 fair_cli-0.8.3/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.3/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.3/fair/run.py
--rw-r--r--   0        0        0    51996 2023-07-11 16:34:34.115371 fair_cli-0.8.3/fair/session.py
--rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.8.3/fair/staging.py
--rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.8.3/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.3/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.3/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.8.3/fair/testing.py
--rw-r--r--   0        0        0    54227 2023-07-11 16:34:34.116289 fair_cli-0.8.3/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.3/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.8.3/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.3/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.3/fair/virtualenv.py
--rw-r--r--   0        0        0     2496 2023-07-11 16:34:34.116650 fair_cli-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-07-11 20:06:03.658140 fair_cli-0.8.4/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.4/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.4/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.4/fair/__init__.py
+-rw-r--r--   0        0        0    21730 2023-07-11 16:34:34.113408 fair_cli-0.8.4/fair/cli.py
+-rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.8.4/fair/common.py
+-rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.8.4/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.4/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.4/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.4/fair/files.txt
+-rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.8.4/fair/history.py
+-rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.4/fair/identifiers.py
+-rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.8.4/fair/logging.py
+-rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.4/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.4/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.4/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.8.4/fair/registry/file_types.py
+-rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.8.4/fair/registry/requests.py
+-rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.8.4/fair/registry/server.py
+-rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.8.4/fair/registry/storage.py
+-rw-r--r--   0        0        0    42109 2023-07-11 20:02:27.628130 fair_cli-0.8.4/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.4/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.4/fair/run.py
+-rw-r--r--   0        0        0    51996 2023-07-11 16:34:34.115371 fair_cli-0.8.4/fair/session.py
+-rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.8.4/fair/staging.py
+-rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.8.4/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.4/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.4/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.8.4/fair/testing.py
+-rw-r--r--   0        0        0    54227 2023-07-11 16:34:34.116289 fair_cli-0.8.4/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.4/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.8.4/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.4/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.4/fair/virtualenv.py
+-rw-r--r--   0        0        0     2496 2023-07-11 20:05:52.782490 fair_cli-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.4/PKG-INFO
```

### Comparing `fair_cli-0.8.3/CHANGELOG.md` & `fair_cli-0.8.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/CITATION.cff` & `fair_cli-0.8.4/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - FAIR
 - Data Management
 - Provenance
 license: BSD-2-Clause
 message: If you use this software, please cite it using these metadata.
 repository-code: https://github.com/FAIRDataPipeline/FAIR-CLI/
 title: "The FAIR Data Pipeline command line tool"
-version: 0.8.3
+version: 0.8.4
```

### Comparing `fair_cli-0.8.3/LICENSE` & `fair_cli-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/README.md` & `fair_cli-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/__init__.py` & `fair_cli-0.8.4/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/cli.py` & `fair_cli-0.8.4/fair/cli.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/common.py` & `fair_cli-0.8.4/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/configuration/__init__.py` & `fair_cli-0.8.4/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/configuration/validation.py` & `fair_cli-0.8.4/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/exceptions.py` & `fair_cli-0.8.4/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/files.txt` & `fair_cli-0.8.4/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/history.py` & `fair_cli-0.8.4/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/identifiers.py` & `fair_cli-0.8.4/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/logging.py` & `fair_cli-0.8.4/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/register.py` & `fair_cli-0.8.4/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/registry/file_formats.json` & `fair_cli-0.8.4/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/registry/requests.py` & `fair_cli-0.8.4/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/registry/server.py` & `fair_cli-0.8.4/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/registry/storage.py` & `fair_cli-0.8.4/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/registry/sync.py` & `fair_cli-0.8.4/fair/registry/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,36 @@
         if "storage_root" in _new_obj_data:
             _new_obj_data["storage_root"] = _remote_storage_root_url
             _filters["storage_root"] = fdp_req.get_obj_id_from_url(_remote_storage_root_url)
 
     # if remote_author_url and _obj_type == "object":
     #     _new_obj_data["authors"] = _filters["authors"] = [remote_author_url]
 
+    if _obj_type == "object":
+        _new_author_urls = []
+        _filters["authors"] = []
+        _tmp_obj = fdp_req.url_get(object_url, origin_token)
+        if "authors" in _tmp_obj:
+            for _author_url in _tmp_obj["authors"]:
+                _new_author_urls.append(sync_dependency_chain(
+                    _author_url,
+                    dest_uri,
+                    origin_uri,
+                    dest_token,
+                    origin_token,
+                    local_data_store,
+                    public,
+                    remote_author_url
+                ))
+        for _new_author_dict in _new_author_urls:
+            for _new_author_url in _new_author_dict.values():
+                if "author" in _new_author_url:
+                    _new_obj_data["authors"].append(_new_author_url)
+                    _filters["authors"].append(fdp_req.get_obj_id_from_url(_new_author_url))
+
     if _obj_type == "author":
         if "identifier" in _new_obj_data:
             _author = fdp_req.get_author_exists(
                 dest_uri,
                 token= dest_token,
                 identifier= _new_obj_data['identifier']
             )
```

### Comparing `fair_cli-0.8.3/fair/registry/versioning.py` & `fair_cli-0.8.4/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/run.py` & `fair_cli-0.8.4/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/session.py` & `fair_cli-0.8.4/fair/session.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/staging.py` & `fair_cli-0.8.4/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/templates/__init__.py` & `fair_cli-0.8.4/fair/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/testing.py` & `fair_cli-0.8.4/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/user_config/__init__.py` & `fair_cli-0.8.4/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/user_config/globbing.py` & `fair_cli-0.8.4/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/user_config/validation.py` & `fair_cli-0.8.4/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/utilities.py` & `fair_cli-0.8.4/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/fair/virtualenv.py` & `fair_cli-0.8.4/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.3/pyproject.toml` & `fair_cli-0.8.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.8.3"
+version = "0.8.4"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.8.3/PKG-INFO` & `fair_cli-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.8.3
+Version: 0.8.4
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

