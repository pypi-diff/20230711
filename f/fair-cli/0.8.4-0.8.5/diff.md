# Comparing `tmp/fair_cli-0.8.4.tar.gz` & `tmp/fair_cli-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.8.4.tar", max compression
+gzip compressed data, was "fair_cli-0.8.5.tar", max compression
```

## Comparing `fair_cli-0.8.4.tar` & `fair_cli-0.8.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.4/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-07-11 20:06:03.658140 fair_cli-0.8.4/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.4/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.4/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.4/fair/__init__.py
--rw-r--r--   0        0        0    21730 2023-07-11 16:34:34.113408 fair_cli-0.8.4/fair/cli.py
--rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.8.4/fair/common.py
--rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.8.4/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.4/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.4/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.4/fair/files.txt
--rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.8.4/fair/history.py
--rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.4/fair/identifiers.py
--rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.8.4/fair/logging.py
--rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.4/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.4/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.4/fair/registry/file_formats.json
--rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.8.4/fair/registry/file_types.py
--rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.8.4/fair/registry/requests.py
--rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.8.4/fair/registry/server.py
--rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.8.4/fair/registry/storage.py
--rw-r--r--   0        0        0    42109 2023-07-11 20:02:27.628130 fair_cli-0.8.4/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.4/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.4/fair/run.py
--rw-r--r--   0        0        0    51996 2023-07-11 16:34:34.115371 fair_cli-0.8.4/fair/session.py
--rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.8.4/fair/staging.py
--rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.8.4/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.4/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.4/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.8.4/fair/testing.py
--rw-r--r--   0        0        0    54227 2023-07-11 16:34:34.116289 fair_cli-0.8.4/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.4/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.8.4/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.4/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.4/fair/virtualenv.py
--rw-r--r--   0        0        0     2496 2023-07-11 20:05:52.782490 fair_cli-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-07-11 20:40:08.968781 fair_cli-0.8.5/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.5/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.5/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.5/fair/__init__.py
+-rw-r--r--   0        0        0    21730 2023-07-11 16:34:34.113408 fair_cli-0.8.5/fair/cli.py
+-rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.8.5/fair/common.py
+-rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.8.5/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.5/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.5/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.5/fair/files.txt
+-rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.8.5/fair/history.py
+-rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.5/fair/identifiers.py
+-rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.8.5/fair/logging.py
+-rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.5/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.5/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.5/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.8.5/fair/registry/file_types.py
+-rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.8.5/fair/registry/requests.py
+-rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.8.5/fair/registry/server.py
+-rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.8.5/fair/registry/storage.py
+-rw-r--r--   0        0        0    42144 2023-07-11 20:37:03.466251 fair_cli-0.8.5/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.5/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.5/fair/run.py
+-rw-r--r--   0        0        0    51996 2023-07-11 16:34:34.115371 fair_cli-0.8.5/fair/session.py
+-rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.8.5/fair/staging.py
+-rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.8.5/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.5/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.5/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.8.5/fair/testing.py
+-rw-r--r--   0        0        0    54227 2023-07-11 16:34:34.116289 fair_cli-0.8.5/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.5/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.8.5/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.5/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.5/fair/virtualenv.py
+-rw-r--r--   0        0        0     2496 2023-07-11 20:39:56.996799 fair_cli-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.5/PKG-INFO
```

### Comparing `fair_cli-0.8.4/CHANGELOG.md` & `fair_cli-0.8.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/CITATION.cff` & `fair_cli-0.8.5/CITATION.cff`

 * *Files 6% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - FAIR
 - Data Management
 - Provenance
 license: BSD-2-Clause
 message: If you use this software, please cite it using these metadata.
 repository-code: https://github.com/FAIRDataPipeline/FAIR-CLI/
 title: "The FAIR Data Pipeline command line tool"
-version: 0.8.4
+version: 0.8.5
```

