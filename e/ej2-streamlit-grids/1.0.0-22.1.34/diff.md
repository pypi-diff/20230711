# Comparing `tmp/ej2_streamlit_grids-1.0.0.tar.gz` & `tmp/ej2_streamlit_grids-22.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ej2_streamlit_grids-1.0.0.tar", last modified: Mon Jun 26 08:53:27 2023, max compression
+gzip compressed data, was "ej2_streamlit_grids-22.1.34.tar", last modified: Tue Jul 11 05:06:54 2023, max compression
```

## Comparing `ej2_streamlit_grids-1.0.0.tar` & `ej2_streamlit_grids-22.1.34.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.715649 ej2_streamlit_grids-1.0.0/
--rw-rw-rw-   0        0        0      966 2023-03-22 08:57:35.000000 ej2_streamlit_grids-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       55 2023-03-22 08:41:37.000000 ej2_streamlit_grids-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      208 2023-06-26 08:53:27.715649 ej2_streamlit_grids-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4850 2023-02-24 04:09:23.000000 ej2_streamlit_grids-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.565694 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/
--rw-rw-rw-   0        0        0     6438 2023-05-10 13:06:16.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.541196 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.638491 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/
--rw-rw-rw-   0        0        0      859 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   197459 2022-11-28 23:06:31.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0  6617174 2023-01-22 07:29:36.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/dataset.csv
--rw-rw-rw-   0        0        0     2101 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/index.html
--rw-rw-rw-   0        0        0      564 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/precache-manifest.e2422a9ab2d58baf31368143e40f4498.js
--rw-rw-rw-   0        0        0     1185 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.545238 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.714013 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/
--rw-rw-rw-   0        0        0  3233059 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js
--rw-rw-rw-   0        0        0     1803 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0 10642847 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.map
--rw-rw-rw-   0        0        0     4547 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js
--rw-rw-rw-   0        0        0    12851 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js
--rw-rw-rw-   0        0        0     8317 2023-06-26 08:42:45.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js.map
-drwxrwxrwx   0        0        0        0 2023-06-26 08:53:27.593824 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/
--rw-rw-rw-   0        0        0      208 2023-06-26 08:53:27.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2023-06-26 08:53:27.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:53:27.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-26 08:53:27.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-26 08:53:27.000000 ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 08:53:27.717738 ej2_streamlit_grids-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      527 2023-04-11 13:28:02.000000 ej2_streamlit_grids-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:54.073277 ej2_streamlit_grids-22.1.34/
+-rw-rw-rw-   0        0        0      966 2023-03-22 08:57:35.000000 ej2_streamlit_grids-22.1.34/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-03-22 08:41:37.000000 ej2_streamlit_grids-22.1.34/MANIFEST.in
+-rw-rw-rw-   0        0        0     2097 2023-07-11 05:06:54.070988 ej2_streamlit_grids-22.1.34/PKG-INFO
+-rw-rw-rw-   0        0        0     1571 2023-07-11 04:13:34.000000 ej2_streamlit_grids-22.1.34/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:52.106122 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/
+-rw-rw-rw-   0        0        0     6438 2023-05-10 13:06:16.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:52.038016 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:52.358198 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/
+-rw-rw-rw-   0        0        0      859 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   197459 2022-11-28 23:06:31.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0  6617174 2023-01-22 07:29:36.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/dataset.csv
+-rw-rw-rw-   0        0        0     2101 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/index.html
+-rw-rw-rw-   0        0        0      564 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/precache-manifest.e2422a9ab2d58baf31368143e40f4498.js
+-rw-rw-rw-   0        0        0     1185 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:52.040164 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:54.069107 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/
+-rw-rw-rw-   0        0        0  3233059 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0 10642847 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.map
+-rw-rw-rw-   0        0        0     4547 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js
+-rw-rw-rw-   0        0        0    12851 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-rw-rw-   0        0        0     8317 2023-06-26 08:42:45.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxrwxrwx   0        0        0        0 2023-07-11 05:06:52.185341 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/
+-rw-rw-rw-   0        0        0     2097 2023-07-11 05:06:51.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2023-07-11 05:06:51.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 05:06:51.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 05:06:51.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-11 05:06:51.000000 ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 05:06:54.074113 ej2_streamlit_grids-22.1.34/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-11 05:06:12.000000 ej2_streamlit_grids-22.1.34/setup.py
```

### Comparing `ej2_streamlit_grids-1.0.0/LICENSE` & `ej2_streamlit_grids-22.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/__init__.py` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/__init__.py`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/asset-manifest.json` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/bootstrap.min.css` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/dataset.csv` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/dataset.csv`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/index.html` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/precache-manifest.e2422a9ab2d58baf31368143e40f4498.js` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/precache-manifest.e2422a9ab2d58baf31368143e40f4498.js`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/service-worker.js` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.LICENSE.txt` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.map` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/2.58a04ec1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js.map` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/main.70282647.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js.map` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids/frontend/build/static/js/runtime-main.44d30fc2.js.map`

 * *Files identical despite different names*

### Comparing `ej2_streamlit_grids-1.0.0/ej2_streamlit_grids.egg-info/SOURCES.txt` & `ej2_streamlit_grids-22.1.34/ej2_streamlit_grids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

