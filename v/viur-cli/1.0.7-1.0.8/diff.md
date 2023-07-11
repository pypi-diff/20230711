# Comparing `tmp/viur_cli-1.0.7.tar.gz` & `tmp/viur_cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-1.0.7.tar", last modified: Tue Jul 11 11:05:52 2023, max compression
+gzip compressed data, was "viur_cli-1.0.8.tar", last modified: Tue Jul 11 16:56:52 2023, max compression
```

## Comparing `viur_cli-1.0.7.tar` & `viur_cli-1.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 11:05:42.000000 viur_cli-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 11:05:52.685399 viur_cli-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-11 11:05:42.000000 viur_cli-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 11:05:42.000000 viur_cli-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 11:05:52.685399 viur_cli-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 11:05:42.000000 viur_cli-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.677398 viur_cli-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.681398 viur_cli-1.0.7/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/npm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.685399 viur_cli-1.0.7/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 11:05:42.000000 viur_cli-1.0.7/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:52.681398 viur_cli-1.0.7/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 11:05:52.000000 viur_cli-1.0.7/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.370766 viur_cli-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 16:56:36.000000 viur_cli-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 16:56:52.370766 viur_cli-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-11 16:56:36.000000 viur_cli-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 16:56:36.000000 viur_cli-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 16:56:52.370766 viur_cli-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 16:56:36.000000 viur_cli-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.358766 viur_cli-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.366766 viur_cli-1.0.8/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/npm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.366766 viur_cli-1.0.8/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.370766 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.370766 viur_cli-1.0.8/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.366766 viur_cli-1.0.8/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-1.0.7/LICENSE` & `viur_cli-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/PKG-INFO` & `viur_cli-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 1.0.7
+Version: 1.0.8
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
-Metadata-Version: 2.1 Name: viur_cli Version: 1.0.7 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 1.0.8 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.7/README.md` & `viur_cli-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/setup.cfg` & `viur_cli-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/build.py` & `viur_cli-1.0.8/src/viur_cli/build.py`

 * *Files 23% similar despite different names*

```diff
@@ -56,19 +56,55 @@
 
         case "exec":
             utils.system(build_cfg["command"])
 
         case other:
             utils.echo_fatal(f"Unknown build kind {other!r}")
 
+def _clean(cfg, name, build_cfg):
+    """Internal function to perform steps required to clean a given configuration.
+
+    :param cfg: The project configuration (default, or project-specific)
+    :param name: Name of the app to clean.
+    :param build_cfg: The build-cfg for the specified app.
+    """
+    utils.echo_info(f"""- cleaning {build_cfg["kind"]} {name}""")
+
+    match build_cfg["kind"]:
+        # for flare and npm, drop the target folder and node_modules (npm)
+        case "flare" | "npm":
+            if target_dir := build_cfg.get("target"):
+                target_dir = os.path.join(cfg["distribution_folder"], target_dir)
+                utils.echo_info(f"  - dropping {target_dir}")
+                shutil.rmtree(target_dir)
+
+            if build_cfg["kind"] == "npm":
+                # todo: Later, call "npm run clean" or a similar command when it exists
+
+                node_modules = os.path.join(cfg["sources_folder"], build_cfg["source"], "node_modules")
+                utils.echo_info(f"  - dropping {node_modules}")
+                shutil.rmtree(os.path.join(node_modules))
+
+        case "exec":
+            pass
+
+        case other:
+            utils.echo_fatal(f"Unknown build kind {other!r}")
+
+    # Always execute explicit "clean" command if provided
+    if clean_cmd := build_cfg.get("clean"):
+        utils.echo_info(f"  - executing {clean_cmd=}")
+        utils.system(clean_cmd)
+
 
 @cli.group()
 def build():
     """Build VIUR project or specific apps."""
 
+
 @build.command(context_settings={"ignore_unknown_options": True})
 @click.argument("name", default='develop')
 @click.argument("additional_args", nargs=-1)
 def release(name, additional_args):
     """Build of all relevant apps to deploy this project."""
 
     projectConfig = conf.get_config()
@@ -82,23 +118,46 @@
     utils.echo_info("building started...")
 
     for build_name, build_cfg in cfg.get("builds", {}).items():
         _build(cfg, build_name, build_cfg, additional_args)
 
     utils.echo_info("building finished!")
 
+
 @build.command(context_settings={"ignore_unknown_options": True})
-@click.argument("appname", default="")
+@click.argument("appname")
 @click.argument("additional_args", nargs=-1)
 def app(appname, additional_args):
     """Build specific app."""
 
     projectConfig = conf.get_config()
 
     cfg = projectConfig["default"].copy()
 
     if not (build_cfg := cfg.get("builds").get(appname)):
         utils.echo_fatal(f"""{appname=} must be one of these options: {", ".join(cfg["builds"].keys())}""")
 
     utils.echo_info("building started...")
     _build(cfg, appname, build_cfg, additional_args)
     utils.echo_info("building finished!")
+
+
+@build.command
+@click.argument("target", default="")
+def clean(target):
+    """Clean-up build artefacts."""
+    projectConfig = conf.get_config()
+    cfg = projectConfig["default"].copy()
+
+    builds = cfg.get("builds", {})
+    if target:
+        if not (build_cfg := builds.get(target)):
+            utils.echo_fatal(f"""{target=} must be one of these options: {", ".join(cfg["builds"].keys())}""")
+
+        builds = {target: build_cfg}
+
+    utils.echo_info("clean started...")
+
+    for build_name, build_cfg in builds.items():
+        _clean(cfg, build_name, build_cfg)
+
+    utils.echo_info("clean finished!")
```

### Comparing `viur_cli-1.0.7/src/viur_cli/cli.py` & `viur_cli-1.0.8/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/conf.py` & `viur_cli-1.0.8/src/viur_cli/conf.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/deploy.py` & `viur_cli-1.0.8/src/viur_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/flare.py` & `viur_cli-1.0.8/src/viur_cli/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/install.py` & `viur_cli-1.0.8/src/viur_cli/install.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/local.py` & `viur_cli-1.0.8/src/viur_cli/local.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/npm.py` & `viur_cli-1.0.8/src/viur_cli/npm.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/cli.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scripts/flare.py` & `viur_cli-1.0.8/src/viur_cli/scripts/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-1.0.8/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-1.0.8/src/viur_cli/scripts/viur_2to3.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/setup.py` & `viur_cli-1.0.8/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/tool.py` & `viur_cli-1.0.8/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli/utils.py` & `viur_cli-1.0.8/src/viur_cli/utils.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.7/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-1.0.8/src/viur_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-cli
-Version: 1.0.7
+Version: 1.0.8
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
-Metadata-Version: 2.1 Name: viur-cli Version: 1.0.7 Summary: Command-line
+Metadata-Version: 2.1 Name: viur-cli Version: 1.0.8 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.7/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-1.0.8/src/viur_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

