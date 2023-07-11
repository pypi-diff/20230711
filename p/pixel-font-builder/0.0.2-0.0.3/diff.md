# Comparing `tmp/pixel-font-builder-0.0.2.tar.gz` & `tmp/pixel-font-builder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.2.tar", last modified: Sat Jun  3 02:07:08 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.3.tar", last modified: Tue Jul 11 15:48:43 2023, max compression
```

## Comparing `pixel-font-builder-0.0.2.tar` & `pixel-font-builder-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:07:08.478661 pixel-font-builder-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-03 02:07:08.478661 pixel-font-builder-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 02:07:08.478661 pixel-font-builder-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:07:08.474661 pixel-font-builder-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:07:08.478661 pixel-font-builder-0.0.2/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:07:08.478661 pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-03 02:07:08.000000 pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-03 02:07:08.000000 pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 02:07:08.000000 pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 02:07:08.000000 pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 02:07:08.000000 pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:07:08.478661 pixel-font-builder-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-03 02:06:58.000000 pixel-font-builder-0.0.2/tests/test_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.376712 pixel-font-builder-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.376712 pixel-font-builder-0.0.3/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/tests/test_demo.py
```

### Comparing `pixel-font-builder-0.0.2/LICENSE` & `pixel-font-builder-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.2/PKG-INFO` & `pixel-font-builder-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
@@ -46,17 +46,17 @@
         size=12,
         ascent=10,
         descent=-2,
         x_height=5,
         cap_height=7,
     )
 
