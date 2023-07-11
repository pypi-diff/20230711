# Comparing `tmp/viur_cli-1.0.6.tar.gz` & `tmp/viur_cli-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-1.0.6.tar", last modified: Wed Jun 28 07:05:28 2023, max compression
+gzip compressed data, was "viur_cli-1.0.7.tar", last modified: Tue Jul 11 11:05:52 2023, max compression
```

## Comparing `viur_cli-1.0.6.tar` & `viur_cli-1.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.026944 viur_cli-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-28 07:05:19.000000 viur_cli-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-28 07:05:28.026944 viur_cli-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-28 07:05:19.000000 viur_cli-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-28 07:05:19.000000 viur_cli-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-28 07:05:28.026944 viur_cli-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-28 07:05:19.000000 viur_cli-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.022944 viur_cli-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.022944 viur_cli-1.0.6/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/npm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.022944 viur_cli-1.0.6/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.026944 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.026944 viur_cli-1.0.6/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scripts/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 07:05:19.000000 viur_cli-1.0.6/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:05:28.022944 viur_cli-1.0.6/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-28 07:05:28.000000 viur_cli-1.0.6/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-28 07:05:28.000000 viur_cli-1.0.6/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 07:05:28.000000 viur_cli-1.0.6/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-28 07:05:28.000000 viur_cli-1.0.6/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-28 07:05:28.000000 viur_cli-1.0.6/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 07:05:28.000000 viur_cli-1.0.6/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 11:05:42.000000 viur_cli-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 11:05:52.685399 viur_cli-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-11 11:05:42.000000 viur_cli-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 11:05:42.000000 viur_cli-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 11:05:52.685399 viur_cli-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 11:05:42.000000 viur_cli-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.677398 viur_cli-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.681398 viur_cli-1.0.7/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/npm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.681398 viur_cli-1.0.7/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-1.0.6/LICENSE` & `viur_cli-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/PKG-INFO` & `viur_cli-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 1.0.6 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 1.0.7 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.6/README.md` & `viur_cli-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/setup.cfg` & `viur_cli-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/build.py` & `viur_cli-1.0.7/src/viur_cli/build.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,104 @@
+"""
+Performs build steps configured within the project, or creates any necessary steps for a project deployment build.
+"""
+
 import click, os, zipfile, shutil, urllib, json
-from . import cli, get_config, echo_error, write_config
 from urllib.request import urlretrieve
-from . import cli, echo_error, utils, conf
+from . import cli, conf, utils, get_config, write_config
+
+
+def _build(cfg, name, build_cfg, additional_args):
+    """Internal function to perform steps required for a given build configuration.
+
+    :param cfg: The project configuration (default, or project-specific)
+    :param name: Name of the app to build.
+    :param build_cfg: The build-cfg for the specified app.
+    :param additional_args: List of additional arguments.
+    """
+    utils.echo_info(f"""- {build_cfg["kind"]} {name}""")
+
+    match build_cfg["kind"]:
+        case "flare":
+            # Ensure for local pyodide, if configured!
+            if pyodide_version := cfg.get("pyodide"):
+                utils.echo_info(f"- Ensuring Pyodide {pyodide_version} local install")
+                utils.system(f'get-pyodide -t {cfg["distribution_folder"]}/pyodide -v v{pyodide_version}')
+
+            if "debug" in additional_args:
+                flare_build_type = "debug"
+                flare_build_env = ""
+            else:
+                flare_build_type = "release"
+                flare_build_env = "pyenv exec"
+
+                # enforce python 3.9.5
+                # FIXME: This is highly obsolete...
+                if "3.9.5" not in os.popen("pyenv versions").read():
+                    utils.system(f'pyenv install 3.9.5')
+                utils.system("pyenv local 3.9.5")
+
+            utils.echo_info(f"- Building Flare: {flare_build_type} {name}")
+            utils.system(f'{flare_build_env} viur flare {flare_build_type} {name}')
+
+            if flare_build_type == "release":
+                utils.system("pyenv local system")
+
+        case "npm":
+            utils.system(
+                " && ".join(
+                    (
+                        f'cd {os.path.join(cfg["sources_folder"], build_cfg["source"])}',
+                        "npm install",
+                        f'npm run {build_cfg["command"]}'
+                    )
+                )
+            )
+
+        case "exec":
+            utils.system(build_cfg["command"])
+
+        case other:
+            utils.echo_fatal(f"Unknown build kind {other!r}")
 
 
 @cli.group()
 def build():
-    """Build VIUR project"""
+    """Build VIUR project or specific apps."""
 
 @build.command(context_settings={"ignore_unknown_options": True})
 @click.argument("name", default='develop')
 @click.argument("additional_args", nargs=-1)
 def release(name, additional_args):
