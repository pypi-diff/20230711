# Comparing `tmp/scaneo-2023.7.11.post2.tar.gz` & `tmp/scaneo-2023.7.11.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaneo-2023.7.11.post2.tar", max compression
+gzip compressed data, was "scaneo-2023.7.11.post3.tar", max compression
```

## Comparing `scaneo-2023.7.11.post2.tar` & `scaneo-2023.7.11.post3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      654 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post2/README.md
--rw-r--r--   0        0        0      352 2023-07-11 11:25:59.665305 scaneo-2023.7.11.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/__init__.py
--rw-r--r--   0        0        0      872 2023-06-13 12:37:28.547552 scaneo-2023.7.11.post2/scaneo/api.py
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/cli/__init__.py
--rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/cli/hello.py
--rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/main.py
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/routers/__init__.py
--rw-r--r--   0        0        0     1592 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post2/scaneo/routers/geojson.py
--rw-r--r--   0        0        0      104 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post2/scaneo/routers/image/__init__.py
--rw-r--r--   0        0        0     2026 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post2/scaneo/routers/image/cache.py
--rw-r--r--   0        0        0      575 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post2/scaneo/routers/image/errors.py
--rw-r--r--   0        0        0     6902 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post2/scaneo/routers/image/get_image_tile.py
--rw-r--r--   0        0        0     1919 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post2/scaneo/routers/image/image_utils.py
--rw-r--r--   0        0        0     1720 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post2/scaneo/routers/images.py
--rw-r--r--   0        0        0     1085 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post2/scaneo/routers/labels.py
--rw-r--r--   0        0        0     3365 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post2/scaneo/routers/sam.py
--rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/routers/settings.py
--rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post2/scaneo/routers/test.py
--rw-r--r--   0        0        0    62672 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/0.4946ad59.css
--rw-r--r--   0        0        0    32380 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css
--rw-r--r--   0        0        0    13943 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css
--rw-r--r--   0        0        0    62640 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css
--rw-r--r--   0        0        0    32422 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css
--rw-r--r--   0        0        0     5551 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg
--rw-r--r--   0        0        0    38018 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js
--rw-r--r--   0        0        0     9160 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js
--rw-r--r--   0        0        0   150162 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js
--rw-r--r--   0        0        0     6990 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js
--rw-r--r--   0        0        0    67243 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js
--rw-r--r--   0        0        0     1783 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/optionsStore.110d47c8.js
--rw-r--r--   0        0        0      759 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js
--rw-r--r--   0        0        0     3213 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/singletons.97dcadd1.js
--rw-r--r--   0        0        0      238 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/stores.9bcf7e68.js
--rw-r--r--   0        0        0     5139 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/entry/app.de6989fd.js
--rw-r--r--   0        0        0    23876 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/entry/start.b5a5435b.js
--rw-r--r--   0        0        0      953 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/nodes/0.a83aff18.js
--rw-r--r--   0        0        0      800 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/nodes/1.49f6fc19.js
--rw-r--r--   0        0        0    75539 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/nodes/2.bfd77d29.js
--rw-r--r--   0        0        0       27 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/_app/version.json
--rw-r--r--   0        0        0     1571 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/favicon.png
--rw-r--r--   0        0        0     1174 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/icons/brush.svg
--rw-r--r--   0        0        0     2789 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/icons/eraser.svg
--rw-r--r--   0        0        0      826 2023-07-11 11:25:59.665305 scaneo-2023.7.11.post2/scaneo/ui/icons/size.svg
--rw-r--r--   0        0        0      895 2023-07-11 11:25:59.665305 scaneo-2023.7.11.post2/scaneo/ui/icons/trashcan.svg
--rw-r--r--   0        0        0     2032 2023-07-11 11:25:59.661305 scaneo-2023.7.11.post2/scaneo/ui/index.html
--rw-r--r--   0        0        0       86 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post2/scaneo/yarn.lock
--rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post2/setup.py
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post2/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post3/README.md
+-rw-r--r--   0        0        0      499 2023-07-11 11:30:52.418266 scaneo-2023.7.11.post3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/__init__.py
+-rw-r--r--   0        0        0      872 2023-06-13 12:37:28.547552 scaneo-2023.7.11.post3/scaneo/api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/cli/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/cli/hello.py
+-rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/main.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/routers/__init__.py
+-rw-r--r--   0        0        0     1592 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post3/scaneo/routers/geojson.py
+-rw-r--r--   0        0        0      104 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post3/scaneo/routers/image/__init__.py
+-rw-r--r--   0        0        0     2026 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post3/scaneo/routers/image/cache.py
+-rw-r--r--   0        0        0      575 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post3/scaneo/routers/image/errors.py
+-rw-r--r--   0        0        0     6902 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post3/scaneo/routers/image/get_image_tile.py
+-rw-r--r--   0        0        0     1919 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post3/scaneo/routers/image/image_utils.py
+-rw-r--r--   0        0        0     1720 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post3/scaneo/routers/images.py
+-rw-r--r--   0        0        0     1085 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post3/scaneo/routers/labels.py
+-rw-r--r--   0        0        0     3365 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post3/scaneo/routers/sam.py
+-rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/routers/settings.py
+-rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post3/scaneo/routers/test.py
+-rw-r--r--   0        0        0    62672 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/0.4946ad59.css
+-rw-r--r--   0        0        0    32380 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css
+-rw-r--r--   0        0        0    13943 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css
+-rw-r--r--   0        0        0    62640 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css
+-rw-r--r--   0        0        0    32422 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css
+-rw-r--r--   0        0        0     5551 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg
+-rw-r--r--   0        0        0    38018 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js
+-rw-r--r--   0        0        0     9160 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js
+-rw-r--r--   0        0        0   150162 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js
+-rw-r--r--   0        0        0     6990 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js
+-rw-r--r--   0        0        0    67243 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js
+-rw-r--r--   0        0        0     1783 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/optionsStore.5e9cf8fd.js
+-rw-r--r--   0        0        0      759 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js
+-rw-r--r--   0        0        0     3211 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/singletons.1f79ca33.js
+-rw-r--r--   0        0        0      238 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/stores.5a8d4e4e.js
+-rw-r--r--   0        0        0     5139 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/entry/app.255fb8f1.js
+-rw-r--r--   0        0        0    23876 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/entry/start.b3231a12.js
+-rw-r--r--   0        0        0      953 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/nodes/0.2bd4934f.js
+-rw-r--r--   0        0        0      800 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/nodes/1.a75b771c.js
+-rw-r--r--   0        0        0    75539 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/nodes/2.7cf84de0.js
+-rw-r--r--   0        0        0       27 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/_app/version.json
+-rw-r--r--   0        0        0     1571 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/favicon.png
+-rw-r--r--   0        0        0     1174 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/icons/brush.svg
+-rw-r--r--   0        0        0     2789 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/icons/eraser.svg
+-rw-r--r--   0        0        0      826 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/icons/size.svg
+-rw-r--r--   0        0        0      895 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/icons/trashcan.svg
+-rw-r--r--   0        0        0     2031 2023-07-11 11:30:52.414266 scaneo-2023.7.11.post3/scaneo/ui/index.html
+-rw-r--r--   0        0        0       86 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post3/scaneo/yarn.lock
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post3/setup.py
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post3/PKG-INFO
```

### Comparing `scaneo-2023.7.11.post2/README.md` & `scaneo-2023.7.11.post3/README.md`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/api.py` & `scaneo-2023.7.11.post3/scaneo/api.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/main.py` & `scaneo-2023.7.11.post3/scaneo/main.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/geojson.py` & `scaneo-2023.7.11.post3/scaneo/routers/geojson.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/image/cache.py` & `scaneo-2023.7.11.post3/scaneo/routers/image/cache.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/image/errors.py` & `scaneo-2023.7.11.post3/scaneo/routers/image/errors.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/image/get_image_tile.py` & `scaneo-2023.7.11.post3/scaneo/routers/image/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/image/image_utils.py` & `scaneo-2023.7.11.post3/scaneo/routers/image/image_utils.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/images.py` & `scaneo-2023.7.11.post3/scaneo/routers/images.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/labels.py` & `scaneo-2023.7.11.post3/scaneo/routers/labels.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/routers/sam.py` & `scaneo-2023.7.11.post3/scaneo/routers/sam.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/0.4946ad59.css` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/0.4946ad59.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/optionsStore.110d47c8.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/optionsStore.5e9cf8fd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     w as l
-} from "./singletons.97dcadd1.js";
+} from "./singletons.1f79ca33.js";
 import {
     J as o
 } from "./index.f69b56cb.js";
 const c = {
     defaultUrl: "http://localhost:8000",
     labelsEndpoint: "/labels",
     geojsonEndpoint: "/geojson/",
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/chunks/singletons.97dcadd1.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/chunks/singletons.1f79ca33.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 import {
-    I as p,
+    I as b,
     s as I,
     a2 as R,
     T as S,
     Z as x
 } from "./index.f69b56cb.js";
 const f = [];
 
 function O(e, t) {
     return {
-        subscribe: b(e, t).subscribe
+        subscribe: p(e, t).subscribe
     }
 }
 
-function b(e, t = p) {
+function p(e, t = b) {
     let n;
     const o = new Set;
 
     function a(s) {
         if (I(e, s) && (e = s, n)) {
             const u = !f.length;
             for (const l of o) l[1](), f.push(l, e);
@@ -28,17 +28,17 @@
         }
     }
 
     function i(s) {
         a(s(e))
     }
 
-    function r(s, u = p) {
+    function r(s, u = b) {
         const l = [s, u];
-        return o.add(l), o.size === 1 && (n = t(a) || p), s(e), () => {
+        return o.add(l), o.size === 1 && (n = t(a) || b), s(e), () => {
             o.delete(l), o.size === 0 && n && (n(), n = null)
         }
     }
     return {
         set: a,
         update: i,
         subscribe: r
@@ -49,37 +49,37 @@
     const o = !Array.isArray(e),
         a = o ? [e] : e,
         i = t.length < 2;
     return O(n, r => {
         let s = !1;
         const u = [];
         let l = 0,
-            _ = p;
-        const h = () => {
+            _ = b;
+        const g = () => {
                 if (l) return;
                 _();
                 const c = t(o ? u[0] : u, r);
-                i ? r(c) : _ = x(c) ? c : p
+                i ? r(c) : _ = x(c) ? c : b
             },
-            T = a.map((c, g) => R(c, w => {
-                u[g] = w, l &= ~(1 << g), s && h()
+            T = a.map((c, h) => R(c, w => {
+                u[h] = w, l &= ~(1 << h), s && g()
             }, () => {
-                l |= 1 << g
+                l |= 1 << h
             }));
-        return s = !0, h(),
+        return s = !0, g(),
             function() {
                 S(T), _(), s = !1
             }
     })
 }
 var m;
-const U = ((m = globalThis.__sveltekit_10xip82) == null ? void 0 : m.base) ?? "";
+const U = ((m = globalThis.__sveltekit_h2ilf9) == null ? void 0 : m.base) ?? "";
 var A;
-const L = ((A = globalThis.__sveltekit_10xip82) == null ? void 0 : A.assets) ?? U,
-    N = "1689074755731",
+const L = ((A = globalThis.__sveltekit_h2ilf9) == null ? void 0 : A.assets) ?? U,
+    N = "1689075048338",
     q = "sveltekit:snapshot",
     K = "sveltekit:scroll",
     $ = "sveltekit:index",
     k = {
         tap: 1,
         hover: 2,
         viewport: 3,
@@ -155,15 +155,15 @@
         noscroll: n === "off" ? !1 : n === "" ? !0 : null,
         reload: i === "off" ? !1 : i === "" ? !0 : null,
         replace_state: r === "off" ? !1 : r === "" ? !0 : null
     }
 }
 
 function y(e) {
-    const t = b(e);
+    const t = p(e);
     let n = !0;
 
     function o() {
         n = !0, t.update(r => r)
     }
 
     function a(r) {
@@ -183,15 +183,15 @@
     }
 }
 
 function P() {
     const {
         set: e,
         subscribe: t
-    } = b(!1);
+    } = p(!1);
     let n;
     async function o() {
         clearTimeout(n);
         try {
             const a = await fetch(`${L}/_app/version.json`, {
                 headers: {
                     pragma: "no-cache",
@@ -217,13 +217,13 @@
 
 function B(e) {
     e.client
 }
 const H = {
     url: y({}),
     page: y({}),
-    navigating: b(null),
+    navigating: p(null),
     updated: P()
 };
 export {
-    $ as I, k as P, K as S, q as a, G as b, X as c, C as d, U as e, D as f, z as g, B as h, V as i, j, H as s, b as w
+    $ as I, k as P, K as S, q as a, G as b, X as c, C as d, U as e, D as f, z as g, B as h, V as i, j, H as s, p as w
 };
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/entry/app.de6989fd.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/entry/app.255fb8f1.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -331,15 +331,15 @@
             components: 0,
             form: 2,
             data_0: 3,
             data_1: 4
         })
     }
 }
-const ie = [() => I(() => import("../nodes/0.a83aff18.js"), ["../nodes/0.a83aff18.js", "../chunks/index.f69b56cb.js", "../chunks/stores.9bcf7e68.js", "../chunks/singletons.97dcadd1.js", "../chunks/optionsStore.110d47c8.js", "../assets/0.4946ad59.css"], import.meta.url), () => I(() => import("../nodes/1.49f6fc19.js"), ["../nodes/1.49f6fc19.js", "../chunks/index.f69b56cb.js", "../chunks/stores.9bcf7e68.js", "../chunks/singletons.97dcadd1.js"], import.meta.url), () => I(() => import("../nodes/2.bfd77d29.js"), ["../nodes/2.bfd77d29.js", "../chunks/index.f69b56cb.js", "../chunks/singletons.97dcadd1.js", "../chunks/optionsStore.110d47c8.js", "../chunks/preload-helper.41c905a7.js", "../chunks/stores.9bcf7e68.js", "../assets/2.4d3dc64f.css"], import.meta.url)],
+const ie = [() => I(() => import("../nodes/0.2bd4934f.js"), ["../nodes/0.2bd4934f.js", "../chunks/index.f69b56cb.js", "../chunks/stores.5a8d4e4e.js", "../chunks/singletons.1f79ca33.js", "../chunks/optionsStore.5e9cf8fd.js", "../assets/0.4946ad59.css"], import.meta.url), () => I(() => import("../nodes/1.a75b771c.js"), ["../nodes/1.a75b771c.js", "../chunks/index.f69b56cb.js", "../chunks/stores.5a8d4e4e.js", "../chunks/singletons.1f79ca33.js"], import.meta.url), () => I(() => import("../nodes/2.7cf84de0.js"), ["../nodes/2.7cf84de0.js", "../chunks/index.f69b56cb.js", "../chunks/singletons.1f79ca33.js", "../chunks/optionsStore.5e9cf8fd.js", "../chunks/preload-helper.41c905a7.js", "../chunks/stores.5a8d4e4e.js", "../assets/2.4d3dc64f.css"], import.meta.url)],
     se = [],
     oe = {
         "/": [2]
     },
     re = {
         handleError: ({
             error: r
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/entry/start.b5a5435b.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/entry/start.b3231a12.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
     c as le,
     s as V,
     i as _e,
     d as Q,
     e as K,
     P as Fe,
     h as We
-} from "../chunks/singletons.97dcadd1.js";
+} from "../chunks/singletons.1f79ca33.js";
 
 function Xe(t, o) {
     return t === "/" || o === "ignore" ? t : o === "never" ? t.endsWith("/") ? t.slice(0, -1) : t : o === "always" && !t.endsWith("/") ? t + "/" : t
 }
 
 function Ze(t) {
     return t.split("%25").map(decodeURI).join("%25")
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/nodes/0.a83aff18.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/nodes/0.2bd4934f.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,20 +8,20 @@
     F as m,
     g,
     d,
     G as S
 } from "../chunks/index.f69b56cb.js";
 import {
     p as b
-} from "../chunks/stores.9bcf7e68.js";
+} from "../chunks/stores.5a8d4e4e.js";
 import {
     u as y,
     r as $,
     o as v
-} from "../chunks/optionsStore.110d47c8.js";
+} from "../chunks/optionsStore.5e9cf8fd.js";
 const O = !0,
     h = "always",
     B = Object.freeze(Object.defineProperty({
         __proto__: null,
         prerender: O,
         trailingSlash: h
     }, Symbol.toStringTag, {
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/nodes/1.49f6fc19.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/nodes/1.a75b771c.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
     H as E,
     u as $,
     I as q,
     G as y
 } from "../chunks/index.f69b56cb.js";
 import {
     p as C
-} from "../chunks/stores.9bcf7e68.js";
+} from "../chunks/stores.5a8d4e4e.js";
 
 function G(l) {
     var f;
     let a, t = l[0].status + "",
         r, o, n, p = ((f = l[0].error) == null ? void 0 : f.message) + "",
         c;
     return {
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/_app/immutable/nodes/2.bfd77d29.js` & `scaneo-2023.7.11.post3/scaneo/ui/_app/immutable/nodes/2.7cf84de0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -54,15 +54,15 @@
     $ as Hn,
     a0 as zn,
     a1 as Rn
 } from "../chunks/index.f69b56cb.js";
 import {
     j as Gn,
     w as le
-} from "../chunks/singletons.97dcadd1.js";
+} from "../chunks/singletons.1f79ca33.js";
 import {
     u as pe,
     o as oe,
     i as Un,
     a as qn,
     s as Wn,
     f as Fn,
@@ -73,21 +73,21 @@
     e as sn,
     d as ln,
     h as Qn,
     p as Xn,
     t as Yn,
     n as Kn,
     j as xn
-} from "../chunks/optionsStore.110d47c8.js";
+} from "../chunks/optionsStore.5e9cf8fd.js";
 import {
     _ as ke
 } from "../chunks/preload-helper.41c905a7.js";
 import {
     p as $n
-} from "../chunks/stores.9bcf7e68.js";
+} from "../chunks/stores.5a8d4e4e.js";
 
 function er(r, e, t, n) {
     var s, i, l = !1,
         o = t.length >= 2,
         a = (p, w) => {
             if (s = w, o && (i = p), !l) {
                 let T = e(p, w);
```

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/favicon.png` & `scaneo-2023.7.11.post3/scaneo/ui/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/icons/brush.svg` & `scaneo-2023.7.11.post3/scaneo/ui/icons/brush.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/icons/eraser.svg` & `scaneo-2023.7.11.post3/scaneo/ui/icons/eraser.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/icons/size.svg` & `scaneo-2023.7.11.post3/scaneo/ui/icons/size.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/icons/trashcan.svg` & `scaneo-2023.7.11.post3/scaneo/ui/icons/trashcan.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post2/scaneo/ui/index.html` & `scaneo-2023.7.11.post3/scaneo/ui/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 		<meta charset="utf-8" />
 		<link rel="icon" href="./favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		<meta http-equiv="content-security-policy" content="">
 		<link href="./_app/immutable/assets/0.4946ad59.css" rel="stylesheet">
 		<link href="./_app/immutable/assets/2.4d3dc64f.css" rel="stylesheet">
 		<link href="./_app/immutable/assets/PaintPolygon.4f676f7b.css" rel="stylesheet">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.b5a5435b.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/start.b3231a12.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.f69b56cb.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.97dcadd1.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.de6989fd.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.1f79ca33.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/app.255fb8f1.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/preload-helper.41c905a7.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/0.a83aff18.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/stores.9bcf7e68.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/optionsStore.110d47c8.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/2.bfd77d29.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/0.2bd4934f.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/stores.5a8d4e4e.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/optionsStore.5e9cf8fd.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/2.7cf84de0.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 
 
 <div class="toaster  svelte-1phplh9">
 </div>
 <main class="min-w-full relative min-h-full"><div class="blocker fixed opacity-40 bg-white block h-[100vh] w-[100vw]"></div>
 	</main>
 
 
 			
 			<script>
 				{
-					__sveltekit_10xip82 = {
+					__sveltekit_h2ilf9 = {
 						base: new URL(".", location).pathname.slice(0, -1),
 						env: {"PUBLIC_API_URL":""}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.b5a5435b.js"),
-						import("./_app/immutable/entry/app.de6989fd.js")
+						import("./_app/immutable/entry/start.b3231a12.js"),
+						import("./_app/immutable/entry/app.255fb8f1.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
 							node_ids: [0, 2],
 							data,
 							form: null,
 							error: null
 						});
```

### Comparing `scaneo-2023.7.11.post2/setup.py` & `scaneo-2023.7.11.post3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,28 +10,38 @@
             'ui/_app/*',
             'ui/_app/immutable/assets/*',
             'ui/_app/immutable/chunks/*',
             'ui/_app/immutable/entry/*',
             'ui/_app/immutable/nodes/*',
             'ui/icons/*']}
 
+install_requires = \
+['fastapi>=0.90.0,<0.91.0',
+ 'geopandas>=0.9.0,<0.10.0',
+ 'rasterio>=1.2.0,<2.0.0',
+ 'segment-geospatial>=0.8.4,<0.9.0',
+ 'shapely>=1.7.1,<2.0.0',
+ 'typer>=0.9.0,<0.10.0',
+ 'uvicorn>=0.22.0,<0.23.0']
+
 entry_points = \
 {'console_scripts': ['scaneo = scaneo.main:app']}
 
 setup_kwargs = {
     'name': 'scaneo',
-    'version': '2023.7.11.post2',
+    'version': '2023.7.11.post3',
     'description': '',
     'long_description': '# scan\n\nThis repo contains the code for SCAN\n\n- scaneo: includes the cli, lib and api\n- ui: includes the web ui\n\nThe CLI runs the API, which in turns servers the static files for the UI.\n\nThe library can be installed with\n\n```\npip install scaneo\n```\n\n## Instructions\n\n### Developement\n\nRun the api with the cli\n\n```\ncd scaneo\npython main.py run --reload --data <<folder>>\n```\n\nThen, run the ui\n\n```\ncd ui\nyarn dev\n```\n\n### Production\n\nBuild the ui, copy the build inside scaneo and build the python package\n\n```\nmake build v=<version>\nmake publish\n```\n\n## Notes\n\nDo not add scaneo/ui to gitignore since the build process will fail (missing entry folder)\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

