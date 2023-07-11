# Comparing `tmp/ryantam626_jupyterlab_vim-0.16.1.tar.gz` & `tmp/ryantam626_jupyterlab_vim-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryantam626_jupyterlab_vim-0.16.1.tar", last modified: Tue Jul 11 10:57:01 2023, max compression
+gzip compressed data, was "ryantam626_jupyterlab_vim-0.16.2.tar", last modified: Tue Jul 11 11:03:51 2023, max compression
```

## Comparing `ryantam626_jupyterlab_vim-0.16.1.tar` & `ryantam626_jupyterlab_vim-0.16.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1069 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      413 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/MANIFEST.in
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       93 2023-07-11 10:46:32.000000 ryantam626_jupyterlab_vim-0.16.1/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      189 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/install.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      319 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      440 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/_version.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/package.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.706577 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.706577 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    10940 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/static/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      165 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/static/style.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2620 2023-07-11 10:54:26.000000 ryantam626_jupyterlab_vim-0.16.1/package.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      591 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/pyproject.toml
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      723 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/not-zip-safe
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       15 2023-07-11 10:57:01.000000 ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/top_level.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2714 2023-07-11 10:53:45.000000 ryantam626_jupyterlab_vim-0.16.1/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/src/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9510 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/src/codemirrorCommands.ts
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3846 2023-07-11 10:53:45.000000 ryantam626_jupyterlab_vim-0.16.1/src/index.ts
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    12229 2023-07-11 10:46:32.000000 ryantam626_jupyterlab_vim-0.16.1/src/labCommands.ts
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 10:57:01.710578 ryantam626_jupyterlab_vim-0.16.1/style/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/style/index.css
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/style/index.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      554 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.1/tsconfig.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)   191574 2023-06-01 14:58:00.000000 ryantam626_jupyterlab_vim-0.16.1/yarn.lock
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1069 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      413 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/MANIFEST.in
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       93 2023-07-11 10:46:32.000000 ryantam626_jupyterlab_vim-0.16.2/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      189 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/install.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      319 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      440 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/_version.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2620 2023-07-11 11:00:30.000000 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/package.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.350660 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.350660 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/@ryantam626/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2620 2023-07-11 11:00:30.000000 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/package.json.orig
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    10940 2023-07-11 11:00:30.000000 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/plugin.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/static/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      169 2023-07-11 11:00:30.000000 ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/static/style.js
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2620 2023-07-11 11:02:41.000000 ryantam626_jupyterlab_vim-0.16.2/package.json
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      591 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/pyproject.toml
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-07-11 11:03:51.000000 ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      731 2023-07-11 11:03:51.000000 ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-11 11:03:51.000000 ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-11 11:00:18.000000 ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/not-zip-safe
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       15 2023-07-11 11:03:51.000000 ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/top_level.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/setup.cfg
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2714 2023-07-11 10:53:45.000000 ryantam626_jupyterlab_vim-0.16.2/setup.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/src/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9510 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/src/codemirrorCommands.ts
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3846 2023-07-11 10:53:45.000000 ryantam626_jupyterlab_vim-0.16.2/src/index.ts
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    12229 2023-07-11 10:46:32.000000 ryantam626_jupyterlab_vim-0.16.2/src/labCommands.ts
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-11 11:03:51.354660 ryantam626_jupyterlab_vim-0.16.2/style/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/style/index.css
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/style/index.js
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      554 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.2/tsconfig.json
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)   191574 2023-06-01 14:58:00.000000 ryantam626_jupyterlab_vim-0.16.2/yarn.lock
```

### Comparing `ryantam626_jupyterlab_vim-0.16.1/LICENSE` & `ryantam626_jupyterlab_vim-0.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/PKG-INFO` & `ryantam626_jupyterlab_vim-0.16.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryantam626_jupyterlab_vim
-Version: 0.16.1
+Version: 0.16.2
 Summary: Code cell vim bindings
 Home-page: https://github.com/ryantam626/jupyterlab-vim
 Author: Jupyterlab-vim contributors
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/package.json` & `ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8897058823529411%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/ryantam626/jupyterlab-vim/issues'}",*

 * * "'homepage'": "'https://github.com/ryantam626/jupyterlab-vim'",*

 * * "'name'": "'@ryantam626/jupyterlab_vim'",*

 * * "'repository'": "{'url': 'https://github.com/ryantam626/jupyterlab-vim.git'}",*

 * * "'version'": "'0.16.1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": "Axel Fahy",
     "bugs": {
-        "url": "https://github.com/jupyterlab-contrib/jupyterlab-vim/issues"
+        "url": "https://github.com/ryantam626/jupyterlab-vim/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.0.0-rc.13",
         "@jupyterlab/cells": "^3.0.0-rc.13",
         "@jupyterlab/codemirror": "^3.0.0-rc.13",
         "@jupyterlab/notebook": "^3.0.0-rc.13",
         "@jupyterlab/settingregistry": "^3.0.0-rc.13",
@@ -31,32 +31,32 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/index.js"
     ],
