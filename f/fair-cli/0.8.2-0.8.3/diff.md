# Comparing `tmp/fair_cli-0.8.2.tar.gz` & `tmp/fair_cli-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.8.2.tar", max compression
+gzip compressed data, was "fair_cli-0.8.3.tar", max compression
```

## Comparing `fair_cli-0.8.2.tar` & `fair_cli-0.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-07-11 14:54:18.134032 fair_cli-0.8.2/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.2/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.2/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.2/fair/__init__.py
--rw-r--r--   0        0        0    21694 2023-07-08 08:05:57.895050 fair_cli-0.8.2/fair/cli.py
--rw-r--r--   0        0        0     9375 2023-07-08 08:05:57.895206 fair_cli-0.8.2/fair/common.py
--rw-r--r--   0        0        0    30416 2023-07-11 14:54:18.134332 fair_cli-0.8.2/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.2/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.2/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.2/fair/files.txt
--rw-r--r--   0        0        0     4719 2023-07-08 08:05:57.895862 fair_cli-0.8.2/fair/history.py
--rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.2/fair/identifiers.py
--rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.8.2/fair/logging.py
--rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.2/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.2/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.2/fair/registry/file_formats.json
--rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.8.2/fair/registry/file_types.py
--rw-r--r--   0        0        0    17974 2023-07-11 14:54:18.134981 fair_cli-0.8.2/fair/registry/requests.py
--rw-r--r--   0        0        0    14996 2023-07-08 08:05:57.897060 fair_cli-0.8.2/fair/registry/server.py
--rw-r--r--   0        0        0    24206 2023-07-11 14:54:18.135521 fair_cli-0.8.2/fair/registry/storage.py
--rw-r--r--   0        0        0    41199 2023-07-11 14:54:18.135858 fair_cli-0.8.2/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.2/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.2/fair/run.py
--rw-r--r--   0        0        0    51804 2023-07-11 14:54:18.136433 fair_cli-0.8.2/fair/session.py
--rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.8.2/fair/staging.py
--rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.8.2/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.2/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.2/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3220 2023-07-08 08:05:57.898323 fair_cli-0.8.2/fair/testing.py
--rw-r--r--   0        0        0    54095 2023-07-08 08:05:57.898883 fair_cli-0.8.2/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.2/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.8.2/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.2/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.2/fair/virtualenv.py
--rw-r--r--   0        0        0     2496 2023-07-11 14:54:18.136718 fair_cli-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-07-11 16:34:34.113172 fair_cli-0.8.3/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.3/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.3/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.3/fair/__init__.py
+-rw-r--r--   0        0        0    21730 2023-07-11 16:34:34.113408 fair_cli-0.8.3/fair/cli.py
+-rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.8.3/fair/common.py
+-rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.8.3/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.3/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.3/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.3/fair/files.txt
+-rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.8.3/fair/history.py
+-rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.3/fair/identifiers.py
+-rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.8.3/fair/logging.py
+-rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.3/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.3/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.3/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.8.3/fair/registry/file_types.py
+-rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.8.3/fair/registry/requests.py
+-rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.8.3/fair/registry/server.py
+-rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.8.3/fair/registry/storage.py
+-rw-r--r--   0        0        0    41199 2023-07-11 14:54:18.135858 fair_cli-0.8.3/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.3/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.3/fair/run.py
+-rw-r--r--   0        0        0    51996 2023-07-11 16:34:34.115371 fair_cli-0.8.3/fair/session.py
+-rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.8.3/fair/staging.py
+-rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.8.3/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.3/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.3/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.8.3/fair/testing.py
+-rw-r--r--   0        0        0    54227 2023-07-11 16:34:34.116289 fair_cli-0.8.3/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.3/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.8.3/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.3/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.3/fair/virtualenv.py
+-rw-r--r--   0        0        0     2496 2023-07-11 16:34:34.116650 fair_cli-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.3/PKG-INFO
```

### Comparing `fair_cli-0.8.2/CHANGELOG.md` & `fair_cli-0.8.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/CITATION.cff` & `fair_cli-0.8.3/CITATION.cff`

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
-version: 0.8.2
+version: 0.8.3
```

### Comparing `fair_cli-0.8.2/LICENSE` & `fair_cli-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/README.md` & `fair_cli-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/__init__.py` & `fair_cli-0.8.3/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/cli.py` & `fair_cli-0.8.3/fair/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     ]
 
 
 def complete_data_products(ctx, param, incomplete) -> typing.List[str]:
     _staging_file = fdp_com.staging_cache(os.getcwd())
     if not os.path.exists(_staging_file):
         return []
-    _staging_data = yaml.safe_load(open(_staging_file))
+    _staging_data = yaml.safe_load(open(_staging_file, encoding='utf-8'))
     _candidates = list(_staging_data["data_product"].keys())
     return [
         click.shell_completion.CompletionItem(c)
         for c in _candidates
         if c.startswith(incomplete)
     ]
 
@@ -231,15 +231,15 @@
             _use_dict = {}
             if using:
                 if not os.path.exists(using):
                     raise fdp_exc.FileNotFoundError(
                         f"Cannot load CLI configuration from file '{using}', "
                         "file does not exist."
                     )
