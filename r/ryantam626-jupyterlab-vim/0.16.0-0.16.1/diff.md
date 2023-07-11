# Comparing `tmp/ryantam626_jupyterlab_vim-0.16.0.tar.gz` & `tmp/ryantam626_jupyterlab_vim-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryantam626_jupyterlab_vim-0.16.0.tar", last modified: Thu Jun  1 16:22:23 2023, max compression
+gzip compressed data, was "ryantam626_jupyterlab_vim-0.16.1.tar", last modified: Tue Jul 11 10:57:01 2023, max compression
```

## Comparing `ryantam626_jupyterlab_vim-0.16.0.tar` & `ryantam626_jupyterlab_vim-0.16.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1069 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      413 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/MANIFEST.in
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       93 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      189 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/install.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      319 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      440 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/_version.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/package.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    10940 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      165 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/style.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2616 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/package.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      591 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/pyproject.toml
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      723 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/not-zip-safe
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       15 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/top_level.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2710 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/src/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9510 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/src/codemirrorCommands.ts
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3842 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/src/index.ts
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    12229 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/src/labCommands.ts
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/style/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/style/index.css
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/style/index.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      554 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/tsconfig.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)   191574 2023-06-01 14:58:00.000000 ryantam626_jupyterlab_vim-0.16.0/yarn.lock
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1069 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      413 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/MANIFEST.in
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       93 2023-07-11 10:46:32.000000 ryantam626_jupyterlab_vim-0.16.1/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      189 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/install.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      319 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      440 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/_version.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/package.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.706577 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.706577 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    10940 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/static/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      165 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/static/style.js
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2620 2023-07-11 10:54:26.000000 ryantam626_jupyterlab_vim-0.16.1/package.json
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      591 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/pyproject.toml
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      723 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/not-zip-safe
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       15 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/top_level.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/setup.cfg
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2714 2023-07-11 10:53:45.000000 ryantam626_jupyterlab_vim-0.16.1/setup.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/src/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9510 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/src/codemirrorCommands.ts
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3846 2023-07-11 10:53:45.000000 ryantam626_jupyterlab_vim-0.16.1/src/index.ts
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    12229 2023-07-11 10:46:32.000000 ryantam626_jupyterlab_vim-0.16.1/src/labCommands.ts
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/style/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/style/index.css
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/style/index.js
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      554 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/tsconfig.json
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)   191574 2023-06-01 14:58:00.000000 ryantam626_jupyterlab_vim-0.16.1/yarn.lock
```

### Comparing `ryantam626_jupyterlab_vim-0.16.0/LICENSE` & `ryantam626_jupyterlab_vim-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/PKG-INFO` & `ryantam626_jupyterlab_vim-0.16.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryantam626_jupyterlab_vim
-Version: 0.16.0
+Version: 0.16.1
 Summary: Code cell vim bindings
 Home-page: https://github.com/ryantam626/jupyterlab-vim
 Author: Jupyterlab-vim contributors
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/package.json` & `ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/package.json`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig` & `ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json` & `ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/package.json` & `ryantam626_jupyterlab_vim-0.16.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'name'": "'@ryantam626/jupyterlab_vim'", "'version'": "'0.16.1'"}*

```diff
@@ -45,15 +45,15 @@
         "extension",
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@axlair/jupyterlab_vim",
+    "name": "@ryantam626/jupyterlab_vim",
     "repository": {
         "type": "git",
         "url": "https://github.com/ryantam626/jupyterlab-vim.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
@@ -70,9 +70,9 @@
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.16.0"
+    "version": "0.16.1"
 }
```

### Comparing `ryantam626_jupyterlab_vim-0.16.0/pyproject.toml` & `ryantam626_jupyterlab_vim-0.16.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/PKG-INFO` & `ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryantam626-jupyterlab-vim
-Version: 0.16.0
+Version: 0.16.1
 Summary: Code cell vim bindings
 Home-page: https://github.com/ryantam626/jupyterlab-vim
 Author: Jupyterlab-vim contributors
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt` & `ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/setup.py` & `ryantam626_jupyterlab_vim-0.16.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Representative files that should exist after a successful build
 ensured_targets = [
     str(lab_path / "package.json"),
     str(lab_path / "static/style.js")
 ]
 
-labext_name = "@axlair/jupyterlab_vim"
+labext_name = "@ryantam626/jupyterlab_vim"
 
 data_files_spec = [
     ("share/jupyter/labextensions/%s" % labext_name, str(lab_path.relative_to(HERE)), "**"),
     ("share/jupyter/labextensions/%s" % labext_name, str("."), "install.json"),
 ]
 
 long_description = (HERE / "README.md").read_text()
```

### Comparing `ryantam626_jupyterlab_vim-0.16.0/src/codemirrorCommands.ts` & `ryantam626_jupyterlab_vim-0.16.1/src/codemirrorCommands.ts`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/src/index.ts` & `ryantam626_jupyterlab_vim-0.16.1/src/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import { ICodeMirror, CodeMirrorEditor } from '@jupyterlab/codemirror';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IDisposable } from '@lumino/disposable';
 
 import { VimCellManager, IKeybinding } from './codemirrorCommands';
 import { addJLabCommands } from './labCommands';
 
-const PLUGIN_NAME = '@axlair/jupyterlab_vim';
+const PLUGIN_NAME = '@ryantam626/jupyterlab_vim';
 const TOGGLE_ID = 'jupyterlab-vim:toggle';
 let enabled = false;
 
 /**
  * Initialization data for the jupyterlab_vim extension.
  */
 const extension: JupyterFrontEndPlugin<void> = {
```

### Comparing `ryantam626_jupyterlab_vim-0.16.0/src/labCommands.ts` & `ryantam626_jupyterlab_vim-0.16.1/src/labCommands.ts`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/tsconfig.json` & `ryantam626_jupyterlab_vim-0.16.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.0/yarn.lock` & `ryantam626_jupyterlab_vim-0.16.1/yarn.lock`

 * *Files identical despite different names*