### Comparing `fair_cli-0.8.4/LICENSE` & `fair_cli-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/README.md` & `fair_cli-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/__init__.py` & `fair_cli-0.8.5/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/cli.py` & `fair_cli-0.8.5/fair/cli.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/common.py` & `fair_cli-0.8.5/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/configuration/__init__.py` & `fair_cli-0.8.5/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/configuration/validation.py` & `fair_cli-0.8.5/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/exceptions.py` & `fair_cli-0.8.5/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/files.txt` & `fair_cli-0.8.5/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/history.py` & `fair_cli-0.8.5/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/identifiers.py` & `fair_cli-0.8.5/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/logging.py` & `fair_cli-0.8.5/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/register.py` & `fair_cli-0.8.5/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/registry/file_formats.json` & `fair_cli-0.8.5/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/registry/requests.py` & `fair_cli-0.8.5/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/registry/server.py` & `fair_cli-0.8.5/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/registry/storage.py` & `fair_cli-0.8.5/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/registry/sync.py` & `fair_cli-0.8.5/fair/registry/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,18 +470,15 @@
                 dest_token,
                 params={
                     "namespace": _namespace_id,
                     "name": name,
                     "version": version.replace("v", ""),
                 },
             ) and not force:
-                click.echo(
-                    f"Data product '{data_product}' already present "
-                    f"on remote '{remote_label}', ignoring.",
-                )
+                logger.debug(f"Data product '{data_product}' already present on remote '{remote_label}', ignoring.")
                 continue
 
         # Convert namespace name to an ID for retrieval
         _namespaces = fdp_req.get(
             origin_uri,
             "namespace",
             params={SEARCH_KEYS["namespace"]: namespace},
@@ -558,15 +555,15 @@
                         origin_token,
                         params= {"outputs": fdp_req.get_obj_id_from_url(origin_component_url)}
                     )
                 for origin_output_code_run in origin_output_code_runs:
                     dest_component_url = get_dest_component_url(origin_component_url, dest_uri, dest_token, origin_token)
                     dest_inputs = get_dest_inputs(origin_output_code_run["inputs"], origin_uri, dest_uri, dest_token, origin_token, remote_label, force, remote_author_url)
                     sync_code_run(origin_uri, dest_uri, dest_token, origin_token, origin_output_code_run["uuid"], inputs= dest_inputs, outputs= [dest_component_url], remote_author_url = remote_author_url)
-                    
+        logger.info(f"Synced Data Product: {data_product}")
 def get_dest_component_url(
     origin_component_url: str,
     dest_uri: str,
     dest_token:str,
     origin_token:str) -> str:
     """Get the destination component url for the given origin component url
 
@@ -703,14 +700,15 @@
             _dest_object = fdp_req.url_get(_dest_data_product[0]["object"], dest_token)
             if _origin_data_product_formatted in _inputs_data_products:
                 _dest_inputs += _dest_object["components"]
             if _origin_data_product_formatted in _outputs_data_products:
                 _dest_outputs += _dest_object["components"]
         logger.debug(f'attempting to sync coderun {code_run_uuid} with inputs {_dest_inputs} and outputs {_dest_outputs}')
         sync_code_run(origin_uri, dest_uri, dest_token, origin_token, code_run_uuid, _dest_inputs, _dest_outputs, remote_author_url = remote_author_url)
+        logger.info(f"Synced Code Run: {code_run_uuid}")
 
 # Internal function to return the (remote) object associated with a code_run field containing and object url
 def get_dest_object_url(
     origin_object_url: str,
     dest_uri: str,
     dest_token: str,
     origin_token: str)->str:
```

### Comparing `fair_cli-0.8.4/fair/registry/versioning.py` & `fair_cli-0.8.5/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/run.py` & `fair_cli-0.8.5/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/session.py` & `fair_cli-0.8.5/fair/session.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/staging.py` & `fair_cli-0.8.5/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/templates/__init__.py` & `fair_cli-0.8.5/fair/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/testing.py` & `fair_cli-0.8.5/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/user_config/__init__.py` & `fair_cli-0.8.5/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/user_config/globbing.py` & `fair_cli-0.8.5/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/user_config/validation.py` & `fair_cli-0.8.5/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/utilities.py` & `fair_cli-0.8.5/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/fair/virtualenv.py` & `fair_cli-0.8.5/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.4/pyproject.toml` & `fair_cli-0.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.8.4"
+version = "0.8.5"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.8.4/PKG-INFO` & `fair_cli-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.8.4
+Version: 0.8.5
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

