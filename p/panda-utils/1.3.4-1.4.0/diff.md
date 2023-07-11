# Comparing `tmp/panda_utils-1.3.4.tar.gz` & `tmp/panda_utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.3.4.tar", last modified: Sat Jul  8 05:42:59 2023, max compression
+gzip compressed data, was "panda_utils-1.4.0.tar", last modified: Tue Jul 11 16:26:13 2023, max compression
```

## Comparing `panda_utils-1.3.4.tar` & `panda_utils-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.384063 panda_utils-1.3.4/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.3.4/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    22167 2023-07-08 05:42:59.384063 panda_utils-1.3.4/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    21437 2023-07-08 05:41:53.000000 panda_utils-1.3.4/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.3.4/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.380729 panda_utils-1.3.4/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.4/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.3.4/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.384063 panda_utils-1.3.4/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.3.4/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     4488 2023-07-08 05:09:48.000000 panda_utils-1.3.4/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.3.4/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.3.4/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    11402 2023-07-08 05:17:02.000000 panda_utils-1.3.4/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.3.4/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.384063 panda_utils-1.3.4/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.3.4/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.3.4/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.3.4/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.384063 panda_utils-1.3.4/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.3.4/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5608 2023-07-07 09:32:40.000000 panda_utils-1.3.4/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.3.4/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.384063 panda_utils-1.3.4/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.4/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.3.4/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.3.4/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.3.4/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.3.4/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.3.4/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.3.4/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-08 05:42:59.380729 panda_utils-1.3.4/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    22167 2023-07-08 05:42:59.000000 panda_utils-1.3.4/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-07-08 05:42:59.000000 panda_utils-1.3.4/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-08 05:42:59.000000 panda_utils-1.3.4/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-08 05:42:59.000000 panda_utils-1.3.4/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-08 05:42:59.000000 panda_utils-1.3.4/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-08 05:40:43.000000 panda_utils-1.3.4/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.3.4/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-08 05:42:59.384063 panda_utils-1.3.4/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.0/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-11 16:26:13.308351 panda_utils-1.4.0/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.0/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.0/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.0/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.0/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.0/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     4488 2023-07-08 05:09:48.000000 panda_utils-1.4.0/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.4.0/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      269 2023-07-09 18:02:42.000000 panda_utils-1.4.0/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    12990 2023-07-11 15:46:06.000000 panda_utils-1.4.0/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.0/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.0/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      614 2023-07-11 09:02:42.000000 panda_utils-1.4.0/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.4.0/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.0/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.0/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5608 2023-07-07 09:32:40.000000 panda_utils-1.4.0/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.4.0/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.0/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.0/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.0/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.0/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.0/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.0/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.0/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      950 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-11 15:59:43.000000 panda_utils-1.4.0/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.0/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-11 16:26:13.308351 panda_utils-1.4.0/setup.cfg
```

### Comparing `panda_utils-1.3.4/LICENSE` & `panda_utils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/__main__.py` & `panda_utils-1.4.0/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.4.0/panda_utils/assetpipeline/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/assetpipeline/models.py` & `panda_utils-1.4.0/panda_utils/assetpipeline/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import fnmatch
 import logging
 import os
+import platform
 import re
 import shutil
 import subprocess
 from pathlib import Path
 
 from panda_utils import util
 from panda_utils.eggtree import eggparse, operations
@@ -12,72 +13,123 @@
 from panda_utils.tools.palettize import remove_palette_indices
 from panda_utils.util import get_data_file_path
 
 preblend_regex = re.compile(r".*\.(fbx|obj)")
 logger = logging.getLogger("panda_utils.pipeline.models")
 
 
