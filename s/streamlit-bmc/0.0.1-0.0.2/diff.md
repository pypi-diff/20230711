# Comparing `tmp/streamlit_bmc-0.0.1.tar.gz` & `tmp/streamlit_bmc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bmc-0.0.1.tar", last modified: Tue Jul 11 07:01:56 2023, max compression
+gzip compressed data, was "streamlit_bmc-0.0.2.tar", last modified: Tue Jul 11 09:32:22 2023, max compression
```

## Comparing `streamlit_bmc-0.0.1.tar` & `streamlit_bmc-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 07:01:56.786433 streamlit_bmc-0.0.1/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1063 2023-07-10 08:43:21.000000 streamlit_bmc-0.0.1/LICENSE
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       46 2023-07-11 06:57:47.000000 streamlit_bmc-0.0.1/MANIFEST.in
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      278 2023-07-11 07:01:56.786303 streamlit_bmc-0.0.1/PKG-INFO
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     3016 2023-07-11 06:37:19.000000 streamlit_bmc-0.0.1/README.md
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       38 2023-07-11 07:01:56.786488 streamlit_bmc-0.0.1/setup.cfg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      592 2023-07-11 06:38:52.000000 streamlit_bmc-0.0.1/setup.py
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 07:01:56.785222 streamlit_bmc-0.0.1/streamlit_bmc/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6369 2023-07-11 07:01:08.000000 streamlit_bmc-0.0.1/streamlit_bmc/__init__.py
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 07:01:56.786095 streamlit_bmc-0.0.1/streamlit_bmc.egg-info/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      278 2023-07-11 07:01:56.000000 streamlit_bmc-0.0.1/streamlit_bmc.egg-info/PKG-INFO
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      248 2023-07-11 07:01:56.000000 streamlit_bmc-0.0.1/streamlit_bmc.egg-info/SOURCES.txt
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)        1 2023-07-11 07:01:56.000000 streamlit_bmc-0.0.1/streamlit_bmc.egg-info/dependency_links.txt
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       16 2023-07-11 07:01:56.000000 streamlit_bmc-0.0.1/streamlit_bmc.egg-info/requires.txt
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       14 2023-07-11 07:01:56.000000 streamlit_bmc-0.0.1/streamlit_bmc.egg-info/top_level.txt
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 09:32:22.514788 streamlit_bmc-0.0.2/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1063 2023-07-10 08:43:21.000000 streamlit_bmc-0.0.2/LICENSE
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       47 2023-07-11 09:26:39.000000 streamlit_bmc-0.0.2/MANIFEST.in
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      432 2023-07-11 09:32:22.514630 streamlit_bmc-0.0.2/PKG-INFO
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     2980 2023-07-11 07:09:27.000000 streamlit_bmc-0.0.2/README.md
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       38 2023-07-11 09:32:22.514846 streamlit_bmc-0.0.2/setup.cfg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      767 2023-07-11 09:30:32.000000 streamlit_bmc-0.0.2/setup.py
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 09:32:22.508685 streamlit_bmc-0.0.2/streamlit_bmc/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6370 2023-07-11 09:27:22.000000 streamlit_bmc-0.0.2/streamlit_bmc/__init__.py
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 09:32:22.507423 streamlit_bmc-0.0.2/streamlit_bmc/frontend/
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 09:32:22.510523 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6148 2023-07-11 09:32:09.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/.DS_Store
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 09:32:22.512313 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/build/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       39 2023-07-11 09:26:12.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/build/bundle.css
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      116 2023-07-11 09:26:12.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/build/bundle.css.map
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)   228816 2023-07-11 09:26:12.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/build/bundle.js
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)  1119899 2023-07-11 09:26:12.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/build/bundle.js.map
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1110 2023-07-11 07:30:38.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/index.html
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1361 2023-07-11 04:36:58.000000 streamlit_bmc-0.0.2/streamlit_bmc/frontend/public/style.css
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-11 09:32:22.509472 streamlit_bmc-0.0.2/streamlit_bmc.egg-info/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      432 2023-07-11 09:32:22.000000 streamlit_bmc-0.0.2/streamlit_bmc.egg-info/PKG-INFO
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      563 2023-07-11 09:32:22.000000 streamlit_bmc-0.0.2/streamlit_bmc.egg-info/SOURCES.txt
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)        1 2023-07-11 09:32:22.000000 streamlit_bmc-0.0.2/streamlit_bmc.egg-info/dependency_links.txt
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       16 2023-07-11 09:32:22.000000 streamlit_bmc-0.0.2/streamlit_bmc.egg-info/requires.txt
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       14 2023-07-11 09:32:22.000000 streamlit_bmc-0.0.2/streamlit_bmc.egg-info/top_level.txt
```

### Comparing `streamlit_bmc-0.0.1/LICENSE` & `streamlit_bmc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.1/README.md` & `streamlit_bmc-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # 📝 Streamlit - Business Model Canvas
 
 [![GitHub][github_badge]][github_link] [![PyPI][pypi_badge]][pypi_link] 
 
 ## Installation
 
 ```sh
-pip install streamlit-business-model-canvas
+pip install streamlit-bmc
 ```
 
 ## Getting started
 
 ```python
 import streamlit as st
 
-from streamlit_business_model_canvas import st_bmc
+from streamlit_bmc import st_bmc
 
 # Spawn a new MBC editor
 # Re-generate your JSON data
 data = {
     "visual": {
         "company_name": "Apple"
     },
```

### Comparing `streamlit_bmc-0.0.1/streamlit_bmc/__init__.py` & `streamlit_bmc-0.0.2/streamlit_bmc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,22 @@
         # We give the component a simple, descriptive name ("streamlit_bmc"
         # does not fit this bill, so please choose something better for your
         # own component :)
         "streamlit_bmc",
         # Pass `url` here to tell Streamlit that the component will be served
         # by the local dev server that you run via `npm run start`.
         # (This is useful while your component is in development.)
-        url="http://localhost:3001",
+        url="http://localhost:3000",
     )
 else:
     # When we're distributing a production version of the component, we'll
     # replace the `url` param with `path`, and point it to to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "frontend/build")
+    build_dir = os.path.join(parent_dir, "frontend/public")
     _component_func = components.declare_component("streamlit_bmc", path=build_dir)
 
 
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
```

