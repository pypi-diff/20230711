# Comparing `tmp/scaneo-2023.7.11.post4.tar.gz` & `tmp/scaneo-2023.7.11.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaneo-2023.7.11.post4.tar", max compression
+gzip compressed data, was "scaneo-2023.7.11.post5.tar", max compression
```

## Comparing `scaneo-2023.7.11.post4.tar` & `scaneo-2023.7.11.post5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      654 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post4/README.md
--rw-r--r--   0        0        0      521 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/__init__.py
--rw-r--r--   0        0        0      872 2023-06-13 12:37:28.547552 scaneo-2023.7.11.post4/scaneo/api.py
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/cli/__init__.py
--rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/cli/hello.py
--rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/main.py
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/routers/__init__.py
--rw-r--r--   0        0        0     1592 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post4/scaneo/routers/geojson.py
--rw-r--r--   0        0        0      104 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post4/scaneo/routers/image/__init__.py
--rw-r--r--   0        0        0     2026 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post4/scaneo/routers/image/cache.py
--rw-r--r--   0        0        0      575 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post4/scaneo/routers/image/errors.py
--rw-r--r--   0        0        0     6902 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post4/scaneo/routers/image/get_image_tile.py
--rw-r--r--   0        0        0     1919 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post4/scaneo/routers/image/image_utils.py
--rw-r--r--   0        0        0     1720 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post4/scaneo/routers/images.py
--rw-r--r--   0        0        0     1085 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post4/scaneo/routers/labels.py
--rw-r--r--   0        0        0     3365 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post4/scaneo/routers/sam.py
--rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/routers/settings.py
--rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post4/scaneo/routers/test.py
--rw-r--r--   0        0        0    62672 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/0.4946ad59.css
--rw-r--r--   0        0        0    32380 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css
--rw-r--r--   0        0        0    13943 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css
--rw-r--r--   0        0        0    62640 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css
--rw-r--r--   0        0        0    32422 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css
--rw-r--r--   0        0        0     5551 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg
--rw-r--r--   0        0        0    38018 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js
--rw-r--r--   0        0        0     9160 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js
--rw-r--r--   0        0        0   150162 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js
--rw-r--r--   0        0        0     6990 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js
--rw-r--r--   0        0        0    67243 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js
--rw-r--r--   0        0        0     1783 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/optionsStore.29d4ac2e.js
--rw-r--r--   0        0        0      759 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js
--rw-r--r--   0        0        0     3216 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/singletons.f47525d1.js
--rw-r--r--   0        0        0      238 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/stores.e482a1d3.js
--rw-r--r--   0        0        0     5139 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/entry/app.2abeadab.js
--rw-r--r--   0        0        0    23876 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/entry/start.832840b0.js
--rw-r--r--   0        0        0      953 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/nodes/0.ee612e16.js
--rw-r--r--   0        0        0      800 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/nodes/1.9e3a48a9.js
--rw-r--r--   0        0        0    75539 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/nodes/2.98ac24a9.js
--rw-r--r--   0        0        0       27 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/_app/version.json
--rw-r--r--   0        0        0     1571 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/favicon.png
--rw-r--r--   0        0        0     1174 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/icons/brush.svg
--rw-r--r--   0        0        0     2789 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/icons/eraser.svg
--rw-r--r--   0        0        0      826 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/icons/size.svg
--rw-r--r--   0        0        0      895 2023-07-11 11:32:46.510636 scaneo-2023.7.11.post4/scaneo/ui/icons/trashcan.svg
--rw-r--r--   0        0        0     2031 2023-07-11 11:32:46.506636 scaneo-2023.7.11.post4/scaneo/ui/index.html
--rw-r--r--   0        0        0       86 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post4/scaneo/yarn.lock
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post4/setup.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post4/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post5/README.md
+-rw-r--r--   0        0        0      543 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/__init__.py
+-rw-r--r--   0        0        0      872 2023-06-13 12:37:28.547552 scaneo-2023.7.11.post5/scaneo/api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/cli/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/cli/hello.py
+-rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/main.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/routers/__init__.py
+-rw-r--r--   0        0        0     1592 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post5/scaneo/routers/geojson.py
+-rw-r--r--   0        0        0      104 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post5/scaneo/routers/image/__init__.py
+-rw-r--r--   0        0        0     2026 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post5/scaneo/routers/image/cache.py
+-rw-r--r--   0        0        0      575 2023-06-12 09:10:31.455437 scaneo-2023.7.11.post5/scaneo/routers/image/errors.py
+-rw-r--r--   0        0        0     6902 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post5/scaneo/routers/image/get_image_tile.py
+-rw-r--r--   0        0        0     1919 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post5/scaneo/routers/image/image_utils.py
+-rw-r--r--   0        0        0     1720 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post5/scaneo/routers/images.py
+-rw-r--r--   0        0        0     1085 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post5/scaneo/routers/labels.py
+-rw-r--r--   0        0        0     3365 2023-07-11 10:58:17.063761 scaneo-2023.7.11.post5/scaneo/routers/sam.py
+-rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/routers/settings.py
+-rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.7.11.post5/scaneo/routers/test.py
+-rw-r--r--   0        0        0    62672 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/0.4946ad59.css
+-rw-r--r--   0        0        0    32380 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css
+-rw-r--r--   0        0        0    13943 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css
+-rw-r--r--   0        0        0    62640 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css
+-rw-r--r--   0        0        0    32422 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css
+-rw-r--r--   0        0        0     5551 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg
+-rw-r--r--   0        0        0    38018 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js
+-rw-r--r--   0        0        0     9160 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js
+-rw-r--r--   0        0        0   150162 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js
+-rw-r--r--   0        0        0     6990 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js
+-rw-r--r--   0        0        0    67243 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js
+-rw-r--r--   0        0        0     1783 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/optionsStore.00b5d1d1.js
+-rw-r--r--   0        0        0      759 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js
+-rw-r--r--   0        0        0     3211 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/singletons.45ed74e4.js
+-rw-r--r--   0        0        0      238 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/stores.9f0917f5.js
+-rw-r--r--   0        0        0     5139 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/entry/app.fd7c7338.js
+-rw-r--r--   0        0        0    23876 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/entry/start.38ee7516.js
+-rw-r--r--   0        0        0      953 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/nodes/0.34c0d7da.js
+-rw-r--r--   0        0        0      800 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/nodes/1.bbf394d7.js
+-rw-r--r--   0        0        0    75539 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/nodes/2.5ed722c0.js
+-rw-r--r--   0        0        0       27 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/_app/version.json
+-rw-r--r--   0        0        0     1571 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/favicon.png
+-rw-r--r--   0        0        0     1174 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/icons/brush.svg
+-rw-r--r--   0        0        0     2789 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/icons/eraser.svg
+-rw-r--r--   0        0        0      826 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/icons/size.svg
+-rw-r--r--   0        0        0      895 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/icons/trashcan.svg
+-rw-r--r--   0        0        0     2031 2023-07-11 11:33:31.674782 scaneo-2023.7.11.post5/scaneo/ui/index.html
+-rw-r--r--   0        0        0       86 2023-06-19 09:56:08.942226 scaneo-2023.7.11.post5/scaneo/yarn.lock
+-rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post5/setup.py
+-rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 scaneo-2023.7.11.post5/PKG-INFO
```

### Comparing `scaneo-2023.7.11.post4/README.md` & `scaneo-2023.7.11.post5/README.md`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/pyproject.toml` & `scaneo-2023.7.11.post5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaneo"
-version = "2023.07.11-4"
+version = "2023.07.11-5"
 description = ""
 authors = ["Juan Sensio <it@earthpulse.es>"]
 readme = "README.md"
 packages = [{include = "scaneo"}]
 
 [tool.poetry.scripts]
 scaneo = "scaneo.main:app"
@@ -14,13 +14,14 @@
 typer = "^0.9.0"
 fastapi = "^0.90.0"
 uvicorn = "^0.22.0"
 geopandas = "^0.9.0"
 rasterio = "^1.2.0"
 shapely = "^1.7.1"
 mercantile = "^1.2.1"
+cachetools = "^5.3.1"
 segment-geospatial = "^0.8.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scaneo-2023.7.11.post4/scaneo/api.py` & `scaneo-2023.7.11.post5/scaneo/api.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/main.py` & `scaneo-2023.7.11.post5/scaneo/main.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/geojson.py` & `scaneo-2023.7.11.post5/scaneo/routers/geojson.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/image/cache.py` & `scaneo-2023.7.11.post5/scaneo/routers/image/cache.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/image/errors.py` & `scaneo-2023.7.11.post5/scaneo/routers/image/errors.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/image/get_image_tile.py` & `scaneo-2023.7.11.post5/scaneo/routers/image/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/image/image_utils.py` & `scaneo-2023.7.11.post5/scaneo/routers/image/image_utils.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/images.py` & `scaneo-2023.7.11.post5/scaneo/routers/images.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/labels.py` & `scaneo-2023.7.11.post5/scaneo/routers/labels.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/routers/sam.py` & `scaneo-2023.7.11.post5/scaneo/routers/sam.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/0.4946ad59.css` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/0.4946ad59.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/2.4d3dc64f.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/PaintPolygon.4f676f7b.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/_layout.c3f60e6b.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/_page.0f0b252f.css`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/PaintPolygon.9a9c653d.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/index.f69b56cb.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/leaflet-src.e35a4304.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/leaflet.activearea.bef5e9d0.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/optionsStore.29d4ac2e.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/optionsStore.00b5d1d1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     w as l
-} from "./singletons.f47525d1.js";
+} from "./singletons.45ed74e4.js";
 import {
     J as o
 } from "./index.f69b56cb.js";
 const c = {
     defaultUrl: "http://localhost:8000",
     labelsEndpoint: "/labels",
     geojsonEndpoint: "/geojson/",
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/chunks/singletons.f47525d1.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/chunks/singletons.45ed74e4.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -41,57 +41,57 @@
     return {
         set: a,
         update: i,
         subscribe: r
     }
 }
 
-function Y(e, t, n) {
+function j(e, t, n) {
     const o = !Array.isArray(e),
         a = o ? [e] : e,
         i = t.length < 2;
     return O(n, r => {
         let s = !1;
         const u = [];
         let l = 0,
             _ = b;
-        const g = () => {
+        const h = () => {
                 if (l) return;
                 _();
                 const c = t(o ? u[0] : u, r);
                 i ? r(c) : _ = x(c) ? c : b
             },
-            T = a.map((c, h) => R(c, w => {
-                u[h] = w, l &= ~(1 << h), s && g()
+            E = a.map((c, g) => R(c, T => {
+                u[g] = T, l &= ~(1 << g), s && h()
             }, () => {
-                l |= 1 << h
+                l |= 1 << g
             }));
-        return s = !0, g(),
+        return s = !0, h(),
             function() {
-                S(T), _(), s = !1
+                S(E), _(), s = !1
             }
     })
 }
 var m;
-const U = ((m = globalThis.__sveltekit_nzehox) == null ? void 0 : m.base) ?? "";
-var A;
-const L = ((A = globalThis.__sveltekit_nzehox) == null ? void 0 : A.assets) ?? U,
-    N = "1689075162476",
-    j = "sveltekit:snapshot",
-    q = "sveltekit:scroll",
-    K = "sveltekit:index",
+const U = ((m = globalThis.__sveltekit_twrd4l) == null ? void 0 : m.base) ?? "";
+var w;
+const L = ((w = globalThis.__sveltekit_twrd4l) == null ? void 0 : w.assets) ?? U,
+    N = "1689075207661",
+    q = "sveltekit:snapshot",
+    K = "sveltekit:scroll",
+    $ = "sveltekit:index",
     k = {
         tap: 1,
         hover: 2,
         viewport: 3,
         eager: 4,
         off: -1
     };
 
-function $(e) {
+function z(e) {
     let t = e.baseURI;
     if (!t) {
         const n = e.getElementsByTagName("base");
         t = n.length ? n[0].href : e.URL
     }
     return t
 }
@@ -107,33 +107,33 @@
     return e.getAttribute(`data-sveltekit-${t}`)
 }
 const v = {
     ...k,
     "": k.hover
 };
 
-function E(e) {
+function A(e) {
     let t = e.assignedSlot ?? e.parentNode;
     return (t == null ? void 0 : t.nodeType) === 11 && (t = t.host), t
 }
 
 function D(e, t) {
     for (; e && e !== t;) {
         if (e.nodeName.toUpperCase() === "A" && e.hasAttribute("href")) return e;
-        e = E(e)
+        e = A(e)
     }
 }
 
 function G(e, t) {
     let n;
     try {
         n = new URL(e instanceof SVGAElement ? e.href.baseVal : e.href, document.baseURI)
     } catch {}
     const o = e instanceof SVGAElement ? e.target.baseVal : e.target,
-        a = !n || !!o || P(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
+        a = !n || !!o || V(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
         i = (n == null ? void 0 : n.origin) === location.origin && e.hasAttribute("download");
     return {
         url: n,
         external: a,
         target: o,
         download: i
     }
@@ -143,15 +143,15 @@
     let t = null,
         n = null,
         o = null,
         a = null,
         i = null,
         r = null,
         s = e;
-    for (; s && s !== document.documentElement;) o === null && (o = d(s, "preload-code")), a === null && (a = d(s, "preload-data")), t === null && (t = d(s, "keepfocus")), n === null && (n = d(s, "noscroll")), i === null && (i = d(s, "reload")), r === null && (r = d(s, "replacestate")), s = E(s);
+    for (; s && s !== document.documentElement;) o === null && (o = d(s, "preload-code")), a === null && (a = d(s, "preload-data")), t === null && (t = d(s, "keepfocus")), n === null && (n = d(s, "noscroll")), i === null && (i = d(s, "reload")), r === null && (r = d(s, "replacestate")), s = A(s);
     return {
         preload_code: v[o ?? "off"],
         preload_data: v[a ?? "off"],
         keep_focus: t === "off" ? !1 : t === "" ? !0 : null,
         noscroll: n === "off" ? !1 : n === "" ? !0 : null,
         reload: i === "off" ? !1 : i === "" ? !0 : null,
         replace_state: r === "off" ? !1 : r === "" ? !0 : null
@@ -179,15 +179,15 @@
     return {
         notify: o,
         set: a,
         subscribe: i
     }
 }
 
-function z() {
+function P() {
     const {
         set: e,
         subscribe: t
     } = p(!1);
     let n;
     async function o() {
         clearTimeout(n);
@@ -207,23 +207,23 @@
     }
     return {
         subscribe: t,
         check: o
     }
 }
 
-function P(e, t) {
+function V(e, t) {
     return e.origin !== location.origin || !e.pathname.startsWith(t)
 }
 
 function B(e) {
     e.client
 }
 const H = {
     url: y({}),
     page: y({}),
     navigating: p(null),
-    updated: z()
+    updated: P()
 };
 export {
-    K as I, k as P, q as S, j as a, G as b, X as c, C as d, U as e, D as f, $ as g, B as h, P as i, Y as j, H as s, p as w
+    $ as I, k as P, K as S, q as a, G as b, X as c, C as d, U as e, D as f, z as g, B as h, V as i, j, H as s, p as w
 };
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/entry/app.2abeadab.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/entry/app.fd7c7338.js`

 * *Files 5% similar despite different names*

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
-const ie = [() => I(() => import("../nodes/0.ee612e16.js"), ["../nodes/0.ee612e16.js", "../chunks/index.f69b56cb.js", "../chunks/stores.e482a1d3.js", "../chunks/singletons.f47525d1.js", "../chunks/optionsStore.29d4ac2e.js", "../assets/0.4946ad59.css"], import.meta.url), () => I(() => import("../nodes/1.9e3a48a9.js"), ["../nodes/1.9e3a48a9.js", "../chunks/index.f69b56cb.js", "../chunks/stores.e482a1d3.js", "../chunks/singletons.f47525d1.js"], import.meta.url), () => I(() => import("../nodes/2.98ac24a9.js"), ["../nodes/2.98ac24a9.js", "../chunks/index.f69b56cb.js", "../chunks/singletons.f47525d1.js", "../chunks/optionsStore.29d4ac2e.js", "../chunks/preload-helper.41c905a7.js", "../chunks/stores.e482a1d3.js", "../assets/2.4d3dc64f.css"], import.meta.url)],
+const ie = [() => I(() => import("../nodes/0.34c0d7da.js"), ["../nodes/0.34c0d7da.js", "../chunks/index.f69b56cb.js", "../chunks/stores.9f0917f5.js", "../chunks/singletons.45ed74e4.js", "../chunks/optionsStore.00b5d1d1.js", "../assets/0.4946ad59.css"], import.meta.url), () => I(() => import("../nodes/1.bbf394d7.js"), ["../nodes/1.bbf394d7.js", "../chunks/index.f69b56cb.js", "../chunks/stores.9f0917f5.js", "../chunks/singletons.45ed74e4.js"], import.meta.url), () => I(() => import("../nodes/2.5ed722c0.js"), ["../nodes/2.5ed722c0.js", "../chunks/index.f69b56cb.js", "../chunks/singletons.45ed74e4.js", "../chunks/optionsStore.00b5d1d1.js", "../chunks/preload-helper.41c905a7.js", "../chunks/stores.9f0917f5.js", "../assets/2.4d3dc64f.css"], import.meta.url)],
     se = [],
     oe = {
         "/": [2]
     },
     re = {
         handleError: ({
             error: r
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/entry/start.832840b0.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/entry/start.38ee7516.js`

 * *Files 0% similar despite different names*

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
-} from "../chunks/singletons.f47525d1.js";
+} from "../chunks/singletons.45ed74e4.js";
 
 function Xe(t, o) {
     return t === "/" || o === "ignore" ? t : o === "never" ? t.endsWith("/") ? t.slice(0, -1) : t : o === "always" && !t.endsWith("/") ? t + "/" : t
 }
 
 function Ze(t) {
     return t.split("%25").map(decodeURI).join("%25")
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/nodes/0.ee612e16.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/nodes/0.34c0d7da.js`

 * *Files 5% similar despite different names*

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
-} from "../chunks/stores.e482a1d3.js";
+} from "../chunks/stores.9f0917f5.js";
 import {
     u as y,
     r as $,
     o as v
-} from "../chunks/optionsStore.29d4ac2e.js";
+} from "../chunks/optionsStore.00b5d1d1.js";
 const O = !0,
     h = "always",
     B = Object.freeze(Object.defineProperty({
         __proto__: null,
         prerender: O,
         trailingSlash: h
     }, Symbol.toStringTag, {
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/nodes/1.9e3a48a9.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/nodes/1.bbf394d7.js`

 * *Files 3% similar despite different names*

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
-} from "../chunks/stores.e482a1d3.js";
+} from "../chunks/stores.9f0917f5.js";
 
 function G(l) {
     var f;
     let a, t = l[0].status + "",
         r, o, n, p = ((f = l[0].error) == null ? void 0 : f.message) + "",
         c;
     return {
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/_app/immutable/nodes/2.98ac24a9.js` & `scaneo-2023.7.11.post5/scaneo/ui/_app/immutable/nodes/2.5ed722c0.js`

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
-} from "../chunks/singletons.f47525d1.js";
+} from "../chunks/singletons.45ed74e4.js";
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
-} from "../chunks/optionsStore.29d4ac2e.js";
+} from "../chunks/optionsStore.00b5d1d1.js";
 import {
     _ as ke
 } from "../chunks/preload-helper.41c905a7.js";
 import {
     p as $n
-} from "../chunks/stores.e482a1d3.js";
+} from "../chunks/stores.9f0917f5.js";
 
 function er(r, e, t, n) {
     var s, i, l = !1,
         o = t.length >= 2,
         a = (p, w) => {
             if (s = w, o && (i = p), !l) {
                 let T = e(p, w);
```

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/favicon.png` & `scaneo-2023.7.11.post5/scaneo/ui/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/icons/brush.svg` & `scaneo-2023.7.11.post5/scaneo/ui/icons/brush.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/icons/eraser.svg` & `scaneo-2023.7.11.post5/scaneo/ui/icons/eraser.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/icons/size.svg` & `scaneo-2023.7.11.post5/scaneo/ui/icons/size.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/icons/trashcan.svg` & `scaneo-2023.7.11.post5/scaneo/ui/icons/trashcan.svg`

 * *Files identical despite different names*

### Comparing `scaneo-2023.7.11.post4/scaneo/ui/index.html` & `scaneo-2023.7.11.post5/scaneo/ui/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 		<meta charset="utf-8" />
 		<link rel="icon" href="./favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		<meta http-equiv="content-security-policy" content="">
 		<link href="./_app/immutable/assets/0.4946ad59.css" rel="stylesheet">
 		<link href="./_app/immutable/assets/2.4d3dc64f.css" rel="stylesheet">
 		<link href="./_app/immutable/assets/PaintPolygon.4f676f7b.css" rel="stylesheet">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.832840b0.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/start.38ee7516.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.f69b56cb.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.f47525d1.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.2abeadab.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.45ed74e4.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/app.fd7c7338.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/preload-helper.41c905a7.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/0.ee612e16.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/stores.e482a1d3.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/optionsStore.29d4ac2e.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/2.98ac24a9.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/0.34c0d7da.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/stores.9f0917f5.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/optionsStore.00b5d1d1.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/2.5ed722c0.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 
 
 <div class="toaster  svelte-1phplh9">
 </div>
 <main class="min-w-full relative min-h-full"><div class="blocker fixed opacity-40 bg-white block h-[100vh] w-[100vw]"></div>
 	</main>
 
 
 			
 			<script>
 				{
-					__sveltekit_nzehox = {
+					__sveltekit_twrd4l = {
 						base: new URL(".", location).pathname.slice(0, -1),
 						env: {"PUBLIC_API_URL":""}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.832840b0.js"),
-						import("./_app/immutable/entry/app.2abeadab.js")
+						import("./_app/immutable/entry/start.38ee7516.js"),
+						import("./_app/immutable/entry/app.fd7c7338.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
 							node_ids: [0, 2],
 							data,
 							form: null,
 							error: null
 						});
```

### Comparing `scaneo-2023.7.11.post4/setup.py` & `scaneo-2023.7.11.post5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,30 @@
             'ui/_app/immutable/assets/*',
             'ui/_app/immutable/chunks/*',
             'ui/_app/immutable/entry/*',
             'ui/_app/immutable/nodes/*',
             'ui/icons/*']}
 
 install_requires = \
-['fastapi>=0.90.0,<0.91.0',
+['cachetools>=5.3.1,<6.0.0',
+ 'fastapi>=0.90.0,<0.91.0',
  'geopandas>=0.9.0,<0.10.0',
  'mercantile>=1.2.1,<2.0.0',
  'rasterio>=1.2.0,<2.0.0',
  'segment-geospatial>=0.8.4,<0.9.0',
  'shapely>=1.7.1,<2.0.0',
  'typer>=0.9.0,<0.10.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 entry_points = \
 {'console_scripts': ['scaneo = scaneo.main:app']}
 
 setup_kwargs = {
     'name': 'scaneo',
-    'version': '2023.7.11.post4',
+    'version': '2023.7.11.post5',
     'description': '',
     'long_description': '# scan\n\nThis repo contains the code for SCAN\n\n- scaneo: includes the cli, lib and api\n- ui: includes the web ui\n\nThe CLI runs the API, which in turns servers the static files for the UI.\n\nThe library can be installed with\n\n```\npip install scaneo\n```\n\n## Instructions\n\n### Developement\n\nRun the api with the cli\n\n```\ncd scaneo\npython main.py run --reload --data <<folder>>\n```\n\nThen, run the ui\n\n```\ncd ui\nyarn dev\n```\n\n### Production\n\nBuild the ui, copy the build inside scaneo and build the python package\n\n```\nmake build v=<version>\nmake publish\n```\n\n## Notes\n\nDo not add scaneo/ui to gitignore since the build process will fail (missing entry folder)\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scaneo-2023.7.11.post4/PKG-INFO` & `scaneo-2023.7.11.post5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: scaneo
-Version: 2023.7.11.post4
+Version: 2023.7.11.post5
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: fastapi (>=0.90.0,<0.91.0)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: mercantile (>=1.2.1,<2.0.0)
 Requires-Dist: rasterio (>=1.2.0,<2.0.0)
 Requires-Dist: segment-geospatial (>=0.8.4,<0.9.0)
 Requires-Dist: shapely (>=1.7.1,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