-                _use_dict = yaml.safe_load(open(using))
+                _use_dict = yaml.safe_load(open(using, encoding='utf-8'))
 
             fair_session.initialise(
                 using=_use_dict,
                 registry=registry,
                 export_as=export,
                 local=local,
             )
```

### Comparing `fair_cli-0.8.2/fair/common.py` & `fair_cli-0.8.3/fair/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 def registry_home() -> str:
     if not os.path.exists(global_fdpconfig()):
         if "FAIR_REGISTRY_DIR" in os.environ:
             return os.environ["FAIR_REGISTRY_DIR"]
         else:
             return DEFAULT_REGISTRY_LOCATION
-    _glob_conf = yaml.safe_load(open(global_fdpconfig()))
+    _glob_conf = yaml.safe_load(open(global_fdpconfig(), encoding='utf-8'))
     if not _glob_conf:
         return DEFAULT_REGISTRY_LOCATION
     if "registries" not in _glob_conf:
         raise fdp_exc.CLIConfigurationError(
             "Expected key 'registries' in global CLI configuration"
         )
 
@@ -179,15 +179,15 @@
         registry directory, by default None
 
     Returns
     -------
     int
         current/most recent port used to launch the registry
     """
-    return int(open(registry_session_port_file(registry_dir)).read().strip())
+    return int(open(registry_session_port_file(registry_dir), encoding='utf-8').read().strip())
 
 def registry_session_address(registry_dir: str = None) -> str:
     """Retrieve the registry session address
 
     Unlike 'get_local_address' within the configuration module, this retrieves the
     port number from the file generated by the registry itself
 
@@ -202,15 +202,15 @@
         current/most recent address used to launch the registry
     """
     if not os.path.exists(registry_session_address_file(registry_dir)):
         _logger.warning("Session Address file not found, please make sure your registry is up-to-date")
         _logger.info("Using 127.0.0.1")
         return "127.0.0.1"
 
-    _address = open(registry_session_address_file(registry_dir)).read().strip()
+    _address = open(registry_session_address_file(registry_dir), encoding='utf-8').read().strip()
     if _address != "0.0.0.0":
         return _address
     else:
         return "127.0.0.1"
 
 
 def staging_cache(user_loc: str) -> str:
@@ -222,15 +222,15 @@
 
 def default_data_dir(location: str = "local") -> str:
     """Location of the default data store"""
     if not os.path.exists(global_fdpconfig()):
         raise fdp_exc.InternalError(
             f"Failed to read CLI global config file '{global_fdpconfig()}'"
         )
-    _glob_conf = yaml.safe_load(open(global_fdpconfig()))
+    _glob_conf = yaml.safe_load(open(global_fdpconfig(), encoding='utf-8'))
     if "data_store" in _glob_conf["registries"][location]:
         return _glob_conf["registries"][location]["data_store"]
     if location == "local":
         return os.path.join(USER_FAIR_DIR, f"data{os.path.sep}")
     else:
         raise fdp_exc.UserConfigError(
             "Cannot guess remote data store location"
```

### Comparing `fair_cli-0.8.2/fair/configuration/__init__.py` & `fair_cli-0.8.3/fair/configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         configurations as a mapping
     """
     _local_config: typing.MutableMapping = {}
 
     # Retrieve the location of this repositories CLI config file
     _local_config_file_addr = fdp_com.local_fdpconfig(repo_loc)
     if os.path.exists(_local_config_file_addr):
-        _local_config = yaml.safe_load(open(_local_config_file_addr))
+        _local_config = yaml.safe_load(open(_local_config_file_addr, encoding='utf-8'))
 
     return _local_config
 
 
 def read_global_fdpconfig() -> typing.MutableMapping:
     """Read contents of the global FAIR-CLI configurations.
 
@@ -98,15 +98,15 @@
     """
     _global_config: typing.MutableMapping = {}
 
     # Retrieve the location of the global CLI config file
     _global_config_addr = fdp_com.global_fdpconfig()
 
     if os.path.exists(_global_config_addr):
-        _global_config = yaml.safe_load(open(_global_config_addr))
+        _global_config = yaml.safe_load(open(_global_config_addr, encoding='utf-8'))
 
     return _global_config
 
 
 def set_email(repo_loc: str, email: str, is_global: bool = False) -> None:
     """Update the email address for the user
 
@@ -117,19 +117,19 @@
     email : str
         new email address to set
     is_global : bool, optional
         whether to also override the global settings, by default False
     """
     _loc_conf = read_local_fdpconfig(repo_loc)
     _loc_conf["user"]["email"] = email
-    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), "w"))
+    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), encoding='utf-8', mode= "w"))
     if is_global:
         _glob_conf = read_global_fdpconfig()
         _glob_conf["user"]["email"] = email