-    """create a release build"""
+    """Build of all relevant apps to deploy this project."""
 
-    utils.echo_info("building started...")
     projectConfig = conf.get_config()
 
-    if not os.popen("pyenv versions").read():
-        echo_error(f"pyenv not found!")
-        return
-
     if name not in projectConfig:
-        echo_error(f"{name} is not a valid config name.")
-        return
+        utils.echo_fatal(f"{name} is not a valid config name.")
 
     cfg = projectConfig["default"].copy()
     cfg.update(projectConfig[name])
 
+    utils.echo_info("building started...")
 
-    if builds_cfg := cfg.get("builds"):
-
-        # build all flare apps
-        if flare_apps := [k for k,v in builds_cfg.items() if builds_cfg[k]["kind"] == "flare"]:
-            # we have atlease 1 flare app
-            # Ensure for local pyodide.
-            pyodide_version = cfg.get("pyodide", conf.DEFAULT_PYODIDE_VERSION)
-            utils.echo_info(f"- Ensuring Pyodide {pyodide_version} local install")
-
-            os.system(f'get-pyodide -t {cfg["distribution_folder"]}/pyodide -v v{pyodide_version}')
-
-            if "debug" in additional_args:
-                flare_build_type = "debug"
-                flare_build_env = ""
-            else:
-                flare_build_type = "release"
-                flare_build_env = "pyenv exec"
-
-                #enforce python 3.9.5
-                if "3.9.5" not in os.popen("pyenv versions").read():
-                    os.system(f'pyenv install 3.9.5')
-                os.system("pyenv local 3.9.5")
-
-            for name in flare_apps:
-                utils.echo_info(f"- Building {flare_build_type} {name}")
-                os.system(f'{flare_build_env} viur flare {flare_build_type} {name}')
-
-            if flare_build_type == "release":
-                os.system("pyenv local system")
+    for build_name, build_cfg in cfg.get("builds", {}).items():
+        _build(cfg, build_name, build_cfg, additional_args)
 
-        # build all npm apps
-        if npm_apps := [k for k,v in builds_cfg.items() if builds_cfg[k]["kind"] == "npm"]:
-            for name in npm_apps:
-                utils.echo_info(f"- Building {name}")
-                os.system(f'cd {cfg["sources_folder"]}{builds_cfg[name]["source"]} && npm install && npm run {builds_cfg[name]["command"]}')
-        # build all scripts
-        if script_apps := [k for k, v in builds_cfg.items() if builds_cfg[k]["kind"] == "exec"]:
-            for name in script_apps:
-                utils.echo_info(f"- Building {name}")
-                os.system(builds_cfg[name]["command"])
     utils.echo_info("building finished!")
 
 @build.command(context_settings={"ignore_unknown_options": True})
 @click.argument("appname", default="")
 @click.argument("additional_args", nargs=-1)
 def app(appname, additional_args):
-    """create a release build"""
-    valid_apps = conf.get_config()["default"]["builds"].keys()
-    if not appname or appname not in valid_apps:
-        echo_error("appname musst be one of these options")
-        echo_error(", ".join(valid_apps))
-        return
+    """Build specific app."""
 
-    utils.echo_info("building started...")
     projectConfig = conf.get_config()
 
-    if not os.popen("pyenv versions").read():
-        echo_error(f"pyenv not found!")
-        return
-
     cfg = projectConfig["default"].copy()
 
-    builds_cfg = cfg.get("builds").get(appname)
-
-    if builds_cfg["kind"] == "flare":
-        pyodide_version = cfg.get("pyodide", conf.DEFAULT_PYODIDE_VERSION)
-        utils.echo_info(f"- Ensuring Pyodide {pyodide_version} local install")
-
-        os.system(f'get-pyodide -t {cfg["distribution_folder"]}/pyodide -v v{pyodide_version}')
-
-        if "debug" in additional_args:
-            flare_build_type = "debug"
-            flare_build_env = ""
-        else:
-            flare_build_type = "release"
-            flare_build_env = "pyenv exec"
-
-            # enforce python 3.9.5
-            if "3.9.5" not in os.popen("pyenv versions").read():
-                os.system(f'pyenv install 3.9.5')
-            os.system("pyenv local 3.9.5")
-
-        utils.echo_info(f"- Building Flare: {flare_build_type} {appname}")
-        os.system(f'{flare_build_env} viur flare {flare_build_type} {appname}')
-
-        if flare_build_type == "release":
-            os.system("pyenv local system")
-    elif builds_cfg["kind"] == "npm":
-        utils.echo_info(f"- Building NPM: {appname}")
-        os.system(
-            f'cd {cfg["sources_folder"]}{builds_cfg["source"]} && npm install && npm run {builds_cfg["command"]}')
-    elif builds_cfg["kind"] == "exec":
-        utils.echo_info(f"- Building Script: {appname}")
-        os.system(builds_cfg["command"])
+    if not (build_cfg := cfg.get("builds").get(appname)):
+        utils.echo_fatal(f"""{appname=} must be one of these options: {", ".join(cfg["builds"].keys())}""")
 