+def run_blender(cwd, file, script, *inputs):
+    args = [util.choose_binary("blender"), "--background", "--python", get_data_file_path(script), "--", *inputs]
+    if file is not None:
+        args.insert(1, file)
+    stdout_pipe = subprocess.DEVNULL if not os.getenv("PANDA_UTILS_BLENDER_LOGGING") else None
+    subprocess.run(args, stdout=stdout_pipe, cwd=cwd)
+
+
 def build_asset_mapper(assets, name):
     output = {}
     for counter, item in enumerate(sorted(assets)):
         extension = item.split(".")[-1]
         new_file_name = f"{name}-{counter}.{extension}" if counter else f"{name}.{extension}"
         output[item] = new_file_name
     return output
 
 
+def __patch_filename(filename):
+    osname = platform.system()
+    if osname == "Linux":
+        return filename
+
+    if osname == "Windows":
+        return filename[1] + ":\\" + filename[3:].replace("/", "\\")
+
+    raise RuntimeError(f"Unsupported OS: {osname}")
+
+
 def action_preblend(ctx):
     all_inputs = [file for file in ctx.files if preblend_regex.match(file)]
     logger.info("%s: Converting to blend: %s", ctx.name, ", ".join(all_inputs))
 
     blend_filename = f"{ctx.model_name}.blend"
-    subprocess.run(
-        [util.choose_binary("blender"), "--background", "--python", get_data_file_path("blender/import_model.py"),
-         "--", Path.cwd() / blend_filename, *all_inputs],
-        stdout=subprocess.DEVNULL,
-        cwd=ctx.cwd,
-    )
+    run_blender(ctx.cwd, None, "blender/import_model.py", Path.cwd() / blend_filename, *all_inputs)
 
 
 def action_blendrename(ctx):
     count = 0
     for file in ctx.files:
         if file.endswith(".blend"):
             blend_filename = ctx.model_name
             if count:
                 blend_filename += f"-{count}"
             blend_filename += ".blend"
             count += 1
             shutil.move(file, blend_filename)
 
 
-def action_blend2bam(ctx):
+def __make_blend2bam_args(binary, flags):
+    args = []
+    if "srgb" not in flags:
+        args.append("--no-srgb")
+    if "bullet" in flags:
+        args.append("--collision-shapes" if binary == "gltf2bam" else "--physics-engine")
+        args.append("bullet")
+    if "legacy" in flags:
+        if binary == "gltf2bam":
+            args.append("--legacy-materials")
+        else:
+            args.append("--material-mode")
+            args.append("legacy")
+    return args
+
+
+def __run_export_util(ctx, binary, input_file, output_file, flags):
+    res = subprocess.run(
+        [binary, *__make_blend2bam_args(binary, flags), input_file, output_file],
+        stdout=subprocess.DEVNULL, stderr=subprocess.PIPE, cwd=ctx.cwd
+        )
+    err = res.stderr.decode("utf-8")
+    if err and "KeyError: 'nodes'" in err:
+        logger.error("%s: Blender output an empty model, aborting.", ctx.name)
+        ctx.valid = False
+    elif err:
+        logger.error("%s: Blender failed", ctx.name)
+        print(err)
+        exit(1)
+
+
+def __run_blend2bam(ctx, file, flags):
+    logger.info("%s: Patching texture paths: %s", ctx.name, file)
+    full_path = f"{ctx.cwd}/{file}"
+    run_blender(ctx.cwd, full_path, "blender/patch_paths.py")
+
+    logger.info("%s: Converting to bam: %s", ctx.name, file)
+    bam_filename = file[:-5] + "bam"
+    __run_export_util(ctx, "blend2bam", file, bam_filename, flags)
+
+
+def __run_gltf2bam(ctx, file, flags):
+    logger.info("%s: Exporting to GLTF: %s", ctx.name, file)
+    full_path = f"{ctx.cwd}/{file}"
+    intermediate_file = file[:-5] + "glb"
+    bam_filename = file[:-5] + "bam"
+    target_path = f"{ctx.cwd}/{intermediate_file}"
+    run_blender(ctx.cwd, full_path, "blender/export_glb.py", target_path)
+
+    logger.info("%s: Converting to bam: %s", ctx.name, intermediate_file)
+    __run_export_util(ctx, "gltf2bam", intermediate_file, bam_filename, flags)
+
+
+def action_blend2bam(ctx, flags=""):
+    flags = flags.lower().split(",")
     for file in ctx.files:
         if file.endswith(".blend"):