-        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w"))
 
 
 def set_user(repo_loc: str, name: str, is_global: bool = False) -> None:
     """Update the name for the user
 
     Parameters
     ----------
@@ -145,28 +145,28 @@
         _given_name, _family_name = name.rsplit(" ", 1)
         _loc_conf["user"]["given_names"] = _given_name.title().strip()
         _loc_conf["user"]["family_name"] = _family_name.title().strip()
         if is_global:
             _glob_conf = read_global_fdpconfig()
             _glob_conf["user"]["given_names"] = _given_name.title().strip()
             _glob_conf["user"]["family_name"] = _family_name.title().strip()
-            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w"))
     else:
         _loc_conf["user"]["given_names"] = name.title().strip()
         _loc_conf["user"]["family_name"] = None
         if is_global:
             _glob_conf = read_global_fdpconfig()
             _glob_conf["user"]["given_names"] = name.title().strip()
             _glob_conf["user"]["family_name"] = None
-            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
-    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), "w"))
+            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w"))
+    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), encoding='utf-8', mode= "w"))
     if is_global:
         _glob_conf = read_global_fdpconfig()
         _glob_conf["user"]["name"] = name
-        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w"))
 
 
 def get_current_user_name(repo_loc: str) -> typing.Tuple[str]:
     """Retrieves the name of the current session user as defined in the config
 
     Returns
     -------
@@ -280,15 +280,15 @@
     if not local:
         if not os.path.exists(_token_file):
             raise fdp_exc.FileNotFoundError(
                 f"Cannot read token for registry '{remote}', token file '{_token_file}'"
                 " does not exist"
             )
 
-        _token = open(_token_file).read().strip()
+        _token = open(_token_file, encoding='utf-8').read().strip()
 
         if not _token:
             raise fdp_exc.CLIConfigurationError(
                 f"Cannot read token from file '{_token_file}', file is empty."
             )
 
         return _token
@@ -433,15 +433,15 @@
     uri: str
         new local URI for the registry
     """
     _global_conf = read_global_fdpconfig()
 
     _global_conf["registries"]["local"]["uri"] = uri
 
-    with open(fdp_com.global_fdpconfig(), "w") as out_f:
+    with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as out_f:
         yaml.dump(_global_conf, out_f)
 
 
 def get_local_port(local_uri: str = None) -> int:
     """Retrieve the local port from the local URI"""
     if not local_uri:
         local_uri = get_local_uri()
@@ -459,15 +459,15 @@
     _current_address = fdp_com.registry_session_address(registry_dir)
 
     _new_url = f'http://{_current_address}:{_current_port}/api/'
 
     if os.path.exists(fdp_com.global_fdpconfig()) and read_global_fdpconfig():
         _glob_conf = read_global_fdpconfig()
         _glob_conf["registries"]["local"]["uri"] = _new_url
-        with open(fdp_com.global_fdpconfig(), "w") as out_f:
+        with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as out_f:
             yaml.dump(_glob_conf, out_f)
 
     return _new_url
 
 
 def _handle_orcid(user_orcid: str) -> typing.Tuple[typing.Dict, str]:
     """Extract the name information from an ORCID selection
@@ -729,15 +729,15 @@
             if len(_rem_key) == 40:
                 _rem_key_valid = True
             else:
                 click.echo("Remote token should be 40 characters long")
 
         _rem_key_file = os.path.join(fdp_com.global_config_dir(), "remotetoken.txt")
 
-        with open(_rem_key_file, 'w') as f:
+        with open(_rem_key_file, encoding='utf-8', mode= 'w') as f:
             f.write(_rem_key)
 
         if not os.path.exists(_rem_key_file):
             raise fdp_exc.CLIConfigurationError(f'Token could not be written to {_rem_key_file}')
 
     if not fdp_serv.check_server_running():
         if _ := click.confirm(
@@ -896,15 +896,15 @@
         _def_rem_key = click.prompt(
             "Remote API Token File", default=_def_rem_key
         )
         _def_rem_key = os.path.expandvars(_def_rem_key)
 
         while (
             not os.path.exists(_def_rem_key)
-            or not open(_def_rem_key).read().strip()
+            or not open(_def_rem_key, encoding='utf-8').read().strip()
         ):
             click.echo(
                 f"Token file '{_def_rem_key}' does not exist or is empty, "
                 "please provide a valid token file."
             )
             _def_rem_key = click.prompt("Remote API Token File")
             _def_rem_key = os.path.expandvars(_def_rem_key)
```

### Comparing `fair_cli-0.8.2/fair/configuration/validation.py` & `fair_cli-0.8.3/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/exceptions.py` & `fair_cli-0.8.3/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/files.txt` & `fair_cli-0.8.3/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/history.py` & `fair_cli-0.8.3/fair/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,24 +77,24 @@
     ]
 
     for job_dir, _log_file in zip(_sorted_time_dirs, _log_files):
         # Use the timestamp directory name for the hash
         _job_id = fdp_run.get_job_hash(job_dir)
 
         if _job_id[: len(job_id)] == job_id:
-            with open(_log_file) as f:
+            with open(_log_file, encoding='utf-8') as f:
                 click.echo(f.read())
             _jobs_list = os.path.join(job_dir, "coderuns.txt")
 
             # Check if a code runs file exists for the given job and also
             # print the list of code_run uuids created in the registry
             if os.path.exists(_jobs_list):
                 click.echo("Related Code Runs: ")
                 click.echo(
-                    "\t- " + "\n\t- ".join(open(_jobs_list).readlines())
+                    "\t- " + "\n\t- ".join(open(_jobs_list, encoding='utf-8').readlines())
                 )
 
             return _log_file
 
     raise fdp_exc.FileNotFoundError(
         f"Could not find job matching id '{job_id}'"
     )