-    "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
+    "homepage": "https://github.com/ryantam626/jupyterlab-vim",
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_vim/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
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
-        "url": "https://github.com/jupyterlab-contrib/jupyterlab-vim.git"
+        "url": "https://github.com/ryantam626/jupyterlab-vim.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
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

### Comparing `ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig` & `ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/package.json.orig`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8897058823529411%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/ryantam626/jupyterlab-vim/issues'}",*

 * * "'homepage'": "'https://github.com/ryantam626/jupyterlab-vim'",*

 * * "'name'": "'@ryantam626/jupyterlab_vim'",*

 * * "'repository'": "{'url': 'https://github.com/ryantam626/jupyterlab-vim.git'}",*

 * * "'version'": "'0.16.1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": "Axel Fahy",
     "bugs": {
-        "url": "https://github.com/jupyterlab-contrib/jupyterlab-vim/issues"
+        "url": "https://github.com/ryantam626/jupyterlab-vim/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.0.0-rc.13",
         "@jupyterlab/cells": "^3.0.0-rc.13",
         "@jupyterlab/codemirror": "^3.0.0-rc.13",
         "@jupyterlab/notebook": "^3.0.0-rc.13",
         "@jupyterlab/settingregistry": "^3.0.0-rc.13",
@@ -31,32 +31,32 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/index.js"
     ],
-    "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
+    "homepage": "https://github.com/ryantam626/jupyterlab-vim",
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_vim/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
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
-        "url": "https://github.com/jupyterlab-contrib/jupyterlab-vim.git"
+        "url": "https://github.com/ryantam626/jupyterlab-vim.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
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

### Comparing `ryantam626_jupyterlab_vim-0.16.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json` & `ryantam626_jupyterlab_vim-0.16.2/jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/plugin.json`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/package.json` & `ryantam626_jupyterlab_vim-0.16.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'0.16.2'"}*

```diff
@@ -70,9 +70,9 @@
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.16.1"
+    "version": "0.16.2"
 }
```

### Comparing `ryantam626_jupyterlab_vim-0.16.1/pyproject.toml` & `ryantam626_jupyterlab_vim-0.16.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/PKG-INFO` & `ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryantam626-jupyterlab-vim
-Version: 0.16.1
+Version: 0.16.2
 Summary: Code cell vim bindings
 Home-page: https://github.com/ryantam626/jupyterlab-vim
 Author: Jupyterlab-vim contributors
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `ryantam626_jupyterlab_vim-0.16.1/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt` & `ryantam626_jupyterlab_vim-0.16.2/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 pyproject.toml
 setup.py
 tsconfig.json
 yarn.lock
 jupyterlab_vim/__init__.py
 jupyterlab_vim/_version.py
 jupyterlab_vim/labextension/package.json
-jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
-jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/package.json.orig
+jupyterlab_vim/labextension/schemas/@ryantam626/jupyterlab_vim/plugin.json
 jupyterlab_vim/labextension/static/style.js
 ryantam626_jupyterlab_vim.egg-info/PKG-INFO
 ryantam626_jupyterlab_vim.egg-info/SOURCES.txt
 ryantam626_jupyterlab_vim.egg-info/dependency_links.txt
 ryantam626_jupyterlab_vim.egg-info/not-zip-safe
 ryantam626_jupyterlab_vim.egg-info/top_level.txt
 src/codemirrorCommands.ts
```

### Comparing `ryantam626_jupyterlab_vim-0.16.1/setup.py` & `ryantam626_jupyterlab_vim-0.16.2/setup.py`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/src/codemirrorCommands.ts` & `ryantam626_jupyterlab_vim-0.16.2/src/codemirrorCommands.ts`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/src/index.ts` & `ryantam626_jupyterlab_vim-0.16.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/src/labCommands.ts` & `ryantam626_jupyterlab_vim-0.16.2/src/labCommands.ts`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/tsconfig.json` & `ryantam626_jupyterlab_vim-0.16.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.16.1/yarn.lock` & `ryantam626_jupyterlab_vim-0.16.2/yarn.lock`

 * *Files identical despite different names*