-    builder.character_mapping = {
+    builder.character_mapping.update({
         ord('A'): 'CAP_LETTER_A',
-    }
+    })
 
     builder.add_glyph(Glyph(
         name='.notdef',
         advance_width=8,
         offset=(0, -2),
         data=[
             [1, 1, 1, 1, 1, 1, 1, 1],
```

### Comparing `pixel-font-builder-0.0.2/README.md` & `pixel-font-builder-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         size=12,
         ascent=10,
         descent=-2,
         x_height=5,
         cap_height=7,
     )
 
-    builder.character_mapping = {
+    builder.character_mapping.update({
         ord('A'): 'CAP_LETTER_A',
-    }
+    })
 
     builder.add_glyph(Glyph(
         name='.notdef',
         advance_width=8,
         offset=(0, -2),
         data=[
             [1, 1, 1, 1, 1, 1, 1, 1],
```

### Comparing `pixel-font-builder-0.0.2/pyproject.toml` & `pixel-font-builder-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
@@ -15,17 +15,17 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools>=4.39.4",
+    "fonttools>=4.40.0",
     "Brotli>=1.0.9",
-    "bdffont>=0.0.12",
+    "bdffont>=0.0.13",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/pixel-font-builder"
 source = "https://github.com/TakWolf/pixel-font-builder"
 issues = "https://github.com/TakWolf/pixel-font-builder/issues"
```

### Comparing `pixel-font-builder-0.0.2/src/pixel_font_builder/bdf.py` & `pixel-font-builder-0.0.3/src/pixel_font_builder/bdf.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,22 +49,26 @@
     builder.properties.weight_name = context.meta_infos.style_name
     builder.properties.slant = xlfd.Slant.ROMAN
     builder.properties.setwidth_name = xlfd.SetwidthName.NORMAL
     if context.meta_infos.serif_mode == SerifMode.SERIF:
         builder.properties.add_style_name = xlfd.AddStyleName.SERIF
     elif context.meta_infos.serif_mode == SerifMode.SANS_SERIF:
         builder.properties.add_style_name = xlfd.AddStyleName.SANS_SERIF
+    else:
+        builder.properties.add_style_name = context.meta_infos.serif_mode
     builder.properties.pixel_size = context.size
     builder.properties.point_size = context.size * 10
     builder.properties.resolution_x = context.bdf_configs.resolution_x
     builder.properties.resolution_y = context.bdf_configs.resolution_y
     if context.meta_infos.width_mode == WidthMode.MONOSPACED:
         builder.properties.spacing = xlfd.Spacing.MONOSPACED
     elif context.meta_infos.width_mode == WidthMode.PROPORTIONAL:
         builder.properties.spacing = xlfd.Spacing.PROPORTIONAL
+    else:
+        builder.properties.spacing = context.meta_infos.width_mode
     builder.properties.average_width = round(sum([glyph.device_width_x * 10 for glyph in builder.code_point_to_glyph.values()]) / builder.get_glyphs_count())
     builder.properties.charset_registry = xlfd.CharsetRegistry.ISO10646
     builder.properties.charset_encoding = '1'
 
     builder.properties.default_char = -1
     builder.properties.font_ascent = context.ascent
     builder.properties.font_descent = context.descent
```

### Comparing `pixel-font-builder-0.0.2/src/pixel_font_builder/font.py` & `pixel-font-builder-0.0.3/src/pixel_font_builder/font.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     ):
         self.size = size
         self.ascent = ascent
         self.descent = descent
         self.x_height = x_height
         self.cap_height = cap_height
 
-        self.character_mapping: dict[int, str] = {}
-        self._name_to_glyph: dict[str, Glyph] = {}
+        self.character_mapping = dict[int, str]()
+        self._name_to_glyph = dict[str, Glyph]()
 
         self.meta_infos = MetaInfos()
         self.opentype_configs = opentype.Configs()
         self.bdf_configs = bdf.Configs()
 
     @property
     def line_height(self) -> int:
```

### Comparing `pixel-font-builder-0.0.2/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.3/src/pixel_font_builder/glyph.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             offset: tuple[int, int] = (0, 0),
             data: list[list[int]] = None,
     ):
         self.name = name
         self.advance_width = advance_width
         self.offset_x, self.offset_y = offset
         if data is None:
-            data = []
+            data = list[list[int]]()
         self.data = data
 
     @property
     def offset(self) -> tuple[int, int]:
         return self.offset_x, self.offset_y
 
     @offset.setter
```

### Comparing `pixel-font-builder-0.0.2/src/pixel_font_builder/info.py` & `pixel-font-builder-0.0.3/src/pixel_font_builder/info.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.2/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.3/src/pixel_font_builder/opentype.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     if context.meta_infos.license_info is not None:
         name_strings['licenseDescription'] = context.meta_infos.license_info
     if context.meta_infos.license_url is not None:
         name_strings['licenseInfoURL'] = context.meta_infos.license_url
     return name_strings
 
 
-def _get_outlines(glyph_data, px_to_units) -> list[list[tuple[int, int]]]:
+def _get_outlines(glyph_data: list[list[int]], px_to_units: int) -> list[list[tuple[int, int]]]:
     """
     将字形数据转换为轮廓数据，左上角原点坐标系
     """
     # 相邻像素分组
     point_group_list = []
     for y, glyph_data_row in enumerate(glyph_data):
         for x, alpha in enumerate(glyph_data_row):
@@ -168,15 +168,15 @@
 
 def _create_glyph(context: 'font.FontBuilder', glyph_name: str, is_ttf: bool) -> T2CharString | Glyph:
     glyph = context.get_glyph(glyph_name)
     outlines = _get_outlines(glyph.data, context.opentype_configs.px_to_units)
     if is_ttf:
         pen = TTGlyphPen()
     else:
-        pen = T2CharStringPen(0, None)
+        pen = T2CharStringPen(glyph.advance_width * context.opentype_configs.px_to_units, None)
     if len(outlines) > 0:
         for outline_index, outline in enumerate(outlines):
             for point_index, point in enumerate(outline):
 
                 # 转换左上角原点坐标系为左下角原点坐标系
                 x, y = point
                 x += glyph.offset_x * context.opentype_configs.px_to_units
```

### Comparing `pixel-font-builder-0.0.2/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
@@ -46,17 +46,17 @@
         size=12,
         ascent=10,
         descent=-2,
         x_height=5,
         cap_height=7,
     )
 
-    builder.character_mapping = {
+    builder.character_mapping.update({
         ord('A'): 'CAP_LETTER_A',
-    }
+    })
 
     builder.add_glyph(Glyph(
         name='.notdef',
         advance_width=8,
         offset=(0, -2),
         data=[
             [1, 1, 1, 1, 1, 1, 1, 1],
```