-            logger.info("%s: Patching texture paths: %s", ctx.name, file)
-            full_path = f"{ctx.cwd}/{file}"
-            subprocess.run(
-                [util.choose_binary("blender"), full_path, "--background",
-                 "--python", get_data_file_path("blender/patch_paths.py")],
-                stdout=subprocess.DEVNULL,
-                cwd=ctx.cwd,
-            )
-
-            logger.info("%s: Converting to bam: %s", ctx.name, file)
-            bam_filename = file[:-5] + "bam"
-            res = subprocess.run(["blend2bam", "--no-srgb", file, bam_filename],
-                                 stdout=subprocess.DEVNULL, stderr=subprocess.PIPE, cwd=ctx.cwd)
-            err = res.stderr.decode("utf-8")
-            if err and "KeyError: 'nodes'" in err:
-                logger.error("%s: Blender output an empty model, aborting.", ctx.name)
-                ctx.valid = False
-            elif err:
-                logger.error("%s: Blender failed", ctx.name)
-                print(err)
-                exit(1)
+            if "b2b" in flags:
+                __run_blend2bam(ctx, file, flags)
+            else:
+                __run_gltf2bam(ctx, file, flags)
 
 
 def action_bam2egg(ctx):
     for file in ctx.files:
         if file.endswith(".bam"):
             logger.info("%s: Converting %s from Bam to Egg", ctx.name, file)
             bam2egg(ctx.putil_ctx, file)
@@ -88,14 +140,15 @@
     ctx.cache_eggs()
     for tree in ctx.eggs.values():
         for tex in tree.findall("Texture"):
             textures.add(eggparse.sanitize_string(tex.get_child(0).value))
 
     texture_mapper = build_asset_mapper(textures, ctx.model_name)
     for fnold, fnnew in texture_mapper.items():
+        fnold = __patch_filename(fnold)
         shutil.move(fnold, fnnew)
 
     for file, eggtree in ctx.eggs.items():
         logger.info("%s: Optimizing model: %s", ctx.name, file)
         # The first thing we should do is patch the texture paths
         for tex in eggtree.findall("Texture"):
             tex_node = tex.get_child(0)
```

### Comparing `panda_utils-1.3.4/panda_utils/assetpipeline/textures.py` & `panda_utils-1.4.0/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/blender/import_model.py` & `panda_utils-1.4.0/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/eggtree/eggparse.py` & `panda_utils-1.4.0/panda_utils/eggtree/eggparse.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/eggtree/operations.py` & `panda_utils-1.4.0/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/tools/animconvert.py` & `panda_utils-1.4.0/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/tools/convert.py` & `panda_utils-1.4.0/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/tools/downscale.py` & `panda_utils-1.4.0/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/tools/palettize.py` & `panda_utils-1.4.0/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/tools/toontown.py` & `panda_utils-1.4.0/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils/util.py` & `panda_utils-1.4.0/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.4/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.4.0/panda_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 panda_utils/assetpipeline/__init__.py
 panda_utils/assetpipeline/__main__.py
 panda_utils/assetpipeline/imports.py
 panda_utils/assetpipeline/misc.py
 panda_utils/assetpipeline/models.py
 panda_utils/assetpipeline/textures.py
 panda_utils/blender/__init__.py
+panda_utils/blender/export_glb.py
 panda_utils/blender/import_model.py
 panda_utils/blender/patch_paths.py
 panda_utils/eggtree/__init__.py
 panda_utils/eggtree/eggparse.py
 panda_utils/eggtree/operations.py
 panda_utils/tools/__init__.py
 panda_utils/tools/animconvert.py
```

### Comparing `panda_utils-1.3.4/pyproject.toml` & `panda_utils-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.3.4"
+version = "1.4.0"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