@@ -129,15 +129,15 @@
         zip(_sorted_time_dirs, _log_files)
     ):
         _job_id = fdp_run.get_job_hash(job_dir)
         if not os.path.exists(_log_file):
             raise fdp_exc.FileNotFoundError(
                 f"Cannot open log for job '{_job_id}'"
             )
-        with open(_log_file) as f:
+        with open(_log_file, encoding='utf-8') as f:
             _log_lines = f.readlines()
             _metadata = []
             for line in _log_lines:
                 if "------- time taken " in line:
                     break
                 if " = " in line:
                     _metadata.append(line)
```

### Comparing `fair_cli-0.8.2/fair/identifiers.py` & `fair_cli-0.8.3/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/logging.py` & `fair_cli-0.8.3/fair/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         command : str
             command executed
         """
         # Record the time the job was commenced, create a log and both
         # print output and write it to the log file
         _timestamp = self._now.strftime("%Y-%m-%d_%H_%M_%S_%f")
         _out_file = os.path.join(self._directory, f"job_{_timestamp}.log")
-        self._file_stream = open(_out_file, "w")
+        self._file_stream = open(_out_file, encoding= 'utf-8', mode= "w")
         _out_str = self._now.strftime("%a %b %d %H:%M:%S %Y %Z")
         _user = fdp_conf.get_current_user_name(self._project)
         _email = fdp_conf.get_current_user_email(self._project)
         self._log += [
             "--------------------------------",
             f" Commenced = {_out_str}",
             f" Author    = {' '.join(_user)} <{_email}>",
```

### Comparing `fair_cli-0.8.2/fair/register.py` & `fair_cli-0.8.3/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/registry/file_formats.json` & `fair_cli-0.8.3/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/registry/requests.py` & `fair_cli-0.8.3/fair/registry/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     if not os.path.exists(_local_token_file):
         raise fdp_exc.FileNotFoundError(
             f"Failed to find local registry token, file '{_local_token_file}'"
             " does not exist.",
             hint="Try creating the file by manually starting the registry "
             "by running 'fair registry start'",
         )
-    _file_lines = open(_local_token_file).readlines()
+    _file_lines = open(_local_token_file, encoding='utf-8').readlines()
 
     if not _file_lines:
         raise fdp_exc.FileNotFoundError(
             f"Expected token in file {_local_token_file}, but file is empty"
         )
 
     return _file_lines[0].strip()
@@ -503,15 +503,15 @@
     Raises:
         fdp_exc.RegistryError: If the upload fails a RegistryError will be raised
 
     Returns:
         bool: Will return True if the upload succeeded.
     """
     s = requests.Session()
-    _req = s.put(upload_url, data= open(file_loc,'rb').read())
+    _req = s.put(upload_url, data= open(file_loc, mode='rb').read())
     if _req.status_code not in [200, 201]:
         raise fdp_exc.RegistryError(f"File: {file_loc} could not be uploaded, Registry Returned: {_req.status_code}")
     return True
 
 def download_file(url: str, chunk_size: int = 8192) -> str:
     """Download a file from a given URL
 
@@ -542,15 +542,15 @@
                 f" due to connection error: {traceback.format_exc()}"
             ) from e
     else:
         try:
             requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
             headers = {'User-Agent':str(UserAgent().chrome)}
             response = requests.get(url, allow_redirects = True, verify = False, headers = headers)
-            open(_fname, 'wb').write(response.content)
+            open(_fname, mode= 'wb').write(response.content)
         except Exception as e:
             raise fdp_exc.FAIRCLIException(
                 f"Failed to download file '{url}'"
                 f" due to connection error: {traceback.format_exc()}"
             ) from e
 
     return _fname
```

### Comparing `fair_cli-0.8.2/fair/registry/server.py` & `fair_cli-0.8.3/fair/registry/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     os.makedirs(fdp_com.global_config_dir(), exist_ok=True)
 
     logger.debug("Updating registry path in global CLI configuration")
     if os.path.exists(fdp_com.global_fdpconfig()):
         _glob_conf = fdp_util.flatten_dict(fdp_conf.read_global_fdpconfig())
         _glob_conf["registries.local.directory"] = install_dir
 
-        with open(fdp_com.global_fdpconfig(), "w") as out_conf:
+        with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as out_conf:
             yaml.dump(fdp_util.expand_dict(_glob_conf), out_conf)
 
     if force:
         logger.debug("Removing existing installation at '%s'", install_dir)
         if platform.system() == "Windows":
             fdp_com.set_file_permissions(install_dir)
         shutil.rmtree(install_dir, onerror=fdp_com.remove_readonly)
```

### Comparing `fair_cli-0.8.2/fair/registry/storage.py` & `fair_cli-0.8.3/fair/registry/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,23 +222,23 @@
     fair.exceptions.RegistryAPICallError
         if bad status code returned from the registry
     """
     logger.debug("Storing working config on registry")
 
     _root_store = get_write_storage(uri, work_cfg_yml, token)
 