-    utils.echo_info("building finished!")
+    utils.echo_info("building started...")
+    _build(cfg, appname, build_cfg, additional_args)
+    utils.echo_info("building finished!")
```

### Comparing `viur_cli-1.0.6/src/viur_cli/cli.py` & `viur_cli-1.0.7/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/conf.py` & `viur_cli-1.0.7/src/viur_cli/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         "default": {
             "format":"1.0.0",
             "distribution_folder": deployFolder,
             "sources_folder": sourcesFolder,
             "builds": {},
             "vi": "submodule",
             "core": "submodule",
-            "pyodide": click.prompt('pyodide', default=DEFAULT_PYODIDE_VERSION)
         },
 
         "develop": {
             "application_name": click.prompt('application name'),
             "version": click.prompt('develop version name')
         }
     }
@@ -254,21 +253,18 @@
     assert projectConfig, "load_config() must be called first!"
 
     assert projectConfig["default"]["format"] in ["1.0.0", "1.0.1", "1.1.0", "1.1.1"], "Invalid formatversion, you have to fix it manually"
 
     if "format" not in projectConfig["default"]:
         projectConfig["default"]["format"] = "1.0.1"
 
-    if "pyodide" not in projectConfig["default"]:
-        projectConfig["default"]["pyodide"] = DEFAULT_PYODIDE_VERSION
-
     ##################### Version 1.0.1
 
-    if projectConfig["default"]["pyodide"].startswith("v"):
-        projectConfig["default"]["pyodide"] = projectConfig["default"]["pyodide"][1:] #remove v prefix
+    if (pyodide_version := projectConfig["default"].get("pyodide")) and pyodide_version.startswith("v"):
+        projectConfig["default"]["pyodide"] = pyodide_version[1:] #remove v prefix
 
     if projectConfig["default"]["vi"].startswith("v"):
         projectConfig["default"]["vi"] = projectConfig["default"]["vi"][1:]  # remove v prefix
 
     if projectConfig["default"]["format"] == "1.0.0":
         projectConfig["default"]["format"] = "1.0.1"
```

### Comparing `viur_cli-1.0.6/src/viur_cli/deploy.py` & `viur_cli-1.0.7/src/viur_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/flare.py` & `viur_cli-1.0.7/src/viur_cli/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/install.py` & `viur_cli-1.0.7/src/viur_cli/install.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/local.py` & `viur_cli-1.0.7/src/viur_cli/local.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/npm.py` & `viur_cli-1.0.7/src/viur_cli/npm.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/cli.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scripts/flare.py` & `viur_cli-1.0.7/src/viur_cli/scripts/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-1.0.7/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-1.0.7/src/viur_cli/scripts/viur_2to3.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "utils.currentLanguage": "current.language",
     "utils.currentRequest": "current.request",
     "utils.currentRequestData": "current.request_data",
     "utils.currentSession": "current.session",
     "utils.getCurrentUser": "current.user.get",
     "utils.isLocalDevelopmentServer": "conf[\"viur.instance.is_dev_server\"]",
     "utils.projectID": "conf[\"viur.instance.project_id\"]",
+    "clearUpdateTag=True": "update_relations=False",
 }
 
 bones = [
     "base",
     "boolean",
     "captcha",
     "color",
```

### Comparing `viur_cli-1.0.6/src/viur_cli/setup.py` & `viur_cli-1.0.7/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/tool.py` & `viur_cli-1.0.7/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.6/src/viur_cli/utils.py` & `viur_cli-1.0.7/src/viur_cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-import click, sys, typing, datetime, getpass
+import os, click, sys, typing, datetime, getpass
+
+
+def system(cmd):
+    """Performs an os.system() call with the given command, but throws an echo_fatal on error and stops viur-cli."""
+    if os.system(cmd) != 0:
+        echo_fatal(f"Failed to execute {cmd!r}")
 
 
 def echo_error(msg):
     """colored cli feedback"""
     click.echo(click.style("ERROR: " + msg, fg="red"))
```

### Comparing `viur_cli-1.0.6/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-1.0.7/src/viur_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-cli Version: 1.0.6 Summary: Command-line
+Metadata-Version: 2.1 Name: viur-cli Version: 1.0.7 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.6/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-1.0.7/src/viur_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