-    _work_cfg = yaml.safe_load(open(work_cfg_yml))
+    _work_cfg = yaml.safe_load(open(work_cfg_yml, encoding='utf-8'))
     _work_cfg_data_store = _work_cfg["run_metadata"]["write_data_store"]
     _rel_path = os.path.relpath(work_cfg_yml, _work_cfg_data_store)
     _time_stamp_dir = os.path.basename(os.path.dirname(work_cfg_yml))
 
     # Construct hash from config contents and time stamp
     # NOTE: You can have the same file stored N times for N job runs
     # hence the use of a timestamp in the hashing
-    _hashable = open(work_cfg_yml).read() + _time_stamp_dir
+    _hashable = open(work_cfg_yml, encoding='utf-8').read() + _time_stamp_dir
 
     _hash = hashlib.sha1(_hashable.encode("utf-8")).hexdigest()
 
     _storage_loc_data = {
         "path": _rel_path,
         "storage_root": _root_store,
         "public": _work_cfg["run_metadata"].get("public", True),
@@ -301,26 +301,26 @@
     Raises
     ------
     fair.exceptions.RegistryAPICallError
         if bad status code returned from the registry
     """
     logger.debug("Storing working script on registry")
 
-    _work_cfg = yaml.safe_load(open(working_config))
+    _work_cfg = yaml.safe_load(open(working_config, encoding='utf-8'))
     _root_store = get_write_storage(uri, working_config, token)
     _data_store = _work_cfg["run_metadata"]["write_data_store"]
 
     _rel_path = os.path.relpath(script_path, _data_store)
 
     _time_stamp_dir = os.path.basename(os.path.dirname(working_config))
 
     # Construct hash from config contents and time
     # NOTE: You can have the same file stored N times for N job runs
     # hence the use of a timestamp in the hashing
-    _hashable = open(script_path).read() + _time_stamp_dir
+    _hashable = open(script_path, encoding='utf-8').read() + _time_stamp_dir
 
     _hash = hashlib.sha1(_hashable.encode("utf-8")).hexdigest()
 
     _storage_loc_data = {
         "path": _rel_path,
         "storage_root": _root_store,
         "public": _work_cfg["run_metadata"].get("public", True),
@@ -696,15 +696,15 @@
     -------
     str
         SHA1 hash for file
     """
     # If the file is large we do not want to hash it in one go
     _input_hasher = hashlib.sha1()
 
-    with open(file_name, "rb") as in_f:
+    with open(file_name, mode= "rb") as in_f:
         _buffer = in_f.read(buffer_size)
         while len(_buffer) > 0:
             _input_hasher.update(_buffer)
             _buffer = in_f.read(buffer_size)
 
     return _input_hasher.hexdigest()
```

### Comparing `fair_cli-0.8.2/fair/registry/sync.py` & `fair_cli-0.8.3/fair/registry/sync.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/registry/versioning.py` & `fair_cli-0.8.3/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/run.py` & `fair_cli-0.8.3/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/session.py` & `fair_cli-0.8.3/fair/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1076,15 +1076,15 @@
         if "registries" not in self._local_config:
             raise fdp_exc.CLIConfigurationError(
                 "Cannot generate user 'config.yaml'",
                 hint="You need to set the remote URL"
                 " by running: \n\n\tfair remote add <url>\n",
             )
 
-        with open(output_file_name, "w") as f:
+        with open(output_file_name, encoding='utf-8', mode= "w") as f:
             _yaml_str = fdp_tpl.config_template.render(
                 instance=self,
                 data_dir=fdp_com.default_data_dir(),
                 local_repo=os.path.abspath(
                     fdp_com.find_fair_root(self._session_loc)
                 ),
             )
@@ -1094,15 +1094,15 @@
 
     def _export_cli_configuration(self, output_file: str) -> None:
         _cli_config = fdp_conf.read_global_fdpconfig()
         _loc_config = fdp_conf.read_local_fdpconfig(self._session_loc)
         _cli_config["git"] = _loc_config["git"]
         _cli_config["registries"].update(_loc_config["registries"])
         _cli_config["user"].update(_loc_config["user"])
-        with open(output_file, "w") as f:
+        with open(output_file, encoding='utf-8', mode= "w") as f:
             yaml.dump(_cli_config, f)
 
     # noqa: C901
     def initialise(
         self,
         using: typing.Dict = None,
         registry: str = None,
@@ -1189,17 +1189,17 @@
                     click.echo("Setup will now ask you questions regarding this repo configuration")
                 self._local_config = fdp_conf.local_config_query(
                     self._global_config, local=local
                 )
             except (fdp_exc.CLIConfigurationError, click.Abort) as e:
                 self._clean_reset(_fair_dir, e, True)
         if not using:
-            with open(fdp_com.local_fdpconfig(self._session_loc), "w") as f:
+            with open(fdp_com.local_fdpconfig(self._session_loc), encoding='utf-8', mode= "w") as f:
                 yaml.dump(self._local_config, f)
-            with open(fdp_com.global_fdpconfig(), "w") as f:
+            with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as f:
                 yaml.dump(self._global_config, f)
         else:
             if not self._testing:
                 click.echo("Setup will now ask you questions regarding the global configuration")
             self._global_config = fdp_conf.read_global_fdpconfig()
             if not self._testing:
                 click.echo("Setup will now ask you questions regarding this repo configuration")
@@ -1261,18 +1261,18 @@
             # Remove the session cache file
             _cache_addr = os.path.join(
                 fdp_com.session_cache_dir(), f"{self._session_id}.run"
             )
             os.remove(_cache_addr)
 
         if os.path.exists(fdp_com.global_config_dir()):
-            with open(fdp_com.global_fdpconfig(), "w") as f:
+            with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as f:
                 yaml.dump(self._global_config, f)
         if os.path.exists(os.path.dirname(fdp_com.local_fdpconfig())):
-            with open(fdp_com.local_fdpconfig(self._session_loc), "w") as f:
+            with open(fdp_com.local_fdpconfig(self._session_loc), encoding='utf-8', mode= "w") as f:
                 yaml.dump(self._local_config, f)
 
     def _validate_and_load_cli_config(self, cli_config: typing.Dict):
         _exp_keys = ["registries", "namespaces", "user", "git"]
 
         for key in _exp_keys:
             if key not in cli_config:
@@ -1334,18 +1334,18 @@
         _glob_cfg = copy.deepcopy(cli_config)
         _loc_cfg = copy.deepcopy(cli_config)
         del _glob_cfg["git"]
         if "description" in _glob_cfg:
             del _glob_cfg["description"]
         del _loc_cfg["registries"]["local"]
 
-        with open(fdp_com.global_fdpconfig(), "w") as f:
+        with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as f:
             yaml.dump(_glob_cfg, f)
 
-        with open(fdp_com.local_fdpconfig(self._session_loc), "w") as f:
+        with open(fdp_com.local_fdpconfig(self._session_loc), encoding='utf-8', mode= "w") as f:
             yaml.dump(_loc_cfg, f)
 
     def _set_logger_info(self):
         handler = logging.StreamHandler()
         handler.setFormatter(
             fdp_logging.LevelFormatter(
                 {
```

### Comparing `fair_cli-0.8.2/fair/staging.py` & `fair_cli-0.8.3/fair/staging.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,19 +80,19 @@
     def _create_staging_file(self) -> None:
         _staging_dict = {
             "job": {},
             "file": {},
             "data_product": {},
             "code_run": {},
         }
-        yaml.dump(_staging_dict, open(self._staging_file, "w"))
+        yaml.dump(_staging_dict, open(self._staging_file, encoding='utf-8', mode= "w"))
 
     def reset_staged(self) -> None:
         """Change staging state of all items to unstaged"""
-        _staging_dict = yaml.safe_load(open(self._staging_file))
+        _staging_dict = yaml.safe_load(open(self._staging_file, encoding='utf-8'))
         for obj_type in _staging_dict:
             for item in _staging_dict[obj_type]:
                 _staging_dict[obj_type][item] = False
         yaml.dump(_staging_dict, open(self._staging_file, "w"))        
 
     def add_to_staging(self, identifier: str, item_type: str) -> None:
         """Add an item to tracking
@@ -101,20 +101,20 @@
         ----------
         identifier : str
             unique identifier for the item
         item_type : str
             the item type
         """
         # Open the staging dictionary first
-        with open(self._staging_file) as f:
+        with open(self._staging_file, encoding='utf-8') as f:
             _staging_dict = yaml.safe_load(f)
 
         _staging_dict[item_type][identifier] = False
 
-        with open(self._staging_file, "w") as f:
+        with open(self._staging_file, encoding='utf-8', mode= "w") as f:
             yaml.dump(_staging_dict, f)
 
     def change_stage_status(
         self,
         identifier: str,
         item_type: str,
         stage: bool = True,
@@ -132,23 +132,23 @@
         if not self.is_in_staging_dict(identifier, item_type):
             raise fdp_exc.StagingError(
                 f"Cannot stage '{item_type}' with label '{identifier}', "
                 "item does not exist."
             )
         
         # Open the staging dictionary first
-        _staging_dict = yaml.safe_load(open(self._staging_file))
+        _staging_dict = yaml.safe_load(open(self._staging_file, encoding='utf-8'))
         _staging_dict[item_type][identifier] = stage
 
-        with open(self._staging_file, "w") as f:
+        with open(self._staging_file, encoding='utf-8', mode= "w") as f:
             yaml.dump(_staging_dict, f)
 
     def is_in_staging_dict(self, identifier, item_type):
         # Open the staging dictionary first
-        _staging_dict = yaml.safe_load(open(self._staging_file))
+        _staging_dict = yaml.safe_load(open(self._staging_file, encoding='utf-8'))
 
         if identifier in _staging_dict[item_type]:
             return True
         return False
 
     def change_data_product_stage_status(
         self, data_product_id: str, stage: bool = True
@@ -246,18 +246,18 @@
         )
         # Check if any code_runs are present for the given job
         _code_run_file = os.path.join(job_dir, "coderuns.txt")
         _code_run_urls = []
 
         if (
             os.path.exists(_code_run_file)
-            and open(_code_run_file).read().strip()
+            and open(_code_run_file, encoding='utf-8').read().strip()
         ):
             self._logger.debug("Found coderuns file, extracting runs")
-            _runs = [i.strip() for i in open(_code_run_file).readlines()]
+            _runs = [i.strip() for i in open(_code_run_file, encoding='utf-8').readlines()]
 
             for run in _runs:
                 _results = fdp_req.get(
                     local_uri,
                     "code_run",
                     fdp_req.local_token(),
                     params={"uuid": run},
@@ -334,15 +334,15 @@
             raise fdp_exc.FileNotFoundError(
                 f"Cannot stage job '{identifier}' "
                 f"Expected config.yaml in '{_directory}'"
             )
 
         # Find this job script on the local registry, as the script
         # can have any name obtain this information from the config.yaml
-        _config_dict = yaml.safe_load(open(_config_yaml))
+        _config_dict = yaml.safe_load(open(_config_yaml, encoding='utf-8'))
 
         if (
             "run_metadata" not in _config_dict
             or "script_path" not in _config_dict["run_metadata"]
         ):
             _script_url = None
         else:
@@ -390,56 +390,56 @@
         ----------
             identifier : str
                 name or ID of item
             stage_type: str, optional
                 type of stage item either job (default) or file
         """
         # Open the staging dictionary first
-        _staging_dict = yaml.safe_load(open(self._staging_file))
+        _staging_dict = yaml.safe_load(open(self._staging_file, encoding='utf-8'))
 
         if stage_type not in _staging_dict:
             raise fdp_exc.StagingError(
                 f"Cannot remove staging item of unrecognised type '{stage_type}'"
             )
 
         if identifier not in _staging_dict[stage_type]:
             raise fdp_exc.StagingError(
                 f"Cannot remove item '{identifier}' of stage type '{stage_type}', "
                 "item is not in staging."
             )
 
         del _staging_dict[stage_type][identifier]
 
-        with open(self._staging_file, "w") as f:
+        with open(self._staging_file, encoding='utf-8', mode= "w") as f:
             yaml.dump(_staging_dict, f)
 
     def get_item_list(
         self, staged: bool = True, stage_type: str = "job"
     ) -> typing.List[str]:
         """Returns a list of items of type 'stage_type' which are staged/unstaged
 
         Parameters
         ----------
             staged : bool
                 list staged/unstaged items
             stage_type : str, optional
                 type of stage item either job (default) or file
         """
-        _staging_dict = yaml.safe_load(open(self._staging_file))
+        _staging_dict = yaml.safe_load(open(self._staging_file, encoding='utf-8'))
 
         if stage_type not in _staging_dict:
             raise fdp_exc.StagingError(
                 f"Cannot remove staging item of unrecognised type '{stage_type}'"
             )
 
         return [k for k, v in _staging_dict[stage_type].items() if v == staged]
 
     def update_data_product_staging(self) -> None:
         """Update DataProduct list in staging file."""
-        with open(self._staging_file) as f:
+        with open(self._staging_file, encoding='utf-8') as f:
             _staging_dict = yaml.safe_load(f)
 
         result = fdp_req.url_get(
             f"{fdp_com.DEFAULT_LOCAL_REGISTRY_URL}data_product",
             fdp_req.local_token(),
         )
 
@@ -449,37 +449,37 @@
             )["name"]
             name = data_product["name"]
             version = data_product["version"]
             key = f"{namespace}:{name}@v{version}"
             if key not in _staging_dict["data_product"]:
                 _staging_dict["data_product"][key] = False
 
-        with open(self._staging_file, "w") as f:
+        with open(self._staging_file, encoding='utf-8', mode= "w") as f:
             yaml.dump(_staging_dict, f)
 
     def update_code_run_staging(self) -> None:
         """Update code_run(s) list in staging file."""
-        with open(self._staging_file) as f:
+        with open(self._staging_file, encoding='utf-8') as f:
             _staging_dict = yaml.safe_load(f)
 
         result = fdp_req.url_get(
             f"{fdp_com.DEFAULT_LOCAL_REGISTRY_URL}code_run",
             fdp_req.local_token(),
         )
 
         for code_run in result:
             key = code_run["uuid"]
             if key not in _staging_dict["code_run"]:
                 _staging_dict["code_run"][key] = False
 
-        with open(self._staging_file, "w") as f:
+        with open(self._staging_file, encoding='utf-8', mode="w") as f:
             yaml.dump(_staging_dict, f)
 
     def _load_from_file(self, file_name: str = None) -> typing.Dict[str, bool]:
         if not file_name:
             file_name = self._staging_file
 
-        with open(file_name, "w") as f:
+        with open(file_name, encoding='utf-8', mode= "w") as f:
             _staging_dict = yaml.safe_load(f)
 
         self._staging_file = file_name
         return _staging_dict
```

### Comparing `fair_cli-0.8.2/fair/testing.py` & `fair_cli-0.8.3/fair/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     _loc_data_store = os.path.join(testing_dir, "data_store") + os.path.sep
     _proj_dir = os.path.join(testing_dir, "project")
 
     if tokenless:
         _token = "t35tt0k3n"
         _token_file = os.path.join(registry_dir, "token.txt")
-        with open(_token_file, "w") as out_f:
+        with open(_token_file, encoding='utf-8', mode= "w") as out_f:
             out_f.write(_token)
 
     if not local_git_dir:
         local_git_dir = _no_git_setup(_proj_dir)
     os.makedirs(_loc_data_store, exist_ok=True)
     _local_uri = "http://127.0.0.1:8000/api/"
     _origin_uri = "http://127.0.0.1:8001/api/"
```

### Comparing `fair_cli-0.8.2/fair/user_config/__init__.py` & `fair_cli-0.8.3/fair/user_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             if not os.path.exists(config_yaml):
                 raise fdp_exc.FileNotFoundError(
                     f"Cannot load job configuration from file '{config_yaml}', "
                     "file does not exist"
                 )
 
             self._logger.debug("Loading file '%s'", config_yaml)
-            self._config: typing.Dict = yaml.safe_load(open(config_yaml))
+            self._config: typing.Dict = yaml.safe_load(open(config_yaml, encoding='utf-8'))
 
         self._fill_missing()
 
         self._now = datetime.datetime.now()
         self._parsed = {"namespace": [], "author": []}
         self.env = None
         self._job_dir = None
@@ -573,29 +573,29 @@
             if "extension" not in SHELLS[_shell]:
                 raise fdp_exc.InternalError(
                     f"Failed to retrieve an extension for shell '{_shell}'"
                 )
             _ext = SHELLS[_shell]["extension"]
             _out_file = os.path.join(self._job_dir, f"script.{_ext}")
             if _cmd:
-                with open(_out_file, "w") as f:
+                with open(_out_file, encoding='utf-8', mode= "w") as f:
                     f.write(_cmd)
 
         elif "script_path" in self["run_metadata"]:
             _path = self["run_metadata.script_path"]
             if not os.path.exists(_path):
                 raise fdp_exc.CommandExecutionError(
                     f"Failed to execute run, script '{_path}' was not found, or"
                     " failed to be created.",
                     exit_code=1,
                 )
-            _cmd = open(_path).read()
+            _cmd = open(_path, encoding='utf-8').read()
             _out_file = os.path.join(self._job_dir, os.path.basename(_path))
             if _cmd:
-                with open(_out_file, "w") as f:
+                with open(_out_file, encoding='utf-8', mode= "w") as f:
                     f.write(_cmd)
 
         self._logger.debug("Script command: %s", _cmd)
         self._logger.debug("Script written to: %s", _out_file)
 
         if not _cmd or not _out_file:
             raise fdp_exc.UserConfigError(
@@ -732,15 +732,15 @@
 
         _time_stamp = self._now.strftime("%Y-%m-%d_%H_%M_%S_%f")
         self._log_file_path = os.path.join(_logs_dir, f"job_{_time_stamp}.log")
         self._logger.debug(
             f"Will write session log to '{self._log_file_path}'"
         )
         command = command or self.command
-        self._log_file = open(self._log_file_path, "w")
+        self._log_file = open(self._log_file_path, encoding='utf-8', mode= "w")
 
     def prepare(
         self,
         job_mode: CMD_MODE,
         allow_dirty: bool = False,
         remote_uri: str = None,
         remote_token: str = None,
@@ -1486,15 +1486,15 @@
         if not output_file:
             if not self._job_dir:
                 raise fdp_exc.UserConfigError(
                     "Cannot write new user configuration file, "
                     "no job directory created and no alternative filename provided"
                 )
             output_file = os.path.join(self._job_dir, fdp_com.USER_CONFIG_FILE)
-        with open(output_file, "w") as out_f:
+        with open(output_file, encoding='utf-8', mode= "w") as out_f:
             yaml.dump(self._config, out_f)
 
         self.env = self._create_environment()
 
         self._logger.debug(f"Configuration written to '{output_file}'")
 
         return output_file
```

### Comparing `fair_cli-0.8.2/fair/user_config/globbing.py` & `fair_cli-0.8.3/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/user_config/validation.py` & `fair_cli-0.8.3/fair/user_config/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,9 +315,9 @@
     import argparse
 
     import yaml
 
     parser = argparse.ArgumentParser()
     parser.add_argument("in_file")
 
-    _data = yaml.safe_load(open(parser.parse_args().in_file))
+    _data = yaml.safe_load(open(parser.parse_args().in_file, encoding='utf-8'))
     UserConfigModel(**_data)
```

### Comparing `fair_cli-0.8.2/fair/utilities.py` & `fair_cli-0.8.3/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/fair/virtualenv.py` & `fair_cli-0.8.3/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.2/pyproject.toml` & `fair_cli-0.8.3/pyproject.toml`

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
-version = "0.8.2"
+version = "0.8.3"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.8.2/PKG-INFO` & `fair_cli-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.8.2
+Version: 0.8.3
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

