# Comparing `tmp/EOmaps-6.5.tar.gz` & `tmp/EOmaps-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EOmaps-6.5.tar", last modified: Fri May 19 22:13:11 2023, max compression
+gzip compressed data, was "dist/EOmaps-7.0.tar", last modified: Tue Jul 11 21:03:15 2023, max compression
```

## Comparing `EOmaps-6.5.tar` & `EOmaps-7.0.tar`

### file list

```diff
@@ -1,76 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 22:13:01.000000 EOmaps-6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-19 22:13:11.000000 EOmaps-6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-19 22:13:01.000000 EOmaps-6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_cb_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27548 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    62949 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46463 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    47507 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)   182461 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    82477 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20422 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_top_active.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    47565 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/wms.py
--rw-r--r--   0 runner    (1001) docker     (123)    52347 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:13:11.000000 EOmaps-6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-19 22:13:01.000000 EOmaps-6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 21:03:15.000000 EOmaps-7.0/EOmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 21:03:01.000000 EOmaps-7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-11 21:03:15.000000 EOmaps-7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-11 21:03:01.000000 EOmaps-7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/annotation_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45029 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72250 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49597 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28612 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)   191414 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34539 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96938 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/inset_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20964 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/edit_layout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/edit_layout_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/edit_layout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/info_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/info_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/layers_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/open_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/peek_top_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/icons/plus_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/signal_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55157 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51396 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55191 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/scalebar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:15.000000 EOmaps-7.0/eomaps/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/scripts/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62414 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20710 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82049 2023-07-11 21:03:02.000000 EOmaps-7.0/eomaps/webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:03:15.000000 EOmaps-7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-11 21:03:02.000000 EOmaps-7.0/setup.py
```

### Comparing `EOmaps-6.5/EOmaps.egg-info/SOURCES.txt` & `EOmaps-7.0/EOmaps.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 LICENSE
 README.md
 setup.py
 EOmaps.egg-info/PKG-INFO
 EOmaps.egg-info/SOURCES.txt
 EOmaps.egg-info/dependency_links.txt
+EOmaps.egg-info/entry_points.txt
 EOmaps.egg-info/requires.txt
 EOmaps.egg-info/top_level.txt
 eomaps/NE_features.json
 eomaps/__init__.py
-eomaps/_cb_container.py
 eomaps/_containers.py
 eomaps/_data_manager.py
-eomaps/_shapes.py
 eomaps/_version.py
 eomaps/_webmap.py
-eomaps/_webmap_containers.py
+eomaps/annotation_editor.py
 eomaps/callbacks.py
+eomaps/cb_container.py
 eomaps/colorbar.py
 eomaps/compass.py
 eomaps/draw.py
 eomaps/eomaps.py
 eomaps/grid.py
 eomaps/helpers.py
+eomaps/inset_maps.py
 eomaps/logo.png
 eomaps/mapsgrid.py
 eomaps/ne_features.py
 eomaps/projections.py
 eomaps/reader.py
 eomaps/scalebar.py
+eomaps/shapes.py
 eomaps/utilities.py
+eomaps/webmap_containers.py
 eomaps/qtcompanion/__init__.py
 eomaps/qtcompanion/app.py
 eomaps/qtcompanion/base.py
 eomaps/qtcompanion/common.py
+eomaps/qtcompanion/signal_container.py
 eomaps/qtcompanion/icons/close.png
+eomaps/qtcompanion/icons/edit_layout.png
+eomaps/qtcompanion/icons/edit_layout_active.png
+eomaps/qtcompanion/icons/edit_layout_hover.png
 eomaps/qtcompanion/icons/eye_closed.png
 eomaps/qtcompanion/icons/eye_open.png
+eomaps/qtcompanion/icons/info.png
+eomaps/qtcompanion/icons/info_checked.png
+eomaps/qtcompanion/icons/info_hoover.png
+eomaps/qtcompanion/icons/layers.png
+eomaps/qtcompanion/icons/layers_hover.png
 eomaps/qtcompanion/icons/logo.png
 eomaps/qtcompanion/icons/maximize.png
+eomaps/qtcompanion/icons/open.png
+eomaps/qtcompanion/icons/open_hover.png
 eomaps/qtcompanion/icons/peek_bottom.png
 eomaps/qtcompanion/icons/peek_bottom_active.png
 eomaps/qtcompanion/icons/peek_circle.png
 eomaps/qtcompanion/icons/peek_circle_active.png
 eomaps/qtcompanion/icons/peek_ellipse.png
 eomaps/qtcompanion/icons/peek_ellipse_active.png
 eomaps/qtcompanion/icons/peek_left.png
@@ -50,19 +64,23 @@
 eomaps/qtcompanion/icons/peek_rectangle_active.png
 eomaps/qtcompanion/icons/peek_right.png
 eomaps/qtcompanion/icons/peek_right_active.png
 eomaps/qtcompanion/icons/peek_square.png
 eomaps/qtcompanion/icons/peek_square_active.png
 eomaps/qtcompanion/icons/peek_top.png
 eomaps/qtcompanion/icons/peek_top_active.png
+eomaps/qtcompanion/icons/plus.png
+eomaps/qtcompanion/icons/plus_hoover.png
 eomaps/qtcompanion/widgets/__init__.py
 eomaps/qtcompanion/widgets/annotate.py
 eomaps/qtcompanion/widgets/click_callbacks.py
 eomaps/qtcompanion/widgets/draw.py
 eomaps/qtcompanion/widgets/editor.py
 eomaps/qtcompanion/widgets/extent.py
 eomaps/qtcompanion/widgets/files.py
 eomaps/qtcompanion/widgets/layer.py
 eomaps/qtcompanion/widgets/peek.py
 eomaps/qtcompanion/widgets/save.py
 eomaps/qtcompanion/widgets/utils.py
-eomaps/qtcompanion/widgets/wms.py
+eomaps/qtcompanion/widgets/wms.py
+eomaps/scripts/__init__.py
+eomaps/scripts/open.py
```

### Comparing `EOmaps-6.5/LICENSE` & `EOmaps-7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/NE_features.json` & `EOmaps-7.0/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/_cb_container.py` & `EOmaps-7.0/eomaps/cb_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-from eomaps.callbacks import (
-    click_callbacks,
-    pick_callbacks,
-    keypress_callbacks,
-    move_callbacks,
-)
-from types import SimpleNamespace
+"""Container classes for callback management"""
 
+import logging
+from types import SimpleNamespace
 from functools import update_wrapper, partial, wraps
-import matplotlib.pyplot as plt
+from itertools import chain
 
-from pyproj import Transformer
+from .callbacks import (
+    ClickCallbacks,
+    PickCallbacks,
+    KeypressCallbacks,
+    MoveCallbacks,
+)
+from .helpers import register_modules
 
+import matplotlib.pyplot as plt
+from pyproj import Transformer
 import numpy as np
 
-gpd = None
-
+_log = logging.getLogger(__name__)
 
-def _register_geopandas():
-    global gpd
-    try:
-        import geopandas as gpd
-    except ImportError:
-        return False
 
-    return True
+class GeoDataFramePicker:
+    """Collection of pick-methods for geopandas.GeoDataFrames"""
 
-
-class _gpd_picker:
-    # a collection of pick-methods for geopandas.GeoDataFrames
     def __init__(self, gdf, val_key, pick_method):
         self.gdf = gdf
         self.val_key = val_key
         self.pick_method = pick_method
 
     def get_picker(self):
-        assert _register_geopandas(), (
-            "EOmaps: Missing dependency `geopandas`!\n"
-            + "please install '(conda install -c conda-forge geopandas)'"
-            + "to make geopandas GeoDataFrames pickable."
-        )
-
+        (gpd,) = register_modules("geopandas")
         if self.pick_method == "contains":
             return self._contains_picker
         elif self.pick_method == "centroids":
             from scipy.spatial import cKDTree
 
             self.tree = cKDTree(
                 list(map(lambda x: (x.x, x.y), self.gdf.geometry.centroid))
@@ -51,14 +41,16 @@
             return self._centroids_picker
         else:
             raise TypeError(
                 f"EOmaps: {self.pick_method} is not a valid " "pick_method!"
             )
 
     def _contains_picker(self, artist, mouseevent):
+        (gpd,) = register_modules("geopandas")
+
         try:
             query = getattr(self.gdf, "contains")(
                 gpd.points_from_xy(
                     np.atleast_1d(mouseevent.xdata),
                     np.atleast_1d(mouseevent.ydata),
                 )[0]
             )
@@ -111,36 +103,39 @@
 
             return True, dict(ID=ID, pos=pos, val=val, ind=ind, val_color=val_color)
 
         except Exception:
             return False, dict()
 
 
-class _cb_container(object):
+class _CallbackContainer(object):
     """Base-class for callback containers."""
 
-    def __init__(self, m, cb_class=None, method="click", tmp_artists=None):
+    def __init__(self, m, cb_class=None, method="click", parent_container=None):
         self._m = m
+        self._parent_container = parent_container
 
-        if tmp_artists is None:
+        if self._parent_container is None:
             self._temporary_artists = []
         else:
-            self._temporary_artists = tmp_artists
+            self._temporary_artists = self._parent_container._temporary_artists
 
         self._cb = cb_class(m, self._temporary_artists)
         self._cb_list = cb_class._cb_list
 
         self.attach = self._attach(self)
         self.get = self._get(self)
 
         self._fwd_cbs = dict()
 
         self._method = method
         self._event = None
 
+        self._execute_on_all_layers = False
+
     def _getobj(self, m):
         """Get the equivalent callback container on another maps object."""
         return getattr(m.cb, self._method, None)
 
     @property
     def _objs(self):
         """Get the callback-container objects associated with the event-axes."""
@@ -149,24 +144,33 @@
         objs = []
         if self._event is not None:
             if hasattr(self._event, "mouseevent"):
                 event = self._event.mouseevent
             else:
                 event = self._event
 
+            # make sure that "all" layer callbacks are executed before other callbacks
+            ms, malls = [], []
+            for m in reversed((*self._m.parent._children, self._m.parent)):
+                if m.layer == "all":
+                    malls.append(m)
+                else:
+                    ms.append(m)
+            ms = ms + malls
+
             if self._method in ["keypress"]:
-                for m in [*self._m.parent._children, self._m.parent]:
+                for m in ms:
                     # always execute keypress callbacks irrespective of the mouse-pos
                     obj = self._getobj(m)
 
                     # only include objects that are on the same layer
                     if obj is not None and self._execute_cb(obj._m.layer):
                         objs.append(obj)
             else:
-                for m in [*self._m.parent._children, self._m.parent]:
+                for m in ms:
                     # don't use "is" in here since Maps-children are proxies
                     # (and so are their attributes)!
                     if event.inaxes == m.ax:
                         obj = self._getobj(m)
                         # only include objects that are on the same layer
                         if obj is not None and self._execute_cb(obj._m.layer):
                             objs.append(obj)
@@ -236,14 +240,22 @@
         layer : str or None, optional
             The layer to put the artist on.
             If None, the layer of the used Maps-object is used. (e.g. `m.layer`)
         """
         if layer is None:
             layer = self._m.layer
 
+        # in case the artist has already been added as normal or background
+        # artist, remove it first!
+        if artist in chain(*self._m.BM._bg_artists.values()):
+            self._m.BM.remove_bg_artist(artist)
+
+        if artist in chain(*self._m.BM._artists.values()):
+            self._m.BM.remove_artist(artist)
+
         self._m.BM.add_artist(artist, layer=layer)
         self._temporary_artists.append(artist)
 
     def _execute_cb(self, layer):
         """
         Get bool if a callback assigned on "layer" should be executed.
 
@@ -259,14 +271,18 @@
 
         Returns
         -------
         bool
             Indicator if the callback should be executed on the currently visible
             layer or not.
         """
+
+        if self.execute_on_all_layers:
+            return True
+
         visible_layer = self._m.BM.bg_layer
         if layer == "all":
             # the all layer is always executed
             return True
         elif "|" in visible_layer:
             if layer == visible_layer:
                 # return true for the multi-layer itself
@@ -276,16 +292,48 @@
                 # (make sure to strip off transparency assignments, e.g. "layer{}" )
                 return any(
                     i.strip().split("{")[0] == layer for i in visible_layer.split("|")
                 )
         else:
             return layer == visible_layer
 
+    @property
+    def execute_on_all_layers(self):
+        if self._parent_container is not None:
+            return self._parent_container._execute_on_all_layers
+
+        return self._execute_on_all_layers
+
+    def set_execute_on_all_layers(self, q):
+        """
+        If True, callbacks of this container are executed even if the associated
+        layer is not visible.
+
+        (By default, callbacks are only executed if the associated layer is visible!)
+
+        Parameters
+        ----------
+        q : bool
+            True if callbacks should be executed irrespective of the visible layer.
+        """
+
+        if q:
+            _log.debug(
+                f"EOmaps: {self._method} callbacks of the Maps-object {self._m} "
+                "are executed on all layers!"
+            )
+
+        if self._parent_container is not None:
+            raise TypeError(
+                f"EOmaps: 'execute_on_all_layers' is inherited for {self._method}!"
+            )
+        self._execute_on_all_layers = q
 
-class _click_container(_cb_container):
+
+class _ClickContainer(_CallbackContainer):
     """
     A container for attaching callbacks and accessing return-objects.
 
     attach : accessor for callbacks.
         Executing the functions will attach the associated callback to the map!
 
     get : accessor for return-objects
@@ -456,37 +504,47 @@
             self.cbs = dict()
 
         @property
         def picked_object(self):
             if hasattr(self.cb, "picked_object"):
                 return self.cb.picked_object
             else:
-                print("EOmaps: attach the 'load' callback first!")
+                _log.warning(
+                    "EOmaps: No picked objects found. Attach "
+                    "the 'load' callback first!"
+                )
 
         @property
         def picked_vals(self):
             if hasattr(self.cb, "picked_vals"):
                 return self.cb.picked_vals
             else:
-                print("EOmaps: attach the 'get_vals' callback first!")
+                _log.warning(
+                    "EOmaps: No picked values found. Attach "
+                    "the 'get_vals' callback first!"
+                )
 
         @property
         def permanent_markers(self):
             if hasattr(self.cb, "permanent_markers"):
                 return self.cb.permanent_markers
             else:
-                print("EOmaps: attach the 'mark' callback with 'permanent=True' first!")
+                _log.warning(
+                    "EOmaps: No permanent markers found. Attach "
+                    "the 'mark' callback with 'permanent=True' first!"
+                )
 
         @property
         def permanent_annotations(self):
             if hasattr(self.cb, "permanent_annotations"):
                 return self.cb.permanent_annotations
             else:
-                print(
-                    "EOmaps: attach the 'annotate' callback with 'permanent=True' first!"
+                _log.warning(
+                    "EOmaps: No permanent annotations found. Attach "
+                    "the 'annotate' callback with 'permanent=True' first!"
                 )
 
         @property
         def attached_callbacks(self):
             cbs = []
             for ds, dsdict in self.cbs.items():
                 for b, bdict in dsdict.items():
@@ -549,30 +607,30 @@
         bname = f"{b}__{m}"
         dsdict = self.get.cbs.get(ds, None)
 
         if dsdict is not None:
             if bname in dsdict:
                 bdict = dsdict.get(bname)
             else:
-                print(f"EOmaps: there is no callback named {callback}")
+                _log.error(f"EOmaps: There is no callback named {callback}")
                 return
         else:
-            print(f"EOmaps: there is no callback named {callback}")
+            _log.error(f"EOmaps: There is no callback named {callback}")
             return
 
         if bdict is not None:
             if cbname in bdict:
                 del bdict[cbname]
 
                 # call cleanup methods on removal
                 fname = name.rsplit("_", 1)[0]
                 if hasattr(self._cb, f"_{fname}_cleanup"):
                     getattr(self._cb, f"_{fname}_cleanup")()
             else:
-                print(f"EOmaps: there is no callback named {callback}")
+                _log.error(f"EOmaps: There is no callback named {callback}")
 
     def set_sticky_modifiers(self, *args):
         """
         Define keys on the keyboard that should be treated as "sticky modifiers".
 
         "sticky modifiers" are used in "click"- "pick"- and "move" callbacks to define
         modifiers that should remain active even if the corresponding key on the
@@ -607,25 +665,24 @@
         assert (
             self._m.coll is not None
         ), "you can only attach pick-callbacks after calling `plot_map()`!"
 
         try:
             # Lazily make a plotted dataset pickable a
             if getattr(self._m, "tree", None) is None:
-                from .helpers import searchtree
+                from .helpers import SearchTree
 
-                self._m.tree = searchtree(m=self._m._proxy(self._m))
+                self._m.tree = SearchTree(m=self._m._proxy(self._m))
                 self._m.cb.pick._set_artist(self._m.coll)
                 self._m.cb.pick._init_cbs()
                 self._m.cb._methods.add("pick")
         except Exception as ex:
-            print(
+            _log.exception(
                 "EOmaps: There was an error while trying to initialize "
-                "pick-callbacks!",
-                ex,
+                f"pick-callbacks!",
             )
 
     def _add_callback(
         self,
         *args,
         callback=None,
         double_click=False,
@@ -728,15 +785,17 @@
                 callback=callback,
                 double_click=double_click,
                 button=button,
                 modifier=modifier,
                 **kwargs,
             )
         elif on_motion is True:
-            print("EOmaps: 'on_motion=True' is only possible for 'click' callbacks!")
+            _log.warning(
+                "EOmaps: 'on_motion=True' is only possible for " "'click' callbacks!"
+            )
 
         assert not all(
             i in kwargs for i in ["pos", "ID", "val", "double_click", "button"]
         ), 'the names "pos", "ID", "val" cannot be used as keyword-arguments!'
 
         if isinstance(callback, str):
             assert hasattr(self._cb, callback), (
@@ -778,15 +837,15 @@
 
         if movecb_name is not None:
             self._connected_move_cbs[cbname] = [movecb_name]
 
         return cbname
 
 
-class cb_click_container(_click_container):
+class ClickContainer(_ClickContainer):
     """
     Callbacks that are executed if you click anywhere on the Map.
 
     NOTE
     ----
     You can use `on_motion=False` when attaching a callback to avoid triggering
     the callback if the mouse is moved while a button is pressed.
@@ -812,28 +871,51 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._cid_button_press_event = None
         self._cid_button_release_event = None
         self._cid_motion_event = None
 
+        self._event = None
+
     def _init_cbs(self):
         if self._m.parent is self._m:
             self._add_click_callback()
 
     def _get_clickdict(self, event):
         clickdict = dict(
             pos=(event.xdata, event.ydata),
             ID=None,
             val=None,
             ind=None,
         )
 
         return clickdict
 
+    def _execute_cbs(self, event, cids):
+        """
+        Execute a list of callbacks based on an event and the cid
+
+        Parameters
+        ----------
+        event :
+            The event to use.
+        cids : list of str
+            A list of the cids of the callbacks that should be executed.
+
+        """
+        clickdict = self._get_clickdict(event)
+
+        for cid in cids:
+            name, layer, ds, button, mod = self._parse_cid(cid)
+            cbs = self.get.cbs.get(ds, dict()).get(f"{button}__{mod}", dict())
+            cb = cbs.get(f"{name}__{layer}", None)
+            if cb is not None:
+                cb(**clickdict)
+
     def _onclick(self, event):
         clickdict = self._get_clickdict(event)
 
         if event.dblclick:
             cbs = self.get.cbs.get("double", dict())
         else:
             cbs = self.get.cbs.get("single", dict())
@@ -846,14 +928,16 @@
             # in case sticky_modifiers are defined, use the last pressed modifier
             event_key = self._m.cb.keypress._modifier
         else:
             event_key = event.key
 
         button_modifier = f"{event.button}__{event_key}"
 
+        self._event = event
+
         if button_modifier in cbs:
             bcbs = cbs[button_modifier]
 
             for key in self._sort_cbs(bcbs):
                 layer = key.split("__", 1)[1]
                 if not self._execute_cb(layer):
                     return
@@ -880,14 +964,18 @@
         if button_modifier in cbs:
             clickdict = self._get_clickdict(event)
             bcbs = cbs[button_modifier]
             for cb in bcbs.values():
                 cb(**clickdict)
 
     def _reset_cids(self):
+        # clear all temporary artists
+        self._clear_temporary_artists()
+        self._m.BM._clear_temp_artists(self._method)
+
         if self._cid_button_press_event:
             self._m.f.canvas.mpl_disconnect(self._cid_button_press_event)
         self._cid_button_press_event = None
 
         if self._cid_motion_event:
             self._m.f.canvas.mpl_disconnect(self._cid_motion_event)
         self._cid_motion_event = None
@@ -928,14 +1016,16 @@
                 pass
 
         def releasecb(event):
             if not self._m.cb.get_execute_callbacks():
                 return
 
             try:
+                self._event = event
+
                 # don't execute callbacks if a toolbar-action is active
                 if (
                     self._m.f.canvas.toolbar is not None
                 ) and self._m.f.canvas.toolbar.mode != "":
                     return
 
                 # execute onclick on the maps object that belongs to the clicked axis
@@ -1003,15 +1093,15 @@
                     # x=event.mouseevent.x,
                     # y=event.mouseevent.y,
                 )
 
                 obj._onclick(dummymouseevent)
 
 
-class cb_move_container(cb_click_container):
+class MoveContainer(ClickContainer):
     """
     Callbacks that are executed if you move the mouse without holding down a button.
 
     Methods
     -------
     attach : accessor for callbacks.
         Executing the functions will attach the associated callback to the map!
@@ -1025,28 +1115,32 @@
 
     share_events : share events between connected maps-objects (e.g. forward both ways)
 
     set_sticky_modifiers : define keypress-modifiers that remain active after release
 
     """
 
-    # this is just a copy of cb_click_container to manage motion-sensitive callbacks
+    # this is just a copy of ClickContainer to manage motion-sensitive callbacks
 
     def __init__(self, button_down=False, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._cid_motion_event = None
 
         self._button_down = button_down
 
     def _init_cbs(self):
         if self._m.parent is self._m:
             self._add_move_callback()
 
     def _reset_cids(self):
+        # clear all temporary artists
+        self._clear_temporary_artists()
+        self._m.BM._clear_temp_artists(self._method)
+
         if self._cid_motion_event:
             self._m.f.canvas.mpl_disconnect(self._cid_motion_event)
         self._cid_motion_event = None
 
     def _add_move_callback(self):
         def movecb(event):
             if not self._m.cb.get_execute_callbacks():
@@ -1112,15 +1206,15 @@
         if self._cid_motion_event is None:
             # for click-callbacks, allow motion-detection
             self._cid_motion_event = self._m.f.canvas.mpl_connect(
                 "motion_notify_event", movecb
             )
 
 
-class cb_pick_container(_click_container):
+class PickContainer(_ClickContainer):
     """
     Callbacks that select the nearest datapoint if you click on the map.
 
     The event will search for the closest data-point and execute the callback
     with the properties (e.g. position , ID, value) of the selected point.
 
     Note
@@ -1175,15 +1269,15 @@
             container_name = "_pick__" + name[1:]
         else:
             container_name = "pick__" + name
 
         if hasattr(self._m.cb, container_name):
             return getattr(self._m.cb, container_name)
         else:
-            print(
+            _log.error(
                 f"the picker {name} does not exist...", "use `m.cb.add_picker` first!"
             )
 
     def set_props(
         self,
         n=None,
         consecutive_pick=None,
@@ -1216,22 +1310,23 @@
             - If False: pick (n) nearest neighbours based on the click-position
 
             The default is True.
         search_radius : int, float, str or None optional
             Set the radius of the area that is used to limit the number of
             pixels when searching for nearest-neighbours.
 
-            if `int` or `float`:
-                The radius of the circle in units of the plot_crs
-            if `str:
-                A multiplication-factor for the estimated pixel-radius.
-                (e.g. a circle with (r=search_radius * m.shape.radius) is
-                used if possible and else np.inf is used.
+            - if `int` or `float`, the radius of the circle in units of the plot_crs
+            - if `str`, a multiplication-factor for the estimated data-radius.
 
-            The default is "50" (e.g. 50 times the pixel-radius).
+              NOTE: The multiplied radius is defined in the plot projection!
+              If the data was provided in a different projection, the radius
+              estimated from the re-projected data is used (might be different
+              from the actual shape radius!)
+
+            The default is "50" (e.g. 50 times the data-radius).
 
         """
         if n is not None:
             self._n_ids = n
 
         if consecutive_pick is not None:
             self._consecutive_multipick = consecutive_pick
@@ -1419,14 +1514,18 @@
                     if self._consecutive_multipick is False:
                         cb(**clickdict)
                     else:
                         for c in clickdict:
                             cb(**c)
 
     def _reset_cids(self):
+        # clear all temporary artists
+        self._clear_temporary_artists()
+        self._m.BM._clear_temp_artists(self._method)
+
         for method, cid in self._cid_pick_event.items():
             self._m.f.canvas.mpl_disconnect(cid)
         self._cid_pick_event.clear()
 
     def _add_pick_callback(self):
         # execute onpick and forward the event to all connected Maps-objects
 
@@ -1515,15 +1614,15 @@
                 dummyevent.val_color = pick[1].get("val_color", None)
             else:
                 dummyevent.ind = None
 
             obj._onpick(dummyevent)
 
 
-class keypress_container(_cb_container):
+class KeypressContainer(_CallbackContainer):
     """
     Callbacks that are executed if you press a key on the keyboard.
 
     Methods
     -------
     attach : accessor for callbacks.
         Executing the functions will attach the associated callback to the map!
@@ -1550,14 +1649,18 @@
         self._modifier = None
 
     def _init_cbs(self):
         if self._m.parent is self._m:
             self._initialize_callbacks()
 
     def _reset_cids(self):
+        # clear all temporary artists
+        self._clear_temporary_artists()
+        self._m.BM._clear_temp_artists(self._method)
+
         if self._cid_keypress_event:
             self._m.f.canvas.mpl_disconnect(self._cid_keypress_event)
         self._cid_keypress_event = None
 
     def _initialize_callbacks(self):
         def _onpress(event):
             if not self._m.cb.get_execute_callbacks():
@@ -1570,28 +1673,31 @@
                 # click or pick callbacks
                 k = str(event.key)
 
                 if self._modifier is not None and (
                     k == "ctrl+" + self._modifier or k == "escape"
                 ):
                     self._modifier = None
-                    print("EOmaps: sticky modifier: None")
+                    _log.info("EOmaps: sticky modifier set to: None")
                 elif self._modifier != k:
                     methods = []
                     if k in self._m.cb.click._sticky_modifiers:
                         methods.append("click")
 
                     if k in self._m.cb.pick._sticky_modifiers:
                         methods.append("pick")
 
                     if k in self._m.cb.move._sticky_modifiers:
                         methods.append("move")
 
                     if methods:
-                        print(f"EOmaps: sticky modifier: {k} ({', '.join(methods)})")
+                        _log.info(
+                            "EOmaps: sticky modifier set to: "
+                            f"{k} ({', '.join(methods)})"
+                        )
                         self._modifier = k
 
                 for obj in self._objs:
                     # only trigger callbacks on the right layer
                     if not self._execute_cb(obj._m.layer):
                         continue
                     if any(i in obj.get.cbs for i in (event.key, None)):
@@ -1744,17 +1850,17 @@
                 del cbs[cbname]
 
                 # call cleanup methods on removal
                 fname = name.rsplit("_", 1)[0]
                 if hasattr(self._cb, f"_{fname}_cleanup"):
                     getattr(self._cb, f"_{fname}_cleanup")()
             else:
-                print(f"EOmaps: there is no callback named {callback}")
+                _log.error(f"EOmaps: there is no callback named {callback}")
         else:
-            print(f"EOmaps: there is no callback named {callback}")
+            _log.error(f"EOmaps: there is no callback named {callback}")
 
     def _add_callback(self, callback, key="x", **kwargs):
         """
         Attach a callback to the plot that will be executed if a key is pressed.
 
         A list of pre-defined callbacks (accessible via `m.cb`) or customly defined
         functions can be used.
@@ -1810,15 +1916,15 @@
 
         # append the callback
         cbdict[cbkey] = partial(callback, **kwargs)
 
         return cbkey + f"__{key}"
 
 
-class cb_container:
+class CallbackContainer:
     """
     Accessor for attaching callbacks and accessing return-objects.
 
     Methods
     -------
     - **click** : Execute functions when clicking on the map
 
@@ -1828,47 +1934,47 @@
     - **keypress** : Execute functions if you press a key on the keyboard
 
     """
 
     def __init__(self, m):
         self._m = m
 
-        self._methods = {"click", "move", "keypress", "_click_move"}
+        self._methods = {"click", "pick", "move", "keypress", "_click_move"}
 
-        self._click = cb_click_container(
+        self._click = ClickContainer(
             m=self._m,
-            cb_cls=click_callbacks,
+            cb_cls=ClickCallbacks,
             method="click",
         )
         # a move-container that shares temporary artists with the click-container
-        self._click_move = cb_move_container(
+        self._click_move = MoveContainer(
             m=self._m,
-            cb_cls=click_callbacks,
+            cb_cls=ClickCallbacks,
             method="_click_move",
-            tmp_artists=self._click._temporary_artists,
+            parent_container=self._click,
             button_down=True,
         )
 
-        self._move = cb_move_container(
+        self._move = MoveContainer(
             m=self._m,
-            cb_cls=move_callbacks,
+            cb_cls=MoveCallbacks,
             method="move",
             button_down=False,
             default_button=None,
         )
 
-        self._pick = cb_pick_container(
+        self._pick = PickContainer(
             m=self._m,
-            cb_cls=pick_callbacks,
+            cb_cls=PickCallbacks,
             method="pick",
         )
 
-        self._keypress = keypress_container(
+        self._keypress = KeypressContainer(
             m=self._m,
-            cb_cls=keypress_callbacks,
+            cb_cls=KeypressCallbacks,
             method="keypress",
         )
 
     def get_execute_callbacks(self):
         """
         Get if callbacks should be executed or not.
 
@@ -1888,33 +1994,33 @@
         ----------
         val : bool
             If True, callbacks will be executed.
         """
         self._m.parent._execute_callbacks = val
 
     @property
-    @wraps(cb_click_container)
+    @wraps(ClickContainer)
     def click(self):
         """Attach click callbacks."""
         return self._click
 
     @property
-    @wraps(cb_move_container)
+    @wraps(MoveContainer)
     def move(self):
         """Attach move callbacks."""
         return self._move
 
     @property
-    @wraps(cb_pick_container)
+    @wraps(PickContainer)
     def pick(self):
         """Attach pick callbacks."""
         return self._pick
 
     @property
-    @wraps(keypress_container)
+    @wraps(KeypressContainer)
     def keypress(self):
         """Attach keypress callbacks."""
         return self._keypress
 
     def add_picker(self, name, artist, picker):
         """
         Attach a custom picker to an artist.
@@ -1944,15 +2050,15 @@
             >>>     # if the pick is successful:
             >>>     return True, dict(ID, pos, val, ind)
 
         Note
         ----
         If the name starts with an underscore (e.g. "_MyPicker") then the
         associated container will be accessible via `m._cb._pick__MyPicker`
-        or via `m.cb.pick["_MyPicker"]. (This is useful to setup pickers that
+        or via `m.cb.pick["_MyPicker"]`. (This is useful to setup pickers that
         are only used internally)
         """
         name = str(name)
 
         if picker is not None:
             assert name != "default", "'default' is not a valid picker name!"
 
@@ -1963,22 +2069,22 @@
             method = "pick"
         else:
             if name.startswith("_"):
                 method = "_pick__" + name[1:]
             else:
                 method = "pick__" + name
 
-        new_pick = cb_pick_container(
+        new_pick = PickContainer(
             m=self._m,
-            cb_cls=pick_callbacks,
+            cb_cls=PickCallbacks,
             method=method,
             picker_name=name,
             picker=picker,
         )
-        new_pick.__doc__ == cb_pick_container.__doc__
+        new_pick.__doc__ == PickContainer.__doc__
         new_pick._set_artist(artist)
         new_pick._init_cbs()
 
         # add the picker method to the accessible cbs
         setattr(self._m.cb, new_pick._method, new_pick)
         self._methods.add(new_pick._method)
```

### Comparing `EOmaps-6.5/eomaps/_containers.py` & `EOmaps-7.0/eomaps/_containers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,20 @@
+import logging
 from textwrap import dedent, indent, fill
-
-from warnings import warn
 from operator import attrgetter
 from inspect import signature, _empty
 from types import SimpleNamespace
 
+from .helpers import register_modules
 
-pd = None
-
-
-def _register_pandas():
-    global pd
-    try:
-        import pandas as pd
-    except ImportError:
-        return False
-
-    return True
-
-
-gpd = None
-
-
-def _register_geopandas():
-    global gpd
-    try:
-        import geopandas as gpd
-    except ImportError:
-        return False
-
-    return True
-
+_log = logging.getLogger(__name__)
 
-mapclassify = None
 
-
-def _register_mapclassify():
-    global mapclassify
-    try:
-        import mapclassify
-    except ImportError:
-        return False
-
-    return True
-
-
-class data_specs(object):
-    """
-    a container for accessing the data-properties
-    """
+class DataSpecs(object):
+    """Container for accessing the data-properties."""
 
     def __init__(
         self,
         m,
         data=None,
         x="lon",
         y="lat",
@@ -201,32 +163,32 @@
 
     @parameter.setter
     def parameter(self, parameter):
         self._parameter = parameter
 
     @parameter.getter
     def parameter(self):
+        if self._parameter is None:
+            (pd,) = register_modules("pandas", raise_exception=False)
 
-        if (
-            self._parameter is None
-            and _register_pandas()
-            and isinstance(self.data, pd.DataFrame)
-        ):
-            if self.data is not None and self.x is not None and self.y is not None:
-
+            if (
+                pd
+                and isinstance(self.data, pd.DataFrame)
+                and not any(i is None for i in (self.data, self.x, self.y))
+            ):
                 try:
                     self.parameter = next(
                         i for i in self.data.keys() if i not in [self.x, self.y]
                     )
-                    print(f"EOmaps: Parameter was set to: '{self.parameter}'")
+                    _log.info(f"EOmaps: Parameter was set to: '{self.parameter}'")
 
                 except Exception:
-                    warn(
+                    _log.error(
                         "EOmaps: Parameter-name could not be identified!"
-                        + "\nCheck the data-specs!"
+                        "Check the data-specs!"
                     )
 
         return self._parameter
 
     @property
     def encoding(self):
         return self._encoding
@@ -250,15 +212,15 @@
         return self._cpos_radius
 
     @cpos_radius.setter
     def cpos_radius(self, cpos_radius):
         self._cpos_radius = cpos_radius
 
 
-class classify_specs(object):
+class ClassifySpecs(object):
     """
     a container for accessing the data classification specifications
 
     SCHEMES : accessor Namespace for the available classification-schemes
 
     """
 
@@ -317,25 +279,22 @@
 
     @scheme.setter
     def scheme(self, val):
         self._scheme = val
         self._keys = set()
         s = self._get_default_args()
         if len(self._keys) > 0:
-            print(f"EOmaps: classification has been reset to '{val}{s}'")
+            _log.info(f"EOmaps: classification has been reset to '{val}{s}'")
         for key, val in self._defaults.items():
             if val != _empty:
                 setattr(self, key, val)
 
     def _get_default_args(self):
         if hasattr(self, "_scheme") and self._scheme is not None:
-            assert _register_mapclassify(), (
-                "EOmaps: Missing dependency: 'mapclassify' \n ... please install"
-                + " (conda install -c conda-forge mapclassify) to use data-classifications."
-            )
+            (mapclassify,) = register_modules("mapclassify")
 
             assert self._scheme in mapclassify.CLASSIFIERS, (
                 f"the classification-scheme '{self._scheme}' is not valid... "
                 + " use one of:"
                 + ", ".join(mapclassify.CLASSIFIERS)
             )
             s = signature(getattr(mapclassify, self._scheme))
@@ -363,22 +322,19 @@
         args = (
             "("
             + ", ".join([f"{key}={self[key]}" for key, val in self._defaults.items()])
             + ")"
         )
 
         if reset:
-            print(f"EOmaps: classification has been reset to '{scheme}{args}'")
+            _log.info(f"EOmaps: classification has been reset to '{scheme}{args}'")
 
     @property
     def SCHEMES(self):
         """
         accessor for possible classification schemes
         """
-        assert _register_mapclassify(), (
-            "EOmaps: Missing dependency: 'mapclassify' \n ... please install"
-            + " (conda install -c conda-forge mapclassify) to use data-classifications."
-        )
+        (mapclassify,) = register_modules("mapclassify")
 
         return SimpleNamespace(
             **dict(zip(mapclassify.CLASSIFIERS, mapclassify.CLASSIFIERS))
         )
```

### Comparing `EOmaps-6.5/eomaps/_data_manager.py` & `EOmaps-7.0/eomaps/_data_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import logging
+
 import numpy as np
 from pyproj import CRS, Transformer
 
+_log = logging.getLogger(__name__)
+
 
 class DataManager:
     def __init__(self, m):
         self.m = m
         self.last_extent = None
         self._all_data = dict()
 
@@ -90,25 +94,28 @@
         layer,
         assume_sorted=True,
         update_coll_on_fetch=True,
         indicate_masked_points=True,
         dynamic=False,
         only_pick=False,
     ):
+        # cleanup existing callbacks before attaching new ones
+        self.cleanup_callbacks()
+
         self._only_pick = only_pick
 
         if self.m._data_plotted:
             self._remove_existing_coll()
 
         self._all_data = self._prepare_data(assume_sorted=assume_sorted)
         self._indicate_masked_points = indicate_masked_points
         self.layer = layer
 
         if len(self.x0) == 0:
-            print("EOmaps: There is no data to plot")
+            _log.info("EOmaps: There is no data to plot")
             return
 
         if self.x0_1D is not None:
             # if we have 1D coordinates, use them to get the extent
             self._x0min, self._x0max = np.nanmin(self.x0_1D), np.nanmax(self.x0_1D)
             self._y0min, self._y0max = np.nanmin(self.y0_1D), np.nanmax(self.y0_1D)
         else:
@@ -129,21 +136,29 @@
             self._r = None
             self._radius_margin = None
 
         if update_coll_on_fetch:
             # attach a hook that updates the collection whenever a new
             # background is fetched
             # ("shade" shapes take care about updating the data themselves!)
+            self.attach_callbacks(dynamic=dynamic)
 
-            if dynamic is True:
-                if self.on_fetch_bg not in self.m.BM._before_update_actions:
-                    self.m.BM._before_update_actions.append(self.on_fetch_bg)
-            else:
-                if self.on_fetch_bg not in self.m.BM._before_fetch_bg_actions:
-                    self.m.BM._before_fetch_bg_actions.append(self.on_fetch_bg)
+    def attach_callbacks(self, dynamic):
+        if dynamic is True:
+            if self.on_fetch_bg not in self.m.BM._before_update_actions:
+                self.m.BM._before_update_actions.append(self.on_fetch_bg)
+        else:
+            if self.on_fetch_bg not in self.m.BM._before_fetch_bg_actions:
+                self.m.BM._before_fetch_bg_actions.append(self.on_fetch_bg)
+
+    def cleanup_callbacks(self):
+        if self.on_fetch_bg in self.m.BM._before_fetch_bg_actions:
+            self.m.BM._before_fetch_bg_actions.remove(self.on_fetch_bg)
+        if self.on_fetch_bg in self.m.BM._before_update_actions:
+            self.m.BM._before_update_actions.remove(self.on_fetch_bg)
 
     def _prepare_data(self, assume_sorted=True):
         in_crs = self.m.data_specs.crs
         cpos = self.m.data_specs.cpos
         cpos_radius = self.m.data_specs.cpos_radius
 
         props = dict()
@@ -178,33 +193,34 @@
         if assume_sorted is False:
             if used_shape.name in ["raster", "shade_raster"]:
                 if (
                     len(xorig.shape) == 1
                     and len(yorig.shape) == 1
                     and len(z_data.shape) == 2
                 ):
+                    _log.info("EOmaps: Sorting coordinates...")
 
                     xs, ys = np.argsort(xorig), np.argsort(yorig)
                     np.take(xorig, xs, out=xorig, mode="wrap")
                     np.take(yorig, ys, out=yorig, mode="wrap")
                     np.take(
                         np.take(z_data, xs, 0),
                         indices=ys,
                         axis=1,
                         out=z_data,
                         mode="wrap",
                     )
                 else:
-                    print(
+                    _log.info(
                         "EOmaps: using 'assume_sorted=False' is only possible"
                         + "if you use 1D coordinates + 2D data!"
                         + "...continuing without sorting."
                     )
             else:
-                print(
+                _log.info(
                     "EOmaps: using 'assume_sorted=False' is only relevant for "
                     + "the shapes ['raster', 'shade_raster']! "
                     + "...continuing without sorting."
                 )
 
         self._z_transposed = False
 
@@ -225,14 +241,16 @@
 
                     z_data = z_data.T
                     self._z_transposed = True
 
             x0, y0 = xorig, yorig
 
         else:
+            _log.info(f"EOmaps: Starting to reproject {z_data.size} datapoints")
+
             # transform center-points to the plot_crs
             transformer = Transformer.from_crs(
                 crs1,
                 crs2,
                 always_xy=True,
             )
             # convert 1D data to 2D to make sure re-projection is correct
@@ -242,14 +260,15 @@
                 and len(z_data.shape) == 2
             ):
                 xorig, yorig = np.meshgrid(xorig, yorig, copy=False)
                 z_data = z_data.T
                 self._z_transposed = True
 
             x0, y0 = transformer.transform(xorig, yorig)
+            _log.info("EOmaps: Done reprojecting")
 
         # use np.asanyarray to ensure that the output is a proper numpy-array
         # (relevant for categorical dtypes in pandas.DataFrames)
         props["xorig"] = np.asanyarray(xorig)
         props["yorig"] = np.asanyarray(yorig)
         props["ids"] = ids
         props["z_data"] = np.asanyarray(z_data)
@@ -281,15 +300,15 @@
             x = x - radiusx
             y = y - radiusx
 
         return x, y
 
     @property
     def current_extent(self):
-        return self.m.get_extent(self.m.ax.projection)
+        return self.m.get_extent(self.m.crs_plot)
 
     @property
     def extent_changed(self):
         return not self.current_extent == self.last_extent
 
     def _set_lims(self):
         # set the extent...
@@ -328,27 +347,27 @@
     def indicate_masked_points(self, **kwargs):
         # remove previous mask artist
         if self._masked_points_artist is not None:
             try:
                 self.m.BM.remove_bg_artist(self._masked_points_artist)
                 self._masked_points_artist.remove()
                 self._masked_points_artist = None
-            except Exception as ex:
-                print(ex)
+            except Exception:
+                _log.exception("EOmaps: Error while indicating masked points.")
 
         if not hasattr(self.m, "_data_mask") or self.m._data_mask is None:
             return
 
         mask = self.m._data_mask.ravel()
         npts = np.count_nonzero(mask)
         if npts == 0:
             return
 
         if npts > 1e5:
-            print(
+            _log.warning(
                 "EOmaps: There are more than 100 000 masked points! "
                 "... indicating masked points will affect performance!"
             )
 
         kwargs.setdefault("ec", "r")
         kwargs.setdefault("lw", 0.25)
         kwargs.setdefault("c", self._current_data["z_data"].ravel()[~mask])
@@ -411,16 +430,16 @@
                 else:
                     self.m.BM.remove_bg_artist(self.m._coll)
 
                 # if the collection is still attached to the axes, remove it
                 if self.m.coll.axes is not None:
                     self.m.coll.remove()
                 self.m._coll = None
-            except Exception as ex:
-                print(ex)
+            except Exception:
+                _log.exception("EOmaps: Error while trying to remove collection.")
 
     def _get_current_datasize(self):
         if self._current_data:
             return self._get_datasize(**self._current_data)
         else:
             return 99
 
@@ -456,14 +475,16 @@
 
             # remove previous collection from the map
             self._remove_existing_coll()
             # draw the new collection
             coll = self.m._get_coll(props, **self.m._coll_kwargs)
             coll.set_clim(self.m._vmin, self.m._vmax)
 
+            coll.set_label("Dataset " f"({self.m.shape.name}  |  {self.z_data.shape})")
+
             if self.m.shape.name != "scatter_points":
                 # avoid use "autolim=True" since it can cause problems in
                 # case the data-limits are infinite (e.g. for projected
                 # datasets containing points outside the used projection)
                 # the extent is set by calling "._set_lims()" in `m.plot_map()`
                 self.m.ax.add_collection(coll, autolim=False)
 
@@ -488,18 +509,17 @@
             # (=lazily initialize the picker when the layer is fetched)
             while len(self._on_next_fetch) > 0:
                 self._on_next_fetch.pop(-1)()
 
             self.m.cb.pick._set_artist(coll)
 
         except Exception as ex:
-            print(
-                f"EOmaps: Unable to plot the data for the layer '{layer}' !"
-                f"\n        {ex}"
-            )
+            raise AssertionError(
+                f"EOmaps: Unable to plot the data for the layer '{layer}'!"
+            ) from ex
 
     def data_in_extent(self, extent):
         # check if the data extent collides with the map extent
         x0, x1, y0, y1 = extent
         if x0 > self._x0max or self._x0min > x1:
             return False
         if y0 > self._y0max or self._y0min > y1:
@@ -668,33 +688,33 @@
         if name in ["raster"]:
             if s < 2e6:
                 return
             else:
                 txt = f"EOmaps: Plotting {s:.1E} points as {self.m.shape.name}"
 
             if s < 5e6:
-                print(f"{txt}...\n       this might take a few seconds...")
+                _log.info(f"{txt}...\n       this might take a few seconds...")
             elif s < 2e7:
-                print(f"{txt}...\n       this might take some time...")
+                _log.info(f"{txt}...\n       this might take some time...")
             else:
-                print(f"{txt}...\n       this might take A VERY LONG TIME❗❗")
+                _log.info(f"{txt}...\n       this might take A VERY LONG TIME❗❗")
         else:
             if name in ["rectangles", "ellipses", "geod_circles"]:
                 txt = f"EOmaps: Plotting {s:.1E} {self.m.shape.name}"
             elif name in ["voronoi_diagram", "delaunay_triangulation"]:
                 txt = f"EOmaps: Plotting a {self.m.shape.name} of {s:.1E}"
             else:
                 return
 
             if s < 5e5:
-                print(f"{txt}...\n       this might take a few seconds...")
+                _log.info(f"{txt}...\n       this might take a few seconds...")
             elif s < 1e6:
-                print(f"{txt}...\n       this might take some time...")
+                _log.info(f"{txt}...\n       this might take some time...")
             else:
-                print(f"{txt}...\n       this might take A VERY LONG TIME❗❗")
+                _log.info(f"{txt}...\n       this might take A VERY LONG TIME❗❗")
 
     def _get_xy_from_index(self, ind, reprojected=False):
         """
         Get x and y coordinates from a list of numerical data indexes
 
         Parameters
         ----------
@@ -811,15 +831,12 @@
             inds = np.flatnonzero(np.isin(ids, ID))
         else:
             inds = None
 
         return self._get_xy_from_index(inds, reprojected=reprojected)
 
     def cleanup(self):
+        self.cleanup_callbacks()
+
         self._all_data.clear()
         self._current_data.clear()
         self.last_extent = None
-
-        if self.on_fetch_bg in self.m.BM._before_fetch_bg_actions:
-            self.m.BM._before_fetch_bg_actions.remove(self.on_fetch_bg)
-        if self.on_fetch_bg in self.m.BM._before_update_actions:
-            self.m.BM._before_update_actions.remove(self.on_fetch_bg)
```

### Comparing `EOmaps-6.5/eomaps/_shapes.py` & `EOmaps-7.0/eomaps/shapes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from matplotlib.collections import PolyCollection, QuadMesh, TriMesh
-from matplotlib.tri import Triangulation
-import numpy as np
-
-from pyproj import CRS, Transformer
-from functools import partial, wraps, lru_cache
-import warnings
+"""Plot shape classes (for data visualization)."""
 
-ds = None
+import logging
+from functools import partial, wraps
 
+from matplotlib.collections import PolyCollection, QuadMesh, TriMesh
+from matplotlib.tri import Triangulation
 
-def _register_datashader():
-    global ds
+from pyproj import CRS
+import numpy as np
 
-    try:
-        import datashader as ds
-    except ImportError:
-        return False
+from .helpers import register_modules
 
-    return True
+_log = logging.getLogger(__name__)
 
 
-class shapes(object):
+class Shapes(object):
     """
     Set the plot-shape to represent the data-points.
 
     By default, "ellipses" is used for datasets smaller than 500k pixels and shading
     with "shade_raster" is used for larger datasets (if datashader is installed).
 
     Possible shapes are:
@@ -79,42 +73,44 @@
     ]
 
     def __init__(self, m):
         self._m = m
         self._radius_estimation_range = 100000
 
     def _get(self, shape, **kwargs):
-        shp = getattr(self, f"_{shape}")(self._m)
+        # get the name of the class for a given shape
+        # (CamelCase without underscores)
+        shapeclass_name = "_" + "".join(i.capitalize() for i in shape.split("_"))
+
+        shp = getattr(self, shapeclass_name)(self._m)
         for key, val in kwargs.items():
             setattr(shp, key, val)
         return shp
 
     @staticmethod
     def _get_radius(m, radius, radius_crs):
         if (isinstance(radius, str) and radius == "estimate") or radius is None:
             if m._estimated_radius is None:
                 # make sure props are defined otherwise we can't estimate the radius!
                 if m._data_manager.x0 is None:
                     m._data_manager.set_props(None)
 
-                print("EOmaps: estimating radius...")
-                radiusx, radiusy = shapes._estimate_radius(m, radius_crs)
+                _log.info("EOmaps: Estimating shape radius...")
+                radiusx, radiusy = Shapes._estimate_radius(m, radius_crs)
 
                 if radiusx == radiusy:
-                    print(
-                        "EOmaps: radius:",
-                        np.format_float_scientific(radiusx, precision=4),
+                    _log.info(
+                        "EOmaps: radius = "
+                        f"{np.format_float_scientific(radiusx, precision=4)}"
                     )
                 else:
-                    print(
-                        "EOmaps: radius:" "(",
-                        np.format_float_scientific(radiusx, precision=4),
-                        ",",
-                        np.format_float_scientific(radiusy, precision=4),
-                        ")",
+                    _log.info(
+                        "EOmaps: radius = "
+                        f"({np.format_float_scientific(radiusx, precision=4)}, "
+                        f"{np.format_float_scientific(radiusy, precision=4)})"
                     )
                 radius = (radiusx, radiusy)
                 # remember estimated radius to avoid re-calculating it all the time
                 m._estimated_radius = (radiusx, radiusy)
             else:
                 radius = m._estimated_radius
         else:
@@ -259,21 +255,14 @@
 
         if len(color_vals) == 0:
             return {"array": array}
         else:
             color_vals["array"] = None
             return color_vals
 
-    @staticmethod
-    @lru_cache()
-    def _get_transformer(in_crs, out_crs):
-        # cache transformers to avoid re-initialization for each feature
-        t = Transformer.from_crs(in_crs, out_crs, always_xy=True)
-        return t
-
     # a base class for shapes that support setting the number of intermediate points
     class _ShapeBase:
         name = "none"
 
         def __init__(self, m):
             self._m = m
             self._n = None
@@ -311,22 +300,20 @@
             else:
                 return self._n
 
         @n.setter
         def n(self, val):
             if self.name == "rectangles" and self.mesh is True:
                 if val is not None and val != 1:
-                    warnings.warn(
-                        "EOmaps: rectangles with 'mesh=True' only supports n=1"
-                    )
+                    _log.info("EOmaps: rectangles with 'mesh=True' only support n=1")
                 self._n = 1
             else:
                 self._n = val
 
-    class _geod_circles(_ShapeBase):
+    class _GeodCircles(_ShapeBase):
         name = "geod_circles"
 
         def __init__(self, m):
             super().__init__(m=m)
 
         def __call__(self, radius=None, n=None):
             """
@@ -375,15 +362,15 @@
 
         @radius.setter
         def radius(self, val):
             self._radius = np.asanyarray(np.atleast_1d(val))
 
         @property
         def radius_crs(self):
-            return self._m.get_crs("geod")
+            return "geod"
 
         def __repr__(self):
             try:
                 s = f"geod_circles(radius={self.radius}, n={self.n})"
             except AttributeError:
                 s = "geod_circles(radius, n)"
             return s
@@ -422,35 +409,35 @@
                 if radius.size != lon.size:
                     radius = np.broadcast_to(radius[:, None], (size, n))
                 else:
                     radius = np.broadcast_to(radius.ravel()[:, None], (size, n))
 
             geod = self._m.crs_plot.get_geod()
             lons, lats, back_azim = geod.fwd(
-                np.broadcast_to(lon[:, None], (size, n)),
-                np.broadcast_to(lat[:, None], (size, n)),
-                np.linspace(
+                lons=np.broadcast_to(lon[:, None], (size, n)),
+                lats=np.broadcast_to(lat[:, None], (size, n)),
+                az=np.linspace(
                     [start_angle] * size, [360 - start_angle] * size, n, axis=1
                 ),
-                radius,
+                dist=radius,
                 radians=False,
             )
 
             return lons.T, lats.T
 
         def _get_geod_circle_points(self, x, y, crs, radius, n=20):
             x, y = np.asarray(x), np.asarray(y)
 
             # transform from in-crs to lon/lat
-            radius_t = shapes._get_transformer(
+            radius_t = self._m._get_transformer(
                 self._m.get_crs(crs),
                 self._m.CRS.PlateCarree(globe=self._m.crs_plot.globe),
             )
             # transform from lon/lat to the plot_crs
-            plot_t = shapes._get_transformer(
+            plot_t = self._m._get_transformer(
                 self._m.CRS.PlateCarree(globe=self._m.crs_plot.globe),
                 CRS.from_user_input(self._m.crs_plot),
             )
 
             lon, lat = radius_t.transform(x, y)
             # calculate some points on the geodesic circle
             lons, lats = self._calc_geod_circle_points(lon, lat, radius, n=n)
@@ -494,26 +481,26 @@
                 verts,
                 np.broadcast_to(~mask[:, None].T.swapaxes(1, 2), verts.shape),
             )
             verts = list(
                 i.compressed().reshape(-1, 2) for i, m in zip(verts, vertmask) if m
             )
 
-            color_and_array = shapes._get_colors_and_array(kwargs, vertmask)
+            color_and_array = Shapes._get_colors_and_array(kwargs, vertmask)
 
             coll = PolyCollection(
                 verts,
                 # transOffset=self._m.ax.transData,
                 **color_and_array,
                 **kwargs,
             )
 
             return coll
 
-    class _ellipses(_ShapeBase):
+    class _Ellipses(_ShapeBase):
         name = "ellipses"
 
         def __init__(self, m):
             super().__init__(m=m)
 
         def __call__(self, radius="estimate", radius_crs="in", n=None):
             """
@@ -549,15 +536,15 @@
 
         @property
         def _initargs(self):
             return dict(radius=self._radius, radius_crs=self.radius_crs, n=self._n)
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, self._radius, self.radius_crs)
+            radius = Shapes._get_radius(self._m, self._radius, self.radius_crs)
             return radius
 
         @radius.setter
         def radius(self, val):
             if isinstance(val, (list, np.ndarray)):
                 self._radius = np.asanyarray(val).ravel()
             else:
@@ -616,19 +603,19 @@
             )
             return (xs, ys)
 
         def _get_ellipse_points(self, x, y, crs, radius, radius_crs="in", n=20):
             crs = self._m.get_crs(crs)
             radius_crs = self._m.get_crs(radius_crs)
             # transform from crs to the plot_crs
-            t_in_plot = shapes._get_transformer(crs, self._m.crs_plot)
+            t_in_plot = self._m._get_transformer(crs, self._m.crs_plot)
             # transform from crs to the radius_crs
-            t_in_radius = shapes._get_transformer(crs, radius_crs)
+            t_in_radius = self._m._get_transformer(crs, radius_crs)
             # transform from crs to the radius_crs
-            t_radius_plot = shapes._get_transformer(radius_crs, self._m.crs_plot)
+            t_radius_plot = self._m._get_transformer(radius_crs, self._m.crs_plot)
 
             if isinstance(radius, (int, float, np.number)):
                 rx, ry = radius, radius
             else:
                 rx, ry = radius
 
             # transform corner-points
@@ -685,16 +672,16 @@
                     quadrant = x < xc
                     quadrants[quadrant] = 0
                     quadrant = x > xc
                     quadrants[quadrant] = 1
 
                     return quadrants
 
-                t_in_lonlat = shapes._get_transformer(crs, 4326)
-                t_plot_lonlat = shapes._get_transformer(self._m.crs_plot, 4326)
+                t_in_lonlat = self._m._get_transformer(crs, 4326)
+                t_plot_lonlat = self._m._get_transformer(self._m.crs_plot, 4326)
 
                 # transform the coordinates to lon/lat
                 xp, _ = t_in_lonlat.transform(x, y)
                 xsp, _ = t_plot_lonlat.transform(xs, ys)
 
                 quadrants, pts_quadrants = getQ(xp, xc), getQ(xsp, xc)
 
@@ -727,26 +714,26 @@
                 np.column_stack((x.compressed(), y.compressed()))
                 for i, (x, y) in enumerate(zip(xs, ys))
                 if mask[i]
             )
             # remember masked points
             self._m._data_mask = mask
 
-            color_and_array = shapes._get_colors_and_array(kwargs, mask)
+            color_and_array = Shapes._get_colors_and_array(kwargs, mask)
 
             coll = PolyCollection(
                 verts,
                 # transOffset=self._m.ax.transData,
                 **color_and_array,
                 **kwargs,
             )
 
             return coll
 
-    class _rectangles(_ShapeBase):
+    class _Rectangles(_ShapeBase):
         name = "rectangles"
 
         def __init__(self, m):
             super().__init__(m=m)
 
         def __call__(self, radius="estimate", radius_crs="in", mesh=False, n=None):
             """
@@ -798,15 +785,15 @@
                 radius_crs=self.radius_crs,
                 n=self._n,
                 mesh=self.mesh,
             )
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, self._radius, self.radius_crs)
+            radius = Shapes._get_radius(self._m, self._radius, self.radius_crs)
             return radius
 
         @radius.setter
         def radius(self, val):
             if isinstance(val, (list, np.ndarray)):
                 self._radius = np.asanyarray(val).ravel()
             else:
@@ -828,21 +815,21 @@
             else:
                 rx, ry = radius
 
             # transform corner-points
             if radius_crs == crs:
                 in_crs = self._m.get_crs(crs)
                 # transform from crs to the plot_crs
-                t = shapes._get_transformer(
+                t = self._m._get_transformer(
                     CRS.from_user_input(in_crs), self._m.crs_plot
                 )
 
                 # make sure we do not transform out of bounds (if possible)
                 if in_crs.area_of_use is not None:
-                    transformer = shapes._get_transformer(in_crs.geodetic_crs, in_crs)
+                    transformer = self._m._get_transformer(in_crs.geodetic_crs, in_crs)
 
                     xmin, ymin, xmax, ymax = transformer.transform_bounds(
                         *in_crs.area_of_use.bounds
                     )
 
                     clipx = partial(np.clip, a_min=xmin, a_max=xmax)
                     clipy = partial(np.clip, a_min=ymin, a_max=ymax)
@@ -850,21 +837,21 @@
                     clipx, clipy = lambda x: x, lambda y: y
                 p = x, y
 
             else:
                 r_crs = self._m.get_crs(radius_crs)
 
                 # transform from crs to the radius_crs
-                t_in_radius = shapes._get_transformer(in_crs, r_crs)
+                t_in_radius = self._m._get_transformer(in_crs, r_crs)
                 # transform from radius_crs to the plot_crs
-                t = shapes._get_transformer(r_crs, self._m.crs_plot)
+                t = self._m._get_transformer(r_crs, self._m.crs_plot)
 
                 # make sure we do not transform out of bounds (if possible)
                 if r_crs.area_of_use is not None:
-                    transformer = shapes._get_transformer(r_crs.geodetic_crs, r_crs)
+                    transformer = self._m._get_transformer(r_crs.geodetic_crs, r_crs)
 
                     xmin, ymin, xmax, ymax = transformer.transform_bounds(
                         *r_crs.area_of_use.bounds
                     )
 
                     clipx = partial(np.clip, a_min=xmin, a_max=xmax)
                     clipy = partial(np.clip, a_min=ymin, a_max=ymax)
@@ -913,15 +900,15 @@
         def _get_polygon_coll(self, x, y, crs, **kwargs):
             verts, mask = self._get_rectangle_verts(
                 x, y, crs, self.radius, self.radius_crs, self.n
             )
 
             # remember masked points
             self._m._data_mask = mask
-            color_and_array = shapes._get_colors_and_array(kwargs, mask)
+            color_and_array = Shapes._get_colors_and_array(kwargs, mask)
 
             coll = PolyCollection(
                 verts=verts,
                 # transOffset=self._m.ax.transData,
                 **color_and_array,
                 **kwargs,
             )
@@ -966,15 +953,15 @@
         def _get_trimesh_coll(self, x, y, crs, **kwargs):
             tri, mask = self._get_trimesh_rectangle_triangulation(
                 x, y, crs, self.radius, self.radius_crs, self.n
             )
             # remember masked points
             self._m._data_mask = mask
 
-            color_and_array = shapes._get_colors_and_array(kwargs, mask)
+            color_and_array = Shapes._get_colors_and_array(kwargs, mask)
 
             def broadcast_colors_and_array(array):
                 if array is None:
                     return
                 # tri-contour meshes need 3 values for each triangle
                 array = np.broadcast_to(array, (3, len(array))).T
                 # we plot 2 triangles per rectangle
@@ -998,15 +985,15 @@
 
         def get_coll(self, x, y, crs, **kwargs):
             if self.mesh is True:
                 return self._get_trimesh_coll(x, y, crs, **kwargs)
             else:
                 return self._get_polygon_coll(x, y, crs, **kwargs)
 
-    class _scatter_points(object):
+    class _ScatterPoints(object):
         name = "scatter_points"
 
         def __init__(self, m):
             self._m = m
 
         def __call__(self, size=None, marker=None):
             """
@@ -1039,32 +1026,32 @@
 
         @property
         def _initargs(self):
             return dict(size=self._size, marker=self._marker)
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, "estimate", "in")
+            radius = Shapes._get_radius(self._m, "estimate", "in")
             return radius
 
         @property
         def radius_crs(self):
             return "in"
 
         def get_coll(self, x, y, crs, **kwargs):
-            color_and_array = shapes._get_colors_and_array(
+            color_and_array = Shapes._get_colors_and_array(
                 kwargs, np.full((x.size,), True)
             )
             color_and_array["c"] = color_and_array["array"]
             coll = self._m.ax.scatter(
                 x, y, s=self._size, marker=self._marker, **color_and_array, **kwargs
             )
             return coll
 
-    class _voronoi_diagram(object):
+    class _VoronoiDiagram(object):
         name = "voronoi_diagram"
 
         def __init__(self, m):
             self._m = m
             self._mask_radius = None
 
         def __call__(self, masked=True, mask_radius=None):
@@ -1101,15 +1088,15 @@
             except AttributeError:
                 s = "voronoi_diagram(mask_radius, masked)"
 
             return s
 
         @property
         def mask_radius(self):
-            r = shapes._get_radius(self._m, self._mask_radius, "out")
+            r = Shapes._get_radius(self._m, self._mask_radius, "out")
             if self._mask_radius is None:
                 return (i * 4 for i in r)
             else:
                 return r
 
         @mask_radius.setter
         def mask_radius(self, val):
@@ -1119,15 +1106,15 @@
             try:
                 from scipy.spatial import Voronoi
                 from itertools import zip_longest
             except ImportError:
                 raise ImportError("'scipy' is required for 'voronoi'!")
 
             # transform from crs to the plot_crs
-            t_in_plot = shapes._get_transformer(self._m.get_crs(crs), self._m.crs_plot)
+            t_in_plot = self._m._get_transformer(self._m.get_crs(crs), self._m.crs_plot)
 
             x0, y0 = t_in_plot.transform(x, y)
 
             datamask = np.isfinite(x0) & np.isfinite(y0)
             [radiusx, radiusy] = radius
 
             maxdist = 2 * np.mean(np.sqrt(radiusx**2 + radiusy**2))
@@ -1169,37 +1156,37 @@
 
             # find the masked points that are not masked by the datamask
             mask2 = ~datamask.copy()
             mask2[np.where(datamask)[0][mask]] = True
             # remember the mask
             self._m._data_mask = mask2
 
-            color_and_array = shapes._get_colors_and_array(
+            color_and_array = Shapes._get_colors_and_array(
                 kwargs, np.logical_and(datamask, mask)
             )
 
             coll = PolyCollection(
                 verts=verts,
                 **color_and_array,
                 # transOffset=self._m.ax.transData,
                 **kwargs,
             )
 
             return coll
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, "estimate", "in")
+            radius = Shapes._get_radius(self._m, "estimate", "in")
             return radius
 
         @property
         def radius_crs(self):
             return "in"
 
-    class _delaunay_triangulation(object):
+    class _DelaunayTriangulation(object):
         name = "delaunay_triangulation"
 
         def __init__(self, m):
             self._m = m
             self._mask_radius = None
 
         def __call__(
@@ -1253,15 +1240,15 @@
             except AttributeError:
                 s = "delaunay_triangulation(mask_radius, mask_radius_crs, masked, flat)"
             return s
 
         @property
         def mask_radius(self):
             if self.masked:
-                r = shapes._get_radius(self._m, self._mask_radius, self.mask_radius_crs)
+                r = Shapes._get_radius(self._m, self._mask_radius, self.mask_radius_crs)
                 if self._mask_radius is None:
                     return (i * 4 for i in r)
                 else:
                     return r
             else:
                 return None
 
@@ -1276,15 +1263,15 @@
             # prepare data
             try:
                 from scipy.spatial import Delaunay
             except ImportError:
                 raise ImportError("'scipy' is required for 'delaunay_triangulation'!")
 
             # transform from crs to the plot_crs
-            t_in_plot = shapes._get_transformer(self._m.get_crs(crs), self._m.crs_plot)
+            t_in_plot = self._m._get_transformer(self._m.get_crs(crs), self._m.crs_plot)
 
             x0, y0 = t_in_plot.transform(x, y)
             datamask = np.isfinite(x0) & np.isfinite(y0)
 
             d = Delaunay(
                 np.column_stack((x0[datamask], y0[datamask])), qhull_options="QJ"
             )
@@ -1336,15 +1323,15 @@
             mask = ~datamask.copy()
             if self.masked:
                 mask[np.where(datamask)[0][list(set(maskedTris.flat))]] = True
 
             # remember the mask
             self._m._data_mask = mask
 
-            color_and_array = shapes._get_colors_and_array(kwargs, datamask)
+            color_and_array = Shapes._get_colors_and_array(kwargs, datamask)
 
             if self.flat == False:
                 for key, val in color_and_array.items():
                     if val is None:
                         continue
 
                     if key == "array":
@@ -1383,22 +1370,22 @@
                     **kwargs,
                 )
 
             return coll
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, "estimate", "in")
+            radius = Shapes._get_radius(self._m, "estimate", "in")
             return radius
 
         @property
         def radius_crs(self):
             return "in"
 
-    class _shade_points(object):
+    class _ShadePoints(object):
         name = "shade_points"
 
         def __init__(self, m):
             self._m = m
 
         def __repr__(self):
             return "Point-based shading with datashader"
@@ -1423,18 +1410,15 @@
             agg_hook : callable, optional
                 A callable that takes the computed aggregate as an argument, and returns
                 another aggregate. This can be used to do preprocessing before the
                 aggregate is converted to an image.
                 The default is None.
             """
 
-            assert _register_datashader(), (
-                "EOmaps: Missing dependency: 'datashader' \n ... please install"
-                + " (conda install -c conda-forge datashader) to use 'shade_points'"
-            )
+            (ds,) = register_modules("datashader")
 
             if aggregator is None:
                 aggregator = ds.mean("val")
             elif isinstance(aggregator, str):
                 aggregator = getattr(ds, aggregator)("val")
 
             if shade_hook is None:
@@ -1463,22 +1447,22 @@
                 aggregator=self.aggregator,
                 shade_hook=self.shade_hook,
                 agg_hook=self.agg_hook,
             )
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, "estimate", "in")
+            radius = Shapes._get_radius(self._m, "estimate", "in")
             return radius
 
         @property
         def radius_crs(self):
             return "in"
 
-    class _shade_raster(object):
+    class _ShadeRaster(object):
         name = "shade_raster"
 
         def __init__(self, m):
             self._m = m
 
         def __repr__(self):
             return "Raster-shading with datashader"
@@ -1523,31 +1507,28 @@
             agg_hook : callable, optional
                 A callable that takes the computed aggregate as an argument, and returns
                 another aggregate. This can be used to do preprocessing before the
                 aggregate is converted to an image.
                 The default is None.
             """
 
-            assert _register_datashader(), (
-                "EOmaps: Missing dependency: 'datashader' \n ... please install"
-                + " (conda install -c conda-forge datashader) to use 'shade_raster'"
-            )
+            (ds,) = register_modules("datashader")
 
             if aggregator is None:
                 aggregator = ds.mean("val")
             if isinstance(aggregator, str):
                 aggregator = getattr(ds, aggregator)("val")
 
             if shade_hook is None:
                 shade_hook = None
 
             if agg_hook is None:
                 pass
 
-            # this might be changed by m._shade_raster depending on the dataset-shape
+            # this might be changed by m._ShadeRaster depending on the dataset-shape
             glyph = None
 
             from . import MapsGrid  # do this here to avoid circular imports!
 
             for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
                 shape = self.__class__(m)
                 shape.aggregator = aggregator
@@ -1563,22 +1544,22 @@
                 aggregator=self.aggregator,
                 shade_hook=self.shade_hook,
                 agg_hook=self.agg_hook,
             )
 
         @property
         def radius(self):
-            radius = shapes._get_radius(self._m, "estimate", "in")
+            radius = Shapes._get_radius(self._m, "estimate", "in")
             return radius
 
         @property
         def radius_crs(self):
             return "in"
 
-    class _raster(object):
+    class _Raster(object):
         name = "raster"
 
         def __init__(self, m):
             self._m = m
             self._radius = None
             self.radius_crs = "in"
 
@@ -1625,15 +1606,15 @@
         @property
         def _initargs(self):
             return dict()
 
         @property
         def radius(self):
             if self._radius is None:
-                radius = shapes._get_radius(self._m, self._radius, self.radius_crs)
+                radius = Shapes._get_radius(self._m, self._radius, self.radius_crs)
                 return radius
 
             return self._radius
 
         def __repr__(self):
             try:
                 s = f"raster(radius={self.radius}, radius_crs={self.radius_crs})"
@@ -1656,19 +1637,19 @@
             y = y - dy
 
             in_crs = self._m.get_crs(crs)
 
             # transform corner-points
             in_crs = self._m.get_crs(crs)
             # transform from crs to the plot_crs
-            t = shapes._get_transformer(in_crs, self._m.crs_plot)
+            t = self._m._get_transformer(in_crs, self._m.crs_plot)
 
             # make sure we do not transform out of bounds (if possible)
             if in_crs.area_of_use is not None:
-                transformer = shapes._get_transformer(in_crs.geodetic_crs, in_crs)
+                transformer = self._m._get_transformer(in_crs.geodetic_crs, in_crs)
 
                 xmin, ymin, xmax, ymax = transformer.transform_bounds(
                     *in_crs.area_of_use.bounds
                 )
 
                 clipx = partial(np.clip, a_min=xmin, a_max=xmax)
                 clipy = partial(np.clip, a_min=ymin, a_max=ymax)
@@ -1702,15 +1683,15 @@
                 y,
                 crs,
             )
 
             # TODO masking is skipped for now...
             self._m._data_mask = None
             # don't use a mask here since we need the full 2D array
-            color_and_array = shapes._get_colors_and_array(
+            color_and_array = Shapes._get_colors_and_array(
                 kwargs, np.full_like(mask, True)
             )
 
             coll = QuadMesh(
                 verts,
                 **color_and_array,
                 **kwargs,
@@ -1730,55 +1711,55 @@
             x, y = np.asanyarray(x), np.asanyarray(y)
             # don't use antialiasing by default since it introduces unwanted
             # transparency for reprojected QuadMeshes!
             kwargs.setdefault("antialiased", False)
 
             return self._get_polygon_coll(x, y, crs, **kwargs)
 
-    @wraps(_scatter_points.__call__)
+    @wraps(_ScatterPoints.__call__)
     def scatter_points(self, *args, **kwargs):
-        shp = self._scatter_points(m=self._m)
+        shp = self._ScatterPoints(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_geod_circles.__call__)
+    @wraps(_GeodCircles.__call__)
     def geod_circles(self, *args, **kwargs):
-        shp = self._geod_circles(m=self._m)
+        shp = self._GeodCircles(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_ellipses.__call__)
+    @wraps(_Ellipses.__call__)
     def ellipses(self, *args, **kwargs):
-        shp = self._ellipses(m=self._m)
+        shp = self._Ellipses(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_rectangles.__call__)
+    @wraps(_Rectangles.__call__)
     def rectangles(self, *args, **kwargs):
-        shp = self._rectangles(m=self._m)
+        shp = self._Rectangles(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_raster.__call__)
+    @wraps(_Raster.__call__)
     def raster(self, *args, **kwargs):
-        shp = self._raster(m=self._m)
+        shp = self._Raster(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_voronoi_diagram.__call__)
+    @wraps(_VoronoiDiagram.__call__)
     def voronoi_diagram(self, *args, **kwargs):
-        shp = self._voronoi_diagram(m=self._m)
+        shp = self._VoronoiDiagram(m=self._m)
         # increase radius margins for voronoi diagrams since
         # outer points are otherwise always masked!
         self._m._data_manager.set_margin_factors(20, 0.1)
 
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_delaunay_triangulation.__call__)
+    @wraps(_DelaunayTriangulation.__call__)
     def delaunay_triangulation(self, *args, **kwargs):
-        shp = self._delaunay_triangulation(m=self._m)
+        shp = self._DelaunayTriangulation(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_shade_points.__call__)
+    @wraps(_ShadePoints.__call__)
     def shade_points(self, *args, **kwargs):
-        shp = self._shade_points(m=self._m)
+        shp = self._ShadePoints(m=self._m)
         return shp.__call__(*args, **kwargs)
 
-    @wraps(_shade_raster.__call__)
+    @wraps(_ShadeRaster.__call__)
     def shade_raster(self, *args, **kwargs):
-        shp = self._shade_raster(m=self._m)
+        shp = self._ShadeRaster(m=self._m)
         return shp.__call__(*args, **kwargs)
```

### Comparing `EOmaps-6.5/eomaps/_webmap.py` & `EOmaps-7.0/eomaps/_webmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
+import logging
+
+import requests
 from functools import lru_cache, partial
 from warnings import warn, filterwarnings, catch_warnings
 from types import SimpleNamespace
 from contextlib import contextmanager
+from urllib3.exceptions import InsecureRequestWarning
+from io import BytesIO
+from pprint import PrettyPrinter
 
 from packaging import version
 
 from PIL import Image
-from io import BytesIO
-from pprint import PrettyPrinter
-
-from cartopy.io.img_tiles import GoogleWTS
-from cartopy import crs as ccrs
 import numpy as np
-
 from pyproj import CRS, Transformer
 
-from owslib.wmts import WebMapTileService
-from owslib.wms import WebMapService
-import requests
-from urllib3.exceptions import InsecureRequestWarning
+import cartopy
+from cartopy import crs as ccrs
+from cartopy.io.img_tiles import GoogleWTS
+from cartopy.io import RasterSource
 
 from .helpers import _sanitize
 
-import cartopy
-from cartopy.io import ogc_clients
-from cartopy.io import RasterSource
-from cartopy.io.ogc_clients import _target_extents
+_log = logging.getLogger(__name__)
 
 
-class _WebMap_layer:
-    # base class for adding methods to the _wms_layer- and wmts_layer objects
+def _add_pending_webmap(m, layer, name):
+    # indicate that there is a pending webmap in the companion-widget editor
+    m.BM._pending_webmaps.setdefault(layer, []).append(name)
+
+
+class _WebMapLayer:
+    # base class for adding methods to the _WMSLayer- and _WMTSLayer objects
     def __init__(self, m, wms, name):
+        from cartopy.io.ogc_clients import _CRS_TO_OGC_SRS
+
         self._m = m
         self.name = name
         self._wms = wms
         self.wms_layer = self._wms.contents[name]
 
         styles = list(self.wms_layer.styles)
         if len(styles) == 0:
@@ -47,40 +51,33 @@
         #    https://github.com/SciTools/cartopy/pull/2138
         if version.parse(cartopy.__version__) < version.parse("0.21.2"):
             # hardcode support for EPSG:3857 == GOOGLE_MERCATOR for now
             # since cartopy hardcoded only  EPSG:900913
             # (see from cartopy.io.ogc_clients import _CRS_TO_OGC_SRS)
             if hasattr(self.wms_layer, "crsOptions"):
                 if "EPSG:3857" in self.wms_layer.crsOptions:
-                    ogc_clients._CRS_TO_OGC_SRS[ccrs.GOOGLE_MERCATOR] = "EPSG:3857"
+                    _CRS_TO_OGC_SRS[ccrs.GOOGLE_MERCATOR] = "EPSG:3857"
                     if "epsg:3857" in self.wms_layer.crsOptions:
-                        ogc_clients._CRS_TO_OGC_SRS[ccrs.GOOGLE_MERCATOR] = "epsg:3857"
+                        _CRS_TO_OGC_SRS[ccrs.GOOGLE_MERCATOR] = "epsg:3857"
 
     @property
     def info(self):
-        """
-        pretty-print the available properties of the wms_layer to the console
-        """
-
+        """Pretty-print the available properties of the wms_layer to the console."""
         txt = ""
         for key, val in self.wms_layer.__dict__.items():
             if not val:
                 continue
             p = PrettyPrinter(depth=1, indent=len(key) + 4, width=60 - len(key))
             s = p.pformat(val).split("\n")
             s = "\n".join([s[0].replace(" " * (len(key) + 3), ""), *s[1:]])
 
             txt += f"{key} : {s}\n"
 
         try:
-
-            if any(("legend" in val for key, val in self.wms_layer.styles.items())):
-                legQ = True
-            else:
-                legQ = False
+            legQ = any(("legend" in val for key, val in self.wms_layer.styles.items()))
         except Exception:
             legQ = False
 
         print(f"\n LEGEND available: {legQ}\n\n" + txt)
 
     def fetch_legend(self, style=None, silent=True):
         if style is None:
@@ -106,26 +103,27 @@
             if not silent:
                 warn("EOmaps: could not fetch the legend")
             return None
         return img
 
     def add_legend(self, style=None, img=None):
         """
-        Add a legend to the plot (if available)
+        Add a legend to the plot (if available).
 
         If you click on the legend you can drag it around!
         The size of the legend can be changed by turning the mouse-wheel
         while clicking on the legend.
 
         Parameters
         ----------
         style : str, optional
             The style to use. The default is "default".
         img : BytesIO
             A pre-fetched legend (if provided the "style" kwarg is ignored!)
+
         Returns
         -------
         legax : matpltolib.axes
             The axes-object.
 
         """
         from matplotlib.transforms import Bbox
@@ -139,30 +137,32 @@
         else:
             legend = img
 
         if legend is not None:
             if not hasattr(self, "_layer"):
                 # use the currently active layer if the webmap service has not yet
                 # been added to the map
-                print("EOmaps: The WebMap for the legend is not yet added to the map!")
+                _log.warning(
+                    "EOmaps: The WebMap for the legend is not yet added to the map!"
+                )
                 self._layer = self._m.BM._bg_layer
 
             axpos = self._m.ax.get_position()
             legax = self._m.f.add_axes((axpos.x0, axpos.y0, 0.25, 0.5))
 
             legax.patch.set_visible(False)
             legax.tick_params(
                 left=False, labelleft=False, bottom=False, labelbottom=False
             )
             legax.set_frame_on(False)
             legax.set_aspect(1, anchor="SW")
             legax.imshow(legend)
 
             # hide the legend if the corresponding layer is not active at the moment
-            if self._layer not in self._m.BM._bg_layer.split("|"):
+            if self._layer not in self._m.BM._get_layers_alphas()[0]:
                 legax.set_visible(False)
 
             self._m.BM.add_artist(legax, self._layer)
 
             def cb_move(event):
                 if not self._legend_picked:
                     return
@@ -278,17 +278,18 @@
         """
 
         bbox = getattr(self.wms_layer, "boundingBox", None)
         try:
             (x0, y0, x1, y1, crs) = bbox
             incrs = CRS.from_user_input(crs)
         except Exception:
-            print(
+            _log.error(
                 "EOmaps: could not determine bbox from 'boundingBox'... "
-                + "defaulting to 'boundingBoxWGS84'"
+                + "defaulting to 'boundingBoxWGS84'",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
             )
             (x0, y0, x1, y1) = getattr(self.wms_layer, "boundingBoxWGS84", None)
             incrs = CRS.from_user_input(4326)
 
         if shrink:
             assert shrink >= 0, "EOmaps: shrink must be > 0!"
             assert shrink < 1, "EOmaps: shrink must be < 1!"
@@ -322,20 +323,19 @@
             self._style = style[0]
         else:
             style = [self._style]
 
         return style
 
 
-class _wmts_layer(_WebMap_layer):
+class _WMTSLayer(_WebMapLayer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        pass
 
-    def __call__(self, layer=None, zorder=-5, alpha=1, **kwargs):
+    def __call__(self, layer=None, zorder=0, alpha=1, **kwargs):
         """
         Add the WMTS layer to the map
 
         Parameters
         ----------
         layer : int, str or None, optional
             The name of the layer at which map-features are plotted.
@@ -371,25 +371,26 @@
 
         for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
             if layer is None:
                 self._layer = m.layer
             else:
                 self._layer = layer
 
-            if self._layer == "all" or self._layer in m.BM.bg_layer.split("|"):
+            if self._layer == "all" or self._layer in m.BM._get_layers_alphas()[0]:
                 # add the layer immediately if the layer is already active
                 self._do_add_layer(
                     self._m,
                     layer=self._layer,
                     wms_kwargs=kwargs,
                     zorder=zorder,
                     alpha=alpha,
                 )
             else:
                 # delay adding the layer until it is effectively activated
+                _add_pending_webmap(self._m, self._layer, self.name)
                 self._m.BM.on_layer(
                     func=partial(
                         self._do_add_layer,
                         wms_kwargs=kwargs,
                         zorder=zorder,
                         alpha=alpha,
                     ),
@@ -407,37 +408,38 @@
         from cartopy.io.ogc_clients import WMTSRasterSource
 
         wms = WMTSRasterSource(wms, layers, gettile_extra_kwargs=wms_kwargs)
 
         # Allow a fail-fast error if the raster source cannot provide
         # images in the current projection.
         wms.validate_projection(ax.projection)
-        img = SlippyImageArtist_NEW(ax, wms, **kwargs)
+        img = SlippyImageArtistNew(ax, wms, **kwargs)
         with ax.hold_limits():
             ax.add_image(img)
         return img
 
     def _do_add_layer(self, m, layer, **kwargs):
         # actually add the layer to the map.
-        print(f"EOmaps: Adding wmts-layer: {self.name}")
+        _log.info(f"EOmaps: Adding wmts-layer: {self.name}")
 
         # use slightly adapted implementation of cartopy's ax.add_wmts
         art = self._add_wmts(
             m.ax, self._wms, self.name, interpolation="spline36", **kwargs
         )
 
+        art.set_label(f"WebMap service: {self.name}")
+
         m.BM.add_bg_artist(art, layer=layer)
 
 
-class _wms_layer(_WebMap_layer):
+class _WMSLayer(_WebMapLayer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        pass
 
-    def __call__(self, layer=None, zorder=-5, alpha=1, **kwargs):
+    def __call__(self, layer=None, zorder=0, alpha=1, **kwargs):
         """
         Add the WMS layer to the map
 
         Parameters
         ----------
         layer : int, str or None, optional
             The name of the layer at which map-features are plotted.
@@ -485,14 +487,15 @@
                     layer=self._layer,
                     wms_kwargs=kwargs,
                     zorder=zorder,
                     alpha=alpha,
                 )
             else:
                 # delay adding the layer until it is effectively activated
+                _add_pending_webmap(self._m, self._layer, self.name)
                 m.BM.on_layer(
                     func=partial(
                         self._do_add_layer,
                         wms_kwargs=kwargs,
                         zorder=zorder,
                         alpha=alpha,
                     ),
@@ -510,15 +513,15 @@
     def _add_wms(ax, wms, layers, wms_kwargs=None, **kwargs):
         # fix of native-crs identifications for older cartopy versions
         # ...ported to cartopy >= 0.21.2:
         #    https://github.com/SciTools/cartopy/pull/2136
         if version.parse(cartopy.__version__) < version.parse("0.21.2"):
             from cartopy.io.ogc_clients import WMSRasterSource
 
-            class WMSRasterSource_NEW(WMSRasterSource):
+            class WMSRasterSourceNew(WMSRasterSource):
 
                 # Temporary fix for WMS services provided in a known srs but not
                 # in the srs of the axis
                 # (for example ESA_WorldCover.add_layer.WORLDCOVER_2020_MAP())
                 def _native_srs(self, *args, **kwargs):
                     native_srs = super()._native_srs(*args, **kwargs)
 
@@ -536,54 +539,56 @@
                         )
 
                         if native_OK:
                             return native_srs
                         else:
                             return None
 
-            wms = WMSRasterSource_NEW(wms, layers, getmap_extra_kwargs=wms_kwargs)
+            wms = WMSRasterSourceNew(wms, layers, getmap_extra_kwargs=wms_kwargs)
         else:
             wms = WMSRasterSource(wms, layers, getmap_extra_kwargs=wms_kwargs)
 
         # Allow a fail-fast error if the raster source cannot provide
         # images in the current projection.
         wms.validate_projection(ax.projection)
-        img = SlippyImageArtist_NEW(ax, wms, **kwargs)
+        img = SlippyImageArtistNew(ax, wms, **kwargs)
         with ax.hold_limits():
             ax.add_image(img)
 
         return img
 
     def _do_add_layer(self, m, layer, **kwargs):
         # actually add the layer to the map.
-        print(f"EOmaps: ... adding wms-layer {self.name}")
+        _log.info(f"EOmaps: ... adding wms-layer {self.name}")
 
         # use slightly adapted implementation of cartopy's ax.add_wms
         art = self._add_wms(
             m.ax, self._wms, self.name, interpolation="spline36", **kwargs
         )
 
+        art.set_label(f"WebMap service: {self.name}")
+
         m.BM.add_bg_artist(art, layer=layer)
 
 
-class _WebServiec_collection(object):
+class _WebServiceCollection:
     def __init__(self, m, service_type="wmts", url=None):
         self._m = m
         self._service_type = service_type
         if url is not None:
             self._url = url
 
     def __getitem__(self, key):
         return self.add_layer.__dict__[key]
 
     def __repr__(self):
         if hasattr(self, "info"):
             return self.info
-        else:
-            return object.__repr__(self)
+
+        return object.__repr__(self)
 
     @property
     @lru_cache()
     def layers(self):
         """
         get a list of all available layers
         """
@@ -606,40 +611,48 @@
 
         """
         return [i for i in self.layers if name.lower() in i.lower()]
 
     @staticmethod
     def _get_wmts(url):
         # TODO expose useragent
+
+        # lazy import used to avoid long import times
+        from owslib.wmts import WebMapTileService
+
         return WebMapTileService(url)
 
     @staticmethod
     def _get_wms(url):
         # TODO expose useragent
+
+        # lazy import used to avoid long import times
+        from owslib.wms import WebMapService
+
         return WebMapService(url)
 
     @property
     @lru_cache()
     def add_layer(self):
         if self._service_type == "wmts":
             wmts = self._get_wmts(self._url)
             layers = dict()
             for key in wmts.contents.keys():
-                layers[_sanitize(key)] = _wmts_layer(self._m, wmts, key)
+                layers[_sanitize(key)] = _WMTSLayer(self._m, wmts, key)
 
         elif self._service_type == "wms":
             wms = self._get_wms(self._url)
             layers = dict()
             for key in wms.contents.keys():
-                layers[_sanitize(key)] = _wms_layer(self._m, wms, key)
+                layers[_sanitize(key)] = _WMSLayer(self._m, wms, key)
 
         return SimpleNamespace(**layers)
 
 
-class REST_API_services:
+class RestApiServices:
     def __init__(
         self, m, url, name, service_type="wmts", layers=None, _params={"f": "pjson"}
     ):
         """
         fetch layers from a Rest API
 
         Parameters
@@ -659,20 +672,20 @@
             If None or empty, layers are immediately fetched!
             The default is None.
         _params : set, optional
             additional parameters passed to the API. The default is {"f": "pjson"}.
 
         """
         self._m = m
-        self._REST_url = url
+        self._rest_url = url
         self._name = name
         self._service_type = service_type
         self._params = _params
         self._fetched = False
-        self._REST_API = None
+        self._rest_api = None
 
         if layers is None:
             layers = set()
         self._layers = layers
 
         for i in self._layers:
             setattr(self, i, "NOT FOUND")
@@ -693,57 +706,56 @@
 
     def _fetch_services(self):
         if self._fetched:
             return
         # set _fetched to True immediately to avoid issues in __getattribute__
         self._fetched = True
 
-        if self._REST_API is None:
-            print(f"EOmaps: ... fetching services for '{self._name}'")
-            self._REST_API = _REST_API(self._REST_url, _params=self._params)
+        if self._rest_api is None:
+            _log.info(f"EOmaps: ... fetching services for '{self._name}'")
+            self._rest_api = _RestApi(self._rest_url, _params=self._params)
 
             found_folders = set()
-            for foldername, services in self._REST_API._structure.items():
+            for foldername, services in self._rest_api._structure.items():
                 setattr(
                     self,
                     foldername,
-                    _multi_REST_WMSservice(
+                    _MultiRestWmsService(
                         m=self._m,
                         services=services,
                         service_type=self._service_type,
-                        url=self._REST_url,
+                        url=self._rest_url,
                     ),
                 )
                 found_folders.add(foldername)
 
             new_layers = found_folders - self._layers
             if len(new_layers) > 0:
-                print(f"EOmaps: ... found some new folders: {new_layers}")
+                _log.info(f"EOmaps: ... found some new folders: {new_layers}")
 
             invalid_layers = self._layers - found_folders
             if len(invalid_layers) > 0:
-                print(f"EOmaps: ... could not find the folders: {invalid_layers}")
+                _log.info(f"EOmaps: ... could not find the folders: {invalid_layers}")
             for i in invalid_layers:
                 delattr(self, i)
 
-            print("EOmaps: done!")
+            _log.info("EOmaps: done!")
 
 
-class _REST_WMSservice(_WebServiec_collection):
+class _RestWmsService(_WebServiceCollection):
     def __init__(self, service, s_name, s_type, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._service = service
         self._s_name = s_name
         self._s_type = s_type
 
         self._layers = None
 
     @property
     def _url(self):
-        print(self._s_name)
         url = "/".join([self._service, self._s_name, self._s_type])
 
         if self._service_type == "wms":
             suffix = "/WMSServer?request=GetCapabilities&service=WMS"
             WMSurl = url.replace("/rest/", "/") + suffix
             if requests.get(WMSurl).status_code == 200:
                 url = WMSurl
@@ -769,64 +781,66 @@
         self._layers = dict()
         url = self._url
         if url is not None:
             if self._service_type == "wms":
                 wms = self._get_wms(url)
                 layer_names = list(wms.contents.keys())
                 for lname in layer_names:
-                    self._layers["layer_" + _sanitize(lname)] = _wms_layer(
+                    self._layers["layer_" + _sanitize(lname)] = _WMSLayer(
                         self._m, wms, lname
                     )
             elif self._service_type == "wmts":
                 wmts = self._get_wmts(url)
                 layer_names = list(wmts.contents.keys())
                 for lname in layer_names:
-                    self._layers["layer_" + _sanitize(lname)] = _wmts_layer(
+                    self._layers["layer_" + _sanitize(lname)] = _WMTSLayer(
                         self._m, wmts, lname
                     )
             elif self._service_type == "xyz":
-                self._layers["xyz_layer"] = _xyz_tile_service(
+                self._layers["xyz_layer"] = _XyzTileService(
                     self._m, url, 19, "xyz_layer"
                 )
 
     @property
     @lru_cache()
     def add_layer(self):
         self._fetch_layers()
         if len(self._layers) == 0:
-            print(f"EOmaps: found no {self._service_type} layers for {self._s_name}")
+            _log.error(
+                f"EOmaps: found no {self._service_type} layers for {self._s_name}"
+            )
             return
-        else:
-            return SimpleNamespace(**self._layers)
+
+        return SimpleNamespace(**self._layers)
 
 
-class _multi_REST_WMSservice:
+class _MultiRestWmsService:
     def __init__(self, m, services, service_type, url, *args, **kwargs):
         self._m = m
         self._services = services
         self._service_type = service_type
         self._url = url
 
         self._fetch_services()
 
     @lru_cache()
     def _fetch_services(self):
         for (s_name, s_type) in self._services:
-            wms_layer = _REST_WMSservice(
+            wms_layer = _RestWmsService(
                 m=self._m,
                 service=self._url,
                 s_name=s_name,
                 s_type=s_type,
                 service_type=self._service_type,
             )
 
             setattr(self, _sanitize(s_name), wms_layer)
 
 
-class _REST_API(object):
+class _RestApi(object):
     # adapted from https://gis.stackexchange.com/a/113213
     def __init__(self, url, _params={"f": "pjson"}):
         self._url = url
         self._params = _params
 
         self._structure = self._get_structure(self._url)
 
@@ -890,28 +904,29 @@
 
         if isinstance(self._url, str):
             return self._url.format(x=x, y=y, z=z)
         if callable(self._url):
             return self._url(x=x, y=y, z=z)
 
 
-class xyzRasterSource(RasterSource):
-    """
-    A RasterSource that can be used with a SlippyImageArtist to fetch tiles.
-    """
+class XyzRasterSource(RasterSource):
+    """RasterSource that can be used with a SlippyImageArtist to fetch tiles."""
 
     def __init__(self, url, crs, maxzoom=19, transparent=True):
         """
+        Class to fetch tiles from xyz services with a SlippyImageArtist.
+
         Parameters
         ----------
         service: string or WebMapService instance
             The WebMapService instance, or URL of a WMS service,
             from whence to retrieve the image.
         layers: string or list of strings
             The name(s) of layers to use from the WMS service.
+
         """
         self.url = url
 
         self._crs = crs
         self._maxzoom = maxzoom
 
         if transparent is True:
@@ -974,14 +989,15 @@
         wms_srs,
         wms_extent,
         output_proj,
         output_extent,
         target_resolution,
     ):
         import shapely.geometry as sgeom
+        from cartopy.io.ogc_clients import LocatedImage, _target_extents
 
         x0, x1, y0, y1 = wms_extent
 
         domain = sgeom.box(x0, y0, x1, y1)
 
         img, extent, origin = self._factory.image_for_domain(
             domain,
@@ -1008,15 +1024,15 @@
                 # It is implicitly assumed by the regridding operation that the
                 # origin of the image is 'lower', so simply adjust for that
                 # here.
                 img = img[::-1]
 
             # reproject the extent to the output-crs
 
-            target_extent = ogc_clients._target_extents(extent, wms_proj, output_proj)
+            target_extent = _target_extents(extent, wms_proj, output_proj)
             if len(target_extent) > 0:
                 target_extent = target_extent[0]
             else:
                 # TODO properly check what's going on here
                 # (only relevant for Equi7Grid projections if a xyz-layer is added
                 # without zooming first)
                 target_extent = output_extent
@@ -1039,19 +1055,19 @@
                 mask_extrapolated=True,
             )
 
             if origin == "upper":
                 # revert to the initial origin
                 img = img[::-1]
 
-        from cartopy.io.ogc_clients import LocatedImage
-
         return LocatedImage(img, extent)
 
     def fetch_raster(self, projection, extent, target_resolution):
+        from cartopy.io.ogc_clients import _target_extents
+
         target_resolution = [np.ceil(val) for val in target_resolution]
 
         if projection == self._crs:
             wms_extents = [extent]
         else:
             # Calculate the bounding box(es) in WMS projection.
             wms_extents = _target_extents(extent, projection, self._crs)
@@ -1068,40 +1084,36 @@
             )
             if img:
                 located_images.append(img)
 
         return located_images
 
 
-class _xyz_tile_service:
-    """
-    general class for using x/y/z tile-service urls as WebMap layers
-    """
+class _XyzTileService:
+    """General class for using x/y/z tile-service urls as WebMap layers."""
 
     def __init__(self, m, url, maxzoom=19, name=None):
         self._m = m
         self._factory = None
         self._artist = None
 
         self.url = url
         self._maxzoom = maxzoom
         self.name = name
 
     def _reinit(self, m):
-        return _xyz_tile_service(
-            m, url=self.url, maxzoom=self._maxzoom, name=self._name
-        )
+        return _XyzTileService(m, url=self.url, maxzoom=self._maxzoom, name=self.name)
 
     def __call__(
         self,
         layer=None,
         transparent=False,
         alpha=1,
         interpolation="spline36",
-        zorder=-5,
+        zorder=0,
         **kwargs,
     ):
         """
         Parameters
         ----------
         layer : int, str or None, optional
             The name of the layer at which map-features are plotted.
@@ -1149,56 +1161,59 @@
         else:
 
             kwargs.setdefault("interpolation", interpolation)
             kwargs.setdefault("zorder", zorder)
             kwargs.setdefault("alpha", alpha)
             kwargs.setdefault("origin", "lower")
 
-            if self._layer == "all" or self._m.BM.bg_layer == self._layer:
+            if self._layer in ["all", self._m.BM.bg_layer]:
                 # add the layer immediately if the layer is already active
                 self._do_add_layer(self._m, layer=self._layer, **kwargs)
             else:
                 # delay adding the layer until it is effectively activated
+                _add_pending_webmap(self._m, self._layer, self.name)
                 self._m.BM.on_layer(
                     func=partial(self._do_add_layer, **kwargs),
                     layer=self._layer,
                     persistent=False,
                     m=self._m,
                 )
 
     def _do_add_layer(self, m, layer, **kwargs):
         # actually add the layer to the map.
-        print(f"EOmaps: ... adding wms-layer {self.name}")
+        _log.info(f"EOmaps: ... adding wms-layer {self.name}")
 
-        self._raster_source = xyzRasterSource(
+        self._raster_source = XyzRasterSource(
             self.url,
             crs=ccrs.GOOGLE_MERCATOR,
             maxzoom=self._maxzoom,
             transparent=self._transparent,
         )
 
         # avoid using "add_raster" and use the subclassed SlippyImageArtist
         # self._artist = self._m.ax.add_raster(self._raster_source, **self.kwargs)
 
         # ------- following lines are equivalent to ax.add_raster
         #         (only SlippyImageArtist has been subclassed)
 
         self._raster_source.validate_projection(m.ax.projection)
-        img = SlippyImageArtist_NEW(m.ax, self._raster_source, **kwargs)
+        img = SlippyImageArtistNew(m.ax, self._raster_source, **kwargs)
         with self._m.ax.hold_limits():
             m.ax.add_image(img)
         self._artist = img
 
+        self._artist.set_label(f"WebMap service: {self.name}")
+
         m.BM.add_bg_artist(self._artist, layer=layer)
 
 
-class _xyz_tile_service_nonearth(_xyz_tile_service):
+class _XyzTileServiceNonEarth(_XyzTileService):
     def __call__(self, *args, **kwargs):
-        print(
-            f"EOmaps WARNING: The WebMap service '{self.name}' shows images from a "
+        _log.info(
+            f"EOmaps: The WebMap service '{self.name}' shows images from a "
             "different celestrial body projected to an earth-based crs! "
             "Units used in scalebars, geod_crices etc. represent earth-based units!"
         )
         super().__call__(*args, **kwargs)
 
 
 # ------------------------------------------------------------------------------
@@ -1223,45 +1238,44 @@
     - The axis that shows the wms-service is re-sized
     - The figure is re-sized
     - The figure dpi changes
     - The figure is saved with a dpi-value other than the current figure dpi
 
     By default, WebMap services are dynamically re-fetched on any size-change.
     (this also means that saving figures at high dpi-values will cause a
-     re-fetch of webmap services which might result in a different look
-     of the exported image!)
+    re-fetch of webmap services which might result in a different look
+    of the exported image!)
 
     Note
     ----
     This will set the GLOBAL behavior for ALL EOmaps WebMap services!
 
     Parameters
     ----------
     refetch : bool
 
         - If True: WebMap services are dynamically re-fetched on size changes
         - If False: WebMap services are only re-fetched if the axis-extent
           changes.
     """
-    SlippyImageArtist_NEW._refetch_on_size_change = refetch
+    SlippyImageArtistNew._refetch_on_size_change = refetch
 
 
 @contextmanager
 def _cx_refetch_wms_on_size_change(refetch):
-    val = SlippyImageArtist_NEW._refetch_on_size_change
+    val = SlippyImageArtistNew._refetch_on_size_change
 
     try:
-        SlippyImageArtist_NEW._refetch_on_size_change = refetch
+        SlippyImageArtistNew._refetch_on_size_change = refetch
         yield
     finally:
-        SlippyImageArtist_NEW._refetch_on_size_change = val
-
+        SlippyImageArtistNew._refetch_on_size_change = val
 
-class SlippyImageArtist_NEW(AxesImage):
 
+class SlippyImageArtistNew(AxesImage):
     """
     A subclass of :class:`~matplotlib.image.AxesImage` which provides an
     interface for getting a raster from the given object with interactive
     slippy map type functionality.
 
     Kwargs are passed to the AxesImage constructor.
 
@@ -1338,25 +1352,32 @@
                     # (otherwise the path might still correspond to a previous extent)
                     clippath._adjust_location()
 
                     self.set_clip_path(
                         clippath.get_path(),
                         transform=self.axes.projection._as_mpl_transform(self.axes),
                     )
-                except:
-                    print("EOmaps: unable to set clippath for WMS images")
+                except Exception:
+                    _log.error(
+                        "EOmaps: unable to set clippath for WMS images",
+                        exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+                    )
 
                 with ax.hold_limits():
                     self.set_array(img)
                     self.set_extent(extent)
                     super().draw(renderer, *args, **kwargs)
             self.stale = False
 
         except Exception:
-            print("EOmaps: ... could not fetch WebMap service")
+            _log.error(
+                "EOmaps: ... could not fetch WebMap service",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
+
             if self in self.axes._mouseover_set:
                 self.axes._mouseover_set.remove(self)
 
     def can_composite(self):
         # As per https://github.com/SciTools/cartopy/issues/689, disable
         # compositing multiple raster sources.
         return False
```

### Comparing `EOmaps-6.5/eomaps/_webmap_containers.py` & `EOmaps-7.0/eomaps/webmap_containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+"""Collection of WebMap services."""
+
+import logging
 from functools import lru_cache
 from textwrap import dedent
-
 from types import SimpleNamespace
 
+_log = logging.getLogger(__name__)
+
 
-def combdoc(*args):
+def _combdoc(*args):
     """Combine docstrings."""
     return "\n".join(dedent(str(i)) for i in args)
 
 
 def _register_imports():
-    global _WebServiec_collection
-    global REST_API_services
-    global _xyz_tile_service
-    global _xyz_tile_service_nonearth
+    global _WebServiceCollection
+    global RestApiServices
+    global _XyzTileService
+    global _XyzTileServiceNonEarth
 
     from ._webmap import (
-        _WebServiec_collection,
-        REST_API_services,
-        _xyz_tile_service,
-        _xyz_tile_service_nonearth,
+        _WebServiceCollection,
+        RestApiServices,
+        _XyzTileService,
+        _XyzTileServiceNonEarth,
     )
 
 
-class wms_container(object):
+class WebMapContainer(object):
     """
     A collection of open-access WebMap services that can be added to the maps.
 
     Layers can be added in 2 ways (either with . access or with [] access):
         >>> m.add_wms.< SERVICE > ... .add_layer.<LAYER-NAME>(**kwargs)
         >>> m.add_wms.< SERVICE > ... [<LAYER-NAME>](**kwargs)
 
@@ -77,15 +81,15 @@
 
         # since this is not an ArcGIS REST API it needs some special treatment...
         def __init__(self, m, service_type="wms"):
             self._m = m
             self._service_type = service_type
             self._fetched = False
 
-            # default layers (see REST_API_services for details)
+            # default layers (see RestApiServices for details)
             self._layers = {
                 "nitrogen",
                 "phh2o",
                 "soc",
                 "silt",
                 "ocd",
                 "cfvo",
@@ -107,15 +111,15 @@
             # fetch layers on first attempt to get a non-private attribute
             if not self._fetched:
                 self._fetch_services()
 
             return object.__getattribute__(self, name)
 
         def _fetch_services(self):
-            print("EOmaps: fetching IRIS layers...")
+            _log.info("EOmaps: fetching IRIS layers...")
 
             import requests
             import json
 
             if self._fetched:
                 return
             # set _fetched to True immediately to avoid issues in __getattribute__
@@ -125,28 +129,28 @@
                 "https://rest.isric.org/soilgrids/v2.0/properties/layers"
             )
             _layers = json.loads(layers.content.decode())["layers"]
 
             found_layers = set()
             for i in _layers:
                 name = i["property"]
-                setattr(self, name, _WebServiec_collection(self._m, service_type="wms"))
+                setattr(self, name, _WebServiceCollection(self._m, service_type="wms"))
                 getattr(
                     self, name
                 )._url = f"https://maps.isric.org/mapserv?map=/map/{name}.map"
 
                 found_layers.add(name)
 
             new_layers = found_layers - self._layers
             if len(new_layers) > 0:
-                print(f"EOmaps: ... found some new folders: {new_layers}")
+                _log.info(f"EOmaps: ... found some new folders: {new_layers}")
 
             invalid_layers = self._layers - found_layers
             if len(invalid_layers) > 0:
-                print(f"EOmaps: ... could not find the folders: {invalid_layers}")
+                _log.info(f"EOmaps: ... could not find the folders: {invalid_layers}")
             for i in invalid_layers:
                 delattr(self, i)
 
             self._layers = found_layers
 
     @property
     @lru_cache()
@@ -181,21 +185,21 @@
         Creative Commons Attribution 4.0 International License.
 
         Publications, models and data products that make use of these
         datasets must include proper acknowledgement, including citing the
         datasets and the journal article as in the following citation.
         """
         if self._m.parent._preferred_wms_service == "wms":
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://services.terrascope.be/wms/v2",
             )
         elif self._m.parent._preferred_wms_service == "wmts":
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wmts",
                 url="https://services.terrascope.be/wmts/v2",
             )
 
         WMS.__doc__ = type(self).ESA_WorldCover.__doc__
         return WMS
@@ -232,15 +236,15 @@
 
         "Imagery reproduced from the GEBCO_2021 Grid, GEBCO Compilation Group (2021)
         GEBCO 2021 Grid (doi:10.5285/c6612cbe-50b3-0cff-e053-6c86abc09f8f)"
 
         (check: https://www.gebco.net/ for full details)
 
         """
-        WMS = _WebServiec_collection(
+        WMS = _WebServiceCollection(
             m=self._m,
             service_type="wms",
             url="https://www.gebco.net/data_and_products/gebco_web_services/web_map_service/mapserv?request=getcapabilities&service=wms&version=1.1.1",
         )
 
         WMS.__doc__ = type(self).GEBCO.__doc__
         return WMS
@@ -273,15 +277,15 @@
         R. Zemsky (2009), Global Multi-Resolution Topography (GMRT) synthesis data set,
         Geochem. Geophys. Geosyst., 10, Q03014, doi:10.1029/2008GC002332.
         Data doi: 10.1594/IEDA.100001
 
         (check: https://gmrt.org/about/terms_of_use.php for full details)
 
         """
-        WMS = _WebServiec_collection(
+        WMS = _WebServiceCollection(
             m=self._m,
             service_type="wms",
             url="https://www.gmrt.org/services/mapserver/wms_merc?request=GetCapabilities&service=WMS&version=1.3.0",
         )
 
         WMS.__doc__ = type(self).GMRT.__doc__
         return WMS
@@ -298,15 +302,15 @@
         Note
         ----
         **LICENSE-info (without any warranty for correctness!!)**
 
         (check: https://glad.earthengine.app/ for full details)
 
         """
-        WMS = _WebServiec_collection(
+        WMS = _WebServiceCollection(
             m=self._m,
             service_type="wms",
             url="https://glad.umd.edu/mapcache/?SERVICE=WMS",
         )
 
         WMS.__doc__ = type(self).GLAD.__doc__
         return WMS
@@ -339,15 +343,15 @@
         We acknowledge the use of imagery provided by services from NASA's
         Global Imagery Browse Services (GIBS), part of NASA's Earth Observing
         System Data and Information System (EOSDIS).
         """
         if self._m._preferred_wms_service == "wms":
             WMS = self._NASA_GIBS(self._m)
         elif self._m._preferred_wms_service == "wmts":
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wmts",
                 url="https://gibs.earthdata.nasa.gov/wmts/epsg4326/all/1.0.0/WMTSCapabilities.xml",
             )
 
         WMS.__doc__ = type(self).NASA_GIBS.__doc__
         return WMS
@@ -356,48 +360,48 @@
         # WMS links for NASA GIBS
         def __init__(self, m):
             self._m = m
 
         @property
         @lru_cache()
         def EPSG_4326(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://gibs.earthdata.nasa.gov/wms/epsg4326/best/wms.cgi?SERVICE=WMS&REQUEST=GetCapabilities&VERSION=1.1.1",
             )
             WMS.__doc__ = type(self).__doc__
             return WMS
 
         @property
         @lru_cache()
         def EPSG_3857(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://gibs.earthdata.nasa.gov/wms/epsg3857/best/wms.cgi?SERVICE=WMS&REQUEST=GetCapabilities&VERSION=1.1.1",
             )
             WMS.__doc__ = type(self).__doc__
             return WMS
 
         @property
         @lru_cache()
         def EPSG_3413(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://gibs.earthdata.nasa.gov/wms/epsg3413/best/wms.cgi?SERVICE=WMS&REQUEST=GetCapabilities&VERSION=1.1.1",
             )
             WMS.__doc__ = type(self).__doc__
             return WMS
 
         @property
         @lru_cache()
         def EPSG_3031(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://gibs.earthdata.nasa.gov/wms/epsg3031/best/wms.cgi?SERVICE=WMS&REQUEST=GetCapabilities&VERSION=1.1.1",
             )
             WMS.__doc__ = type(self).__doc__
             return WMS
 
@@ -468,58 +472,58 @@
             self.OSM_openrailwaymap = self._OSM_openrailwaymap(self._m)
             self.OSM_cartodb = self._OSM_cartodb(self._m)
 
         class _OSM:
             def __init__(self, m):
                 self._m = m
 
-                self.default = _xyz_tile_service(
+                self.default = _XyzTileService(
                     self._m,
                     "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
                     name="OSM_default",
                 )
-                self.default.__doc__ = combdoc(
+                self.default.__doc__ = _combdoc(
                     """
                     OpenStreetMap's standard tile layer
                     https://www.openstreetmap.org/
 
                     Note
                     ----
                     **LICENSE-info (without any warranty for correctness!!)**
 
                     check: https://operations.osmfoundation.org/policies/tiles/
                     """,
                     self.default.__call__.__doc__,
                 )
 
-                self.default_german = _xyz_tile_service(
+                self.default_german = _XyzTileService(
                     self._m,
                     "https://tile.openstreetmap.de/{z}/{x}/{y}.png",
                     name="OSM_default_german",
                 )
-                self.default_german.__doc__ = combdoc(
+                self.default_german.__doc__ = _combdoc(
                     """
                     German fork of OpenStreetMap's standard tile layer
                     https://www.openstreetmap.de/
 
                     Note
                     ----
                     **LICENSE-info (without any warranty for correctness!!)**
 
                     check: https://www.openstreetmap.de/germanstyle.html
                     """,
                     self.default_german.__call__.__doc__,
                 )
 
-                self.humanitarian = _xyz_tile_service(
+                self.humanitarian = _XyzTileService(
                     self._m,
                     "https://a.tile.openstreetmap.fr/hot/{z}/{x}/{y}.png",
                     name="OSM_humanitarian",
                 )
-                self.humanitarian.__doc__ = combdoc(
+                self.humanitarian.__doc__ = _combdoc(
                     """
                     OpenStreetMap's Humanitarian style
 
                     Focuses on the developing countries with an emphasis on features
                     related to development and humanitarian work.
 
                     Good contrasting style in terms of overall colour choices. Terrain
@@ -539,21 +543,21 @@
 
                     - https://operations.osmfoundation.org/policies/tiles/
                     - https://www.openstreetmap.fr/fonds-de-carte/
                     """,
                     self.humanitarian.__call__.__doc__,
                 )
 
-                self.OpenTopoMap = _xyz_tile_service(
+                self.OpenTopoMap = _XyzTileService(
                     m=self._m,
                     url="https://c.tile.opentopomap.org/{z}/{x}/{y}.png",
                     maxzoom=16,
                     name="OSM_OpenTopoMap",
                 )
-                self.OpenTopoMap.__doc__ = combdoc(
+                self.OpenTopoMap.__doc__ = _combdoc(
                     """
                     A project aiming at rendering topographic maps from OSM
                     and SRTM data. The map style is similar to some official
                     German or French topographic maps, such as TK50 or TOP 25.
                     https://www.opentopomap.org/
 
                     Note
@@ -561,21 +565,21 @@
                     **LICENSE-info (without any warranty for correctness!!)**
 
                     check: https://wiki.openstreetmap.org/wiki/OpenTopoMap
                     """,
                     self.OpenTopoMap.__call__.__doc__,
                 )
 
-                self.OpenRiverboatMap = _xyz_tile_service(
+                self.OpenRiverboatMap = _XyzTileService(
                     m=self._m,
                     url="https://a.tile.openstreetmap.fr/openriverboatmap/{z}/{x}/{y}.png",
                     maxzoom=16,
                     name="OSM_OpenRiverboatMap",
                 )
-                self.OpenRiverboatMap.__doc__ = combdoc(
+                self.OpenRiverboatMap.__doc__ = _combdoc(
                     """
                     Open Riverboat Map plans to make an open source CartoCSS map style
                     of navigable waterways, on top of OpenStreetMap project.
 
                     https://github.com/tilery/OpenRiverboatMap
 
                     Note
@@ -588,21 +592,21 @@
                         - https://openstreetmap.fr
                         - https://operations.osmfoundation.org/policies/tiles/
 
                     """,
                     self.OpenRiverboatMap.__call__.__doc__,
                 )
 
-                self.OpenSeaMap = _xyz_tile_service(
+                self.OpenSeaMap = _XyzTileService(
                     m=self._m,
                     url="http://tiles.openseamap.org/seamark/{z}/{x}/{y}.png",
                     maxzoom=16,
                     name="OSM_OpenSeaMap",
                 )
-                self.OpenSeaMap.__doc__ = combdoc(
+                self.OpenSeaMap.__doc__ = _combdoc(
                     """
                     OpenSeaMap is an open source, worldwide project to create a free
                     nautical chart. There is a great need for freely accessible maps
                     for navigation purposes, so in 2009, OpenSeaMap came into life.
                     The goal of OpenSeaMap is to record interesting and useful nautical
                     information for the sailor which is then incorporated into a free
                     map of the world. This includes beacons, buoys and other navigation
@@ -620,21 +624,21 @@
                         - https://wiki.openstreetmap.org/wiki/OpenSeaMap
                         - https://operations.osmfoundation.org/policies/tiles/
 
                     """,
                     self.OpenSeaMap.__call__.__doc__,
                 )
 
-                self.CyclOSM = _xyz_tile_service(
+                self.CyclOSM = _XyzTileService(
                     m=self._m,
                     url="https://a.tile-cyclosm.openstreetmap.fr/cyclosm/{z}/{x}/{y}.png",
                     maxzoom=16,
                     name="CyclOSM",
                 )
-                self.CyclOSM.__doc__ = combdoc(
+                self.CyclOSM.__doc__ = _combdoc(
                     """
                     CyclOSM is a bicycle-oriented map built on top of OpenStreetMap data.
                     It aims at providing a beautiful and practical map for cyclists, no
                     matter their cycling habits or abilities.
 
                     https://www.cyclosm.org/
 
@@ -650,22 +654,22 @@
                         - https://openstreetmap.fr
                         - https://operations.osmfoundation.org/policies/tiles/
 
                     """,
                     self.CyclOSM.__call__.__doc__,
                 )
 
-                self.CyclOSM_lite = _xyz_tile_service(
+                self.CyclOSM_lite = _XyzTileService(
                     m=self._m,
                     url="https://a.tile-cyclosm.openstreetmap.fr/cyclosm-lite/{z}/{x}/{y}.png",
                     maxzoom=16,
                     name="CyclOSM",
                 )
 
-                self.CyclOSM_lite.__doc__ = combdoc(
+                self.CyclOSM_lite.__doc__ = _combdoc(
                     """
                     CyclOSM is a bicycle-oriented map built on top of OpenStreetMap data.
                     It aims at providing a beautiful and practical map for cyclists, no
                     matter their cycling habits or abilities.
 
                     https://www.cyclosm.org/
 
@@ -681,22 +685,22 @@
                         - https://openstreetmap.fr
                         - https://operations.osmfoundation.org/policies/tiles/
 
                     """,
                     self.CyclOSM_lite.__call__.__doc__,
                 )
 
-                self.OEPNV_public_transport = _xyz_tile_service(
+                self.OEPNV_public_transport = _XyzTileService(
                     m=self._m,
                     url="http://tile.memomaps.de/tilegen/{z}/{x}/{y}.png",
                     maxzoom=16,
                     name="CyclOSM",
                 )
 
-                self.OEPNV_public_transport.__doc__ = combdoc(
+                self.OEPNV_public_transport.__doc__ = _combdoc(
                     """
                     We display worldwide public transport facilities on a uniform map,
                     so that you can forget about browsing individual operators websites.
 
                     https://www.öpnvkarte.de
 
                     Note
@@ -709,68 +713,68 @@
                         - https://memomaps.de/
                         - https://operations.osmfoundation.org/policies/tiles/
 
                     """,
                     self.OEPNV_public_transport.__call__.__doc__,
                 )
 
-                self.stamen_toner = _xyz_tile_service(
+                self.stamen_toner = _XyzTileService(
                     self._m,
                     "https://stamen-tiles.a.ssl.fastly.net/toner/{z}/{x}/{y}.png",
                     name="OSM_stamen_toner",
                 )
-                self.stamen_toner_lines = _xyz_tile_service(
+                self.stamen_toner_lines = _XyzTileService(
                     self._m,
                     "https://stamen-tiles.a.ssl.fastly.net/toner-lines/{z}/{x}/{y}.png",
                     name="OSM_stamen_toner_lines",
                 )
-                self.stamen_toner_background = _xyz_tile_service(
+                self.stamen_toner_background = _XyzTileService(
                     self._m,
                     "https://stamen-tiles.a.ssl.fastly.net/toner-background/{z}/{x}/{y}.png",
                     name="OSM_stamen_toner_background",
                 )
-                self.stamen_toner_lite = _xyz_tile_service(
+                self.stamen_toner_lite = _XyzTileService(
                     self._m,
                     "https://stamen-tiles.a.ssl.fastly.net/toner-lite/{z}/{x}/{y}.png",
                     name="OSM_stamen_toner_lite",
                 )
-                self.stamen_toner_hybrid = _xyz_tile_service(
+                self.stamen_toner_hybrid = _XyzTileService(
                     self._m,
                     "https://stamen-tiles.a.ssl.fastly.net/toner-hybrid/{z}/{x}/{y}.png",
                     name="OSM_stamen_toner_hybrid",
                 )
-                self.stamen_toner_labels = _xyz_tile_service(
+                self.stamen_toner_labels = _XyzTileService(
                     self._m,
                     "https://stamen-tiles.a.ssl.fastly.net/toner-labels/{z}/{x}/{y}.png",
                     name="OSM_stamen_toner_labels",
                 )
 
-                self.stamen_watercolor = _xyz_tile_service(
+                self.stamen_watercolor = _XyzTileService(
                     self._m,
                     "http://c.tile.stamen.com/watercolor/{z}/{x}/{y}.jpg",
                     name="OSM_stamen_watercolor",
                     maxzoom=18,
                 )
 
-                self.stamen_terrain = _xyz_tile_service(
+                self.stamen_terrain = _XyzTileService(
                     self._m,
                     "http://c.tile.stamen.com/terrain/{z}/{x}/{y}.jpg",
                     name="OSM_stamen_terrain",
                 )
-                self.stamen_terrain_lines = _xyz_tile_service(
+                self.stamen_terrain_lines = _XyzTileService(
                     self._m,
                     "http://c.tile.stamen.com/terrain-lines/{z}/{x}/{y}.jpg",
                     name="OSM_stamen_terrain_lines",
                 )
-                self.stamen_terrain_labels = _xyz_tile_service(
+                self.stamen_terrain_labels = _XyzTileService(
                     self._m,
                     "http://c.tile.stamen.com/terrain-labels/{z}/{x}/{y}.jpg",
                     name="OSM_stamen_terrain_labels",
                 )
-                self.stamen_terrain_background = _xyz_tile_service(
+                self.stamen_terrain_background = _XyzTileService(
                     self._m,
                     "http://c.tile.stamen.com/terrain-background/{z}/{x}/{y}.jpg",
                     name="OSM_stamen_terrain_background",
                 )
 
                 stamen_doc = """
 
@@ -790,36 +794,36 @@
                     We’d love to see these maps used around the web, so we’ve
                     included some brief instructions to help you use them in
                     the mapping system of your choice. These maps are available
                     free of charge. If you use these tiles, you must use the
                     attribution provided in the link above.
                     """
 
-                stamen_toner_doc = combdoc(
+                stamen_toner_doc = _combdoc(
                     """
                     **Stamen Toner**
 
                     High-contrast B+W (black and white) maps provided by Stamen
                     """,
                     stamen_doc,
                     self.stamen_toner.__call__.__doc__,
                 )
 
-                stamen_terrain_doc = combdoc(
+                stamen_terrain_doc = _combdoc(
                     """
                     **Stamen Terrain**
 
                     Terrain maps with hill-shading and natural vegetation colors
                     provided by Stamen
                     """,
                     stamen_doc,
                     self.stamen_toner.__call__.__doc__,
                 )
 
-                stamen_watercolor_doc = combdoc(
+                stamen_watercolor_doc = _combdoc(
                     """
                     **Stamen Watercolor**
 
                     A maps-style reminiscent of hand-drawn watercolor maps
                     provided by Stamen
                     """,
                     stamen_doc,
@@ -868,27 +872,27 @@
                         "cycling",
                         "mtb",
                         "slopes",
                         "riding",
                         "skating",
                     ]:
 
-                        srv = _xyz_tile_service(
+                        srv = _XyzTileService(
                             m,
                             (
                                 "https://tile.waymarkedtrails.org/"
                                 + v
                                 + "/{z}/{x}/{y}.png"
                             ),
                             name=f"OSM_WaymarkedTrails_{v}",
                         )
 
                         setattr(self, v, srv)
 
-                        getattr(self, v).__doc__ = combdoc(
+                        getattr(self, v).__doc__ = _combdoc(
                             (
                                 f"WaymarkedTrails {v} layer\n"
                                 "\n"
                                 "Note\n"
                                 "----\n"
                                 "**LICENSE-info (without any warranty for correctness!!)**\n"
                                 "\n"
@@ -923,27 +927,27 @@
                         "standard",
                         "maxspeed",
                         "signals",
                         "electrification",
                         "gauge",
                     ]:
 
-                        srv = _xyz_tile_service(
+                        srv = _XyzTileService(
                             m,
                             (
                                 "https://a.tiles.openrailwaymap.org/"
                                 + v
                                 + "/{z}/{x}/{y}.png"
                             ),
                             name=f"OSM_OpenRailwayMap_{v}",
                         )
 
                         setattr(self, v, srv)
 
-                        getattr(self, v).__doc__ = combdoc(
+                        getattr(self, v).__doc__ = _combdoc(
                             (
                                 f"OpenRailwayMap {v} layer\n"
                                 "\n"
                                 "Note\n"
                                 "----\n"
                                 "**LICENSE-info (without any warranty for correctness!!)**\n"
                                 "\n"
@@ -985,29 +989,29 @@
                         "base-antique",
                         "rastertiles/voyager",
                         "rastertiles/voyager_nolabels",
                         "rastertiles/voyager_only_labels",
                         "rastertiles/voyager_labels_under",
                     ]:
 
-                        srv = _xyz_tile_service(
+                        srv = _XyzTileService(
                             m,
                             (
                                 "https://cartodb-basemaps-a.global.ssl.fastly.net/"
                                 + v
                                 + "/{z}/{x}/{y}.png"
                             ),
                             name=f"OSM_CartoDB_{v}",
                         )
 
                         name = v.replace(r"/", "_").replace("-", "_")
 
                         setattr(self, name, srv)
 
-                        getattr(self, name).__doc__ = combdoc(
+                        getattr(self, name).__doc__ = _combdoc(
                             (
                                 f"CartoDB basemap {v} layer\n"
                                 "\n"
                                 "Note\n"
                                 "----\n"
                                 "**LICENSE-info (without any warranty for correctness!!)**\n"
                                 "\n"
@@ -1015,20 +1019,20 @@
                             ),
                             getattr(self, name).__call__.__doc__,
                         )
 
         @property
         @lru_cache()
         def OSM_terrestis(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://ows.terrestris.de/osm/service?SERVICE=WMS&VERSION=1.1.1&REQUEST=GetCapabilities",
             )
-            WMS.__doc__ = combdoc(
+            WMS.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
 
                 ... this service is hosted by Terrestris... check:
@@ -1036,20 +1040,20 @@
                 """,
             )
             return WMS
 
         @property
         @lru_cache()
         def OSM_mundialis(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="http://ows.mundialis.de/services/service?",
             )
-            WMS.__doc__ = combdoc(
+            WMS.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
 
                 ... this service is hosted by Mundialis... check:
@@ -1057,20 +1061,20 @@
                 """,
             )
             return WMS
 
         @property
         @lru_cache()
         def OSM_wheregroup(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url="https://osm-demo.wheregroup.com/service?REQUEST=GetCapabilities",
             )
-            WMS.__doc__ = combdoc(
+            WMS.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
 
                 ... this service is hosted by WhereGroup...
@@ -1081,20 +1085,20 @@
                 """,
             )
             return WMS
 
         @property
         @lru_cache()
         def OSM_wms(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url=r"https://maps.heigit.org/osm-wms/service?REQUEST=GetCapabilities&SERVICE=WMS",
             )
-            WMS.__doc__ = combdoc(
+            WMS.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 The first version of osm-wms.de was put online at 13th of February
                 2009. Since these days it serves OpenStreetMap based maps. As the
                 name indicates it does provide the maps via the OGC-WMS format
                 other than the usual map tile providers. This increases the
                 flexibility of the usage of this service as you are able to use the
@@ -1133,20 +1137,20 @@
                 """,
             )
             return WMS
 
         @property
         @lru_cache()
         def OSM_landuse(self):
-            WMS = _WebServiec_collection(
+            WMS = _WebServiceCollection(
                 m=self._m,
                 service_type="wms",
                 url=r"https://maps.heigit.org/osmlanduse/service?REQUEST=GetCapabilities",
             )
-            WMS.__doc__ = combdoc(
+            WMS.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 OSM Landuse Landcover is a WebGIS application to explore the
                 OpenStreetMap database specifically in terms of landuse and
                 landcover information. Land use tags were predicted when absent
                 using belows (Schultz et al. 2020 in prep, Schultz et al. 2017)
                 method. This was first addressed for Germany (2017) and now (2020)
@@ -1225,21 +1229,21 @@
         @property
         @lru_cache()
         def Image(self):
             """
             European Environment Agency discomap Image collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://image.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_Image",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'Image' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1258,21 +1262,21 @@
         @property
         @lru_cache()
         def Land(self):
             """
             European Environment Agency discomap Land collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://land.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_Land",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'Land' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1291,21 +1295,21 @@
         @property
         @lru_cache()
         def Climate(self):
             """
             European Environment Agency discomap Climate collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://climate.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_Climate",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'Climate' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1324,21 +1328,21 @@
         @property
         @lru_cache()
         def Bio(self):
             """
             European Environment Agency discomap Bio collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://bio.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_Bio",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'Bio' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1357,21 +1361,21 @@
         @property
         @lru_cache()
         def Copernicus(self):
             """
             European Environment Agency discomap Copernicus collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://copernicus.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_Copernicus",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'Copernicus' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1390,21 +1394,21 @@
         @property
         @lru_cache()
         def Water(self):
             """
             European Environment Agency discomap Water collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://water.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_Water",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'Water' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1423,21 +1427,21 @@
         @property
         @lru_cache()
         def SOER(self):
             """
             European Environment Agency discomap SOER collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://soer.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_SOER",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'SOER' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1456,21 +1460,21 @@
         @property
         @lru_cache()
         def MARATLAS(self):
             """
             European Environment Agency discomap MARATLAS collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://maratlas.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_SOER",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'MARATLAS' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1489,21 +1493,21 @@
         @property
         @lru_cache()
         def MARINE(self):
             """
             European Environment Agency discomap MARINE collection
             https://discomap.eea.europa.eu/Index/
             """
-            API = REST_API_services(
+            API = RestApiServices(
                 m=self._m,
                 url="https://marine.discomap.eea.europa.eu/arcgis/rest/services",
                 name="EEA_REST_SOER",
                 service_type="wms",
             )
-            API.__doc__ = combdoc(
+            API.__doc__ = _combdoc(
                 type(self).__doc__,
                 """
                 ... access to the 'MARINE' subfolder
 
                 Note
                 ----
                 **LICENSE-info (without any warranty for correctness!!)**
@@ -1561,33 +1565,33 @@
 
     class _S1GBM_layers:
         def __init__(self, m):
             self._m = m
 
         @property
         def vv(self):
-            WMS = _xyz_tile_service(
+            WMS = _XyzTileService(
                 self._m,
                 lambda x, y, z: f"https://s1map.eodc.eu/vv/{z}/{x}/{2**z-1-y}.png",
                 13,
                 name="S1GBM_vv",
             )
 
-            WMS.__doc__ = combdoc("Polarization: VV", type(self).__doc__)
+            WMS.__doc__ = _combdoc("Polarization: VV", type(self).__doc__)
             return WMS
 
         @property
         def vh(self):
-            WMS = _xyz_tile_service(
+            WMS = _XyzTileService(
                 self._m,
                 lambda x, y, z: f"https://s1map.eodc.eu/vh/{z}/{x}/{2**z-1-y}.png",
                 13,
                 name="S1GBM_vh",
             )
-            WMS.__doc__ = combdoc("Polarization: VH", type(self).__doc__)
+            WMS.__doc__ = _combdoc("Polarization: VH", type(self).__doc__)
             return WMS
 
     class _OpenPlanetary:
         """
         Planetary layers (Moon & Mars) provided by OpenPlanetary
         https://www.openplanetary.org
 
@@ -1648,21 +1652,21 @@
                             "\n"
                             f"check: https://www.openplanetary.org\n"
                         )
 
                         self._addlayer(v, url, f"OPM_Moon_{v}", docstring)
 
                 def _addlayer(self, name, url, srv_name, docstring, maxzoom=19):
-                    srv = _xyz_tile_service_nonearth(
+                    srv = _XyzTileServiceNonEarth(
                         self._m, url, name=srv_name, maxzoom=maxzoom
                     )
 
                     setattr(self, name, srv)
 
-                    getattr(self, name).__doc__ = combdoc(
+                    getattr(self, name).__doc__ = _combdoc(
                         docstring,
                         getattr(self, name).__call__.__doc__,
                     )
 
         class _OPM_mars_basemap:
             """
             This basemap of the Mars in a combination of multiple raster and vector
@@ -1840,34 +1844,40 @@
                         lambda x, y, z: f"http://s3-eu-west-1.amazonaws.com/whereonmars.cartodb.net/mola_color-noshade_global/{z}/{x}/{2**z-1-y}.png",
                         f"OPM_Mars_mola_color_noshade",
                         docstring=docstring,
                         maxzoom=6,
                     )
 
                 def _addlayer(self, name, url, srv_name, docstring, maxzoom=19):
-                    srv = _xyz_tile_service_nonearth(
+                    srv = _XyzTileServiceNonEarth(
                         self._m, url, name=srv_name, maxzoom=maxzoom
                     )
 
                     setattr(self, name, srv)
 
-                    getattr(self, name).__doc__ = combdoc(
+                    getattr(self, name).__doc__ = _combdoc(
                         docstring,
                         getattr(self, name).__call__.__doc__,
                     )
 
     @property
     def OpenPlanetary(self):
         WMS = self._OpenPlanetary(self._m)
         WMS.__doc__ = type(self)._OpenPlanetary.__doc__
         return WMS
 
     OpenPlanetary.__doc__ = _OpenPlanetary.__doc__
 
     class _GOOGLE_layers:
+        """
+        WebMaps provided by GOOGLE
+        https://www.google.com
+
+        """
+
         def __init__(self, m):
             self._m = m
             self.add_layer = self._add_layer(m)
             self.layers = [i for i in self.add_layer.__dict__ if not i.startswith("_")]
 
         class _add_layer:
             def __init__(self, m):
@@ -1898,19 +1908,19 @@
                         "\n"
                         f"check: https://www.google.com\n"
                     )
 
                     self._addlayer(v, url, f"GOOGLE_{v}", docstring)
 
             def _addlayer(self, name, url, srv_name, docstring, maxzoom=19):
-                srv = _xyz_tile_service(self._m, url, name=srv_name, maxzoom=maxzoom)
+                srv = _XyzTileService(self._m, url, name=srv_name, maxzoom=maxzoom)
 
                 setattr(self, name, srv)
 
-                getattr(self, name).__doc__ = combdoc(
+                getattr(self, name).__doc__ = _combdoc(
                     docstring,
                     getattr(self, name).__call__.__doc__,
                 )
 
     @property
     def GOOGLE(self):
         WMS = self._GOOGLE_layers(self._m)
@@ -1944,15 +1954,15 @@
         displayed legibly and in proximity to the usage, in on-line publications
         (social-networks etc.) it shall include the links and show the text as
         described below.
 
         (check: https://s2maps.eu/ for full details)
 
         """
-        WMS = _WebServiec_collection(
+        WMS = _WebServiceCollection(
             m=self._m,
             service_type="wms",
             url="https://tiles.maps.eox.at/wms?service=wms&request=getcapabilities",
         )
 
         WMS.__doc__ = type(self).S2_cloudless.__doc__
         return WMS
@@ -1983,15 +1993,15 @@
         All users of Copernicus Products must provide clear and visible attribution
         to the Copernicus programme. The Licensee will communicate to the public
         the source of the Copernicus Products by crediting the Copernicus Climate
         Change and Atmosphere Monitoring Services.
 
         (check: https://apps.ecmwf.int/datasets/licences/copernicus/ for full details)
         """
-        WMS = _WebServiec_collection(
+        WMS = _WebServiceCollection(
             m=self._m,
             service_type="wms",
             url="https://eccharts.ecmwf.int/wms/?token=public",
         )
 
         WMS.__doc__ = type(self).CAMS.__doc__
         return WMS
@@ -2027,21 +2037,21 @@
         exemplary damages or lost profits resulting from any use or misuse of
         these data. The user of these maps cannot claim any rights pertaining to
         its usage.
 
         (check: https://geoservice.dlr.de/web/about for full details)
         """
 
-        WMS = _WebServiec_collection(
+        WMS = _WebServiceCollection(
             m=self._m,
             service_type="wms",
             url="https://geoservice.dlr.de/eoc/basemap/wms?SERVICE=WMS&REQUEST=GetCapabilities",
         )
 
-        WMS.__doc__ = type(self).CAMS.__doc__
+        WMS.__doc__ = type(self).DLR_basemaps.__doc__
         return WMS
 
     @property
     @lru_cache()
     def ESRI_ArcGIS(self):
         """
         Interface to the ERSI ArcGIS REST Services Directory
@@ -2052,15 +2062,15 @@
         **LICENSE-info (without any warranty for correctness!!)**
 
         For licensing etc. check the individual layer-descriptions at
         http://services.arcgisonline.com/arcgis/rest/services
 
         """
 
-        API = REST_API_services(
+        API = RestApiServices(
             m=self._m,
             url="http://server.arcgisonline.com/arcgis/rest/services",
             name="ERSI_ArcGIS_REST",
             service_type="xyz",
             layers={
                 "Canvas",
                 "Elevation",
@@ -2070,25 +2080,80 @@
                 "SERVICES",
                 "Specialty",
             },
         )
 
         return API
 
+    class _Austria:
+        # container for WebMap services specific to Austria
+        def __init__(self, m):
+            _register_imports()
+
+            self._m = m
+
+        @property
+        @lru_cache()
+        def AT_basemap(self):
+            """
+            Basemap for Austria
+            https://basemap.at/
+
+            Note
+            ----
+            **LICENSE-info (without any warranty for correctness!!)**
+
+            (check: https://basemap.at/#lizenz for full details)
+
+            basemap.at ist gemäß der Open Government Data Österreich Lizenz
+            CC-BY 4.0 sowohl für private als auch kommerzielle Zwecke frei
+            sowie entgeltfrei nutzbar.
+            """
+            WMTS = _WebServiceCollection(
+                m=self._m,
+                service_type="wmts",
+                url="http://maps.wien.gv.at/basemap/1.0.0/WMTSCapabilities.xml",
+            )
+            WMTS.__doc__ = type(self).AT_basemap.__doc__
+            return WMTS
+
+        @property
+        @lru_cache()
+        def Wien_basemap(self):
+            """
+            Basemaps for the city of Vienna (Austria)
+            https://www.wien.gv.at
+
+            Note
+            ----
+            **LICENSE-info (without any warranty for correctness!!)**
+
+            check: https://www.data.gv.at/katalog/dataset/stadt-wien_webmaptileservicewmtswien
+
+            Most services are under CC-BY 4.0
+            """
+            WMTS = _WebServiceCollection(
+                m=self._m,
+                service_type="wmts",
+                url="http://maps.wien.gv.at/wmts/1.0.0/WMTSCapabilities.xml",
+            )
+            WMTS.__doc__ = type(self).Wien_basemap.__doc__
+            return WMTS
+
     @property
     @lru_cache()
     def Austria(self):
         """
         Services specific to Austria (Europe).
         (They ONLY work if the extent is set to a location inside Austria!)
 
             - AT_basemap: Basemaps for whole of austria
             - Wien: Basemaps for the city of Vienna
         """
-        WMS = Austria(self._m)
+        WMS = self._Austria(self._m)
         WMS.__doc__ = type(self).Austria.__doc__
         return WMS
 
     def get_service(self, url, service_type="wms", rest_API=False, maxzoom=19):
         """
         Get a object that can be used to add WMS, WMTS or XYZ services based on
         a GetCapabilities-link or a link to a ArcGIS REST API
@@ -2135,15 +2200,15 @@
             ONLY relevant if service_type="xyz"!
 
             The maximum zoom-level available (to avoid http-request errors) for too
             high zoom levels. The default is 19.
 
         Returns
         -------
-        service : _WebServiec_collection
+        service : _WebServiceCollection
             An object that behaves just like `m.add_wms.<service>`
             and provides easy-access to available WMS layers
 
         Examples
         --------
 
         WMS Example:
@@ -2187,80 +2252,26 @@
           >>> def url(x, y, z):
           >>>     return rf"https://tile.openstreetmap.org/{z}/{x}/{y}.png"
           >>> s = m.add_wms.get_service(url, "xyz")
 
         """
         if service_type == "xyz":
             if rest_API:
-                print("EOmaps: rest_API=True is not supported for service_type='xyz'")
+                _log.warning(
+                    "EOmaps: rest_API=True is not supported for service_type='xyz'"
+                )
 
-            s = _xyz_tile_service(self._m, url, maxzoom=maxzoom)
+            s = _XyzTileService(self._m, url, maxzoom=maxzoom)
             service = SimpleNamespace(add_layer=SimpleNamespace(xyz_layer=s))
 
         else:
             if rest_API:
-                service = REST_API_services(
+                service = RestApiServices(
                     m=self._m,
                     url=url,
                     name="custom_service",
                     service_type=service_type,
                 )
             else:
-                service = _WebServiec_collection(self._m, service_type="wms", url=url)
+                service = _WebServiceCollection(self._m, service_type="wms", url=url)
 
         return service
-
-
-class Austria:
-    # container for WebMap services specific to Austria
-    def __init__(self, m):
-        _register_imports()
-
-        self._m = m
-
-    @property
-    @lru_cache()
-    def AT_basemap(self):
-        """
-        Basemap for Austria
-        https://basemap.at/
-
-        Note
-        ----
-        **LICENSE-info (without any warranty for correctness!!)**
-
-        (check: https://basemap.at/#lizenz for full details)
-
-        basemap.at ist gemäß der Open Government Data Österreich Lizenz
-        CC-BY 4.0 sowohl für private als auch kommerzielle Zwecke frei
-        sowie entgeltfrei nutzbar.
-        """
-        WMTS = _WebServiec_collection(
-            m=self._m,
-            service_type="wmts",
-            url="http://maps.wien.gv.at/basemap/1.0.0/WMTSCapabilities.xml",
-        )
-        WMTS.__doc__ = type(self).AT_basemap.__doc__
-        return WMTS
-
-    @property
-    @lru_cache()
-    def Wien_basemap(self):
-        """
-        Basemaps for the city of Vienna (Austria)
-        https://www.wien.gv.at
-
-        Note
-        ----
-        **LICENSE-info (without any warranty for correctness!!)**
-
-        check: https://www.data.gv.at/katalog/dataset/stadt-wien_webmaptileservicewmtswien
-
-        Most services are under CC-BY 4.0
-        """
-        WMTS = _WebServiec_collection(
-            m=self._m,
-            service_type="wmts",
-            url="http://maps.wien.gv.at/wmts/1.0.0/WMTSCapabilities.xml",
-        )
-        WMTS.__doc__ = type(self).Wien_basemap.__doc__
-        return WMTS
```

### Comparing `EOmaps-6.5/eomaps/callbacks.py` & `EOmaps-7.0/eomaps/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+"""Collection of pre-defined click/pick/move/keypress callbacks."""
+
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.patches import PathPatch
 from matplotlib.transforms import TransformedPath
 import warnings
+import logging
+
+_log = logging.getLogger(__name__)
 
 
-class _click_callbacks(object):
+class _ClickCallbacks(object):
     """
     A collection of callback-functions.
 
     to attach a callback, use:
         >>> cid = m.cb.click.attach.annotate(**kwargs)
         or
         >>> cid = m.cb.pick.attach.annotate(**kwargs)
@@ -93,63 +98,239 @@
         # copy-pasteable
         kwargs.setdefault("separator", ",")
         try:
             return np.array2string(np.asanyarray(x), **kwargs)
         except Exception:
             return str(x)
 
-    def print_to_console(self, **kwargs):
+    def print_to_console(
+        self,
+        pos_precision=4,
+        val_precision=4,
+        text=None,
+        show_all_values=True,
+        **kwargs,
+    ):
         """
         Print details on the clicked pixel to the console.
 
-        Additional kwargs are passed to `numpy.array2string()`
-        to control the formatting of the printed values.
+        Parameters
+        ----------
+
+        pos_precision : int
+            The floating-point precision of the coordinates.
+            The default is 4.
+        val_precision : int
+            The floating-point precision of the parameter-values (only used if
+            "val_fmt=None"). The default is 4.
+        text : callable or str, optional
+            if str: the string to print
+            if callable: A function that returns the string that should be
+            printed in the annotation with the following call-signature:
+
+                >>> def text(m, ID, val, pos, ind):
+                >>>     # m   ... the Maps object
+                >>>     # ID  ... the ID in the dataframe
+                >>>     # pos ... the position
+                >>>     # val ... the value
+                >>>     # ind ... the index
+                >>>
+                >>>     return "the string to print"
+
+            The default is None.
+        show_all_values : bool, optional
+            If True, show all values and coordinates of picked points.
+            If False, only (min...max) values are shown if multiple datapoints are
+            picked. The default is True.
         """
         ID, pos, val, ind, picker_name, val_color = self._popargs(kwargs)
 
+        printstr = self._get_annotation_text(
+            ID=ID,
+            pos=pos,
+            val=val,
+            ind=ind,
+            pos_precision=pos_precision,
+            val_precision=val_precision,
+            text=text,
+            show_all_values=show_all_values,
+        )
+
+        if text is None:
+            print("\n# ---------------\n" + printstr)
+        else:
+            print(printstr)
+
+    def _get_annotation_text(
+        self,
+        ID=None,
+        pos=None,
+        val=None,
+        ind=None,
+        pos_precision=4,
+        val_precision=4,
+        text=None,
+        show_all_values=False,
+    ):
+
+        if isinstance(ind, (list, np.ndarray)):
+            try:
+                n_ids = len(ind)
+            except TypeError:
+                n_ids = "??"
+
+            if n_ids == 1:
+                multipick = False
+            else:
+                multipick = True
+        else:
+            multipick = False
+
         if isinstance(self.m.data_specs.x, str):
             xlabel = self.m.data_specs.x
-            ylabel = self.m.data_specs.y
         else:
             xlabel = "x"
+        if isinstance(self.m.data_specs.y, str):
+            ylabel = self.m.data_specs.y
+        else:
             ylabel = "y"
 
-        if ID is not None:
-            x, y = pos
+        if self.m.data_specs.parameter is None:
+            parameter = "value"
+        else:
+            parameter = self.m.data_specs.parameter
 
-            printstr = (
-                "---------------\n"
-                f"{xlabel} = {self._fmt(x, **kwargs)}\n"
-                f"{ylabel} = {self._fmt(y, **kwargs)}\n"
-                f"ID = {self._fmt(ID, **kwargs)}\n"
-            )
+        crs_is_lonlat = self.m._get_cartopy_crs(4326) is self.m.crs_plot
 
-            paramname = self.m.data_specs.parameter
-            if paramname is None:
-                paramname = "val"
-            printstr += f"{paramname} = {self._fmt(val)}"
-        else:
-            lon, lat = self.m._transf_plot_to_lonlat.transform(*pos)
+        if text is None:
+            # use "ind is not None" to distinguish between click and pick
+            # TODO implement better distinction between click and pick!
+            if self.m.data is not None and ind is not None:
+                if not multipick:
+                    x, y = [
+                        np.format_float_positional(i, trim="-", precision=pos_precision)
+                        for i in self.m._data_manager._get_xy_from_index(ind)
+                    ]
+                    x0, y0 = [
+                        np.format_float_positional(i, trim="-", precision=pos_precision)
+                        for i in pos
+                    ]
 
-            printstr = (
-                "---------------\n"
-                f"xy = ({self._fmt(pos[0], **kwargs)}, {self._fmt(pos[1], **kwargs)})\n"
-                f"lonlat = ({self._fmt(lon, **kwargs)}, {self._fmt(lat, **kwargs)})\n"
-            )
+                    if isinstance(val, (int, float)):
+                        val = np.format_float_positional(
+                            val, trim="-", precision=val_precision
+                        )
+                else:
+                    if not show_all_values:
+                        # only show min-max values of picked points
+                        coords = [
+                            *self.m._data_manager._get_xy_from_index(ind),
+                            *self.m._data_manager._get_xy_from_index(
+                                ind, reprojected=True
+                            ),
+                        ]
 
-        print(printstr)
+                        for n, c in enumerate(coords):
+                            mi = np.format_float_positional(
+                                np.nanmin(c), trim="-", precision=pos_precision
+                            )
+                            ma = np.format_float_positional(
+                                np.nanmax(c), trim="-", precision=pos_precision
+                            )
+                            coords[n] = f"{mi} ... {ma}"
+
+                        x, y, x0, y0 = coords
+
+                        if ID is not None:
+                            ID = f"{np.nanmin(ID)} ... {np.nanmax(ID)}"
+
+                        if val is not None:
+                            val = np.array(val, dtype=float)  # to handle None
+
+                            # catch warnings here to avoid showing "all-nan-slice"
+                            # all the time when clicking on empty pixels
+                            with warnings.catch_warnings():
+                                mi = np.format_float_positional(
+                                    np.nanmin(val), trim="-", precision=pos_precision
+                                )
+                                ma = np.format_float_positional(
+                                    np.nanmax(val), trim="-", precision=pos_precision
+                                )
+                            val = f"{mi}...{ma}"
+                    else:
+                        coords = (
+                            *self.m._data_manager._get_xy_from_index(ind),
+                            *self.m._data_manager._get_xy_from_index(
+                                ind, reprojected=True
+                            ),
+                        )
+
+                        x, y, x0, y0 = map(
+                            lambda x: self._fmt(x, precision=pos_precision), coords
+                        )
+                        if val is not None:
+                            val = self._fmt(
+                                np.array(val, dtype=float), precision=val_precision
+                            )
+                        if ID is not None:
+                            ID = self._fmt(np.asanyarray(ID))
+
+                equal_crs = self.m.data_specs.crs == self.m._crs_plot
+                printstr = (
+                    (f"# Picked {n_ids} points\n" if multipick else "")
+                    + f"{xlabel} = {x}\n"
+                    + (f"{xlabel}_plot = {x0}\n" if not equal_crs else "")
+                    + f"{ylabel} = {y}\n"
+                    + (f"{ylabel}_plot = {y0}\n" if not equal_crs else "")
+                    + (f"ID = {ID}\n" if ID is not None else "")
+                    + (f"{parameter} = {val}" if val is not None else "")
+                )
+
+            else:
+                if not crs_is_lonlat:
+                    xlabel, ylabel = "x", "y"
+                    lon, lat = self.m._transf_plot_to_lonlat.transform(*pos)
+                    lon, lat = [
+                        np.format_float_positional(i, trim="-", precision=pos_precision)
+                        for i in (lon, lat)
+                    ]
+                else:
+                    xlabel, ylabel = "lon", "lat"
+
+                x, y = [
+                    np.format_float_positional(i, trim="-", precision=pos_precision)
+                    for i in pos
+                ]
+
+                printstr = (
+                    f"{xlabel} = {x}\n"
+                    + f"{ylabel} = {y}"
+                    + (f"\nlon = {lon}" if not crs_is_lonlat else "")
+                    + (f"\nlat = {lat}" if not crs_is_lonlat else "")
+                    + (f"\nvalue = {val}" if val is not None else "")
+                )
+
+        elif isinstance(text, str):
+            printstr = text
+        elif callable(text):
+            printstr = text(m=self.m, ID=ID, val=val, pos=pos, ind=ind)
+        else:
+            printstr = None
+
+        return printstr
 
     def annotate(
         self,
         pos_precision=4,
         val_precision=4,
         permanent=False,
         text=None,
         zorder=20,
         layer=None,
+        show_all_values=False,
         **kwargs,
     ):
         """
         Add a text-annotation to the plot at the position where the map was clicked.
 
         Parameters
         ----------
@@ -191,14 +372,18 @@
             - https://matplotlib.org/stable/gallery/misc/zorder_demo.html
 
             The default is 20
         layer : str or None, optional
             The layer to put the marker on.
             If None, the layer associated with the used Maps-object (e.g. `m.layer`)
             The default is None
+        show_all_values : bool, optional
+            If True, show all values and coordinates of picked points.
+            If False, only (min...max) values are shown if multiple datapoints are
+            picked. The default is True.
         kwargs
             kwargs passed to matplotlib.pyplot.annotate(). The default is:
 
             >>> dict(xytext=(20, 20),
             >>>      textcoords="offset points",
             >>>      bbox=dict(boxstyle="round", fc="w"),
             >>>      arrowprops=dict(arrowstyle="->"),
@@ -224,115 +409,24 @@
             else:
                 multipick = True
 
         else:
             multipick = False
             picked_pos = pos
 
-        if isinstance(self.m.data_specs.x, str):
-            xlabel = self.m.data_specs.x
-        else:
-            xlabel = "x"
-        if isinstance(self.m.data_specs.y, str):
-            ylabel = self.m.data_specs.y
-        else:
-            ylabel = "y"
-
-        if self.m.data_specs.parameter is None:
-            parameter = "value"
-        else:
-            parameter = self.m.data_specs.parameter
-
-        ax = self.m.ax
-        if text is None:
-            # use "ind is not None" to distinguish between click and pick
-            # TODO implement better distinction between click and pick!
-            if self.m.data is not None and ind is not None:
-                if not multipick:
-                    x, y = [
-                        np.format_float_positional(i, trim="-", precision=pos_precision)
-                        for i in self.m._data_manager._get_xy_from_index(ind)
-                    ]
-                    x0, y0 = [
-                        np.format_float_positional(i, trim="-", precision=pos_precision)
-                        for i in pos
-                    ]
-
-                    if isinstance(val, (int, float)):
-                        val = np.format_float_positional(
-                            val, trim="-", precision=val_precision
-                        )
-                else:
-                    coords = [
-                        *self.m._data_manager._get_xy_from_index(ind),
-                        *self.m._data_manager._get_xy_from_index(ind, reprojected=True),
-                    ]
-
-                    for n, c in enumerate(coords):
-                        mi = np.format_float_positional(
-                            np.nanmin(c), trim="-", precision=pos_precision
-                        )
-                        ma = np.format_float_positional(
-                            np.nanmax(c), trim="-", precision=pos_precision
-                        )
-                        coords[n] = f"{mi} ... {ma}"
-
-                    x, y, x0, y0 = coords
-
-                    if ID is not None:
-                        ID = f"{np.nanmin(ID)} ... {np.nanmax(ID)}"
-
-                    if val is not None:
-                        val = np.array(val, dtype=float)  # to handle None
-
-                        # catch warnings here to avoid showing "all-nan-slice"
-                        # all the time when clicking on empty pixels
-                        with warnings.catch_warnings():
-                            mi = np.format_float_positional(
-                                np.nanmin(val), trim="-", precision=pos_precision
-                            )
-                            ma = np.format_float_positional(
-                                np.nanmax(val), trim="-", precision=pos_precision
-                            )
-                        val = f"{mi}...{ma}"
-
-                equal_crs = self.m.data_specs.crs != self.m._crs_plot
-                printstr = (
-                    (f"Picked {n_ids} points\n" if multipick else "")
-                    + f"{xlabel} = {x}"
-                    + (f" ({x0})\n" if equal_crs else "\n")
-                    + f"{ylabel} = {y}"
-                    + (f" ({y0})\n" if equal_crs else "\n")
-                    + (f"ID = {ID}" if ID is not None else "")
-                    + (f"\n{parameter} = {val}" if val is not None else "")
-                )
-
-            else:
-                lon, lat = self.m._transf_plot_to_lonlat.transform(*pos)
-                x, y = [
-                    np.format_float_positional(i, trim="-", precision=pos_precision)
-                    for i in pos
-                ]
-                lon, lat = [
-                    np.format_float_positional(i, trim="-", precision=pos_precision)
-                    for i in (lon, lat)
-                ]
-
-                printstr = (
-                    f"x = {x}\n"
-                    + f"y = {y}\n"
-                    + f"lon = {lon}\n"
-                    + f"lat = {lat}"
-                    + (f"\nvalue = {val}" if val is not None else "")
-                )
-
-        elif isinstance(text, str):
-            printstr = text
-        elif callable(text):
-            printstr = text(m=self.m, ID=ID, val=val, pos=pos, ind=ind)
+        printstr = self._get_annotation_text(
+            ID=ID,
+            pos=pos,
+            val=val,
+            ind=ind,
+            pos_precision=4,
+            val_precision=4,
+            text=text,
+            show_all_values=show_all_values,
+        )
 
         if printstr is not None:
             # create a new annotation
             if not multipick:
                 bbox = dict(boxstyle="round", fc="w", ec=val_color)
                 bbox.update(kwargs.pop("bbox", dict()))
             else:
@@ -344,33 +438,51 @@
                 textcoords="offset points",
                 bbox=bbox,
                 arrowprops=dict(arrowstyle="->"),
                 annotation_clip=True,
             )
 
             styledict.update(**kwargs)
-            annotation = ax.annotate("", xy=picked_pos, **styledict)
+            annotation = self.m.ax.annotate("", xy=picked_pos, **styledict)
             annotation.set_zorder(zorder)
 
+            # remember text (in case functions are used so that annotation texts can be
+            # dynamically updated later as well)
+            if text is None:
+                annotation._EOmaps_text = self._get_annotation_text
+            else:
+                annotation._EOmaps_text = text
+
             if permanent is False:
                 # make the annotation temporary
                 self._temporary_artists.append(annotation)
                 self.m.BM.add_artist(annotation, layer=layer)
             else:
                 self.m.BM.add_artist(annotation, layer=layer)
 
                 if permanent is True:
                     if not hasattr(self, "permanent_annotations"):
-                        self.permanent_annotations = [annotation]
-                    else:
-                        self.permanent_annotations.append(annotation)
+                        self.permanent_annotations = []
+
+                    self.permanent_annotations.append(annotation)
+
+                    # permanent annotations are also editable!
+                    self.m._edit_annotations._add(
+                        a=annotation,
+                        kwargs={"ID": ID, "xy": picked_pos, "text": text, **styledict},
+                        transf=None,
+                        drag_coords=ID is None,
+                    )
 
             annotation.set_visible(True)
             annotation.xy = picked_pos
             annotation.set_text(printstr)
+            annotation.set_label(f"Annotation {pos}")
+
+            return annotation
 
     def clear_annotations(self, **kwargs):
         """Remove all temporary and permanent annotations from the plot."""
         if hasattr(self, "permanent_annotations"):
             while len(self.permanent_annotations) > 0:
                 ann = self.permanent_annotations.pop(0)
                 self.m.BM.remove_artist(ann)
@@ -527,15 +639,15 @@
             pos_crs = "in"
         else:
             pos_crs = "out"
 
         if isinstance(radius, str) and radius == "pixel":
             pixelQ = True
             if not hasattr(self.m.shape, "radius"):
-                print(
+                _log.error(
                     "EOmaps: You cannot attach markers with 'radius=pixel' if the "
                     + "plot-shape does not set a radius! Please specify it explicitly."
                 )
                 return
             radius = self.m.shape.radius
         else:
             pixelQ = False
@@ -583,23 +695,27 @@
             np.atleast_1d(pos[0]), np.atleast_1d(pos[1]), pos_crs, **kwargs
         )
 
         marker = self.m.ax.add_collection(coll, autolim=False)
 
         marker.set_zorder(zorder)
 
+        marker.set_label(f"Marker {pos}")
+
         if layer is None:
             layer = self.m.layer
 
         # explicitly use True/False here to allow overriding the "permanent"
         # behavior by using permanent=None (or anything other than True/False)
         if permanent is False:
             # make the annotation temporary
             self._temporary_artists.append(marker)
             self.m.BM.add_artist(marker, layer)
+        elif permanent is None:
+            self.m.BM.add_bg_artist(marker, layer)
         elif permanent is True:
             self.m.BM.add_artist(marker, layer)
 
             if not hasattr(self, "permanent_markers"):
                 self.permanent_markers = [marker]
             else:
                 self.permanent_markers.append(marker)
@@ -697,14 +813,22 @@
             The default is "left".
         alpha : float, optional
             The transparency of the peeked layer. (between 0 and 1)
             If you overlay a (possibly transparent) combination of multiple layers,
             this transparency will be assigned as a global transparency for the
             obtained "combined layer".
             The default is 1.
+        shape : str, optional
+            The shape of the peek-window.
+
+            - "rectangular": peek a rectangle
+            - "round": peek an ellipse
+
+            The default is "rectangular"
+
         **kwargs :
             additional kwargs passed to a rectangle-marker.
             the default is `(fc="none", ec="k", lw=1)`
 
 
         Examples
         --------
@@ -729,15 +853,15 @@
         """
         shape = "ellipses" if shape == "round" else "rectangles"
 
         if not isinstance(layer, str):
             layer = self.m._get_combined_layer_name(*layer)
 
         # add spines and relevant inset-map layers to the specified peek-layer
-        layer = self.m.BM._get_showlayer_name(layer)
+        layer = self.m.BM._get_showlayer_name(layer, transparent=True)
 
         ID, pos, val, ind, picker_name, val_color = self._popargs(kwargs)
 
         ax = self.m.ax
 
         # default boundary args
         args = dict(fc="none", ec="k", lw=1.1)
@@ -846,19 +970,20 @@
             raise TypeError(f"EOmaps: {how} is not a valid peek method!")
 
         if clip_path is not None:
             patch = PathPatch(clip_path, ec="k", fc="none")
             marker = self.m.ax.add_patch(patch)
             self.m.cb.click.add_temporary_artist(marker)
 
-            # make sure to clear the marker at the next update
+            # make sure to clear the marker at the next update to avoid savefig issues
             def doit():
-                self.m.BM._artists_to_clear.setdefault("move", []).append(marker)
+                self.m.BM._artists_to_clear.setdefault("peek", []).append(marker)
+                self.m.BM._clear_temp_artists("peek")
 
-            self.m.BM._after_restore_actions.append(doit)
+            self.m.BM._after_update_actions.append(doit)
 
         # create a TransformedPath as needed for clipping
         clip_path = TransformedPath(
             clip_path, self.m.ax.projection._as_mpl_transform(self.m.ax)
         )
 
         self.m.BM._after_restore_actions.append(
@@ -901,15 +1026,17 @@
                 ), "The provided database has no method '{load_method}'"
                 pick = getattr(database, load_method)(ID)
             elif callable(load_method):
                 pick = load_method(database, ID)
             else:
                 raise TypeError("load_method must be a string or a callable!")
         except Exception:
-            print(f"could not load object with ID:  '{ID}' from {database}")
+            _log.error(
+                f"EOmaps: Unable to load object with ID:  '{ID}' from {database}"
+            )
         if load_multiple is True:
             self.picked_object = getattr(self, "picked_object", list()) + [pick]
         else:
             self.picked_object = pick
 
     def _load_cleanup(self):
         if hasattr(self, "picked_object"):
@@ -996,15 +1123,15 @@
             del self._pick_f
         if hasattr(self, "_pick_ax"):
             del self._pick_ax
         if hasattr(self, "_pick_l"):
             del self._pick_l
 
 
-class pick_callbacks(_click_callbacks):
+class PickCallbacks(_ClickCallbacks):
     """A collection of callbacks that are executed if you click on a datapoint."""
 
     _cb_list = [
         "get_values",
         "load",
         "print_to_console",
         "annotate",
@@ -1034,15 +1161,15 @@
         if ID is not None:
             # get the selected geometry and re-project it to the desired crs
             geom = self.m.cb.pick[picker_name].data.loc[[ID]].geometry
             # add the geometry to the map
             self.m.add_gdf(geom, temporary_picker=picker_name, **kwargs)
 
 
-class click_callbacks(_click_callbacks):
+class ClickCallbacks(_ClickCallbacks):
     """Collection of callbacks that are executed if you click anywhere on the map."""
 
     _cb_list = [
         "get_values",
         "print_to_console",
         "annotate",
         "mark",
@@ -1051,29 +1178,29 @@
         "clear_markers",
     ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class move_callbacks(_click_callbacks):
+class MoveCallbacks(_ClickCallbacks):
     """Collection of callbacks that are executed on mouse-movement."""
 
     _cb_list = [
         "print_to_console",
         "annotate",
         "mark",
         "peek_layer",
     ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class keypress_callbacks:
+class KeypressCallbacks:
     """Collection of callbacks that are executed if you press a key on the keyboard."""
 
     _cb_list = ["switch_layer", "fetch_layers"]
 
     def __init__(self, m, temp_artists):
         self._temporary_artists = temp_artists
         self._m = m
```

### Comparing `EOmaps-6.5/eomaps/colorbar.py` & `EOmaps-7.0/eomaps/colorbar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-from matplotlib.gridspec import GridSpecFromSubplotSpec, SubplotSpec
+"""Interactive Colorbar."""
+
+import logging
+from functools import partial, lru_cache
+from textwrap import dedent
+import copy
+
+import numpy as np
 
+from matplotlib.gridspec import GridSpecFromSubplotSpec, SubplotSpec
 import matplotlib.transforms as mtransforms
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap
 
-import numpy as np
-import copy
-
-from functools import partial, wraps
-from textwrap import dedent
-
-from .helpers import pairwise, _TransformedBoundsLocator
-
-
-ds, mpl_ext = None, None
-
-
-def _register_datashader():
-    global ds
-    global mpl_ext
-
-    try:
-        import datashader as ds
-        from datashader import mpl_ext
-    except ImportError:
-        return False
+from .helpers import pairwise, _TransformedBoundsLocator, register_modules
 
-    return True
+_log = logging.getLogger(__name__)
 
 
 def get_named_bins_formatter(bins, names, show_values=False):
     """
     A formatter to format the tick-labels of the colorbar with respect to
     labels for a given set of bins.
 
@@ -66,14 +54,16 @@
         else:
             return names[b]
 
     return formatter
 
 
 class ColorBar:
+    """Class to draw colorbars with a histogram on top."""
+
     def __init__(
         self,
         m,
         pos=0.4,
         inherit_position=None,
         margin=None,
         hist_size=0.8,
@@ -109,15 +99,15 @@
         ----------
         pos : float or 4-tuple, optional
 
             - float: fraction of the axis size that is used to create the colorbar.
               The axes of the Maps-object will be shrinked accordingly to make space
               for the colorbar.
             - 4-tuple (x0, y0, width, height):
-              Absolute position at which the colorbar should be placed in units.
+              Absolute position of the colorbar in relative figure-units (0-1).
               In this case, existing axes are NOT automatically re-positioned!
 
             Note: By default, multiple colorbars on different layers share their
             position! To force placement of a colorbar, use "inherit_position=False".
 
             The default is 0.4.
         inherit_position : bool or None optional
@@ -230,15 +220,15 @@
             The label used for the y-axis of the colorbar. The default is None
         kwargs :
             All additional kwargs are passed to the creation of the colorbar
             (e.g. `plt.colorbar()`)
 
         See Also
         --------
-        set_bin_labels:  Use custom names for classified colorbar bins.
+        ColorBar.set_bin_labels:  Use custom names for classified colorbar bins.
 
         Examples
         --------
 
         >>> x = y = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
         >>> data = [1, 2, 6, 6, 6, 8, 7, 3, 9, 10]
         >>> m = Maps()
@@ -292,15 +282,16 @@
 
         self._show_outline = show_outline
         self._tick_precision = tick_precision
         self._tick_formatter = tick_formatter
         self._log = log
         self._out_of_range_vals = out_of_range_vals
 
-        kwargs["label"] = label
+        # kwargs["label"] = label
+
         self._kwargs = copy.deepcopy(kwargs)
 
         self._coll = self._m.coll
         self._vmin = self._coll.norm.vmin
         self._vmax = self._coll.norm.vmax
 
         self._classified = self._m.classify_specs._classified
@@ -315,15 +306,15 @@
         self.ax_cb = None
         self.ax_cb_plot = None
 
         self._cid_redraw = False
 
         self._set_data()
         self._setup_axes()
-
+        self.set_labels(label)
         if ylabel is not None:
             self.ax_cb_plot.set_ylabel(ylabel)
 
     def set_visible(self, vis):
         """
         Set the visibility of the colorbar.
 
@@ -350,20 +341,43 @@
                 "cb_label": None,
                 "hist_label": hist_label,
                 **kwargs,
             }
 
         if self._orientation == "horizontal":
             if cb_label:
-                self._cb_label = self.ax_cb.set_xlabel(cb_label, **kwargs)
+                if self._hist_size < 0.001:
+                    # label colorbar
+                    self.ax_cb_plot.set_xlabel("")
+                    label = self.ax_cb.set_xlabel(cb_label, **kwargs)
+                elif self._hist_size > 0.999:
+                    # label plot
+                    self.ax_cb_plot.set_xlabel(cb_label, **kwargs)
+                    self.ax_cb.set_xlabel("")
+                else:
+                    # label colorbar
+                    self.ax_cb_plot.set_xlabel("")
+                    label = self.ax_cb.set_xlabel(cb_label, **kwargs)
             if hist_label:
                 self._hist_label = self.ax_cb_plot.set_ylabel(hist_label, **kwargs)
         else:
             if cb_label:
-                self._cb_label = self.ax_cb.set_ylabel(cb_label, **kwargs)
+                if self._hist_size < 0.001:
+                    # label colorbar
+                    self.ax_cb_plot.set_ylabel("")
+                    label = self.ax_cb.set_ylabel(cb_label, **kwargs)
+                elif self._hist_size > 0.999:
+                    # label plot
+                    self.ax_cb_plot.set_ylabel(cb_label, **kwargs)
+                    self.ax_cb.set_xlabel("")
+                else:
+                    # label colorbar
+                    self.ax_cb_plot.set_ylabel("")
+                    label = self.ax_cb.set_ylabel(cb_label, **kwargs)
+
             if hist_label:
                 self._hist_label = self.ax_cb_plot.set_xlabel(hist_label, **kwargs)
 
     def set_labels(self, cb_label=None, hist_label=None, **kwargs):
         """
         Set the labels (and the styling) for the colorbar (and the histogram).
 
@@ -393,30 +407,35 @@
 
         Use different styles for the colorbar and histogram labels
 
         >>> cb.set_labels(cb_label="The parameter", color="r", labelpad=10)
         >>> cb.set_labels(hist_label="histogram count", fontsize=6, color="k")
 
         """
+
+        self._label_kwargs = {"cb_label": cb_label, "hist_label": hist_label, **kwargs}
+
         self._set_labels(cb_label=cb_label, hist_label=hist_label, **kwargs)
 
         if not self._dynamic_shade_indicator:
             # no need to redraw the background for dynamically updated artists
             self._m.redraw(self._m.layer)
         else:
             self._m.BM.update()
 
+    @lru_cache()
     def _default_cb_tick_formatter(self, x, pos, precision=None):
         """
         A formatter to format the tick-labels of the colorbar for encoded datasets.
         (used in xaxis.set_major_formatter() )
         """
         # if precision=None the shortest representation of the number is used
         return np.format_float_positional(self._m._decode_values(x), precision)
 
+    @lru_cache()
     def _classified_cb_tick_formatter(self, x, pos, precision=None):
         """
         A formatter to format the tick-labels of the colorbar for classified datasets.
         (used in xaxis.set_major_formatter() )
         """
         # if precision=None the shortest representation of the number is used
         if x >= self._vmin and x <= self._vmax:
@@ -480,23 +499,35 @@
 
             # in case the histogram has not yet been plotted, plot it!
             if not self._histogram_plotted:
                 self._plot_histogram()
         else:
             self.ax_cb_plot.set_visible(False)  # to avoid singular matrix errors
 
-        if self.ax_cb.bbox.width > 1 and self.ax_cb.bbox.height > 1:
+        # avoid singular matrix errors caused by visible axes with 0 size
+        # when activating the layout editor
+        if self._hist_size > 0.999:
+            self.ax_cb.set_visible(False)  # to avoid singular matrix errors
+            self.ax_cb_plot.set_visible(True)
+            [i.set_visible(False) for i in self.ax_cb.patches]
+            [i.set_visible(False) for i in self.ax_cb.collections]
+            self.ax_cb_plot.tick_params(bottom=True, labelbottom=True)
+        elif self._hist_size < 0.001:
             self.ax_cb.set_visible(True)
+            self.ax_cb_plot.set_visible(False)  # to avoid singular matrix errors
             [i.set_visible(True) for i in self.ax_cb.patches]
             [i.set_visible(True) for i in self.ax_cb.collections]
         else:
-            self.ax_cb.set_visible(False)  # to avoid singular matrix errors
-            [i.set_visible(False) for i in self.ax_cb.patches]
-            [i.set_visible(False) for i in self.ax_cb.collections]
+            self.ax_cb.set_visible(True)
+            self.ax_cb_plot.set_visible(True)
+            self.ax_cb_plot.tick_params(bottom=False, labelbottom=False)
+            [i.set_visible(True) for i in self.ax_cb.patches]
+            [i.set_visible(True) for i in self.ax_cb.collections]
 
+        self.set_labels(**self._label_kwargs)
         # tag layer for refetch
         self._m.redraw(self._m.layer)
 
     def _identify_parent_cb(self):
         parent_cb = None
         # check if there is already an existing colorbar for a Maps-object that shares
         # the same plot-axis.
@@ -525,53 +556,55 @@
             parent = self
             while parent._parent_cb is not None:
                 parent = parent._parent_cb
 
             return parent
 
     def _setup_axes(self):
-        horizontal = self._orientation == "horizontal"
-        add_hist = self._hist_size > 0.0001
+        zorder = 9999
 
+        horizontal = self._orientation == "horizontal"
+        hide_hist = self._hist_size < 0.0001
+        hide_axes = self._hist_size > 0.999
         # check if one of the parent colorbars has a colorbar, and if so,
         # use it to set the position of the colorbar.
         if self._inherit_position:
             if self._parent_cb is not None:
 
                 try:
                     parent_subplotspec = self._parent_cb._ax.get_subplotspec()
                 except AttributeError:
                     parent_subplotspec = None
 
                 if parent_subplotspec is not None:
                     self._ax = self._m.f.add_subplot(
                         parent_subplotspec,
                         label="cb",
-                        zorder=9999,
+                        zorder=zorder,
                     )
                 else:
                     self._ax = self._m.f.add_axes(
                         self._parent_cb._ax.get_position(),
                         label="cb",
-                        zorder=9999,
+                        zorder=zorder,
                     )
 
                 parent_extend = getattr(
                     self._parent_cb, "_extend", self._parent_cb._init_extend
                 )
 
                 if parent_extend is None:
                     try:
                         self._parent_cb._set_extend()
                         parent_extend = getattr(
                             self._parent_cb, "_extend", self._parent_cb._init_extend
                         )
 
                     except Exception:
-                        print(
+                        _log.exception(
                             "EOmaps: unable to determine automatic extension arrow"
                             "size of parent colorbar."
                         )
 
                 # inherit axis-position from the parent axis position
                 # (e.g. it can no longer be freely moved... its position is determined
                 # by the position of the parent-colorbar axis)
@@ -594,61 +627,67 @@
                         height_ratios=(1, self._pos),
                     )
 
                     self._m.ax.set_subplotspec(gs[0, 0])
                     self._ax = self._m.f.add_subplot(
                         gs[1, 0],
                         label="cb",
-                        zorder=9999,
+                        zorder=zorder,
                     )
                 else:
                     gs = GridSpecFromSubplotSpec(
                         1,
                         2,
                         self._m.ax.get_subplotspec(),
                         width_ratios=(1, self._pos),
                     )
 
                     self._m.ax.set_subplotspec(gs[0, 0])
                     self._ax = self._m.f.add_subplot(
                         gs[0, 1],
                         label="cb",
-                        zorder=9999,
+                        zorder=zorder,
                     )
             elif isinstance(self._pos, SubplotSpec):
                 self._ax = self._m.f.add_subplot(
                     self._pos,
                     label="cb",
-                    zorder=9999,
+                    zorder=zorder,
                 )
             elif isinstance(self._pos, (list, tuple)):
                 x0, y0, w, h = self._pos
                 x1 = x0 + w
                 y1 = y0 + h
                 bbox = mtransforms.Bbox(((x0, y0), (x1, y1)))
 
                 # the parent axes holding the 2 child-axes
-                self._ax = plt.Axes(self._m.f, bbox, label="cb", zorder=9999)
+                self._ax = plt.Axes(self._m.f, bbox, label="cb", zorder=zorder)
                 self._m.f.add_axes(self._ax)
 
         # make all spines, labels etc. invisible for the base-axis
         self._ax.set_axis_off()
 
         # colorbar axes
         self.ax_cb = self._ax.figure.add_axes(
             self._ax.get_position(),
             label="EOmaps_cb",
-            zorder=9998,
+            zorder=zorder - 1,  # make zorder 1 lower than container axes for picking
         )
+
         # histogram axes
         self.ax_cb_plot = self._ax.figure.add_axes(
             self._ax.get_position(),
             label="EOmaps_cb_hist",
-            zorder=9998,
+            zorder=zorder - 1,  # make zorder 1 lower than container axes for picking
         )
+        # hide histogram and coorbar axes if they are 0 size
+        if hide_axes:
+            self.ax_cb.set_visible(False)
+        if hide_hist:
+            self.ax_cb_plot.set_visible(False)
 
         if self._inherit_position:
             # handle axis size in case parent colorbar has extension arrows
             if parent_extend in ["min", "both", None]:
                 padx = -self._parent_cb._extend_frac
             else:
                 padx = 0
@@ -692,18 +731,14 @@
                 self.ax_cb_plot.set_yscale("linear")
         else:
             if self._log is True:
                 self.ax_cb_plot.set_xscale("log")
             else:
                 self.ax_cb_plot.set_xscale("linear")
 
-        # hide histogram axis if no histogram should be drawn
-        if not add_hist:
-            self.ax_cb_plot.set_visible(False)
-
         # add all axes as artists
         for a in self._axes:
             a.set_navigate(False)
             if a is not None:
                 if self._dynamic_shade_indicator is True:
                     self._m.BM.add_artist(a, self._m.layer)
                 else:
@@ -719,15 +754,15 @@
         return (self._ax, self.ax_cb, self.ax_cb_plot)
 
     def _set_extend(self, z_data):
         if self._inherit_position and self._parent_cb is not None:
             self._extend = self._parent_cb._extend
             # warn if provided extend behavior differs from the inherited behavior
             if self._extend != self._init_extend:
-                print(
+                _log.warning(
                     f"EOmaps Warning: m.add_colorbar(extend='{self._extend}') is "
                     "inherited from the parent colorbar! Explicitly set the 'extend' "
                     "behavior to silence this warning."
                 )
             if self._extend is not None:
                 return
 
@@ -746,34 +781,34 @@
             self._extend = extend
 
     def _set_data(self):
         renorm = False
 
         dynamic_shade = False
         if self._dynamic_shade_indicator:
-            if _register_datashader() and isinstance(
-                self._coll, mpl_ext.ScalarDSArtist
-            ):
+            ds, mpl_ext = register_modules("datashader", "datashader.mpl_ext")
+
+            if all((ds, mpl_ext)) and isinstance(self._coll, mpl_ext.ScalarDSArtist):
                 dynamic_shade = True
             else:
-                print(
-                    "EOmaps: using 'dynamic_shade_indicator=True' is only possible "
+                _log.error(
+                    "EOmaps: Using 'dynamic_shade_indicator=True' is only possible "
                     "with 'shade' shapes (e.g. 'shade_raster' or 'shade_points'.\n"
                     "... creating a normal colorbar instead."
                 )
                 self._dynamic_shade_indicator = False
 
         if dynamic_shade:
             aggname = self._m.shape.aggregator.__class__.__name__
             if aggname in ["first", "last", "max", "min", "mean", "mode"]:
                 pass
             else:
                 renorm = True
                 # TODO check this without requiring import of datashader!
-                # print(
+                # _log.error(
                 #     "EOmaps: Only dynamic colorbars are possible when using"
                 #     + f" '{aggname}' as datashader-aggregation reduction method "
                 #     + "...creating a 'dynamic_shade_indicator' colorbar instead."
                 # )
                 # self._dynamic_shade_indicator = True
 
             try:
@@ -923,15 +958,15 @@
             limsetfunc = self.ax_cb.set_xlim
         else:
             limsetfunc = self.ax_cb.set_ylim
 
         if self._vmin != self._vmax:
             limsetfunc(self._vmin, self._vmax)
         else:
-            print(
+            _log.error(
                 "EOMaps-Warning: Attempting to set identical upper and "
                 + "lower limits for the colorbar... limits will be ignored!"
             )
 
         # set the axis_locator to set relative axis positions
         # TODO check why colorbar axis size changes after plot!
         # (e.g. this needs to be called AFTER plotting the colorbar to make sure
@@ -1081,16 +1116,16 @@
         if self._m.layer not in self._m.BM.bg_layer.split("|"):
             return
 
         self._set_data()
         self.ax_cb_plot.clear()
         self._plot_histogram()
 
-        if self._hist_label_kwargs:
-            self._set_labels(**self._hist_label_kwargs)
+        # if self._hist_label_kwargs:
+        #     self._set_labels(**self._hist_label_kwargs)
 
     def set_bin_labels(self, bins, names, tick_lines="center", show_values=False):
         """
         Set the tick-labels of the colorbar to custom names with respect to a given
         set of bins.
 
         The labels will be placed at the center of each bin.
```

### Comparing `EOmaps-6.5/eomaps/compass.py` & `EOmaps-7.0/eomaps/compass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+"""Interactive Compass (or North Arrow)."""
+
+import logging
+
 import numpy as np
 
 from matplotlib.collections import PolyCollection
 from matplotlib.textpath import TextPath
 from matplotlib.patches import PathPatch, CirclePolygon
 from matplotlib.offsetbox import AuxTransformBox
 import matplotlib.transforms as transforms
 
+_log = logging.getLogger(__name__)
+
 
 class Compass:
     """Base class for EOmaps compass objects."""
 
     def __init__(self, m):
         self._m = m
 
@@ -252,23 +258,23 @@
 
         lon, lat = self._m._transf_plot_to_lonlat.transform(*pos)
         x, y = self._m._transf_lonlat_to_plot.transform([lon, lon], [lat, lat + 0.01])
 
         try:
             ang = -np.arctan2(x[1] - x[0], y[1] - y[0])
         except Exception:
-            print("EOmaps: could not add scalebar at the desired location")
+            _log.error("EOmaps: Unable to add a compass at the desired location.")
             return
 
         if np.isnan(ang):
             if not self._ignore_invalid_angles:
                 if self._last_ang != self._ang:
-                    print(
+                    _log.error(
                         "EOmaps: Compass rotation-angle could not be determined! "
-                        f"... using last found angle: {np.rad2deg(self._ang):.2f}"
+                        f"... using angle: {np.rad2deg(self._ang):.2f}"
                     )
                     patch = self._artist.get_children()[0]
                     self._patch_ec = patch.get_edgecolor()
                     patch.set_edgecolor("r")
 
                 self._last_ang = self._ang
             else:
@@ -285,17 +291,24 @@
 
             self._last_ang = 9999
 
         self._ang = ang
         r = transforms.Affine2D().rotate(ang)
         # apply the scale-factor with respect to the current figure dpi to keep the
         # relative size of the north-arrow on dpi-changes!
-        s = transforms.Affine2D().scale(self._scale * self._m.f.dpi / self._init_dpi)
+        s = transforms.Affine2D().scale(
+            self._scale
+        )  # * self._m.f.dpi / self._init_dpi)
         t = transforms.Affine2D().translate(*self._m.ax.transData.transform(pos))
         trans = r + s + t
+
+        # cycle position once through transFigure to ensure correct positioning
+        # of the compass for agg exports (png, jpeg.. pixel-based) and
+        # svg/pdf based exports (point-based)
+        trans = trans + self._m.f.transFigure.inverted() + self._m.f.transFigure
         return trans
 
     def _on_motion(self, evt):
         if not self._layer_visible:
             return
 
         if self._check_still_parented() and self._got_artist:
```

### Comparing `EOmaps-6.5/eomaps/draw.py` & `EOmaps-7.0/eomaps/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,49 @@
 """
-A class to draw shapes on maps created with EOmaps
+Functionalities to draw shapes on maps created with EOmaps.
 
 Known Issues:
--------------
 
 It can happen that geopandas silently ignores the crs when writing shapefiles
 (in case WKT2 strings are required to represent the crs)
 ->>
 
 ... already reported to geopandas... might take some time to resolve:
 https://github.com/geopandas/geopandas/issues/2387
 
 """
+
+import logging
 from contextlib import contextmanager
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-import eomaps._shapes as eoshp
-
-gpd = None
-pd = None
-shapely_Polygon = None
-
-
-def _register_geopandas():
-    global pd
-    global gpd
-    global shapely_Polygon
-    try:
-        import geopandas as gpd
-        import pandas as pd
-        from shapely.geometry import Polygon as shapely_Polygon
-    except ImportError:
-        return False
+from .shapes import Shapes
+from .helpers import register_modules
 
-    return True
+_log = logging.getLogger(__name__)
 
 
 @contextmanager
 def autoscale_turned_off(ax=None):
+    """Contextmanager to revert axis-limits."""
     ax = ax or plt.gca()
     lims = [ax.get_xlim(), ax.get_ylim()]
     yield
     ax.set_xlim(*lims[0])
     ax.set_ylim(*lims[1])
 
 
 # ----------------------------------------------------------------------------------
 
 
 class ShapeDrawer:
+    """Base-class for drawing shapes on a map."""
+
     def __init__(self, m, layer=None, dynamic=True):
         """
         Base-class for drawing shapes on a map.
 
         Parameters
         ----------
         m : eomaps.Maps
@@ -64,14 +53,19 @@
             If None, the currently active layer will be used.
             The default is None.
         dynamic : bool
             If True, shapes are added as dynamic artists to avoid re-drawing
             the background after the draw is finished.
             If False, the shapes are added as background-artists.
         """
+        global gpd, pd, sh_geom
+        gpd, pd, sh_geom = register_modules(
+            "geopandas", "pandas", "shapely.geometry", raise_exception=False
+        )
+        self._can_save = all((gpd, pd, sh_geom))
 
         self._m = m
 
         # # add a slot to remember active drawers
         # # (used to make sure that 2 ShapeDrawer instances do not draw at the same time)
         # if not hasattr(self._m.parent, "_active_drawer"):
         #     self._m.parent._active_drawer = None
@@ -82,15 +76,15 @@
         if self._m.crs_plot == self._m.CRS.PlateCarree():
             # temporary workaround for geopandas issue with WKT2 strings
             # https://github.com/geopandas/geopandas/issues/2387
             self._crs = 4326
         else:
             self._crs = self._m.crs_plot.to_wkt()
 
-        if _register_geopandas():
+        if gpd:
             self.gdf = gpd.GeoDataFrame(geometry=[], crs=self._crs)
             ShapeDrawer.save_shapes.__doc__ = gpd.GeoDataFrame.to_file.__doc__
         else:
             self.gdf = None
 
         self._cids = []
         self._clicks = []
@@ -124,16 +118,17 @@
             return self._m.BM._bg_layer
         else:
             return self._layer
 
     @property
     def _background(self):
         # always use the currently active background as draw-background
+        # (and make sure to cache it)
         layer = self._m.BM._get_showlayer_name(self._m.BM._bg_layer)
-        return self._m.BM._bg_layers.get(layer, None)
+        return self._m.BM._get_background(layer, cache=True)
 
     @_active_drawer.setter
     def _active_drawer(self, val):
         self._m.parent._active_drawer = val
 
     def new_drawer(self, layer=None, dynamic=True):
         """
@@ -178,14 +173,17 @@
         Parameters
         ----------
         cb : callable, optional
             A callable executed after finishing the draw. The default is None.
         """
         self._m.cb.execute_callbacks(True)
 
+        if cb is None:
+            self._m._emit_signal("drawAborted")
+
         active_drawer = self._active_drawer
         if active_drawer is None:
             return
 
         while len(active_drawer._cids) > 0:
             active_drawer._m.f.canvas.mpl_disconnect(active_drawer._cids.pop())
 
@@ -196,21 +194,25 @@
             self._endline = None
             self._shape_indicator = None
 
         if cb is not None:
             try:
                 cb()
             except Exception:
-                print("EOmaps: There was a problem while executing a draw-callback!")
+                _log.exception(
+                    "EOmaps: There was a problem while executing a draw-callback!"
+                )
 
         active_drawer._clicks.clear()
 
         self._m.BM.update()
         self._active_drawer = None
 
+        self._m._emit_signal("drawFinished")
+
     def save_shapes(self, filename, **kwargs):
         """
         Save the drawn shapes to a file.
 
         Parameters
         ----------
         filename : str
@@ -218,33 +220,33 @@
         kwargs :
             Additional kwargs are passed to Geopandas.GeoDataFrame.to_file(...)
 
         """
         if len(self.gdf) > 0:
             self.gdf.to_file(filename, **kwargs)
         else:
-            print("EOmaps: There are no polygons to save!")
+            _log.error("EOmaps: There are no polygons to save!")
 
     def remove_last_shape(self):
         """
         Remove the most recently plotted polygon from the map.
         """
         if len(self._artists) == 0:
-            print("EOmaps: There is no shape to remove!")
+            _log.error("EOmaps: There is no shape to remove!")
             return
 
         ID = list(self._artists)[-1]
         a = self._artists.pop(ID)
         if self._dynamic:
             self._m.BM.remove_artist(a)
         else:
             self._m.BM.remove_bg_artist(a)
         a.remove()
 
-        if _register_geopandas():
+        if self._can_save:
             self.gdf = self.gdf.drop(ID)
 
         for cb in self._on_poly_remove:
             cb()
 
         self._m.BM.on_draw(None)
 
@@ -277,14 +279,15 @@
         return (
             i
             for i in (self._shape_indicator, self._line, self._pointer, self._endline)
             if i is not None
         )
 
     def redraw(self, blit=True, *args):
+        """Trigger re-drawing shapes."""
         # NOTE: If a drawer is active, this function is also called on any ordinary
         # draw-event (e.g. zoom/pan/resize) to keep the indicators visible.
         # see "m.BM.on_draw()"
 
         artists = self._indicator_artists
 
         if self._dynamic:
@@ -348,28 +351,24 @@
         The keyboard can also be used to select points in case your mouse
         does not have one or more of the buttons.  The delete and backspace
         keys act like right clicking (i.e., remove last point), the enter key
         terminates input and any other key (not already used by the window
         manager) selects a point.
         """
 
-        # make sure all active drawings are finished before starting a new one
-        self._active_drawer._finish_drawing()
-        self._active_drawer = self
-
         canvas = self._m.BM.canvas
         # self.fetch_bg()
 
         self._m.cb.execute_callbacks(False)
 
         def handler(event):
             self._init_draw_line()
 
             if event.name == "close_event":
-                self._finish_drawing(cb=cb)
+                self._finish_drawing()
                 return
 
             if (canvas.toolbar is not None) and canvas.toolbar.mode != "":
                 return
 
             is_button = (
                 event.name == "button_press_event"
@@ -519,18 +518,14 @@
         The keyboard can also be used to select points in case your mouse
         does not have one or more of the buttons.  The delete and backspace
         keys act like right clicking (i.e., remove last point), the enter key
         terminates input and any other key (not already used by the window
         manager) selects a point.
         """
 
-        # make sure all active drawings are finished before starting a new one
-        self._active_drawer._finish_drawing()
-        self._active_drawer = self
-
         canvas = self._m.BM.canvas
         # self.fetch_bg()
         self._m.cb.execute_callbacks(False)
 
         def handler(event):
             self._init_draw_line()
             self._init_shape_indicator()
@@ -547,23 +542,14 @@
                     # indicate current mouse-position (e.g. the center of the shape)
                     if len(self._clicks) == 0:
                         self._pointer.set_data([event.xdata], [event.ydata])
                     else:
                         self._pointer.set_data([], [])
 
                     movecb(event, self._clicks)
-
-                artists = (
-                    i for i in (self._shape_indicator, self._line, self._pointer) if i
-                )
-                if self._dynamic:
-                    # draw all previously drawn shapes as well
-                    artists = (*artists, *self._artists.values())
-
-                self._m.BM.blit_artists(artists, bg=self._background)
                 return
 
             is_button = event.name == "button_press_event"
             is_key = event.name == "key_press_event"
             # Quit (even if not in infinite mode; this is consistent with
             # MATLAB and sometimes quite useful, but will require the user to
             # test how many points were actually returned before using data).
@@ -641,14 +627,20 @@
             additional kwargs passed to the shape.
         """
         kwargs.setdefault("zorder", 10)
 
         def cb():
             self._polygon(**kwargs)
 
+        # make sure all active drawings are finished before starting a new one
+        self._active_drawer._finish_drawing()
+        self._active_drawer = self
+
+        self._m._emit_signal("drawStarted", "Polygon")
+
         self._ginput(-1, timeout=-1, draw_on_drag=draw_on_drag, cb=cb)
 
     def _polygon(self, **kwargs):
         pts = self._clicks
         if pts is not None and len(pts) > 2:
             pts = np.asarray(pts)
 
@@ -660,16 +652,16 @@
                 else:
                     self._m.BM.add_bg_artist(ph, layer=self.layer)
                     self._m.BM.on_draw(None)
 
                 ID = max(self._artists) + 1 if self._artists else 0
                 self._artists[ID] = ph
 
-            if _register_geopandas():
-                gdf = gpd.GeoDataFrame(index=[ID], geometry=[shapely_Polygon(pts)])
+            if self._can_save:
+                gdf = gpd.GeoDataFrame(index=[ID], geometry=[sh_geom.Polygon(pts)])
                 gdf = gdf.set_crs(crs=self._crs)
                 self.gdf = pd.concat([self.gdf, gdf])
 
             for cb in self._on_new_poly:
                 cb()
 
     def circle(self, **kwargs):
@@ -699,40 +691,52 @@
             if len(pts) == 1:
                 x, y = event.xdata, event.ydata
                 if (x is None) or (y is None):
                     return
 
                 r = np.sqrt((x - pts[0][0]) ** 2 + (y - pts[0][1]) ** 2)
 
-                pts = eoshp.shapes._ellipses(self._m)._get_ellipse_points(
+                pts = Shapes._Ellipses(self._m)._get_ellipse_points(
                     np.array([pts[0][0]]),
                     np.array([pts[0][1]]),
                     "out",
                     [r, r],
                     "out",
                     100,
                 )
                 self._shape_indicator.set_xy(np.column_stack((pts[0][0], pts[1][0])))
 
                 artists = (self._shape_indicator, self._line)
+
                 if self._dynamic:
                     # draw all previously drawn shapes as well
                     artists = (*artists, *self._artists.values())
 
                 self._m.BM.blit_artists(artists, bg=self._background)
+            else:
+                if self._pointer is not None:
+                    self._m.BM.blit_artists(
+                        (*self._artists.values(), self._pointer), bg=self._background
+                    )
+
+        # make sure all active drawings are finished before starting a new one
+        self._active_drawer._finish_drawing()
+        self._active_drawer = self
+
+        self._m._emit_signal("drawStarted", "Circle")
 
         self._ginput2(2, timeout=-1, draw_on_drag=True, movecb=movecb, cb=cb)
 
     def _circle(self, **kwargs):
         pts = self._clicks
         if pts is not None and len(pts) == 2:
             pts = np.asarray(pts)
 
             r = np.sqrt(sum((pts[1] - pts[0]) ** 2))
-            pts = eoshp.shapes._ellipses(self._m)._get_ellipse_points(
+            pts = Shapes._Ellipses(self._m)._get_ellipse_points(
                 np.array([pts[0][0]]), np.array([pts[0][1]]), "out", [r, r], "out", 100
             )
 
             with autoscale_turned_off(self._m.ax):
                 (ph,) = self._m.ax.fill(pts[0][0], pts[1][0], **kwargs)
 
                 if self._dynamic:
@@ -740,17 +744,17 @@
                 else:
                     self._m.BM.add_bg_artist(ph, layer=self.layer)
                     self._m.BM.on_draw(None)
 
                 ID = max(self._artists) + 1 if self._artists else 0
                 self._artists[ID] = ph
 
-            if _register_geopandas():
+            if self._can_save:
                 pts = np.column_stack((pts[0][0], pts[1][0]))
-                gdf = gpd.GeoDataFrame(index=[ID], geometry=[shapely_Polygon(pts)])
+                gdf = gpd.GeoDataFrame(index=[ID], geometry=[sh_geom.Polygon(pts)])
                 gdf = gdf.set_crs(crs=self._crs)
                 self.gdf = pd.concat([self.gdf, gdf])
 
             for cb in self._on_new_poly:
                 cb()
 
     def rectangle(self, **kwargs):
@@ -778,35 +782,46 @@
         def movecb(event, pts):
             if len(pts) == 1:
                 x, y = event.xdata, event.ydata
                 if (x is None) or (y is None):
                     return
 
                 r = abs(x - pts[0][0]), abs(y - pts[0][1])
-                pts = eoshp.shapes._rectangles(self._m)._get_rectangle_verts(
+                pts = Shapes._Rectangles(self._m)._get_rectangle_verts(
                     np.array([pts[0][0]]), np.array([pts[0][1]]), "out", r, "out", 50
                 )[0][0]
 
                 self._shape_indicator.set_xy(np.column_stack((pts[:, 0], pts[:, 1])))
 
                 artists = (self._shape_indicator, self._line)
                 if self._dynamic:
                     # draw all previously drawn shapes as well
                     artists = (*artists, *self._artists.values())
 
                 self._m.BM.blit_artists(artists, bg=self._background)
+            else:
+                if self._pointer is not None:
+                    self._m.BM.blit_artists(
+                        (*self._artists.values(), self._pointer), bg=self._background
+                    )
+
+        # make sure all active drawings are finished before starting a new one
+        self._active_drawer._finish_drawing()
+        self._active_drawer = self
+
+        self._m._emit_signal("drawStarted", "Rectangle")
 
         self._ginput2(2, timeout=-1, draw_on_drag=True, movecb=movecb, cb=cb)
 
     def _rectangle(self, **kwargs):
         pts = self._clicks
         if pts is not None and len(pts) == 2:
             r = abs(pts[1][0] - pts[0][0]), abs(pts[1][1] - pts[0][1])
 
-            pts = eoshp.shapes._rectangles(self._m)._get_rectangle_verts(
+            pts = Shapes._Rectangles(self._m)._get_rectangle_verts(
                 np.array([pts[0][0]]), np.array([pts[0][1]]), "out", r, "out", 50
             )[0][0]
 
             with autoscale_turned_off(self._m.ax):
                 (ph,) = self._m.ax.fill(pts[:, 0], pts[:, 1], **kwargs)
 
                 if self._dynamic:
@@ -814,14 +829,14 @@
                 else:
                     self._m.BM.add_bg_artist(ph, layer=self.layer)
                     self._m.BM.on_draw(None)
 
                 ID = max(self._artists) + 1 if self._artists else 0
                 self._artists[ID] = ph
 
-            if _register_geopandas():
-                gdf = gpd.GeoDataFrame(index=[ID], geometry=[shapely_Polygon(pts)])
+            if self._can_save:
+                gdf = gpd.GeoDataFrame(index=[ID], geometry=[sh_geom.Polygon(pts)])
                 gdf = gdf.set_crs(crs=self._crs)
                 self.gdf = pd.concat([self.gdf, gdf])
 
             for cb in self._on_new_poly:
                 cb()
```

### Comparing `EOmaps-6.5/eomaps/eomaps.py` & `EOmaps-7.0/eomaps/eomaps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,95 +1,25 @@
-"""A collection of helper-functions to generate map-plots."""
+"""General definition of Maps objects."""
+
+import logging
+
+_log = logging.getLogger(__name__)
 
 from functools import lru_cache, wraps
-from itertools import repeat
-from textwrap import dedent
-import warnings
+from itertools import repeat, chain
 import copy
 from types import SimpleNamespace
 from pathlib import Path
 import weakref
 import gc
 from textwrap import fill
 from contextlib import contextmanager, ExitStack
 
 import numpy as np
 
-# ------- perform lazy delayed imports
-# (for optional dependencies that take long time to import)
-
-
-pd = None
-
-
-def _register_pandas():
-    global pd
-    try:
-        import pandas as pd
-    except ImportError:
-        return False
-
-    return True
-
-
-gpd = None
-
-
-def _register_geopandas():
-    global gpd
-    try:
-        import geopandas as gpd
-    except ImportError:
-        return False
-
-    return True
-
-
-xar = None
-
-
-def _register_xarray():
-    global xar
-    try:
-        import xarray as xar
-    except ImportError:
-        return False
-
-    return True
-
-
-ds, mpl_ext = None, None
-
-
-def _register_datashader():
-    global ds
-    global mpl_ext
-
-    try:
-        import datashader as ds
-        from datashader import mpl_ext
-    except ImportError:
-        return False
-
-    return True
-
-
-mapclassify = None
-
-
-def _register_mapclassify():
-    global mapclassify
-    try:
-        import mapclassify
-    except ImportError:
-        return False
-
-    return True
-
-
 from pyproj import CRS, Transformer
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.gridspec import GridSpec, SubplotSpec
 
 import matplotlib.patches as mpatches
@@ -99,76 +29,106 @@
 
 from .helpers import (
     pairwise,
     cmap_alpha,
     BlitManager,
     LayoutEditor,
     progressbar,
-    searchtree,
+    SearchTree,
     _TransformedBoundsLocator,
     _add_to_docstring,
+    register_modules,
 )
-from ._shapes import shapes
+from .shapes import Shapes
 from .colorbar import ColorBar
 
 from ._containers import (
-    data_specs,
-    classify_specs,
+    DataSpecs,
+    ClassifySpecs,
 )
 
 try:
     from ._webmap import refetch_wms_on_size_change, _cx_refetch_wms_on_size_change
-    from ._webmap_containers import wms_container
+    from .webmap_containers import WebMapContainer
 except ImportError as ex:
-    print("EOmaps: Unable to import required WebMap dependencies:", ex)
+    _log.error(f"EOmaps: Unable to import dependencies required for WebMaps: {ex}")
     refetch_wms_on_size_change = None
     _cx_refetch_wms_on_size_change = None
-    wms_container = None
+    WebMapContainer = None
 
 from .ne_features import NaturalEarth_features
 
-from ._cb_container import cb_container, _gpd_picker
+from .cb_container import CallbackContainer, GeoDataFramePicker
 from .scalebar import ScaleBar
 from .compass import Compass
 from .projections import Equi7Grid_projection  # import to supercharge cartopy.ccrs
 from .reader import read_file, from_file, new_layer_from_file
 from .grid import GridFactory
 
 from .utilities import utilities
 from .draw import ShapeDrawer
+from .annotation_editor import AnnotationEditor
 
 from ._data_manager import DataManager
 
 from ._version import __version__
 
-_backend_warning_shown = False
-
 
 def _handle_backends():
-    global _backend_warning_shown
-
-    if plt.isinteractive():
-        if plt.get_backend() in [
-            "module://ipympl.backend_nbagg",
-            "module://matplotlib_inline.backend_inline",
-        ]:
+    # make sure that the backend is activated
+    # (backends are loaded lazily and values such as plt.isinteractive() might not
+    # yet show the correct value in case the backend is not yet fully loaded)
+
+    # This is especially important for the IPython/inline backend which explicitly
+    # calls plt.ion() when the backend is loaded.
+    # (see https://github.com/matplotlib/matplotlib/issues/26221)
+    plt.install_repl_displayhook()
+
+    active_backend = plt.get_backend()
+
+    if active_backend in ["module://matplotlib_inline.backend_inline"]:
+        plt.ioff()
+
+        if not Maps._backend_warning_shown and not BlitManager._snapshot_on_update:
+            _log.info(
+                "EOmaps disables matplotlib's interactive mode (e.g. 'plt.ioff()') "
+                f"for the backend {plt.get_backend()}.\n"
+                "Call `m.snapshot()` to print a static snapshot of the map "
+                "to a Jupyter Notebook cell (or an IPython console)!"
+            )
+
+            Maps._backend_warning_shown = True
+
+    # to avoid flickering in the layout editor in jupyter notebooks
+    elif active_backend in ["module://ipympl.backend_nbagg"]:
+        plt.ioff()
+    else:
+        if Maps._use_interactive_mode:
+            plt.ion()
+        else:
             plt.ioff()
+            _log.debug(
+                "EOmaps: matplotlib's interactive mode is turned off. "
+                "Call `m.show()` to show the map!"
+            )
 
-            if not _backend_warning_shown:
-                warnings.warn(
-                    "EOmaps disables matplotlib's interactive mode (e.g. 'plt.ioff()') "
-                    f"for the backend {plt.get_backend()}.\n"
-                    "Call `m.snapshot()` to print a static snapshot of the map "
-                    "to a Jupyter Notebook cell (or an IPython console)!"
-                )
-
-                _backend_warning_shown = True
-
+    # check if we are in an ipython console using the inline-backend.
+    # If yes, put a snapshot of the map into the active cell on each update
+    if BlitManager._snapshot_on_update is None:
+        try:
+            __IPYTHON__
+        except NameError:
+            BlitManager._snapshot_on_update = False
+        else:
+            active_backend = plt.get_backend()
+            # print a snapshot to the active ipython cell in case the
+            # inline-backend is used
+            if active_backend in ["module://matplotlib_inline.backend_inline"]:
+                BlitManager._snapshot_on_update = True
 
-_handle_backends()
 
 # hardcoded list of available mapclassify-classifiers
 # (to avoid importing it on startup)
 _CLASSIFIERS = (
     "BoxPlot",
     "EqualInterval",
     "FisherJenks",
@@ -183,27 +143,114 @@
     "Quantiles",
     "Percentiles",
     "StdMean",
     "UserDefined",
 )
 
 
-class Maps(object):
+class _MapsMeta(type):
+
+    _use_interactive_mode = True
+    _always_on_top = False
+
+    _backend_warning_shown = False
+
+    def config(
+        cls,
+        snapshot_on_update=None,
+        companion_widget_key=None,
+        always_on_top=None,
+        use_interactive_mode=True,
+        log_level=None,
+    ):
+        """
+        Set global configuration parameters for figures created with EOmaps.
+
+        This function must be called before initializing any :py:class:`Maps` object!
+
+        >>> from eomaps import Maps
+        >>> Maps.config(always_on_top=True)
+
+        (parameters set to None are NOT updated!)
+
+        Parameters
+        ----------
+        snapshot_on_update : bool, optional
+            Only relevant when using an IPython console or a jupyter notebook together
+            with the `inline` backend! (e.g. using `%matplotlib inline`)
+
+            - If True, figure updates automatically trigger drawing a snapshot
+              of the current state of the figure to the active cell.
+            - If False, an explicit call to `m.show()` is required to draw the figure.
+
+            The default is True.
+        companion_widget_key : str, optional
+            The keyboard shortcut to use for activating the companion-widget.
+            The default is "w".
+        always_on_top : bool, optional
+            Only relevant if `PyQt5` is used as matplotlib backend.
+
+            - If True, the figure will be kept "always on top" of other applications.
+
+            The default is False.
+        use_interactive_mode : bool, optional
+            If True, matplotlibs interactive mode (`plt.ion()`) is activated by default
+            for all backends except jupyter-notebook backends (`inline` and `ipympl`).
+
+            If False, a call to `m.show()` is required to trigger showing the figure!
+
+            The default is True.
+        log_level : str or int, optional
+            The logging level.
+            If set, a StreamHandler will be attached to the logger that prints to
+            the active terminal at the specified log level.
+
+            See :py:meth:`set_loglevel` on how to customize logging format.
+
+            The default is None.
+        """
+
+        from . import set_loglevel
+
+        if companion_widget_key is not None:
+            Maps._companion_widget_key = companion_widget_key
+
+        if always_on_top is not None:
+            Maps._always_on_top = always_on_top
+
+        if snapshot_on_update is not None:
+            BlitManager._snapshot_on_update = snapshot_on_update
+
+        if use_interactive_mode is not None:
+            Maps._use_interactive_mode = use_interactive_mode
+
+        if log_level is not None:
+            set_loglevel(log_level)
+
+
+class Maps(metaclass=_MapsMeta):
     """
     The base-class for generating plots with EOmaps.
 
+    The first Maps object that is initialized will create a new matplotlib `Figure`
+    and a cartopy `GeoAxes` for a map.
+
+    You can then create additional `Maps` objects on the same figure with the following
+    methods:
+
+
     See Also
     --------
     Maps.new_layer : Create a new layer for the map.
 
     Maps.new_map : Add a new map to the figure.
 
     Maps.new_inset_map : Add a new inset-map to the figure.
 
-    MapsGrid : Initialize a grid of Maps objects
+    :py:class:`~eomaps.mapsgrid.MapsGrid` : Initialize a grid of Maps objects
 
     Parameters
     ----------
     crs : int or a cartopy-projection, optional
         The projection of the map.
         If int, it is identified as an epsg-code
         Otherwise you can specify any projection supported by `cartopy.crs`
@@ -258,81 +305,42 @@
         The default is "wms"
     kwargs :
         additional kwargs are passed to `matplotlib.pyplot.figure()`
         - e.g. figsize=(10,5)
 
     Examples
     --------
-    Create a new figure and axes
-
-    >>> m = Maps()
-    >>> ...
-
-    Create a new figure and position the map at (left, bottom, width, height)
-
-    >>> m = Maps(ax=(.25, .5, .5, .5))
+    Create a new Maps object and initialize a figure and axes for a map.
 
-    Use an existing figure and position the map at (left, bottom, width, height)
-
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib.gridspec import GridSpec
-    >>> f = plt.figure()
-    >>> m = Maps(f=f, ax=(.25, .5, .5, .5))
-
-    Use a 3-digit integer to set the grid-position of the map
-    (nrows, ncols, index)
-
-    >>> from matplotlib.gridspec import GridSpec
-    >>> m = Maps(ax=221)
-
-    Use a tuple of 3 integers to set the grid-position of the map
-    (nrows, ncols, index)
-
-    >>> from matplotlib.gridspec import GridSpec
-    >>> m = Maps(ax=(2, 2, 1))
-
-    Put the map at a grid-position of an existing figure
-
-    >>> import matplotlib.pyplot as plt
-    >>> f = plt.figure()
-    >>> ax = f.add_subplot(211)
-    >>> m = Maps(f=f, ax=212)
-
-    Use a subplotspec to set the axis position
-
-    >>> from matplotlib.gridspec import GridSpec
-    >>> gs = GridSpec(2,2)
-    >>> m = Maps(ax=gs[0,0])
-
-    Use an existing axis to create the Maps-object
-    (the associated figure is automatically detected)
-
-    >>> import matplotlib.pyplot as plt
     >>> from eomaps import Maps
-    >>> f = plt.figure()
-    >>> ax = f.add_subplot(projection=Maps.CRS.Mollweide())
-    >>> m = Maps(ax=ax)
+    >>> m = Maps()
+    >>> # add basic background features to the map
+    >>> m.add_feature.preset("coastline", "ocean", "land")
+    >>> # create a new layer and add more features
+    >>> m1 = m.new_layer("layer 1")
+    >>> m1.add_feature.physical.coastline(fc="none", ec="b", lw=2, scale=50)
+    >>> m1.add_feature.cultural.admin_0_countries(fc=(.2,.1,.4,.2), ec="b", lw=1, scale=50)
+    >>> # overlay a part of the new layer in a circle if you click on the map
+    >>> m.cb.click.attach.peek_layer(m1.layer, how=0.4, shape="round")
 
     Use Maps-objects as context-manager to close the map and free memory
     once the map is exported.
 
-    >>> import matplotlib
-    >>> matplotlib.use("agg") # we can use a non-GUI backend since we only export png's
     >>> from eomaps import Maps
     >>> with Maps() as m:
     >>>     m.add_feature.preset.coastline()
     >>>     m.savefig(...)
 
     Attributes
     ----------
     CRS : Accessor for available projections (Supercharged version of cartopy.crs)
 
     CLASSIFIERS : Accessor for available classifiers (provided by mapclassify)
 
-    _companion_widget_key : Keyboard shortcut assigned to show/hide the companion-widget.
+    _companion_widget_key : Keyboard shortcut assigned to show/hide the companion-widget
 
     """
 
     __version__ = __version__
 
     from_file = from_file
     read_file = read_file
@@ -342,27 +350,40 @@
     # the keybord shortcut to activate the companion-widget
     _companion_widget_key = "w"
     # max. number of layers to show all layers as tabs in the widget
     # (otherwise only recently active layers are shown as tabs)
     _companion_widget_n_layer_tabs = 50
 
     CLASSIFIERS = SimpleNamespace(**dict(zip(_CLASSIFIERS, _CLASSIFIERS)))
+    "Accessor for available classification schemes."
 
-    _crs_cache = dict()
-    _transformer_cache = dict()
+    # arguments passed to m.savefig when using "ctrl+c" to export figure to clipboard
+    _clipboard_kwargs = dict()
 
     def __init__(
         self,
         crs=None,
         layer="base",
         f=None,
         ax=None,
         preferred_wms_service="wms",
         **kwargs,
     ):
+        self._log_on_event_messages = dict()
+        self._log_on_event_cids = dict()
+
+        try:
+            from .qtcompanion.signal_container import _SignalContainer
+
+            # initialize the signal container (MUST be done before init of the widget!)
+            self._signal_container = _SignalContainer()
+        except Exception:
+            _log.debug("SignalContainer could not be initialized", exc_info=True)
+            self._signal_container = None
+
         # make sure the used layer-name is valid
         layer = self._check_layer_name(layer)
 
         self._inherit_classification = None
 
         if isinstance(ax, plt.Axes) and hasattr(ax, "figure"):
             if isinstance(ax.figure, plt.Figure):
@@ -392,15 +413,15 @@
             i.layer == layer for i in (self.parent, *self.parent._children) if i != self
         ):
             self._is_sublayer = True
         else:
             self._is_sublayer = False
 
         self._companion_widget = None  # slot for the pyqt widget
-        self._cid_companion_key = None  # callback id for the companion-cb
+        self._cid_keypress = None  # callback id for PyQt5 keypress callbacks
         # a list to remember newly registered colormaps
         self._registered_cmaps = []
 
         # a list of actions that are executed whenever the widget is shown
         self._on_show_companion_widget = []
 
         # preferred way of accessing WMS services (used in the WMS container)
@@ -425,33 +446,33 @@
                 crs = 4326
 
             self._crs_plot = crs
 
         self._crs_plot_cartopy = self._get_cartopy_crs(self._crs_plot)
 
         # default classify specs
-        self.classify_specs = classify_specs(weakref.proxy(self))
+        self.classify_specs = ClassifySpecs(weakref.proxy(self))
 
-        self.data_specs = data_specs(
+        self.data_specs = DataSpecs(
             weakref.proxy(self),
             x="lon",
             y="lat",
             crs=4326,
         )
 
         self._layout_editor = None
 
-        self._cb = cb_container(weakref.proxy(self))  # accessor for the callbacks
+        self._cb = CallbackContainer(weakref.proxy(self))  # accessor for the callbacks
 
         self._init_figure(ax=ax, plot_crs=crs, **kwargs)
-        if wms_container is not None:
-            self._wms_container = wms_container(weakref.proxy(self))
+        if WebMapContainer is not None:
+            self._wms_container = WebMapContainer(weakref.proxy(self))
         self._new_layer_from_file = new_layer_from_file(weakref.proxy(self))
 
-        self._shapes = shapes(weakref.proxy(self))
+        self._shapes = Shapes(weakref.proxy(self))
         self._shape = None
 
         # the radius is estimated when plot_map is called
         self._estimated_radius = None
 
         # a set to hold references to the compass objects
         self._compass = set()
@@ -463,14 +484,16 @@
             self.parent._execute_callbacks = True
 
         # initialize the data-manager
         self._data_manager = DataManager(self._proxy(self))
         self._data_plotted = False
         self._set_extent_on_plot = True
 
+        self._edit_annotations = AnnotationEditor(self)
+
         # Make sure the figure-background patch is on an explicit layer
         # This is used to avoid having the background patch on each fetched
         # background while maintaining the capability of restoring it
         if self.f.patch not in self.BM._bg_artists.get("__BG__", []):
             self.BM.add_bg_artist(self.f.patch, layer="__BG__")
 
         # Treat cartopy geo-spines separately in the blit-manager
@@ -481,14 +504,17 @@
         # TODO find a better way to deal with this!
         self._handle_spines()
 
         # a factory to create gridlines
         if self.parent == self:
             self._grid = GridFactory(self.parent)
 
+            if Maps._always_on_top:
+                self._set_always_on_top(True)
+
     def _handle_spines(self):
         spine = self.ax.spines["geo"]
         if spine not in self.BM._bg_artists.get("__SPINES__", []):
             self.BM.add_bg_artist(spine, layer="__SPINES__")
 
     def __getattribute__(self, key):
         if key == "set_layout":
@@ -509,14 +535,87 @@
 
     def __exit__(self, type, value, traceback):
         self.cleanup()
         if self.parent == self:
             plt.close(self.f)
         gc.collect()
 
+    def _parse_log_level(self, level):
+        """
+        Get the numerical log-level from string (or number).
+
+        Parameters
+        ----------
+        level : str or number
+            The log level
+
+        Returns
+        -------
+        int_level : float
+            The numerical value of the log level.
+
+        """
+        from logging import getLevelNamesMapping
+
+        levels = getLevelNamesMapping()
+
+        if isinstance(level, str) and level.upper() in levels:
+            use_level = levels[level.upper()]
+        else:
+            use_level = float(level)
+
+        return use_level
+
+    def _log_on_event(self, level, msg, event):
+        """
+        Schedule a log message that will be shown on the next matplotlib event.
+
+        Identical scheduled messages are only shown once per event!
+
+        {'CRITICAL': 50, 'FATAL': 50, 'ERROR': 40, 'WARN': 30, 'WARNING': 30,
+         'INFO': 20,  'DEBUG': 10, 'NOTSET': 0}
+
+        Parameters
+        ----------
+        level : int or str
+            The logging level.
+        msg : str
+            The message.
+        event : str
+            The event name (e.g. "button_release_event")
+
+        """
+        level = self._parse_log_level(level)
+
+        messages = self._log_on_event_messages.setdefault(event, [])
+        cid = self._log_on_event_cids.setdefault(event, None)
+
+        # don't attach messages if they are already scheduled
+        if (level, msg) in messages:
+            return
+
+        messages.append((level, msg))
+
+        def log_message(*args, **kwargs):
+            cid = self._log_on_event_cids.get(event, None)
+            messages = self._log_on_event_messages.get(event, [])
+
+            if cid is not None:
+                self.f.canvas.mpl_disconnect(cid)
+                self._log_on_event_cids.pop(event, None)
+
+            while len(messages) > 0:
+                level, msg = messages.pop(0)
+                _log.log(level, msg)
+
+        if cid is None:
+            self._log_on_event_cids[event] = self.f.canvas.mpl_connect(
+                event, log_message
+            )
+
     @property
     def layer(self):
         """The layer-name associated with this Maps-object."""
         return self._layer
 
     @property
     def all(self):
@@ -560,15 +659,15 @@
         """
         if self._shape is None:
             self._set_default_shape()
 
         return self._shape
 
     @property
-    @wraps(cb_container)
+    @wraps(CallbackContainer)
     def cb(self):
         """Accessor to attach callbacks to the map."""
         return self._cb
 
     @property
     @wraps(utilities)
     def util(self):
@@ -688,16 +787,16 @@
                 (e.g. 111 is the same as (1, 1, 1) )
             - `matplotilb.gridspec.SubplotSpec`:
                 Use the SubplotSpec for initializing the axes.
             - `matplotilb.Axes`:
                 Directly use the provided figure and axes instances for plotting.
                 NOTE: The axes MUST be a geo-axes with `m.crs_plot` projection!
         keep_on_top : bool
-            If True, this axis will be drawn on top of all other maps.
-            (same as InsetMaps)
+            If True, this map will be drawn on top of all other axes.
+            (e.g. similar to InsetMaps)
             The default is False.
         preferred_wms_service : str, optional
             Set the preferred way for accessing WebMap services if both WMS and WMTS
             capabilities are possible.
             The default is "wms"
         kwargs :
             additional kwargs are passed to `matplotlib.pyplot.figure()`
@@ -708,16 +807,16 @@
         m: EOmaps.Maps
             The Maps object representing the new map.
 
         """
         m2 = Maps(f=self.f, ax=ax, **kwargs)
 
         if np.allclose(self.ax.bbox.bounds, m2.ax.bbox.bounds):
-            print(
-                "EOmaps: Warning! The new map overlaps exactly with the parent map! "
+            _log.warning(
+                "EOmaps:The new map overlaps exactly with the parent map! "
                 "Use `ax=...` or the LayoutEditor to adjust the position of the map."
             )
 
         if keep_on_top is True:
             m2.ax.set_label("inset_map")
 
             spine = m2.ax.spines["geo"]
@@ -781,32 +880,43 @@
         >>>     ...
         >>>     m2.show()                           # make the layer visible
         >>>     m2.savefig(...)                     # save it as an image
 
 
         See Also
         --------
-        copy : general way for copying Maps objects
+        Maps.copy : general way for copying Maps objects
+
         """
         if layer is None:
             layer = copy.deepcopy(self.layer)
+        else:
+            layer = str(layer)
+            if len(layer) == 0:
+                raise SyntaxError(
+                    "EOmaps: Unable to create a layer with an empty layer-name!"
+                )
 
         m = self.copy(
             data_specs=copy_data_specs,
             classify_specs=copy_classify_specs,
             shape=copy_shape,
             ax=self.ax,
             layer=layer,
         )
         # make sure the new layer does not attempt to reset the extent if
         # it has already been set on the parent layer
         m._set_extent_on_plot = self._set_extent_on_plot
 
         # re-initialize all sliders and buttons to include the new layer
         self.util._reinit_widgets()
+
+        # share the companion-widget with the parent
+        m._companion_widget = self._companion_widget
+
         return m
 
     def new_inset_map(
         self,
         xy=(45, 45),
         xy_crs=4326,
         radius=5,
@@ -899,44 +1009,40 @@
             The default is "ellipses".
         indicate_extent : bool or dict, optional
 
             - If True: add a polygon representing the inset-extent to the parent map.
             - If a dict is provided, it will be used to update the appearance of the
               added polygon (e.g. facecolor, edgecolor, linewidth etc.)
 
-            NOTE: you can also use `m_inset.indicate_inset_extent(...)` to manually
+            NOTE: you can also use `m_inset.add_extent_indicator(...)` to manually
             indicate the inset-shape on arbitrary Maps-objects.
 
             The default is True.
         indicator_line : bool or dict, optional
 
             - If True: add a line that connects the inset-map to the indicated extent
               on the parent map
             - If a dict is provided, it is used to update the appearance of the line
               (e.g. c="r", lw=2, ...)
 
             NOTE: you can also use `m_inset.add_indicator_line(...)` to manually
             indicate the inset-shape on arbitrary Maps-objects.
 
             The default is False.
+
         Returns
         -------
         m : eomaps.Maps
             A eomaps.Maps-object of the inset-map.
             (use it just like any other Maps-object)
 
         See Also
         --------
-        The following additional methods are defined on `InsetMaps` objects
-
-        m.indicate_inset_extent :
-            Plot a polygon representing the extent of the inset map on another Maps
-            object.
-        m.set_inset_position :
-            Set the (center) position and size of the inset-map.
+        Maps.add_extent_indicator : Indicate inset-extent on another map (as polygon).
+        Maps.set_inset_position : Set the (center) position and size of the inset-map.
 
         Examples
         --------
         Simple example:
 
         >>> m = Maps()
         >>> m.add_feature.preset.coastline()
@@ -960,15 +1066,15 @@
         >>>
         >>> m2.add_feature.preset.coastline()
         >>> m2.add_feature.preset.ocean()
         >>> m2.add_feature.preset.land()
         >>> m2.set_data([1, 2, 3], [5, 6, 7], [45, 46, 47], crs=4326)
         >>> m2.plot_map()
         >>> m2.add_annotation(ID=1)
-        >>> m2.indicate_inset_extent(m, ec="g", fc=(0,1,0,.25))
+        >>> m2.add_extent_indicator(m, ec="g", fc=(0,1,0,.25))
 
         Multi-layer inset-maps:
 
         >>> m = Maps(layer="first")
         >>> m.add_feature.preset.coastline()
         >>> m3 = m.new_layer("second")
         >>> m3.add_feature.preset.ocean()
@@ -978,15 +1084,19 @@
         >>> # create a new layer of the inset-map that will be
         >>> # visible if the "second" layer is visible
         >>> m3 = m2.new_layer(layer="second")
         >>> m3.add_feature.preset.coastline()
         >>> m3.add_feature.preset.land()
 
         >>> m.util.layer_selector()
+
         """
+        # to avoid circular imports
+        from .inset_maps import InsetMaps
+
         m2 = InsetMaps(
             parent=self,
             crs=inset_crs,
             layer=layer,
             xy=xy,
             radius=radius,
             plot_position=plot_position,
@@ -998,21 +1108,82 @@
             shape=shape,
             indicate_extent=indicate_extent,
             indicator_line=indicator_line,
         )
 
         return m2
 
+    def _get_always_on_top(self):
+        if "qt" in plt.get_backend().lower():
+            from PyQt5 import QtCore
+
+            w = self.f.canvas.window()
+            return bool(w.windowFlags() & QtCore.Qt.WindowStaysOnTopHint)
+
+        return False
+
+    def _set_always_on_top(self, q):
+        # keep pyqt window on top
+        try:
+            from PyQt5 import QtCore
+
+            if q:
+                # only do this if necessary to avoid flickering
+                # see https://stackoverflow.com/a/40007740/9703451
+                if not self._get_always_on_top():
+                    # in case pyqt is used as backend, also keep the figure on top
+                    if "qt" in plt.get_backend().lower():
+                        w = self.f.canvas.window()
+                        ws = w.size()
+                        w.setWindowFlags(
+                            w.windowFlags() | QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        w.resize(ws)
+                        w.show()
+
+                    # handle the widget in case it was activated (possible also for
+                    # backends other than qt)
+                    if self._companion_widget is not None:
+                        cw = self._companion_widget.window()
+                        cws = cw.size()
+                        cw.setWindowFlags(
+                            cw.windowFlags() | QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        cw.resize(cws)
+                        cw.show()
+
+            else:
+                if self._get_always_on_top():
+                    if "qt" in plt.get_backend().lower():
+                        w = self.f.canvas.window()
+                        ws = w.size()
+                        w.setWindowFlags(
+                            w.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        w.resize(ws)
+                        w.show()
+
+                    if self._companion_widget is not None:
+                        cw = self._companion_widget.window()
+                        cws = cw.size()
+                        cw.setWindowFlags(
+                            cw.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        cw.resize(cws)
+                        cw.show()
+        except Exception:
+            pass
+
     @property
-    @wraps(shapes)
+    @wraps(Shapes)
     def set_shape(self):
         """Set the plot-shape."""
         return self._shapes
 
-    def set_data_specs(
+    def set_data(
         self,
         data=None,
         x=None,
         y=None,
         crs=None,
         encoding=None,
         cpos="c",
@@ -1128,14 +1299,15 @@
         - integer-encoded datasets
 
           >>> lon, lat, vals = [...], [...], [1, 2, 3, ...]
           >>> encoding = dict(scale_factor=0.01, add_offset=1)
           >>> # colorbars and pick-callbacks will now show values as (1 + 0.01 * value)
           >>> # e.g. the "actual" data values are [0.01, 0.02, 0.03, ...]
           >>> m.set_data(vals, x=lon, y=lat, crs=4326, encoding=encoding)
+
         """
         if data is not None:
             self.data_specs.data = data
 
         if x is not None:
             self.data_specs.x = x
 
@@ -1153,15 +1325,30 @@
 
         if cpos_radius is not None:
             self.data_specs.cpos_radius = cpos_radius
 
         if parameter is not None:
             self.data_specs.parameter = parameter
 
-    set_data = set_data_specs
+    @wraps(set_data)
+    def set_data_specs(self, *args, **kwargs):
+        from warnings import warn
+
+        warn(
+            "EOmaps: `m.set_data_specs(...)` is depreciated and will raise  an "
+            "error in future versions! Use `m.set_data(...)` instead!",
+            FutureWarning,
+            stacklevel=2,
+        )
+        self.set_data(*args, **kwargs)
+
+    set_data_specs.__doc__ = (
+        "WARNING: `m.set_data_specs(...)` is depreciated! "
+        "Use `m.set_data(...)` instead!\n\n"
+    ) + set_data_specs.__doc__
 
     @property
     def set_classify(self):
         """
         Interface to the classifiers provided by the 'mapclassify' module.
 
         To set a classification scheme for a given Maps-object, simply use:
@@ -1195,33 +1382,30 @@
         >>> m.set_classify.Quantiles(k=5)
 
         >>> m.set_classify.EqualInterval(k=5)
 
         >>> m.set_classify.UserDefined(bins=[5, 10, 25, 50])
 
         """
-        assert _register_mapclassify(), (
-            "EOmaps: Missing dependency: 'mapclassify' \n ... please install"
-            + " (conda install -c conda-forge mapclassify) to use data-classifications."
-        )
+        (mapclassify,) = register_modules("mapclassify")
 
         s = SimpleNamespace(
             **{
                 i: self._get_mcl_subclass(getattr(mapclassify, i))
                 for i in mapclassify.CLASSIFIERS
             }
         )
 
         s.__doc__ = Maps.set_classify.__doc__
 
         return s
 
     def set_classify_specs(self, scheme=None, **kwargs):
         """
-        Optional way to set classification specifications for the data.
+        Set classification specifications for the data.
 
         The classification is ultimately performed by the `mapclassify` module!
 
         Note
         ----
         The following calls have the same effect:
 
@@ -1256,21 +1440,17 @@
                 - Percentiles (pct)
                 - StdMean (multiples)
                 - UserDefined (bins)
 
         kwargs :
             kwargs passed to the call to the respective mapclassify classifier
             (dependent on the selected scheme... see above)
-        """
-
-        assert _register_mapclassify(), (
-            "EOmaps: Missing dependency: 'mapclassify' \n ... please install"
-            + " (conda install -c conda-forge mapclassify) to use data-classifications."
-        )
 
+        """
+        register_modules("mapclassify")
         self.classify_specs._set_scheme_and_args(scheme, **kwargs)
 
     def set_extent_to_location(self, location, annotate=False, user_agent=None):
         """
         Set the map-extent based on a given location query.
 
         The bounding-box is hereby resolved via the OpenStreetMap Nominatim service.
@@ -1328,16 +1508,105 @@
             else:
                 text = fill(r["display_name"], 20)
 
             self.add_annotation(
                 xy=(r["lon"], r["lat"]), xy_crs=4326, text=text, fontsize=8
             )
         else:
-            print("Centering Map to:\n    ", r["display_name"])
+            _log.info(f"Centering Map to:\n    {r['display_name']}")
+
+    @staticmethod
+    def _set_clipboard_kwargs(**kwargs):
+        # use Maps to make sure InsetMaps do the same thing!
+        Maps._clipboard_kwargs = kwargs
+
+    @staticmethod
+    def set_clipboard_kwargs(**kwargs):
+        """
+        Set GLOBAL savefig parameters for all Maps objects on export to the clipboard.
+
+        - press "control + c" to export the figure to the clipboard
+
+        All arguments are passed to :meth:`Maps.savefig`
 
+        Useful options are
+
+        - dpi : the dots-per-inch of the figure
+        - refetch_wms: re-fetch webmaps with respect to the export-`dpi`
+        - bbox_inches: use "tight" to export figure with a tight boundary
+        - pad_inches: the size of the boundary if `bbox_inches="tight"`
+        - transparent: if `True`, export with a transparent background
+        - facecolor: the background color
+
+
+        Parameters
+        ----------
+        kwargs :
+            Keyword-arguments passed to :meth:`Maps.savefig`.
+
+        Note
+        ----
+        This function sets the clipboard kwargs for all Maps-objects!
+
+        Exporting to the clipboard only works if `PyQt5` is used as matplotlib backend!
+        (the default if `PyQt` is installed)
+
+        See Also
+        --------
+        Maps.savefig : Save the figure as jpeg, png, etc.
+
+        """
+        # use Maps to make sure InsetMaps do the same thing!
+        Maps._set_clipboard_kwargs(**kwargs)
+        # trigger companion-widget setter for all open figures that contain maps
+        for i in plt.get_fignums():
+            try:
+                m = getattr(plt.figure(i), "_EOmaps_parent", None)
+                if m is not None:
+                    if m._companion_widget is not None:
+                        m._emit_signal("clipboardKwargsChanged")
+            except Exception:
+                _log.exception("UPS")
+
+    def add_title(self, title, x=0.5, y=1.01, **kwargs):
+        """
+        Convenience function to add a title to the map.
+
+        (The title will be visible at the assigned layer.)
+
+        Parameters
+        ----------
+        title : str
+            The title.
+        x, y : float, optional
+            The position of the text in axis-coordinates (0-1).
+            The default is 0.5, 1.01.
+        kwargs :
+            Additional kwargs are passed to `m.text()`
+            The defaults are:
+
+            - `"fontsize": "large"`
+            - `horizontalalignment="center"`
+            - `verticalalignment="bottom"`
+
+        See Also
+        --------
+
+        :py:meth:`Maps.text` : General function to add text to the figure.
+
+        """
+        kwargs.setdefault("fontsize", "large")
+        kwargs.setdefault("horizontalalignment", "center")
+        kwargs.setdefault("verticalalignment", "bottom")
+
+        self.text(
+            0.5, 1.01, title, transform=self.ax.transAxes, layer=self.layer, **kwargs
+        )
+
+    @lru_cache()
     def get_crs(self, crs="plot"):
         """
         Get the pyproj CRS instance of a given crs specification.
 
         Parameters
         ----------
         crs : "in", "out" or a crs definition
@@ -1355,20 +1624,15 @@
         # check for strings first to avoid expensive equality checking for CRS objects!
         if isinstance(crs, str):
             if crs == "in":
                 crs = self.data_specs.crs
             elif crs == "out" or crs == "plot":
                 crs = self.crs_plot
 
-        h = hash(crs)
-        if h in self._crs_cache:
-            crs = self._crs_cache[h]
-        else:
-            crs = CRS.from_user_input(crs)
-            self._crs_cache[h] = crs
+        crs = CRS.from_user_input(crs)
         return crs
 
     @wraps(LayoutEditor.get_layout)
     def get_layout(self, *args, **kwargs):
         """Get the current layout."""
         return self.parent._layout_editor.get_layout(*args, **kwargs)
 
@@ -1395,14 +1659,18 @@
 
             NOTE: The file will be overwritten if it already exists!!
             The default is None.
 
         """
         self.parent._layout_editor._make_draggable(filepath=filepath)
 
+    @wraps(AnnotationEditor.__call__)
+    def edit_annotations(self, b=True, **kwargs):
+        self._edit_annotations(b, **kwargs)
+
     @property
     @wraps(NaturalEarth_features)
     def add_feature(self):
         """Add features from NaturalEarth."""
         # lazily initialize NaturalEarth features
         if not hasattr(self, "_add_feature"):
             self._add_feature = NaturalEarth_features(self)
@@ -1427,15 +1695,15 @@
         pick_method="contains",
         val_key=None,
         layer=None,
         temporary_picker=None,
         clip=False,
         reproject="gpd",
         verbose=False,
-        only_valid=True,
+        only_valid=False,
         set_extent=True,
         **kwargs,
     ):
         """
         Plot a `geopandas.GeoDataFrame` on the map.
 
         Parameters
@@ -1562,19 +1830,15 @@
 
         Returns
         -------
         new_artists : matplotlib.Artist
             The matplotlib-artists added to the plot
 
         """
-        assert _register_geopandas(), (
-            "EOmaps: Missing dependency `geopandas`!\n"
-            + "please install '(conda install -c conda-forge geopandas)'"
-            + "to use `m.add_gdf()`."
-        )
+        (gpd,) = register_modules("geopandas")
 
         if isinstance(gdf, (str, Path)):
             gdf = gpd.read_file(gdf)
 
         if val_key is None:
             val_key = kwargs.get("column", None)
 
@@ -1583,15 +1847,15 @@
 
         try:
             # explode the GeoDataFrame to avoid picking multi-part geometries
             gdf = gdf.explode(index_parts=False)
         except Exception:
             # geopandas sometimes has problems exploding geometries...
             # if it does not work, just continue with the Multi-geometries!
-            print("EOmaps: Exploding geometries did not work!")
+            _log.error("EOmaps: Exploding geometries did not work!")
             pass
 
         if clip:
             gdf = self._clip_gdf(gdf, clip)
         if reproject == "gpd":
             gdf = gdf.to_crs(self.crs_plot)
         elif reproject == "cartopy":
@@ -1635,40 +1899,52 @@
         # plot gdf and identify newly added collections
         # (geopandas always uses collections)
         colls = [id(i) for i in self.ax.collections]
         artists, prefixes = [], []
 
         # drop all invalid geometries
         if only_valid:
-            gdf = gdf[gdf.is_valid]
+            valid = gdf.is_valid
+            n_invald = np.count_nonzero(~valid)
+            gdf = gdf[valid]
+            if len(gdf) == 0:
+                _log.error("EOmaps: GeoDataFrame contains only invalid geometries!")
+                return
+            elif n_invald > 0:
+                _log.warning(
+                    "EOmaps: {n_invald} invalid GeoDataFrame geometries are ignored!"
+                )
 
         with self._disable_autoscale(set_extent):
             for geomtype, geoms in gdf.groupby(gdf.geom_type):
                 gdf.plot(ax=self.ax, aspect=self.ax.get_aspect(), **kwargs)
                 artists = [i for i in self.ax.collections if id(i) not in colls]
                 for i in artists:
                     prefixes.append(
                         f"_{i.__class__.__name__.replace('Collection', '')}"
                     )
 
         if picker_name is not None:
             if isinstance(pick_method, str):
-                picker_cls = _gpd_picker(
+                picker_cls = GeoDataFramePicker(
                     gdf=gdf, pick_method=pick_method, val_key=val_key
                 )
                 picker = picker_cls.get_picker()
             elif callable(pick_method):
                 picker = pick_method
                 picker_cls = None
             else:
-                print("EOmaps: I don't know what to do with the provided pick_method")
+                _log.error(
+                    "EOmaps: The provided pick_method is invalid."
+                    "Please provide either a string or a function."
+                )
                 return
 
             if len(artists) > 1:
-                warnings.warn(
+                _log.warning(
                     "EOmaps: Multiple geometry types encountered in `m.add_gdf`. "
                     + "The pick containers are re-named to"
                     + f"{[picker_name + prefix for prefix in prefixes]}"
                 )
             else:
                 prefixes = [""]
 
@@ -1688,14 +1964,15 @@
                 for art, prefix in zip(artists, prefixes):
                     self.cb.pick.add_temporary_artist(art)
             else:
                 for art, prefix in zip(artists, prefixes):
                     self.cb.pick[temporary_picker].add_temporary_artist(art)
         else:
             for art, prefix in zip(artists, prefixes):
+                art.set_label(f"EOmaps GeoDataframe ({prefix.lstrip('_')}, {len(gdf)})")
                 self.BM.add_bg_artist(art, layer)
         return artists
 
     def add_marker(
         self,
         ID=None,
         xy=None,
@@ -1713,15 +1990,15 @@
 
         Parameters
         ----------
         ID : any
             The index-value of the pixel in m.data.
         xy : tuple
             A tuple of the position of the pixel provided in "xy_crs".
-            If None, xy must be provided in the coordinate-system of the plot!
+            If "xy_crs" is None, xy must be provided in the plot-crs!
             The default is None
         xy_crs : any
             the identifier of the coordinate-system for the xy-coordinates
         radius : float or "pixel", optional
             - If float: The radius of the marker.
             - If "pixel": It will represent the dimensions of the selected pixel.
               (check the `buffer` kwarg!)
@@ -1754,15 +2031,15 @@
             kwargs passed to the matplotlib patch.
             (e.g. `zorder`, `facecolor`, `edgecolor`, `linewidth`, `alpha` etc.)
 
         Examples
         --------
             >>> m.add_marker(ID=1, buffer=5)
             >>> m.add_marker(ID=1, radius=2, radius_crs=4326, shape="rectangles")
-            >>> m.add_marker(xy=(45, 35), xy_crs=4326, radius=20000, shape="geod_circles")
+            >>> m.add_marker(xy=(4, 3), xy_crs=4326, radius=20000, shape="geod_circles")
         """
         if ID is not None:
             assert xy is None, "You can only provide 'ID' or 'pos' not both!"
         else:
             if isinstance(radius, str) and radius != "pixel":
                 raise TypeError(f"I don't know what to do with radius='{radius}'")
 
@@ -1797,19 +2074,15 @@
             buffer=buffer,
             n=n,
             layer=layer,
             permanent=None,
             **kwargs,
         )
 
-        if permanent is True:
-            self.BM.add_bg_artist(marker, layer=layer)
-        else:
-            self.BM.add_artist(marker, layer=layer)
-
+        if permanent is False:
             self.BM.update()
 
         return marker
 
     def add_annotation(
         self,
         ID=None,
@@ -1885,68 +2158,94 @@
         >>>                  bbox=dict(boxstyle='circle,pad=0.5',
         >>>                            fc='yellow',
         >>>                            alpha=0.3
         >>>                            )
         >>>                  )
 
         """
+        inp_ID = ID
+
+        if xy is None and ID is None:
+            x = self.ax.bbox.x0 + self.ax.bbox.width / 2
+            y = self.ax.bbox.y0 + self.ax.bbox.height / 2
+            xy = self.ax.transData.inverted().transform((x, y))
+
         if ID is not None:
             assert xy is None, "You can only provide 'ID' or 'pos' not both!"
             # avoid using np.isin directly since it needs a lot of ram
             # for very large datasets!
             mask, ind = self._find_ID(ID)
 
             xy = (
                 self._data_manager.xorig.ravel()[mask],
                 self._data_manager.yorig.ravel()[mask],
             )
             val = self._data_manager.z_data.ravel()[mask]
             ID = np.atleast_1d(ID)
             xy_crs = self.data_specs.crs
+
+            is_ID_annotation = False
         else:
             val = repeat(None)
             ind = repeat(None)
             ID = repeat(None)
 
+            is_ID_annotation = True
+
         assert (
             xy is not None
         ), "EOmaps: you must provide either ID or xy to position the annotation!"
 
         xy = (np.atleast_1d(xy[0]), np.atleast_1d(xy[1]))
 
         if xy_crs is not None:
             # get coordinate transformation
             transformer = self._get_transformer(
                 CRS.from_user_input(xy_crs),
                 self.crs_plot,
             )
             # transform coordinates
             xy = transformer.transform(*xy)
+        else:
+            transformer = None
 
         kwargs.setdefault("permanent", None)
 
         if isinstance(text, str) or callable(text):
-            text = repeat(text)
+            usetext = repeat(text)
         else:
             try:
-                iter(text)
+                usetext = iter(text)
             except TypeError:
-                text = repeat(text)
+                usetext = repeat(text)
 
-        for x, y, texti, vali, indi, IDi in zip(xy[0], xy[1], text, val, ind, ID):
-
-            # add marker
-            self.cb.click._cb.annotate(
+        for x, y, texti, vali, indi, IDi in zip(xy[0], xy[1], usetext, val, ind, ID):
+            ann = self.cb.click._cb.annotate(
                 ID=IDi,
                 pos=(x, y),
                 val=vali,
                 ind=indi,
                 text=texti,
                 **kwargs,
             )
+
+            if kwargs.get("permanent", False) is not False:
+                self._edit_annotations._add(
+                    a=ann,
+                    kwargs={
+                        "ID": inp_ID,
+                        "xy": (x, y),
+                        "xy_crs": xy_crs,
+                        "text": text,
+                        **kwargs,
+                    },
+                    transf=transformer,
+                    drag_coords=is_ID_annotation,
+                )
+
         self.BM.update(clear=False)
 
     @wraps(Compass.__call__)
     def add_compass(self, *args, **kwargs):
         """Add a compass (or north-arrow) to the map."""
         c = Compass(weakref.proxy(self))
         c(*args, **kwargs)
@@ -1989,18 +2288,18 @@
         )
 
         # add the scalebar to the map at the desired position
         s._add_scalebar(pos=pos, azim=rotation, pickable=pickable)
 
         return s
 
-    if wms_container is not None:
+    if WebMapContainer is not None:
 
         @property
-        @wraps(wms_container)
+        @wraps(WebMapContainer)
         def add_wms(self):
             """Accessor to attach WebMap services to the map."""
             return self._wms_container
 
     def add_line(
         self,
         xy,
@@ -2099,15 +2398,15 @@
         if layer is None:
             layer = self.layer
 
         # intermediate and total distances
         out_d_int, out_d_tot = [], []
 
         if len(xy) <= 1:
-            print("you must provide at least 2 points")
+            _log.error("you must provide at least 2 points")
 
         if n is not None:
             assert del_s is None, "EOmaps: Provide either `del_s` or `n`, not both!"
             del_s = 0  # pyproj's geod uses 0 as identifier!
 
             if not isinstance(n, int):
                 assert len(n) == len(xy) - 1, (
@@ -2157,17 +2456,23 @@
                 n = repeat(n)
 
             if del_s is None or isinstance(del_s, (int, float, np.number)):
                 del_s = repeat(del_s)
 
             xs, ys = [], []
             for (x0, x1), (y0, y1), ni, di in zip(pairwise(x), pairwise(y), n, del_s):
-
                 npts, d_int, d_tot, lon, lat, _ = geod.inv_intermediate(
-                    x0, y0, x1, y1, del_s=di, npts=ni, initial_idx=0, terminus_idx=0
+                    lon1=x0,
+                    lat1=y0,
+                    lon2=x1,
+                    lat2=y1,
+                    del_s=di,
+                    npts=ni,
+                    initial_idx=0,
+                    terminus_idx=0,
                 )
 
                 out_d_int.append(d_int)
                 out_d_tot.append(d_tot)
 
                 lon, lat = lon.tolist(), lat.tolist()
                 xi, yi = self._transf_lonlat_to_plot.transform(lon, lat)
@@ -2184,15 +2489,14 @@
             x, y = zip(*xy)
             if isinstance(n, int):
                 # use same number of points for all segments
                 xs = np.linspace(x[:-1], x[1:], n).T.ravel()
                 ys = np.linspace(y[:-1], y[1:], n).T.ravel()
             else:
                 # use different number of points for individual segments
-                from itertools import chain
 
                 xs = list(
                     chain(
                         *(np.linspace(a, b, ni) for (a, b), ni in zip(pairwise(x), n))
                     )
                 )
                 ys = list(
@@ -2203,14 +2507,15 @@
 
             x, y = t_xy_plot.transform(xs, ys)
 
             (art,) = self.ax.plot(x, y, **kwargs)
         else:
             raise TypeError(f"EOmaps: '{connect}' is not a valid connection-method!")
 
+        art.set_label(f"Line ({connect})")
         self.BM.add_bg_artist(art, layer)
 
         if mark_points:
             zorder = kwargs.get("zorder", 10)
 
             if isinstance(mark_points, dict):
                 # only use zorder of the line if no explicit zorder is provided
@@ -2219,14 +2524,15 @@
                 art2 = self.ax.scatter(xplot, yplot, **mark_points)
 
             elif isinstance(mark_points, str):
                 # use matplotlib's single-string style identifiers,
                 # (e.g. "r.", "go", "C0x" etc.)
                 (art2,) = self.ax.plot(xplot, yplot, mark_points, zorder=zorder, lw=0)
 
+            art2.set_label(f"Line Marker ({connect})")
             self.BM.add_bg_artist(art2, layer)
 
         return out_d_int, out_d_tot
 
     def add_logo(
         self,
         filepath=None,
@@ -2373,21 +2679,39 @@
             crs = Maps.CRS.PlateCarree()
 
         self.ax.set_extent(extents, crs=crs)
         self._set_extent_on_plot = False
 
     @wraps(GeoAxes.get_extent)
     def get_extent(self, crs=None):
-        """Get the extent of the map."""
-        # just a wrapper to avoid using m.ax.get_extent()
+        """
+        Get the extent (x0, x1, y0, y1) of the map in the given coordinate system.
+
+        Parameters
+        ----------
+        crs : a crs identifier, optional
+            The coordinate-system in which the extent is evaluated.
+
+            - if None, the extent is provided in epsg=4326 (e.g. lon/lat projection)
+
+            The default is None.
+
+        Returns
+        -------
+        extent : The extent in the given crs (x0, x1, y0, y1).
+
+        """
+        # fast track if plot-crs is requested
+        if crs == self.crs_plot:
+            return (*self.ax.get_xlim(), *self.ax.get_ylim())
 
         if crs is not None:
             crs = self._get_cartopy_crs(crs)
         else:
-            crs = Maps.CRS.PlateCarree()
+            crs = self._get_cartopy_crs(4326)
 
         return self.ax.get_extent(crs=crs)
 
     def _calc_vmin_vmax(self, vmin=None, vmax=None):
         if self._data_manager.z_data is None:
             return vmin, vmax
 
@@ -2434,18 +2758,23 @@
         if self._inherit_classification is not None:
             if not (vmin is None and vmax is None):
                 raise TypeError(
                     "EOmaps: 'vmin' and 'vmax' cannot be set explicitly "
                     "if the classification is inherited!"
                 )
 
-            if self._vmin is None:
-                print("EOmaps: Warning, inherited value for 'vmin' is None!")
-            if self._vmax is None:
-                print("EOmaps: Warning, inherited value for 'vmax' is None!")
+            # in case data is NOT inherited, warn if vmin/vmax is None
+            # (different limits might cause a different appearance of the data!)
+            if self.data_specs._m == self:
+                if self._vmin is None:
+                    _log.warning("EOmaps: Inherited value for 'vmin' is None!")
+                if self._vmax is None:
+                    _log.warning(
+                        "EOmaps: Inherited inherited value for 'vmax' is None!"
+                    )
 
             self._vmin = self._inherit_classification._vmin
             self._vmax = self._inherit_classification._vmax
             return
 
         if not self.shape.name.startswith("shade_"):
             # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
@@ -2458,15 +2787,15 @@
                 self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
             else:
                 # set vmin/vmax for aggregations that do NOT represent data values
                 # allow vmin/vmax = None (e.g. autoscaling)
                 if "count" in aggname:
                     # if the reduction represents a count, don't count empty pixels
                     if vmin and vmin <= 0:
-                        print(
+                        _log.warning(
                             "EOmaps: setting vmin=1 to avoid counting empty pixels..."
                         )
                         self._vmin = 1
 
                     if vmax and vmax > 0:
                         self._vmax = vmax
 
@@ -2485,18 +2814,17 @@
         - To set the data, see `m.set_data()`
         - To change the "shape" that is used to represent the datapoints, see
           `m.set_shape`.
         - To classify the data, see `m.set_classify` or `m.set_classify_specs()`
 
         NOTE
         ----
-        Each call to plot_map will replace the collection used for picking!
-        (only the last collection remains interactive on multiple calls to `m.plot_map()`)
+        Each call to `plot_map(...)` will override the previously plotted dataset!
 
-        If you need multiple responsive datasets, use a new layer for each dataset!
+        If you want to plot multiple datasets, use a new layer for each dataset!
         (e.g. via `m2 = m.new_layer()`)
 
         Parameters
         ----------
         layer : str or None
             The layer at which the dataset will be plotted.
             ONLY relevant if `dynamic = False`!
@@ -2538,52 +2866,42 @@
         Other Parameters
         ----------------
         vmin, vmax : float, optional
             Min- and max. values assigned to the colorbar. The default is None.
         zorder : float
             The zorder of the artist (e.g. the stacking level of overlapping artists)
             The default is 1
-        verbose : int
-            The print-message level.
-
-            - 0: don't print warning and info messages to the console
-            - >= 1: print warnings
-            - >= 10: print warnings and info messages
-
-            The default is 1
         kwargs
             kwargs passed to the initialization of the matpltolib collection
             (dependent on the plot-shape) [linewidth, edgecolor, facecolor, ...]
 
             For "shade_points" or "shade_raster" shapes, kwargs are passed to
             `datashader.mpl_ext.dsshow`
 
         """
-        verbose = kwargs.pop("verbose", 1)
+        verbose = kwargs.pop("verbose", None)
+        if verbose is not None:
+            _log.error("EOmaps: The parameter verbose is ignored.")
 
         # make sure zorder is set to 1 by default
         # (by default shading would use 0 while ordinary collections use 1)
         kwargs.setdefault("zorder", 1)
 
-        if verbose >= 1:
-            if (
-                getattr(self, "coll", None) is not None
-                and len(self.cb.pick.get.cbs) > 0
-            ):
-                print(
-                    "EOmaps-warning: Calling `m.plot_map()` or "
-                    "`m.make_dataset_pickable()` more than once on the "
-                    "same Maps-object overrides the assigned PICK-dataset!"
-                )
+        if getattr(self, "coll", None) is not None and len(self.cb.pick.get.cbs) > 0:
+            _log.info(
+                "EOmaps: Calling `m.plot_map()` or "
+                "`m.make_dataset_pickable()` more than once on the "
+                "same Maps-object overrides the assigned PICK-dataset!"
+            )
 
         if layer is None:
             layer = self.layer
         else:
-            if (verbose > 0) and not isinstance(layer, str):
-                print("EOmaps: The layer-name has been converted to a string!")
+            if not isinstance(layer, str):
+                _log.info("EOmaps: The layer-name has been converted to a string!")
                 layer = str(layer)
 
         useshape = self.shape  # invoke the setter to set the default shape
         shade_q = useshape.name.startswith("shade_")  # indicator if shading is used
 
         # make sure the colormap is properly set and transparencies are assigned
         cmap = kwargs.pop("cmap", "viridis")
@@ -2595,22 +2913,21 @@
             cmap = cmap_alpha(
                 cmap=cmap,
                 alpha=kwargs["alpha"],
                 name=cmapname,
             )
 
             plt.colormaps.register(name=cmapname, cmap=cmap)
-            if self._companion_widget is not None:
-                self._companion_widget.cmapsChanged.emit()
+            self._emit_signal("cmapsChanged")
             # remember registered colormaps (to de-register on close)
             self._registered_cmaps.append(cmapname)
 
         # ---------------------- prepare the data
-        if verbose >= 10:
-            print("EOmaps: Preparing the data")
+
+        _log.debug("EOmaps: Preparing dataset")
 
         # ---------------------- assign the data to the data_manager
 
         # shade shapes use datashader to update the data of the collections!
         update_coll_on_fetch = False if shade_q else True
 
         self._data_manager.set_props(
@@ -2618,17 +2935,17 @@
             assume_sorted=assume_sorted,
             update_coll_on_fetch=update_coll_on_fetch,
             indicate_masked_points=indicate_masked_points,
             dynamic=dynamic,
         )
 
         # ---------------------- classify the data
-        if verbose > 0 and not self._inherit_classification:
+        if not self._inherit_classification:
             if self.classify_specs.scheme is not None:
-                print("EOmaps: Classifying...")
+                _log.debug("EOmaps: Classifying...")
 
         self._set_vmin_vmax(
             vmin=kwargs.pop("vmin", None), vmax=kwargs.pop("vmax", None)
         )
         cbcmap, norm, bins, classified = self._classify_data(
             vmin=self._vmin,
             vmax=self._vmax,
@@ -2653,14 +2970,15 @@
             self._shade_map(
                 layer=layer,
                 dynamic=dynamic,
                 set_extent=set_extent,
                 assume_sorted=assume_sorted,
                 **kwargs,
             )
+            self.f.canvas.draw_idle()
         else:
             # dont set extent if "m.set_extent" was called explicitly
             if set_extent and self._set_extent_on_plot:
                 # note bg-layers are automatically triggered for re-draw
                 # if the extent changes!
                 self._data_manager._set_lims()
 
@@ -2668,24 +2986,27 @@
                 layer=layer,
                 dynamic=dynamic,
                 set_extent=set_extent,
                 assume_sorted=assume_sorted,
                 **kwargs,
             )
 
-        self.BM._refetch_layer(layer)
+            self.BM._refetch_layer(layer)
 
-        if verbose >= 1:
-            if getattr(self, "_data_mask", None) is not None and not np.all(
-                self._data_mask
-            ):
-                print("EOmaps: Warning: some datapoints could not be drawn!")
+        if getattr(self, "_data_mask", None) is not None and not np.all(
+            self._data_mask
+        ):
+            _log.info("EOmaps: Some datapoints could not be drawn!")
 
         self._data_plotted = True
 
+        self._emit_signal("dataPlotted")
+
+        self.BM.update()
+
     def make_dataset_pickable(
         self,
     ):
         """
         Make the associated dataset pickable **without plotting** it first.
 
         After executing this function, `m.cb.pick` callbacks can be attached to the
@@ -2711,15 +3032,15 @@
         >>> m2 = m.new_layer()
             >>> m2.set_data(*np.linspace([0, -180,-90,], [100, 180, 90], 100).T)
         >>> m2.make_dataset_pickable()
         >>> m2.cb.pick.attach.annotate()  # get an annotation for the invisible dataset
         >>> # ...call m2.plot_map() to make the dataset visible...
         """
         if self.coll is not None:
-            print(
+            _log.error(
                 "EOmaps: There is already a dataset plotted on this Maps-object. "
                 "You MUST use a new layer (`m2 = m.new_layer()`) to use "
                 "`m2.make_dataset_pickable()`!"
             )
             return
 
         # ---------------------- prepare the data
@@ -2730,47 +3051,49 @@
         y0, y1 = self._data_manager.y0.min(), self._data_manager.y0.max()
 
         # use a transparent rectangle of the data-extent as artist for picking
         (art,) = self.ax.fill([x0, x1, x1, x0], [y0, y0, y1, y1], fc="none", ec="none")
 
         self._coll = art
 
-        self.tree = searchtree(m=self._proxy(self))
+        self.tree = SearchTree(m=self._proxy(self))
         self.cb.pick._set_artist(art)
         self.cb.pick._init_cbs()
         self.cb._methods.add("pick")
 
         self._coll_kwargs = dict()
         self._coll_dynamic = True
 
         # set _data_plotted to True to trigger updates in the data-manager
         self._data_plotted = True
 
+    @lru_cache()
     def _get_combined_layer_name(self, *args):
-        if len(args) == 1:
-            assert isinstance(
-                args[0], str
-            ), "EOmaps: Single arguments passed to 'show_layer()', must be strings!"
-            return args[0]
-
         try:
             combnames = []
             for i in args:
                 if isinstance(i, str):
                     combnames.append(i)
                 elif isinstance(i, (list, tuple)):
                     assert (
-                        len(i) == 2 and isinstance(i[0], str) and i[1] > 0 and i[1] < 1
+                        len(i) == 2
+                        and isinstance(i[0], str)
+                        and i[1] >= 0
+                        and i[1] <= 1
                     ), (
                         f"EOmaps: unable to identify the layer-assignment: {i} .\n"
                         "You can provide either a single layer-name as string, a list "
                         "of layer-names or a list of tuples of the form: "
                         "(< layer-name (str) >, < layer-transparency [0-1] > )"
                     )
-                    combnames.append(i[0] + "{" + str(i[1]) + "}")
+
+                    if i[1] < 1:
+                        combnames.append(i[0] + "{" + str(i[1]) + "}")
+                    else:
+                        combnames.append(i[0])
                 else:
                     raise TypeError(
                         f"EOmaps: unable to identify the layer-assignment: {i} .\n"
                         "You can provide either a single layer-name as string, a list "
                         "of layer-names or a list of tuples of the form: "
                         "(< layer-name (str) >, < layer-transparency [0-1] > )"
                     )
@@ -2814,24 +3137,24 @@
 
         Provide the combined layer-name, e.g.:
 
         >>> m.show_layer("A|B{0.5}|C{0.25}")
 
         See Also
         --------
-        - Maps.util.layer_selector
-        - Maps.util.layer_slider
+        Maps.util.layer_selector : Add a button-widget to switch layers to the map.
+        Maps.util.layer_slider : Add a slider to switch layers to the map.
 
         """
         name = self._get_combined_layer_name(*args)
 
         layers = self._get_layers()
 
         if not isinstance(name, str):
-            print("EOmaps: All layer-names are converted to strings!")
+            _log.info("EOmaps: All layer-names are converted to strings!")
             name = str(name)
 
         if "|" in name:
             # take special care of "_" to allow 'private' (e.g. hidden) multi-layers
             names = [i.strip() for i in name.split("|") if i != "_"]
         else:
             names = [name]
@@ -2843,37 +3166,58 @@
 
             if "{" in i and i.endswith("}"):
                 i = i.split("{")[0]  # strip off transparency assignments
 
             if i not in layers:
                 lstr = " - " + "\n - ".join(map(str, layers))
 
-                print(
+                _log.error(
                     f"EOmaps: The layer '{i}' does not exist...\n"
                     + f"Use one of: \n{lstr}"
                 )
                 return
 
         # invoke the bg_layer setter of the blit-manager
         self.BM.bg_layer = name
         self.BM.update()
 
-    def show(self):
+    def show(self, clear=True):
         """
         Make the layer of this `Maps`-object visible.
 
         This is just a shortcut for `m.show_layer(m.layer)`
 
         If matploltib is used in non-interactive mode, (e.g. `plt.ioff()`)
         `plt.show()` is called as well!
+
+        Parameters
+        ----------
+        clear : bool, optional
+            Only relevant if the `inline` backend is used in a jupyter-notebook
+            or an Ipython console.
+
+            If True, clear the active cell before plotting a snapshot of the figure.
+            The default is True.
         """
+
         self.show_layer(self.layer)
 
         if not plt.isinteractive():
-            plt.show()
+            try:
+                __IPYTHON__
+            except NameError:
+                plt.show()
+            else:
+                active_backend = plt.get_backend()
+                # print a snapshot to the active ipython cell in case the
+                # inline-backend is used
+                if active_backend in ["module://matplotlib_inline.backend_inline"]:
+                    self.BM.update(clear=clear)
+                else:
+                    plt.show()
 
     def snapshot(self, *layer, transparent=False, clear=False):
         """
         Print a static image of the figure to the active IPython display.
 
         This is useful if you want to print a snapshot of the current state of the map
         to the active Jupyter Notebook cell or the currently active IPython console
@@ -2902,50 +3246,55 @@
         >>> m = Maps(layer="base")
         >>> m.add_feature.preset.coastline()
         >>> m2 = m.new_layer("ocean")
         >>> m.add_feature.preset.ocean()
         >>> m.snapshot("base", ("ocean", .5), transparent=True)
 
         """
-        from PIL import Image
-        from IPython.display import display
-
-        with ExitStack() as stack:
-            # don't clear on layer-changes
-            stack.enter_context(self.BM._cx_dont_clear_on_layer_change())
+        try:
+            self._snapshotting = True
 
-            if len(layer) == 0:
-                layer = None
+            from PIL import Image
+            from IPython.display import display
 
-            # hide companion-widget indicator
-            self._indicate_companion_map(False)
+            with ExitStack() as stack:
+                # don't clear on layer-changes
+                stack.enter_context(self.BM._cx_dont_clear_on_layer_change())
 
-            if layer is not None:
-                layer = self._get_combined_layer_name(*layer)
+                if len(layer) == 0:
+                    layer = None
 
-            # add the figure background patch as the bottom layer
-            initial_layer = self.BM.bg_layer
+                # hide companion-widget indicator
+                self._indicate_companion_map(False)
 
-            if transparent is False:
-                showlayer_name = self.BM._get_showlayer_name(layer=layer)
-                layer_with_bg = "|".join(["__BG__", showlayer_name])
-                self.show_layer(layer_with_bg)
-                sn = self._get_snapshot()
-                # restore the previous layer
-                self.BM._refetch_layer(layer_with_bg)
-                self.show_layer(initial_layer)
-            else:
                 if layer is not None:
-                    self.show_layer(layer)
+                    layer = self._get_combined_layer_name(*layer)
+
+                # add the figure background patch as the bottom layer
+                initial_layer = self.BM.bg_layer
+
+                if transparent is False:
+                    showlayer_name = self.BM._get_showlayer_name(layer=layer)
+                    layer_with_bg = "|".join(["__BG__", showlayer_name])
+                    self.show_layer(layer_with_bg)
                     sn = self._get_snapshot()
+                    # restore the previous layer
+                    self.BM._refetch_layer(layer_with_bg)
                     self.show_layer(initial_layer)
                 else:
-                    sn = self._get_snapshot()
+                    if layer is not None:
+                        self.show_layer(layer)
+                        sn = self._get_snapshot()
+                        self.show_layer(initial_layer)
+                    else:
+                        sn = self._get_snapshot()
 
-        display(Image.fromarray(sn, "RGBA"), display_id=True, clear=clear)
+            display(Image.fromarray(sn, "RGBA"), display_id=True, clear=clear)
+        finally:
+            self._snapshotting = False
 
     @wraps(plt.Figure.text)
     def text(self, *args, layer=None, **kwargs):
         """Add text to the map."""
         kwargs.setdefault("animated", True)
         kwargs.setdefault("horizontalalignment", "center")
         kwargs.setdefault("verticalalignment", "center")
@@ -2970,63 +3319,149 @@
                 "\n\n    See `m.refetch_wms_on_size_change()` for more details. "
                 "The default is False",
                 1,
             )
         }
     )
     @wraps(plt.savefig)
-    def savefig(self, *args, refetch_wms=False, **kwargs):
+    def savefig(self, *args, refetch_wms=False, rasterize_data=True, **kwargs):
         """Save the figure."""
         with ExitStack() as stack:
             if refetch_wms is False:
                 if _cx_refetch_wms_on_size_change is not None:
                     stack.enter_context(_cx_refetch_wms_on_size_change(refetch_wms))
 
                 # don't clear on layer-changes
                 stack.enter_context(self.BM._cx_dont_clear_on_layer_change())
 
             # hide companion-widget indicator
             self._indicate_companion_map(False)
 
-            dpi = kwargs.get("dpi", None)
-
             # add the figure background patch as the bottom layer
             transparent = kwargs.get("transparent", False)
             if transparent is False:
                 initial_layer = self.BM.bg_layer
                 showlayer_name = self.BM._get_showlayer_name(initial_layer)
                 layer_with_bg = "|".join(["__BG__", showlayer_name])
                 self.show_layer(layer_with_bg)
 
+            dpi = kwargs.get("dpi", None)
+
             redraw = False
             if dpi is not None and dpi != self.f.dpi or "bbox_inches" in kwargs:
                 redraw = True
 
                 # clear all cached background layers before saving to make sure they
                 # are re-drawn with the correct dpi-settings
                 self.BM._refetch_bg = True
 
                 # set the shading-axis-size to reflect the used dpi setting
                 self._update_shade_axis_size(dpi=dpi)
 
+            # get all layer names that should be drawn
+            savelayers, alphas = self.BM._get_layers_alphas(
+                self.BM._get_showlayer_name(
+                    self._get_combined_layer_name(self.BM.bg_layer)
+                )
+            )
+            # make sure inset-maps are drawn on top of normal maps
+            savelayers.sort(key=lambda x: x.startswith("__inset_"))
+
+            for m in (self.parent, *self.parent._children):
+                # re-enable normal axis draw cycle by making axes non-animated.
+                # This is needed for backward-compatibility, since saving a figure
+                # ignores the animated attribute for axis-children but not for the axis
+                # itself. See:
+                # https://github.com/matplotlib/matplotlib/issues/26007#issuecomment-1568812089
+                stack.enter_context(m.ax._cm_set(animated=False))
+
+                # handle colorbars
+                for cb in m._colorbars:
+                    for a in cb._axes:
+                        stack.enter_context(a._cm_set(animated=False))
+
+                # set if data should be rasterized on vektor export
+                if m.coll is not None:
+                    stack.enter_context(m.coll._cm_set(rasterized=rasterize_data))
+
+            # explicitly set axes to non-animated to re-enable draw cycle
+            for a in m.BM._managed_axes:
+                stack.enter_context(a._cm_set(animated=False))
+
+            zorder = 0
+            for layer, alpha in zip(savelayers, alphas):
+                # get all (sorted) artists of a layer
+                if layer.startswith("__inset"):
+                    artists = self.BM.get_bg_artists(["__inset_all", layer])
+                else:
+                    if layer.startswith("__"):
+                        artists = self.BM.get_bg_artists([layer])
+                    else:
+                        artists = self.BM.get_bg_artists(["all", layer])
+
+                for a in artists:
+                    if isinstance(a, plt.Axes):
+                        continue
+                    zorder += 1
+                    stack.enter_context(a._cm_set(zorder=zorder, animated=False))
+
+                    if alpha < 1:
+                        current_alpha = a.get_alpha()
+                        if current_alpha is None:
+                            current_alpha = alpha
+                        else:
+                            current_alpha = current_alpha * alpha
+
+                        stack.enter_context(a._cm_set(alpha=current_alpha))
+
+            for key, val in self.BM._bg_artists.items():
+                if key not in ["all", "__inset_all", *savelayers]:
+                    for a in val:
+                        stack.enter_context(a._cm_set(visible=False, animated=True))
+
+            if any(l.startswith("__inset") for l in savelayers):
+                if "__inset_all" not in savelayers:
+                    savelayers.append("__inset_all")
+                    alphas.append(1)
+            if "all" not in savelayers:
+                savelayers.append("all")
+                alphas.append(1)
+
+            # always draw dynamic artists on top of background artists
+            for layer, alpha in zip(savelayers, alphas):
+                # get all (sorted) artists of a layer
+                artists = self.BM.get_artists([layer])
+
+                for a in artists:
+                    zorder += 1
+                    stack.enter_context(a._cm_set(zorder=zorder, animated=False))
+
+            for key, val in self.BM._artists.items():
+                if key not in savelayers:
+                    for a in val:
+                        stack.enter_context(a._cm_set(visible=False, animated=True))
+
+            # trigger a redraw of all savelayers to make sure unmanaged artists
+            # and ordinary matplotlib axes are properly drawn
+            self.redraw(*savelayers)
             self.f.savefig(*args, **kwargs)
 
         if redraw is True:
             # reset the shading-axis-size to the used figure dpi
             self._update_shade_axis_size()
             # redraw after the save to ensure that backgrounds are correctly cached
             self.redraw()
 
         # restore the previous layer
         if transparent is False:
             self.BM._refetch_layer(layer_with_bg)
             self.show_layer(initial_layer)
             self.BM.on_draw(None)
 
-    def fetch_layers(self, layers=None, verbose=True):
+    def fetch_layers(self, layers=None):
         """
         Fetch (and cache) the layers of a map.
 
         This is particularly useful if you want to use sliders or buttons to quickly
         switch between the layers (e.g. once the backgrounds are cached, switching
         layers will be fast).
 
@@ -3035,21 +3470,18 @@
 
         Parameters
         ----------
         layers : list or None, optional
             A list of layer-names that should be fetched.
             If None, all layers (except the "all" layer) are fetched.
             The default is None.
-        verbose : bool
-            Indicator if status-messages should be printed or not.
-            The default is True.
 
         See Also
         --------
-        m.cb.keypress.attach.fetch_layers : use a keypress callback to fetch layers
+        Maps.cb.keypress.attach.fetch_layers : use a keypress callback to fetch layers
 
         """
         active_layer = self.BM._bg_layer
         all_layers = self._get_layers()
 
         if layers is None:
             layers = all_layers
@@ -3062,16 +3494,15 @@
                     + "\n - ".join(set(layers).difference(all_layers))
                 )
 
         nlayers = len(layers)
         assert nlayers > 0, "EOmaps: There are no layers to fetch."
 
         for i, l in enumerate(layers):
-            if verbose:
-                print("EOmaps: fetching layer", f"{i + 1}/{nlayers}:", l)
+            _log.info(f"EOmaps: fetching layer {i + 1}/{nlayers}: {l}")
             self.show_layer(l)
 
         self.show_layer(active_layer)
         self.BM.update()
 
     def join_limits(self, *args):
         """
@@ -3116,15 +3547,15 @@
         copy_cls : eomaps.Maps object
             a new Maps class.
         """
         copy_cls = Maps(**kwargs)
 
         if data_specs is True:
             data_specs = list(self.data_specs.keys())
-            copy_cls.set_data_specs(
+            copy_cls.set_data(
                 **{key: copy.deepcopy(val) for key, val in self.data_specs}
             )
 
         if shape is True:
             if self.shape is not None:
                 getattr(copy_cls.set_shape, self.shape.name)(**self.shape._initargs)
 
@@ -3151,19 +3582,15 @@
             The default is 100.
         crs : any, optional
             A coordinate-system identifier.
             The default is 4326 (e.g. lon/lat).
         kwargs :
             Additional keyword-arguments passed to `m.add_gdf()`.
         """
-        assert _register_geopandas(), (
-            "EOmaps: Missing dependency `geopandas`!\n"
-            + "please install '(conda install -c conda-forge geopandas)'"
-            + "to use `m.indicate_extent()`."
-        )
+        register_modules("geopandas")
 
         gdf = self._make_rect_poly(x0, y0, x1, y1, self.get_crs(crs), npts)
         self.add_gdf(gdf, **kwargs)
 
     def redraw(self, *args):
         """
         Force a re-draw of cached background layers.
@@ -3213,15 +3640,15 @@
         """Adjust the margins of subplots."""
         self.parent._gridspec.update(**kwargs)
         # after changing margins etc. a redraw is required
         # to fetch the updated background!
 
         self.redraw()
 
-    def on_layer_activation(self, func, persistent=False, **kwargs):
+    def on_layer_activation(self, func, layer=None, persistent=False, **kwargs):
         """
         Attach a callback that is executed if the associated layer is activated.
 
         Useful to "lazily" populate layers with features that are expensive to
         create (e.g. fetching data from files etc.).
 
         Parameters
@@ -3229,25 +3656,40 @@
         func : callable
             The callable to use.
             The call-signature is:
 
             >>> def func(m, **kwargs):
             >>>    # m... the Maps-object used for calling this function
 
+            NOTE: The Maps-object that is passed to the function is determined by
+            the 'layer' argument!
+        layer : str or None, optional
+            If provided, a NEW layer will be created and passed to the execution of the
+            function. Otherwise, the calling Maps-object is used.
+
+            To clarify: The following two code-snippets are equivalent:
+
+            >>> m = Maps()
+            >>> m2 = m.new_layer("my_layer")
+            >>> m2.on_layer_activation(func)
+
+            >>> m = Maps()
+            >>> m.on_layer_activation(func, layer="my_layer")
+
         persistent : bool, optional
             Indicator if the function should be called only once (False) or if it
             should be called each time the layer is activated (True).
             The default is False.
         kwargs :
             Additional keyword-arguments passed to the call of the function.
 
         See Also
         --------
-        m.layer : The layer-name associated with the Maps-object
-        m.fetch_layers() : Fetch and cache all layers of the map
+        Maps.layer : The layer-name associated with the Maps-object
+        Maps.fetch_layers : Fetch and cache all layers of the map
 
         Examples
         --------
         >>> m = Maps()
         >>> m.add_feature.preset.coastline()
         >>>
         >>> def f(m, ocean_color, coastline_color):
@@ -3258,19 +3700,25 @@
         >>> # create a new (initially empty) layer "ocean"
         >>> m2 = m.new_layer("ocean")
         >>> # add features to the layer only if it is activated
         >>> m2.on_layer_activation(f, ocean_color="b", coastline_color="r")
         >>> s = m.util.layer_selector()
 
         """
+        if layer is None:
+            layer = self.layer
+            m = self
+        else:
+            layer = str(layer)
+            m = self.new_layer(layer)
 
         def cb(m, layer):
             func(m=m, **kwargs)
 
-        self.BM.on_layer(func=cb, layer=self.layer, persistent=persistent, m=self)
+        self.BM.on_layer(func=cb, layer=layer, persistent=persistent, m=m)
 
     def cleanup(self):
         """
         Cleanup all references to the object so that it can be safely deleted.
 
         This function is primarily used internally to clear objects if the figure
         is closed.
@@ -3285,53 +3733,56 @@
         # disconnect callback on xlim-change (only relevant for parent)
         if not self._is_sublayer:
             try:
                 if hasattr(self, "_cid_xlim"):
                     self.ax.callbacks.disconnect(self._cid_xlim)
                     del self._cid_xlim
             except Exception:
-                print("EOmaps-cleanup: Problem while clearing xlim-cid")
+                _log.error("EOmaps-cleanup: Problem while clearing xlim-cid")
 
         # clear data-specs and all cached properties of the data
         try:
             self._coll = None
             self._data_manager.cleanup()
 
             if hasattr(self, "tree"):
                 del self.tree
             self.data_specs.delete()
         except Exception:
-            print("EOmaps-cleanup: Problem while clearing data specs")
+            _log.error("EOmaps-cleanup: Problem while clearing data specs")
 
         # disconnect all click, pick and keypress callbacks
         try:
             self.cb._reset_cids()
             # cleanup callback-containers
             self.cb._clear_callbacks()
         except Exception:
-            print("EOmaps-cleanup: Problem while clearing callbacks")
+            _log.error("EOmaps-cleanup: Problem while clearing callbacks")
 
         # cleanup all artists and cached background-layers from the blit-manager
         if not self._is_sublayer:
             self.BM.cleanup_layer(self.layer)
 
         # remove the child from the parent Maps object
         if self in self.parent._children:
             self.parent._children.remove(self)
 
         # activate the base-layer (and re-initialize widgets)
         try:
             if self.parent != self:
                 self.show_layer(self.parent.layer)
         except Exception:
-            print("EOmaps-cleanup: Problem while updating map to reflect changes")
+            _log.error(
+                "EOmaps-cleanup: Problem while updating map to reflect changes",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
 
     def _check_layer_name(self, layer):
         if not isinstance(layer, str):
-            print("EOmaps: All layer-names are converted to strings!")
+            _log.info("EOmaps: All layer-names are converted to strings!")
             layer = str(layer)
 
         if layer.startswith("__") and not layer.startswith("__inset_"):
             raise TypeError(
                 "EOmaps: Layer-names starting with '__' are reserved "
                 "for internal use and cannot be used as Maps-layer-names!"
             )
@@ -3356,49 +3807,95 @@
                 raise TypeError(
                     f"EOmaps: The symbol '{symb}' is not allowed in layer-names!\n"
                     + explanation
                 )
 
         return layer
 
-    def _init_figure(self, ax=None, plot_crs=None, **kwargs):
-        # do this on any new figure since "%matpltolib inline" tries to re-activate
-        # interactive mode all the time!
+    def _save_to_clipboard(self, **kwargs):
+        """
+        Export the figure to the clipboard.
+
+        Parameters
+        ----------
+        kwargs :
+            Keyword-arguments passed to :py:meth:`Maps.savefig`
+        """
+        import io
+        import mimetypes
+        from PyQt5.QtCore import QMimeData
+        from PyQt5.QtWidgets import QApplication
+        from PyQt5.QtGui import QImage
+
+        # guess the MIME type from the provided file-extension
+        fmt = kwargs.get("format", "png")
+        mimetype, _ = mimetypes.guess_type(f"dummy.{fmt}")
 
-        _handle_backends()
+        message = f"EOmaps: Exporting figure as '{fmt}' to clipboard..."
+        _log.info(message)
 
+        if self._companion_widget is not None:
+            self._companion_widget.window().statusBar().showMessage(message, 2000)
+
+        with io.BytesIO() as buffer:
+            self.savefig(buffer, **kwargs)
+            data = QMimeData()
+
+            cb = QApplication.clipboard()
+
+            # TODO check why files copied with setMimeData(...) cannot be pasted
+            # properly in other apps
+            if fmt in ["svg", "svgz", "pdf", "eps"]:
+                data.setData(mimetype, buffer.getvalue())
+                cb.clear(mode=cb.Clipboard)
+                cb.setMimeData(data, mode=cb.Clipboard)
+            else:
+                cb.setImage(QImage.fromData(buffer.getvalue()))
+
+    def _on_keypress(self, event):
+        # NOTE: callback is only attached to the parent Maps object!
+        if event.key == self._companion_widget_key:
+            self._open_companion_widget((event.x, event.y))
+        elif event.key == "ctrl+c":
+            self._save_to_clipboard(**Maps._clipboard_kwargs)
+
+    def _init_figure(self, ax=None, plot_crs=None, **kwargs):
         if self.parent.f is None:
+            # do this on any new figure since "%matpltolib inline" tries to re-activate
+            # interactive mode all the time!
+            _handle_backends()
+
             self._f = plt.figure(**kwargs)
+            _log.debug("EOmaps: New figure created")
 
             # make sure we keep a "real" reference otherwise overwriting the
             # variable of the parent Maps-object while keeping the figure open
             # causes all weakrefs to be garbage-collected!
             self.parent.f._EOmaps_parent = self.parent._real_self
 
-            if self.parent._cid_companion_key is None:
-                # attach a callback to show/hide the window with the "w" key
-
-                # NOTE the companion-widget is ONLY attahed to the parent map
-                # since it will identify the clicked map automatically! The
-                # widget will only be initialized on Maps-objects that create
-                # NEW axes. This is required to make sure that any additional
-                # Maps-object on the same axes will then always use the
-                # same widget. (otherwise each layer would get its own widget)
-
-                self.parent._cid_companion_key = self.f.canvas.mpl_connect(
-                    "key_press_event", self.parent._open_companion_widget_cb
-                )
-
             newfig = True
         else:
             newfig = False
             if not hasattr(self.parent.f, "_EOmaps_parent"):
                 self.parent.f._EOmaps_parent = self.parent._real_self
             self.parent._add_child(self)
 
+        # attach a callback to show/hide the companion-widget with the "w" key
+        if self.parent._cid_keypress is None:
+            # NOTE the companion-widget is ONLY attached to the parent map
+            # since it will identify the clicked map automatically! The
+            # widget will only be initialized on Maps-objects that create
+            # NEW axes. This is required to make sure that any additional
+            # Maps-object on the same axes will then always use the
+            # same widget. (otherwise each layer would get its own widget)
+
+            self.parent._cid_keypress = self.f.canvas.mpl_connect(
+                "key_press_event", self.parent._on_keypress
+            )
+
         if isinstance(ax, plt.Axes):
             # check if the axis is already used by another maps-object
             if ax not in (i.ax for i in (self.parent, *self.parent._children)):
                 newax = True
                 ax.set_animated(True)
                 # make sure axes are drawn once to properly set transforms etc.
                 # (otherwise pan/zoom, ax.contains_point etc. will not work)
@@ -3458,16 +3955,14 @@
         if newax:  # only if a new axis has been created
             self._new_axis_map = True
 
             # explicitly set initial limits to global to avoid issues if NE-features
             # are added (and clipped) before actual limits are set
             self.ax.set_global()
 
-            # do this only on xlims and NOT on ylims to avoid recursion
-            # (plot aspect ensures that y changes if x changes)
             self._cid_xlim = self.ax.callbacks.connect(
                 "xlim_changed", self._on_xlims_change
             )
             self._cid_xlim = self.ax.callbacks.connect(
                 "ylim_changed", self._on_ylims_change
             )
         else:
@@ -3486,16 +3981,17 @@
         # if we haven't attached an axpicker so far, do it!
         if self.parent._layout_editor is None:
             self.parent._layout_editor = LayoutEditor(self.parent, modifier="alt+l")
 
         if newfig:
             # we only need to call show if a new figure has been created!
             if (
-                plt.isinteractive()
-                or plt.get_backend() == "module://ipympl.backend_nbagg"
+                # plt.isinteractive() or
+                plt.get_backend()
+                == "module://ipympl.backend_nbagg"
             ):
                 # make sure to call show only if we use an interactive backend...
                 # or within the ipympl backend (otherwise it will block subsequent code!)
                 plt.show()
 
     def _get_ax_label(self):
         return "map"
@@ -3506,32 +4002,35 @@
     def _on_ylims_change(self, *args, **kwargs):
         self.BM._refetch_bg = True
 
     def _on_resize(self, event):
         # make sure the background is re-fetched if the canvas has been resized
         # (required for peeking layers after the canvas has been resized
         #  and for webagg and nbagg backends to correctly re-draw the layer)
+
         self.BM._refetch_bg = True
         self.BM._refetch_blank = True
 
         # update the figure dimensions in case shading is used
         self._update_shade_axis_size()
 
     def _update_shade_axis_size(self, dpi=None):
-
         # set the axis-size that is used to determine the number of pixels used
-        # when using "shade" shapes
+        # when using "shade" shapes for ALL maps objects of a figure
+        w, h = self.ax.bbox.width, self.ax.bbox.height
+        fig_dpi = self.f.dpi
 
-        if self.coll is not None and self.shape.name.startswith("shade_"):
-            if dpi is None:
-                self.coll.plot_width = int(self.ax.bbox.width)
-                self.coll.plot_height = int(self.ax.bbox.height)
-            else:
-                self.coll.plot_width = int(self.ax.bbox.width / self.f.dpi * dpi)
-                self.coll.plot_height = int(self.ax.bbox.height / self.f.dpi * dpi)
+        for m in (self.parent, *self.parent._children):
+            if m.coll is not None and m.shape.name.startswith("shade_"):
+                if dpi is None:
+                    m.coll.plot_width = int(w)
+                    m.coll.plot_height = int(h)
+                else:
+                    m.coll.plot_width = int(w / fig_dpi * dpi)
+                    m.coll.plot_height = int(h / fig_dpi * dpi)
 
     def _on_close(self, event):
         # reset attributes that might use up a lot of memory when the figure is closed
         for m in [self.parent, *self.parent._children]:
             if hasattr(m.f, "_EOmaps_parent"):
                 m.f._EOmaps_parent = None
 
@@ -3546,15 +4045,15 @@
             plt.colormaps.unregister(cmap)
 
         # run garbage-collection to immediately free memory
         gc.collect
 
     def _join_axis_limits(self, m):
         if self.ax.projection != m.ax.projection:
-            warnings.warn(
+            _log.warning(
                 "EOmaps: joining axis-limits is only possible for "
                 + "axes with the same projection!"
             )
             return
 
         self.ax._EOmaps_joined_action = False
         m.ax._EOmaps_joined_action = False
@@ -3594,16 +4093,16 @@
     def _add_child(self, m):
         self.parent._children.add(m)
 
         # execute hooks to notify the gui that a new child was added
         for action in self._after_add_child:
             try:
                 action()
-            except Exception as ex:
-                print("EOmaps: Problem executing 'on_add_child' action:", ex)
+            except Exception:
+                _log.exception("EOmaps: Problem executing 'on_add_child' action:")
 
     def _identify_data(self, data=None, x=None, y=None, parameter=None):
         # identify the way how the data has been provided and convert to the internal
         # structure
 
         if data is None:
             data = self.data_specs.data
@@ -3612,16 +4111,22 @@
         if y is None:
             y = self.data_specs.y
         if parameter is None:
             parameter = self.data_specs.parameter
 
         # check other types before pandas to avoid unnecessary import
         if data is not None and not isinstance(data, (list, tuple, np.ndarray)):
-            if _register_pandas() and isinstance(data, pd.DataFrame):
+            (pd,) = register_modules("pandas", raise_exception=False)
+
+            if pd is None:
+                raise TypeError(
+                    f"EOmaps: Unable to handle the input-data type: {type(data)}"
+                )
 
+            if isinstance(data, pd.DataFrame):
                 if parameter is not None:
                     # get the data-values
                     z_data = data[parameter].values
                 else:
                     z_data = np.repeat(np.nan, len(data))
 
                 # get the index-values
@@ -3645,43 +4150,43 @@
 
                     xorig = np.asanyarray(x)
                     yorig = np.asanyarray(y)
 
                 return z_data, xorig, yorig, ids, parameter
 
         # identify all other types except for pandas.DataFrames
-
         # lazily check if pandas was used
         pandas_series_data = False
         for iname, i in zip(("x", "y", "data"), (x, y, data)):
             if iname == "data" and i is None:
                 # allow empty datasets
                 continue
 
             if not isinstance(i, (list, tuple, np.ndarray)):
-                if _register_pandas() and not isinstance(i, pd.Series):
+                (pd,) = register_modules("pandas", raise_exception=False)
+
+                if pd and not isinstance(i, pd.Series):
                     raise AssertionError(
                         f"{iname} values must be a list, numpy-array or pandas.Series"
                     )
                 else:
                     if iname == "data":
                         pandas_series_data = True
 
         # set coordinates by extent
-
         if isinstance(x, tuple) and isinstance(y, tuple):
             assert data is not None, (
-                "EOmaps: If x- and y are provided as tuples, the data must be a 2D list "
-                "or numpy-array!"
+                "EOmaps: If x- and y are provided as tuples, the data must be a 2D list"
+                " or numpy-array!"
             )
 
             shape = np.shape(data)
             assert len(shape) == 2, (
-                "EOmaps: If x- and y are provided as tuples, the data must be a 2D list "
-                "or numpy-array!"
+                "EOmaps: If x- and y are provided as tuples, the data must be a 2D list"
+                " or numpy-array!"
             )
 
             # get the data-coordinates
             xorig = np.linspace(*x, shape[0])
             yorig = np.linspace(*y, shape[1])
 
         else:
@@ -3763,19 +4268,22 @@
         Parameters
         ----------
         m : eomaps.Maps or None
             The Maps-object that provides the data.
         """
         if m is not None:
             self.data_specs = m.data_specs
-            self.set_data_specs = lambda *args, **kwargs: (
-                "EOmaps: You cannot set data_specs for a Maps object that "
-                "inherits data!"
-            )
-            self.set_data = self.set_data_specs
+
+            def set_data(*args, **kwargs):
+                raise AssertionError(
+                    "EOmaps: You cannot set data for a Maps object that "
+                    "inherits data!"
+                )
+
+            self.set_data = set_data
 
     def _classify_data(
         self,
         z_data=None,
         cmap=None,
         vmin=None,
         vmax=None,
@@ -3802,18 +4310,15 @@
         if isinstance(cmap, str):
             cmap = plt.get_cmap(cmap).copy()
         else:
             cmap = cmap.copy()
 
         # evaluate classification
         if classify_specs is not None and classify_specs.scheme is not None:
-            assert _register_mapclassify(), (
-                "EOmaps: Missing dependency: 'mapclassify' \n ... please install "
-                "(conda install -c conda-forge mapclassify) to use classifications."
-            )
+            (mapclassify,) = register_modules("mapclassify")
 
             classified = True
             if self.classify_specs.scheme == "UserDefined":
                 bins = self.classify_specs.bins
             else:
                 mapc = getattr(mapclassify, classify_specs.scheme)(
                     z_data[~np.isnan(z_data)], **classify_specs
@@ -3824,16 +4329,15 @@
 
             if vmax > max(bins):
                 bins[np.argmax(bins)] = vmax
 
             cbcmap = cmap
             norm = mpl.colors.BoundaryNorm(bins, cmap.N)
 
-            if self._companion_widget is not None:
-                self._companion_widget.cmapsChanged.emit()
+            self._emit_signal("cmapsChanged")
 
             if cmap._rgba_bad:
                 cbcmap.set_bad(cmap._rgba_bad)
             if cmap._rgba_over:
                 cbcmap.set_over(cmap._rgba_over)
             if cmap._rgba_under:
                 cbcmap.set_under(cmap._rgba_under)
@@ -3864,27 +4368,35 @@
             self.parent._add_child(self)
 
     def _set_default_shape(self):
         if self.data is not None:
             size = np.size(self.data)
 
             if len(np.shape(self.data)) == 2 and size > 200_000:
-                if size > 5e6 and _register_datashader():
+                if size > 5e6 and all(
+                    register_modules(
+                        "datashader", "datashader.mpl_ext", raise_exception=False
+                    )
+                ):
                     # only try to use datashader for very large 2D datasets
                     self.set_shape.shade_raster()
                 else:
                     self.set_shape.raster()
             else:
                 if size > 500_000:
-                    if _register_datashader():
+                    if all(
+                        register_modules(
+                            "datashader", "datashader.mpl_ext", raise_exception=False
+                        )
+                    ):
                         # shade_points should work for any dataset
                         self.set_shape.shade_points()
                     else:
-                        print(
-                            "EOmaps-Warning: Attempting to plot a large dataset "
+                        _log.warning(
+                            "EOmaps: Attempting to plot a large dataset "
                             f"({size} datapoints) but the 'datashader' library "
                             "could not be imported! The plot might take long "
                             "to finish! ... defaulting to 'ellipses' "
                             "as plot-shape."
                         )
                         self.set_shape.ellipses()
                 else:
@@ -3940,19 +4452,15 @@
             The default is "crs".
 
         Returns
         -------
         gdf
             A GeoDataFrame with the clipped geometries
         """
-        assert _register_geopandas(), (
-            "EOmaps: Missing dependency `geopandas`!\n"
-            + "please install '(conda install -c conda-forge geopandas)'"
-            + "to use `m.add_gdf()`."
-        )
+        (gpd,) = register_modules("geopandas")
 
         if how.startswith("gdal"):
             methods = ["SymDifference", "Intersection", "Difference", "Union"]
             # "SymDifference", "Intersection", "Difference"
             method = how.split("_")[1]
             assert method in methods, "EOmaps: '{how}' is not a valid clip-method"
             try:
@@ -4032,15 +4540,15 @@
         class scheme:
             @wraps(s)
             def __init__(_, *args, **kwargs):
                 pass
 
             def __new__(cls, **kwargs):
                 if "y" in kwargs:
-                    print(
+                    _log.error(
                         "EOmaps: The values (e.g. the 'y' parameter) are "
                         + "assigned internally... only provide additional "
                         + "parameters that specify the classification scheme!"
                     )
                     kwargs.pop("y")
 
                 self.classify_specs._set_scheme_and_args(scheme=s.__name__, **kwargs)
@@ -4052,14 +4560,18 @@
         self,
         layer=None,
         dynamic=False,
         set_extent=True,
         assume_sorted=True,
         **kwargs,
     ):
+        _log.info(
+            "EOmaps: Plotting "
+            f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
+        )
 
         for key in ("array", "norm"):
             assert (
                 key not in kwargs
             ), f"The key '{key}' is assigned internally by EOmaps!"
 
         try:
@@ -4137,53 +4649,55 @@
             )
 
         if self.shape.name in ["raster"]:
             # if input-data is 1D, try to convert data to 2D (required for raster)
             # TODO make an explicit data-conversion function for 2D-only shapes
             if len(self._xshape) == 2 and len(self._yshape) == 2:
                 coll = self.shape.get_coll(props["xorig"], props["yorig"], "in", **args)
-            elif _register_pandas():
-                if (
-                    (len(self._xshape) == 1)
-                    and (len(self._yshape) == 1)
-                    and (len(self._zshape) == 1)
-                    and (props["x0"].size == props["y0"].size)
-                    and (props["x0"].size == props["z_data"].size)
-                ):
-
-                    df = (
-                        pd.DataFrame(
-                            dict(
-                                x=props["x0"].ravel(),
-                                y=props["y0"].ravel(),
-                                val=props["z_data"].ravel(),
-                            ),
-                            copy=False,
-                        ).set_index(["x", "y"])
-                    )["val"].unstack("y")
+            else:
+                (pd,) = register_modules("pandas")
+                # TODO avoid having pandas as a dependency here
+                if pd:
+                    if (
+                        (len(self._xshape) == 1)
+                        and (len(self._yshape) == 1)
+                        and (len(self._zshape) == 1)
+                        and (props["x0"].size == props["y0"].size)
+                        and (props["x0"].size == props["z_data"].size)
+                    ):
+
+                        df = (
+                            pd.DataFrame(
+                                dict(
+                                    x=props["x0"].ravel(),
+                                    y=props["y0"].ravel(),
+                                    val=props["z_data"].ravel(),
+                                ),
+                                copy=False,
+                            ).set_index(["x", "y"])
+                        )["val"].unstack("y")
 
-                    xg, yg = np.meshgrid(df.index.values, df.columns.values)
+                        xg, yg = np.meshgrid(df.index.values, df.columns.values)
 
-                    if args["array"] is not None:
-                        args["array"] = df.values.T
+                        if args["array"] is not None:
+                            args["array"] = df.values.T
 
-                    coll = self.shape.get_coll(xg, yg, "out", **args)
+                        coll = self.shape.get_coll(xg, yg, "out", **args)
         else:
             # convert to 1D for further processing
             if args["array"] is not None:
                 args["array"] = args["array"].ravel()
 
             coll = self.shape.get_coll(
                 props["x0"].ravel(), props["y0"].ravel(), "out", **args
             )
         return coll
 
     def _shade_map(
         self,
-        verbose=0,
         layer=None,
         dynamic=False,
         set_extent=True,
         assume_sorted=True,
         **kwargs,
     ):
         """
@@ -4200,71 +4714,62 @@
 
         - By default, the shading is performed using a "mean"-value aggregation hook
 
         kwargs :
             kwargs passed to `datashader.mpl_ext.dsshow`
 
         """
-        assert _register_datashader(), (
-            "EOmaps: Missing dependency: 'datashader' \n ... please install"
-            + " (conda install -c conda-forge datashader) to use the plot-shapes "
-            + "'shade_points' and 'shade_raster'"
+        _log.info(
+            "EOmaps: Plotting "
+            f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
+        )
+
+        ds, mpl_ext, pd, xar = register_modules(
+            "datashader", "datashader.mpl_ext", "pandas", "xarray"
         )
 
         # remove previously fetched backgrounds for the used layer
         if dynamic is False:
             self.BM._refetch_layer(layer)
-            # del self.BM._bg_layers[layer]
-            # self.BM._refetch_bg = True
 
         # in case the aggregation does not represent data-values
         # (e.g. count, std, var ... ) use an automatic "linear" normalization
 
         # get the name of the used aggretation reduction
         aggname = self.shape.aggregator.__class__.__name__
 
         if aggname in ["first", "last", "max", "min", "mean", "mode"]:
             kwargs.setdefault("norm", self.classify_specs._norm)
         else:
             kwargs.setdefault("norm", "linear")
 
-        if verbose > 0:
-            print("EOmaps: Plotting...")
-
         zdata = self._data_manager.z_data
         if len(zdata) == 0:
-            print("EOmaps: there was no data to plot")
+            _log.error("EOmaps: there was no data to plot")
             return
 
         plot_width, plot_height = int(self.ax.bbox.width), int(self.ax.bbox.height)
 
         # get rid of unnecessary dimensions in the numpy arrays
         zdata = zdata.squeeze()
         x0 = self._data_manager.x0.squeeze()
         y0 = self._data_manager.y0.squeeze()
 
         # the shape is always set after _prepare data!
         if self.shape.name == "shade_points" and self._data_manager.x0_1D is None:
-            assert (
-                _register_pandas()
-            ), f"EOmaps: missing dependency 'pandas' for {self.shape.name}"
-
             df = pd.DataFrame(
                 dict(
                     x=x0.ravel(),
                     y=y0.ravel(),
                     val=zdata.ravel(),
                 ),
                 copy=False,
             )
 
         else:
-            assert (
-                _register_xarray()
-            ), "EOmaps: missing dependency `xarray` for 'shade_raster'"
             if len(zdata.shape) == 2:
                 if (zdata.shape == x0.shape) and (zdata.shape == y0.shape):
                     # 2D coordinates and 2D raster
 
                     # use a curvilinear QuadMesh
                     if self.shape.name == "shade_raster":
                         self.shape.glyph = ds.glyphs.QuadMeshCurvilinear(
@@ -4313,18 +4818,14 @@
                         dims=["x", "y"],
                         coords=dict(x=x0, y=y0),
                     )
                     df = xar.Dataset(dict(val=df))
             else:
                 # first convert 1D inputs to 2D, then reproject the grid and use
                 # a curvilinear QuadMesh to display the data
-                assert _register_pandas(), (
-                    "EOmaps: missing dependency 'pandas' to convert 1D"
-                    + "datasets to 2D as required for 'shade_raster'"
-                )
 
                 # use pandas to convert to 2D
                 df = (
                     pd.DataFrame(
                         dict(
                             x=x0.ravel(),
                             y=y0.ravel(),
@@ -4391,23 +4892,17 @@
             x_range=x_range,
             y_range=y_range,
             vmin=self._vmin,
             vmax=self._vmax,
             **kwargs,
         )
 
-        self._coll = coll
-        if verbose > 0:
-            print("EOmaps: Indexing for pick-callbacks...")
+        coll.set_label("Dataset " f"({self.shape.name}  |  {zdata.shape})")
 
-        # This is now done lazily (only if a pick-callback is attached)
-        # self.tree = searchtree(m=self._proxy(self))
-        # self.cb.pick._set_artist(coll)
-        # self.cb.pick._init_cbs()
-        # self.cb._methods.add("pick")
+        self._coll = coll
 
         if dynamic is True:
             self.BM.add_artist(coll, layer)
         else:
             self.BM.add_bg_artist(coll, layer)
 
         if dynamic is True:
@@ -4447,18 +4942,16 @@
 
                 if add_offset:
                     val = val - add_offset
                 if scale_factor:
                     val = val / scale_factor
 
                 return val
-            except:
-                print(
-                    "EOmaps: There was an error while trying to encode the data:", val
-                )
+            except Exception:
+                _log.exception(f"EOmaps: Error while trying to encode the data: {val}")
                 return val
         else:
             return val
 
     def _decode_values(self, val):
         """
         Decode data-values with respect to the provided "scale_factor" and "add_offset".
@@ -4490,16 +4983,16 @@
 
                 if scale_factor:
                     val = val * scale_factor
                 if add_offset:
                     val = val + add_offset
 
                 return val
-            except:
-                print("EOmaps: There was an error while trying to decode the data.")
+            except Exception:
+                _log.exception(f"EOmaps: Error while trying to decode the data {val}.")
                 return val
         else:
             return val
 
     def _get_layers(self, exclude=None, exclude_private=True):
         # return a list of all (empty and non-empty) layer-names
         layers = set((m.layer for m in (self.parent, *self.parent._children)))
@@ -4510,31 +5003,31 @@
 
         # add all (possibly still invisible) layers with artists defined
         # (ONLY do this for unique layers... skip multi-layers )
         layers = layers.union({i for i in self.BM._bg_artists if "|" not in i})
 
         # exclude private layers
         if exclude_private:
-            layers = {l for l in layers if not l.startswith("__")}
+            layers = {i for i in layers if not i.startswith("__")}
 
         if exclude:
-            for l in exclude:
-                if l in layers:
-                    layers.remove(l)
+            for i in exclude:
+                if i in layers:
+                    layers.remove(i)
 
         # sort the layers
         layers = sorted(layers, key=lambda x: str(x))
 
         return layers
 
     @lru_cache()
     def _get_nominatim_response(self, q, user_agent=None):
         import requests
 
-        print(f"Querying {q}")
+        _log.info(f"Querying {q}")
         if user_agent is None:
             user_agent = f"EOMaps v{Maps.__version__}"
 
         headers = {
             "User-Agent": user_agent,
         }
 
@@ -4581,29 +5074,41 @@
             )
 
             self.ax.add_artist(self._companion_map_indicator)
             self.BM.add_artist(self._companion_map_indicator, "all")
 
         self.BM.update()
 
-    def _open_companion_widget_cb(self, event):
-        if event.key != self._companion_widget_key:
-            return
+    def _open_companion_widget(self, xy=None):
+        """
+        Open the companion-widget.
 
-        clicked_map = None
-        for m in (self.parent, *self.parent._children):
-            if not m._new_axis_map:
-                # only search for Maps-object that initialized new axes
-                continue
+        Parameters
+        ----------
+        xy : tuple, optional
+            The click position to identify the relevant Maps-object
+            (in figure coordinates).
+            If None, the calling Maps-object is used
+
+            The default is None.
+
+        """
+
+        clicked_map = self
+        if xy is not None:
+            for m in (self.parent, *self.parent._children):
+                if not m._new_axis_map:
+                    # only search for Maps-object that initialized new axes
+                    continue
 
-            if m.ax.contains_point((event.x, event.y)):
-                clicked_map = m
+                if m.ax.contains_point(xy):
+                    clicked_map = m
 
         if clicked_map is None:
-            print(
+            _log.error(
                 "EOmaps: To activate the 'Companion Widget' you must "
                 "position the mouse on top of an EOmaps Map!"
             )
             return
 
         # hide all other companion-widgets
         for m in (self.parent, *self.parent._children):
@@ -4648,55 +5153,105 @@
         Parameters
         ----------
         show_hide_key : str or None, optional
             The keyboard-shortcut that is assigned to show/hide the widget.
             The default is "w".
         """
         try:
-            if plt.get_backend() not in ["QtAgg", "Qt5Agg"]:
-                print(
-                    "EOmaps: Using m.open_widget() is only possible if you use matplotlibs"
-                    + f" 'Qt5Agg' backend! (active backend: '{plt.get_backend()}')"
-                )
-                return
-
             from .qtcompanion.app import MenuWindow
 
             if self._companion_widget is not None:
-                print(
+                _log.error(
                     "EOmaps: There is already an existing companinon widget for this"
                     " Maps-object!"
                 )
                 return
+            if plt.get_backend() in ["QtAgg", "Qt5Agg"]:
+                # only pass parent if Qt is used as a backend for matplotlib!
+                self._companion_widget = MenuWindow(m=self, parent=self.f.canvas)
+            else:
+                self._companion_widget = MenuWindow(m=self)
+                self._companion_widget.toggle_always_on_top()
+
+            # connect any pending signals
+            for key, funcs in getattr(self, "_connect_signals_on_init", dict()).items():
+                while len(funcs) > 0:
+                    self._connect_signal(key, funcs.pop())
 
-            self._companion_widget = MenuWindow(m=self, parent=self.f.canvas)
             # make sure that we clear the colormap-pixmap cache on startup
-            self._companion_widget.cmapsChanged.emit()
+            self._emit_signal("cmapsChanged")
 
-        except Exception as ex:
-            print("EOmaps: Unable to initialize companion widget.", ex)
+        except Exception:
+            _log.exception(
+                "EOmaps: Unable to initialize companion widget.",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
+
+    def _connect_signal(self, name, func):
+        parent = self.parent
+        widget = parent._companion_widget
+
+        # NOTE: use Maps.config(log_level=5) to get signal log messages!
+        if widget is None:
+            if not hasattr(parent, "_connect_signals_on_init"):
+                parent._connect_signals_on_init = dict()
+
+            parent._connect_signals_on_init.setdefault(name, set()).add(func)
+
+        if widget is not None:
+            try:
+                getattr(parent._signal_container, name).connect(func)
+                _log.log(1, f"Signal connected: {name} ({func.__name__})")
+
+            except Exception:
+                _log.log(
+                    1,
+                    f"There was a problem while trying to connect the function {func} "
+                    f"to the signal {name} ",
+                    exc_info=True,
+                )
+
+    def _emit_signal(self, name, *args):
+        parent = self.parent
+        widget = parent._companion_widget
+
+        # NOTE: use Maps.config(log_level=5) to get signal log messages!
+        if widget is not None:
+            try:
+                getattr(parent._signal_container, name).emit(*args)
+                _log.log(1, f"Signal emitted: {name} {args}")
+            except Exception:
+                _log.log(
+                    1,
+                    f"There was a problem while trying to emit the signal {name} "
+                    f"with the args {args}",
+                    exc_info=True,
+                )
 
     @staticmethod
     def _proxy(obj):
         # None cannot be weak-referenced!
         if obj is None:
             return None
 
         # create a proxy if the object is not yet a proxy
         if type(obj) is not weakref.ProxyType:
             return weakref.proxy(obj)
         else:
             return obj
 
     @staticmethod
+    @lru_cache()
     def _get_cartopy_crs(crs):
         if isinstance(crs, Maps.CRS.CRS):  # already a cartopy CRS
             cartopy_proj = crs
         elif crs == 4326:
             cartopy_proj = ccrs.PlateCarree()
+        elif crs == 3857:
+            cartopy_proj = ccrs.Mercator.GOOGLE
         elif isinstance(crs, (int, np.integer)):
             cartopy_proj = ccrs.epsg(crs)
         elif isinstance(crs, CRS):  # pyproj CRS
             cartopy_proj = None
             for (
                 subgrid,
                 equi7crs,
@@ -4709,33 +5264,27 @@
 
         else:
             raise AssertionError(f"EOmaps: cannot identify the CRS for: {crs}")
 
         return cartopy_proj
 
     @staticmethod
+    @lru_cache()
     def _get_transformer(crs_from, crs_to):
-        # create a pyproj Transformer object or return a cached version of it
-        # if it has already been created.
-        c_from = Maps._transformer_cache.setdefault(hash(crs_from), dict())
-        return c_from.setdefault(
-            hash(crs_to), Transformer.from_crs(crs_from, crs_to, always_xy=True)
-        )
+        # create a pyproj Transformer object and cache it for later use
+        return Transformer.from_crs(crs_from, crs_to, always_xy=True)
 
     @property
-    @lru_cache()
     def _transf_plot_to_lonlat(self):
-        # cache commonly used transformers
         return self._get_transformer(
             self.crs_plot,
             self.get_crs(self.crs_plot.as_geodetic()),
         )
 
     @property
-    @lru_cache()
     def _transf_lonlat_to_plot(self):
         return self._get_transformer(
             self.get_crs(self.crs_plot.as_geodetic()),
             self.crs_plot,
         )
 
     @property
@@ -4761,18 +5310,15 @@
 
         Returns
         -------
         gdf : geopandas.GeoDataFrame
             the geodataframe with the shape and crs defined
 
         """
-        assert _register_geopandas(), (
-            "EOmaps: Missing dependency `geopandas`!\n"
-            + "please install '(conda install -c conda-forge geopandas)'"
-        )
+        (gpd,) = register_modules("geopandas")
 
         from shapely.geometry import Polygon
 
         xs, ys = np.linspace([x0, y0], [x1, y1], npts).T
         x0, y0, x1, y1, xs, ys = np.broadcast_arrays(x0, y0, x1, y1, xs, ys)
         verts = np.column_stack(((x0, ys), (xs, y1), (x1, ys[::-1]), (xs[::-1], y0))).T
 
@@ -4803,374 +5349,7 @@
 
     if refetch_wms_on_size_change is not None:
 
         @wraps(refetch_wms_on_size_change)
         def refetch_wms_on_size_change(self, *args, **kwargs):
             """Set the behavior for WebMap services on axis or figure size changes."""
             refetch_wms_on_size_change(*args, **kwargs)
-
-
-class InsetMaps(Maps):
-    # a subclass of Maps that includes some special functions for inset maps
-
-    def __init__(
-        self,
-        parent,
-        crs=4326,
-        layer=None,
-        xy=(45, 45),
-        xy_crs=4326,
-        radius=5,
-        radius_crs=None,
-        plot_position=(0.5, 0.5),
-        plot_size=0.5,
-        shape="ellipses",
-        indicate_extent=True,
-        indicator_line=False,
-        boundary=True,
-        background_color="w",
-        **kwargs,
-    ):
-
-        self._parent = self._proxy(parent)
-
-        # inherit the layer from the parent Maps-object if not explicitly
-        # provided
-        if layer is None:
-            layer = self._parent.layer
-
-        # put all inset-map artists on dedicated layers
-        # NOTE: all artists of inset-map axes are put on a dedicated layer
-        # with a "__inset_" prefix to ensure they appear on top of other artists
-        # (AND on top of spines of normal maps)!
-        # layer = "__inset_" + str(layer)
-
-        possible_shapes = ["ellipses", "rectangles", "geod_circles"]
-        assert (
-            shape in possible_shapes
-        ), f"EOmaps: the inset shape can only be one of {possible_shapes}"
-
-        if shape == "geod_circles":
-            assert radius_crs is None, (
-                "EOmaps: Using 'radius_crs' is not possible if 'geod_circles' is "
-                + "used as shape! (the radius for `geod_circles` is always in meters!)"
-            )
-
-        if radius_crs is None:
-            radius_crs = xy_crs
-
-        extent_kwargs = dict(ec="r", lw=1, fc="none")
-        line_kwargs = dict(c="r", lw=2)
-        boundary_kwargs = dict(ec="r", lw=2)
-
-        if isinstance(boundary, dict):
-            assert (
-                len(set(boundary.keys()).difference({"ec", "lw"})) == 0
-            ), "EOmaps: only 'ec' and 'lw' keys are allowed for the 'boundary' dict!"
-
-            boundary_kwargs.update(boundary)
-            # use same edgecolor for boundary and indicator by default
-            extent_kwargs["ec"] = boundary["ec"]
-            line_kwargs["c"] = boundary["ec"]
-        elif isinstance(boundary, str):
-            boundary_kwargs.update({"ec": boundary})
-            # use same edgecolor for boundary and indicator by default
-            extent_kwargs["ec"] = boundary
-            line_kwargs["c"] = boundary
-
-        if isinstance(indicate_extent, dict):
-            extent_kwargs.update(indicate_extent)
-
-        if isinstance(indicator_line, dict):
-            line_kwargs.update(indicator_line)
-
-        x, y = xy
-        plot_x, plot_y = plot_position
-        left = plot_x - plot_size / 2
-        bottom = plot_y - plot_size / 2
-
-        # initialize a new maps-object with a new axis
-        super().__init__(
-            crs=crs,
-            f=self._parent.f,
-            ax=(left, bottom, plot_size, plot_size),
-            layer=layer,
-            **kwargs,
-        )
-
-        # get the boundary of a ellipse in the inset_crs
-        bnd, bnd_verts = self._get_inset_boundary(
-            x, y, xy_crs, radius, radius_crs, shape
-        )
-
-        # set the map boundary
-        self.ax.set_boundary(bnd)
-        # set the plot-extent to the envelope of the shape
-        (x0, y0), (x1, y1) = bnd_verts.min(axis=0), bnd_verts.max(axis=0)
-        self.ax.set_extent((x0, x1, y0, y1), crs=self.ax.projection)
-
-        # TODO turn off navigation until the matpltolib pull-request on
-        # zoom-events in overlapping axes is resolved
-        # https://github.com/matplotlib/matplotlib/pull/22347
-        self.ax.set_navigate(False)
-
-        if boundary is not False:
-            spine = self.ax.spines["geo"]
-            spine.set_edgecolor(boundary_kwargs["ec"])
-            spine.set_lw(boundary_kwargs["lw"])
-
-        self._inset_props = dict(
-            xy=xy, xy_crs=xy_crs, radius=radius, radius_crs=radius_crs, shape=shape
-        )
-
-        if indicate_extent is not False:
-            self.indicate_inset_extent(
-                self._parent, layer=self._parent.layer, permanent=True, **extent_kwargs
-            )
-
-        self._indicator_lines = []
-        if indicator_line is not False:
-            self.add_indicator_line(**line_kwargs)
-
-        # add a background patch to the "all" layer
-        if background_color is not None:
-            self._bg_patch = self._add_background_patch(
-                color=background_color, layer="all"
-            )
-        else:
-            self._bg_patch = None
-
-    def _add_background_patch(self, color, layer="all"):
-        (art,) = self.ax.fill(
-            [0, 0, 1, 1],
-            [0, 1, 1, 0],
-            fc=color,
-            ec="none",
-            zorder=-np.inf,
-            transform=self.ax.transAxes,
-        )
-        self.BM.add_bg_artist(art, layer=layer)
-        return art
-
-    def _handle_spines(self):
-        spine = self.ax.spines["geo"]
-        if spine not in self.BM._bg_artists.get("__inset___SPINES__", []):
-            self.BM.add_bg_artist(spine, layer="__inset___SPINES__")
-
-    def _get_ax_label(self):
-        return "inset_map"
-
-    def plot_map(self, *args, **kwargs):
-        set_extent = kwargs.pop("set_extent", False)
-        super().plot_map(*args, **kwargs, set_extent=set_extent)
-
-    # a convenience-method to add a boundary-polygon to a map
-    def indicate_inset_extent(self, m, n=100, **kwargs):
-        """
-        Add a polygon to a  map that indicates the extent of the inset-map.
-
-        Parameters
-        ----------
-        m : eomaps.Maps
-            The Maps-object that will be used to draw the marker.
-            (e.g. the map on which the extent of the inset should be indicated)
-        n : int
-            The number of points used to represent the polygon.
-            The default is 100.
-        kwargs :
-            additional keyword-arguments passed to `m.add_marker`
-            (e.g. "facecolor", "edgecolor" etc.)
-
-        """
-        if not any((i in kwargs for i in ["fc", "facecolor"])):
-            kwargs["fc"] = "none"
-        if not any((i in kwargs for i in ["ec", "edgecolor"])):
-            kwargs["ec"] = "r"
-        if not any((i in kwargs for i in ["lw", "linewidth"])):
-            kwargs["lw"] = 1
-
-        kwargs.setdefault("permanent", True)
-        kwargs.setdefault("zorder", 9999)
-
-        m.add_marker(
-            shape=self._inset_props["shape"],
-            xy=self._inset_props["xy"],
-            xy_crs=self._inset_props["xy_crs"],
-            radius=self._inset_props["radius"],
-            radius_crs=self._inset_props["radius_crs"],
-            n=n,
-            **kwargs,
-        )
-
-    def add_indicator_line(self, m=None, **kwargs):
-        """
-        Add a line that connects the inset-map to the inset location on a given map.
-
-        The line connects the current inset-map (center) position to the center of the
-        inset extent on the provided Maps-object.
-
-        It is possible to add multiple indicator-lines for different maps!
-
-        The lines will be automatically updated if axes sizes or positions change.
-
-        Parameters
-        ----------
-        m : eomaps.Maps or None
-            The Maps object for which the inset-line should be added.
-            If None, the parent Maps-object that was used to create the inset-map
-            is used. The default is None.
-
-        kwargs :
-            Additional kwargs are passed to plt.Line2D to style the appearance of the
-            line (e.g. "c", "ls", "lw", ...)
-
-
-        Examples
-        --------
-
-        """
-        if m is None:
-            m = self._parent
-
-        kwargs.setdefault("c", "r")
-        kwargs.setdefault("lw", 2)
-        kwargs.setdefault("zorder", -np.inf)
-
-        l = plt.Line2D([0, 0], [1, 1], **kwargs)
-        l = self.f.add_artist(l)
-        self.BM.add_bg_artist(l, "__inset_all")
-        self._indicator_lines.append((l, m))
-
-        if isinstance(m, InsetMaps):
-            # in order to make the line visible on top of another inset-map
-            # but NOT on the inset-map whose extent is indicated, the line has to
-            # be drawn on the inset-map explicitly.
-
-            # This is because all artists on inset-map axes are always on top of other
-            # (normal map) artists... (and so the line would be behind the background)
-
-            kwargs["zorder"] = np.inf
-            l2 = plt.Line2D([0, 0], [1, 1], **kwargs, transform=m.f.transFigure)
-            l2 = m.ax.add_artist(l2)
-            self.BM.add_bg_artist(l2, "__inset_all")
-            self._indicator_lines.append((l2, m))
-
-        self._update_indicator_lines()
-        self.BM._before_fetch_bg_actions.append(self._update_indicator_lines)
-
-    def _update_indicator_lines(self, *args, **kwargs):
-        props = self._inset_props
-        bbox = self.ax.get_position()
-        # get current inset-map position
-        x1 = (bbox.x1 + bbox.x0) / 2
-        y1 = (bbox.y1 + bbox.y0) / 2
-
-        for l, m in self._indicator_lines:
-            # get inset map extent in ax projection
-            t = m._get_transformer(props["xy_crs"], m.ax.projection)
-            xy = t.transform(*props["xy"])
-            # get inset map extent in figure coordinates
-            x0, y0 = (m.ax.transData + m.f.transFigure.inverted()).transform(xy)
-
-            l.set_xdata([x0, x1])
-            l.set_ydata([y0, y1])
-
-    # a convenience-method to set the position based on the center of the axis
-    def set_inset_position(self, x=None, y=None, size=None):
-        """
-        Set the (center) position and size of the inset-map.
-
-        Parameters
-        ----------
-        x, y : int or float, optional
-            The center position in relative units (0-1) with respect to the figure.
-            If None, the existing position is used.
-            The default is None.
-        size : float, optional
-            The relative radius (0-1) of the inset in relation to the figure width.
-            If None, the existing size is used.
-            The default is None.
-
-        """
-        x0, y1, x1, y0 = self.ax.get_position().bounds
-
-        if size is None:
-            size = abs(x1 - x0)
-
-        if x is None:
-            x = (x0 + x1) / 2
-        if y is None:
-            y = (y0 + y1) / 2
-
-        self.ax.set_position((x - size / 2, y - size / 2, size, size))
-        self.redraw("__inset_" + self.layer, "__inset___SPINES__")
-
-    # a convenience-method to get the position based on the center of the axis
-    def get_inset_position(self, precision=3):
-        """
-        Get the current inset position (and size).
-
-        Parameters
-        ----------
-        precision : int, optional
-            The precision of the returned position and size.
-            The default is 3.
-
-        Returns
-        -------
-        (x, y, size) : (float, float, float)
-            The position and size of the inset-map.
-
-        """
-        bbox = self.ax.get_position()
-        size = round(max(bbox.width, bbox.height), precision)
-        x = round((bbox.x0 + bbox.width / 2), precision)
-        y = round((bbox.y0 + bbox.height / 2), precision)
-
-        return x, y, size
-
-    def _get_inset_boundary(self, x, y, xy_crs, radius, radius_crs, shape, n=100):
-        # get the inset-shape boundary
-
-        shp = self.set_shape._get(shape)
-
-        if shape == "ellipses":
-            shp_pts = shp._get_ellipse_points(
-                x=np.atleast_1d(x),
-                y=np.atleast_1d(y),
-                crs=xy_crs,
-                radius=radius,
-                radius_crs=radius_crs,
-                n=n,
-            )
-            bnd_verts = np.stack(shp_pts[:2], axis=2)[0]
-
-            # make sure vertices are right-handed
-            bnd_verts = bnd_verts[::-1]
-
-        elif shape == "rectangles":
-            shp_pts = shp._get_rectangle_verts(
-                x=np.atleast_1d(x),
-                y=np.atleast_1d(y),
-                crs=xy_crs,
-                radius=radius,
-                radius_crs=radius_crs,
-                n=n,
-            )
-            bnd_verts = shp_pts[0][0]
-
-        elif shape == "geod_circles":
-            shp_pts = shp._get_geod_circle_points(
-                x=np.atleast_1d(x),
-                y=np.atleast_1d(y),
-                crs=xy_crs,
-                radius=radius,
-                # radius_crs=radius_crs,
-                n=n,
-            )
-            bnd_verts = np.stack(shp_pts[:2], axis=2).squeeze()
-            # make sure vertices are right-handed
-            bnd_verts = bnd_verts[::-1]
-
-        boundary = mpl.path.Path(bnd_verts)
-
-        return boundary, bnd_verts
```

### Comparing `EOmaps-6.5/eomaps/grid.py` & `EOmaps-7.0/eomaps/grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from matplotlib.collections import LineCollection
-import numpy as np
+"""Grid lines and grid labels."""
+
+import logging
 from itertools import chain
 from functools import lru_cache
-from .helpers import pairwise
+
+import numpy as np
+
+from matplotlib.collections import LineCollection
+
+_log = logging.getLogger(__name__)
 
 
 class GridLines:
+    """Class to draw grid-lines."""
+
     def __init__(self, m, d=None, auto_n=10, layer=None, bounds=None, n=100):
         self.m = m._proxy(m)
 
         self._d = d
         self._auto_n = auto_n
         self._bounds = bounds
         self._n = n
@@ -18,33 +26,38 @@
         self._coll = None
 
         self._layer = layer
         self._grid_labels = []
 
     @property
     def d(self):
+        """The fixed grid-spacing distance (if specified)."""
         return self._d
 
     @property
     def layer(self):
+        """The layer assigned to the grid"""
         if self._layer is None:
             return self.m.layer
         else:
             return self._layer
 
     @property
     def auto_n(self):
+        """Number of automatic grid-lines to evaluate (if d=None)"""
         return self._auto_n
 
     @property
     def n(self):
+        """Number of intermediate points to draw for each gridline"""
         return self._n
 
     @property
     def bounds(self):
+        """The boundaries of the grid"""
         if self._bounds is None:
             return (-180, 180, -90, 90)
         return self._bounds
 
     def set_bounds(self, bounds):
         """
         Set the extent of the area in which gridlines are drawn.
@@ -54,14 +67,15 @@
         bounds : tuple or None
             A tuple of boundaries in the form:  (lon_min, lon_max, lat_min, lat_max).
             If None, global boundaries are used (e.g. (-180, 180, -90, 90))
 
         """
         self._bounds = bounds
         self._redraw()
+        self.m.redraw(self.layer)
 
     def set_d(self, d):
         """
         Set a fixed gridline distance (in degrees).
 
         Parameters
         ----------
@@ -76,14 +90,15 @@
             - If `None`, gridlines are automatically determined based on the "auto_n"
               parameter.
 
         The default is None
         """
         self._d = d
         self._redraw()
+        self.m.redraw(self.layer)
 
     def set_auto_n(self, auto_n):
         """
         Set the number of (auto) gridlines to draw in the currently visible extent.
 
         Note: this is an approximate value!
 
@@ -93,27 +108,29 @@
             The (rough) number of gridlines to use when evaluating the automatic
             grid-spacing. To use different numbers of gridlines in each direction,
             provide a tuple of ints, e.g.: `(n_lon, n_lat)`.
 
         """
         self._auto_n = auto_n
         self._redraw()
+        self.m.redraw(self.layer)
 
     def set_n(self, n):
         """
         Set the number of intermediate points to calculate for each gridline.
 
         Parameters
         ----------
         n : int
             Number of intermedate points.
 
         """
         self._n = n
         self._redraw()
+        self.m.redraw(self.layer)
 
     def _update_line_props(self, **kwargs):
         color = None
         if "c" in kwargs:
             color = kwargs.pop("c", None)
         if "color" in kwargs:
             color = kwargs.pop("color", None)
@@ -139,14 +156,15 @@
         ----------
         kwargs :
             keyword-arguments used to update the properties of the lines.
 
         """
         self._update_line_props(**kwargs)
         self._redraw()
+        self.m.redraw(self.layer)
 
     @staticmethod
     def _calc_lines(d, bounds, n=100):
         lons, lats, dlon, dlat = None, None, None, None
 
         if isinstance(d, tuple):
             # tuples are used to
@@ -288,16 +306,21 @@
         return coll
 
     def _add_grid(self, **kwargs):
         self._update_line_props(**kwargs)
 
         self._coll = self._get_coll(**self._kwargs)
         if self._coll is not None:
+            # exclude artist in companion widget editor
+            self._coll.set_label("__EOmaps_exclude")
+
             self.m.ax.add_collection(self._coll)
-            self.m.BM.add_bg_artist(self._coll, layer=self.layer)
+            # don't trigger draw since this would result in a recursion!
+            # (_redraw is called on each fetch-bg event)
+            self.m.BM.add_bg_artist(self._coll, layer=self.layer, draw=False)
 
     def _redraw(self):
         self._get_lines.cache_clear()
         try:
             self._remove()
         except Exception as ex:
             # catch exceptions to avoid issues with dynamic re-drawing of
@@ -309,15 +332,17 @@
         for l in self._grid_labels:
             l._redraw()
 
     def _remove(self):
         if self._coll is None:
             return
 
-        self.m.BM.remove_bg_artist(self._coll, layer=self.layer)
+        # don't trigger draw since this would result in a recursion!
+        # (_redraw is called on each fetch-bg event)
+        self.m.BM.remove_bg_artist(self._coll, layer=self.layer, draw=False)
         try:
             self._coll.remove()
         except ValueError:
             pass
 
         self._coll = None
 
@@ -431,14 +456,16 @@
         # remember attached labels
         self._grid_labels.append(gl)
 
         return gl
 
 
 class GridLabels:
+    """Class to draw grid-labels."""
+
     def __init__(
         self,
         g,
         where="tblr",
         offset=10,
         precision=2,
         every=None,
@@ -570,28 +597,29 @@
 
             self._last_extent = extent
             self._last_ax_pos = pos
 
             while len(self._texts) > 0:
                 try:
                     t = self._texts.pop(-1)
-                    t.remove()
-                    self._g.m.BM.remove_bg_artist(t)
-                except Exception as ex:
-                    print("EOmaps: Problem while trying to remove a grid-label:", ex)
+                    try:
+                        t.remove()
+                    except ValueError:
+                        pass
+                    self._g.m.BM.remove_bg_artist(t, draw=False)
+                except Exception:
+                    _log.exception(
+                        "EOmaps: Problem while trying to remove a grid-label:"
+                    )
                     pass
 
             self.add_labels()
-        except Exception as ex:
-            import traceback
-
-            print(
-                "EOmaps: Encountered a problem while re-drawing grid-labels:",
-                ex,
-                traceback.format_exc(),
+        except Exception:
+            _log.exception(
+                "EOmaps: Encountered a problem while re-drawing grid-labels:"
             )
             pass
 
     def _get_bound_verts(self, n=300):
         # get vertices of the grid-boundaries with n intermediate points
         m = self._g.m
         if self._g._bounds is not None:
@@ -602,16 +630,16 @@
             verts = np.column_stack(
                 ((x0, ys), (xs, y1), (x1, ys[::-1]), (xs[::-1], y0))
             ).T
 
             verts = m._transf_lonlat_to_plot.transform(*verts.T)
             verts = m.ax.transData.transform(np.column_stack(verts))
         else:
+            m.ax.spines["geo"]._adjust_location()
             verts = m.ax.spines["geo"].get_verts()
-
         return verts
 
     def _get_spine_intersections(self, lines, axis=None):
 
         m = self._g.m
 
         # get boundary vertices of current axis spine (in figure coordinates)
@@ -777,14 +805,17 @@
             txt_kwargs = self._kwargs
 
         intersection_points = self._get_grid_line_intersections(lines, axis)
 
         if intersection_points is None:
             return
 
+        transf = m.f.transFigure
+        transf_inv = transf.inverted()
+
         if len(intersection_points) > 0:
             # make sure only unique pairs of coordinates are used
             # pts = np.unique(np.rec.fromarrays(pts)).view((pts.dtype, 2)).T
             for i, (label, pts) in enumerate(intersection_points.items()):
                 # TODO currently we take only the first 2 points
                 # to avoid issues with 180° lines etc.
                 for (x, y, r) in pts[self._n_pts]:
@@ -804,29 +835,38 @@
                         uselabel = label
                     else:
                         # use the provided labels (keep existing if None)
                         uselabel = self._labels[i]
                         if uselabel is None:
                             uselabel = label
 
+                    # route positions through dpi_scale_trans to avoid wrong positioning
+                    # on figure export with different dpi since (x, y) are in
+                    # display-coordinates!
+                    x, y = transf_inv.transform((x, y))
                     t = m.ax.text(
                         x,
                         y,
                         uselabel,
-                        transform=None,  # None is the same as using IdentityTransform()
+                        transform=transf,  # None,
                         animated=True,
                         rotation=r,
                         ha="center",
                         va="center",
                         **txt_kwargs,
                     )
-                    m.BM.add_bg_artist(t, layer=self._g.layer)
+                    # exclude artist in companion widget editor
+                    t.set_label("__EOmaps_exclude")
+                    m.BM.add_bg_artist(t, layer=self._g.layer, draw=False)
                     self._texts.append(t)
 
     def add_labels(self):
+        """
+        Add labels to the grid.
+        """
         m = self._g.m
         lines = self._g._get_lines()
         aspect = m.ax.bbox.height / m.ax.bbox.width
 
         if self._where == "all":
             use_axes = (0, 1)
         else:
@@ -837,28 +877,31 @@
                 use_axes.append(1)
 
         for axis in use_axes:
             self._add_axis_labels(lines=lines, axis=axis)
 
 
 class GridFactory:
+    """Class to handle grids on a map."""
+
     def __init__(self, m):
         self.m = m
         self._gridlines = []
         self.m.BM._before_fetch_bg_actions.append(self._update_autogrid)
 
     def add_grid(
         self,
         d=None,
         auto_n=10,
         n=100,
         bounds=None,
         layer=None,
         *,
         m=None,
+        labels=False,
         **kwargs,
     ):
         """
         Add gridlines to the map.
 
         By default, an appropriate grid-spacing is determined via the "auto_n" kwarg.
 
@@ -897,14 +940,24 @@
             A tuple of boundaries to limit the gridlines to a given extent.
             (lon_min, lon_max, lat_min, lat_max)
             The default is None in which case (-180, 180, -90, 90) is used.
         n : int
             The number of intermediate points to draw for each line.
             (e.g. to nicely draw curved grid lines)
             The default is 100
+        labels : bool or dict, optional
+            If True, add grid-labels to the map.
+            If a dict is provided, it is passed to :py:meth:`GridLines.add_labels`.
+
+            This is a shortcut for using:
+
+            >>> g = m.add_gridlines()
+            >>> g.add_labels(fontsize=7, color="b", ...)
+
+            The default is False.
         kwargs :
             Additional kwargs passed to matplotlib.collections.LineCollection.
 
             The default is: (ec="0.2", lw=0.5, zorder=100)
 
         Returns
         -------
@@ -938,14 +991,23 @@
         kwargs.setdefault("lw", lw)
         kwargs.setdefault("zorder", 100)
 
         g = GridLines(m=m, d=d, auto_n=auto_n, n=n, bounds=bounds, layer=layer)
         g._add_grid(**kwargs)
         self._gridlines.append(g)
 
+        if labels:
+            if labels is True:
+                g.add_labels()
+            elif isinstance(labels, dict):
+                g.add_labels(**labels)
+            else:
+                raise TypeError(f"{labels} is not a valid input for labels")
+
+        self.m.f.canvas.draw_idle()
         return g
 
     def _update_autogrid(self, *args, **kwargs):
         for g in self._gridlines:
             if g.d is None:
                 try:
                     g._redraw()
```

### Comparing `EOmaps-6.5/eomaps/helpers.py` & `EOmaps-7.0/eomaps/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,71 @@
 """a collection of useful helper-functions."""
+
+import logging
 from itertools import tee
 import re
 import sys
 from itertools import chain
 from contextlib import contextmanager, ExitStack
+from importlib import import_module
 from textwrap import indent, dedent
-from functools import wraps
+from functools import wraps, lru_cache
 from pathlib import Path
 import json
 import warnings
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.lines import Line2D
 from matplotlib.colors import LinearSegmentedColormap, ListedColormap
 from matplotlib.transforms import Bbox, TransformedBbox
 from matplotlib.axis import XAxis, YAxis
 from matplotlib.spines import Spine
-from matplotlib.text import Text
+
+_log = logging.getLogger(__name__)
+
+
+def _deprecated(message):
+    def deprecated_decorator(func):
+        def deprecated_func(*args, **kwargs):
+            warnings.warn(
+                f"EOmaps: '{func.__name__}' is deprecated and will be removed "
+                f"in upcoming releases. {message}",
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            warnings.simplefilter("default", DeprecationWarning)
+
+            return func(*args, **kwargs)
+
+        return deprecated_func
+
+    return deprecated_decorator
+
+
+@lru_cache()
+def _do_import_module(name):
+    return import_module(name)
+
+
+def register_modules(*names, raise_exception=True):
+    """Lazy-loading for optional dependencies."""
+    modules = []
+    for name in names:
+        try:
+            modules.append(_do_import_module(name))
+        except ImportError as ex:
+            if raise_exception:
+                raise ImportError(
+                    f"EOmaps: Missing required dependency: {name} \n {ex}"
+                )
+            else:
+                modules.append(None)
+    return modules
+
 
 # class copied from matplotlib.axes
 class _TransformedBoundsLocator:
     """
     Axes locator for `.Axes.inset_axes` and similarly positioned Axes.
     The locator is a callable object used in `.Axes.set_aspect` to compute the
     Axes location depending on the renderer.
@@ -107,14 +151,34 @@
 
     return new_cmap
 
 
 # a simple progressbar
 # taken from https://stackoverflow.com/a/34482761/9703451
 def progressbar(it, prefix="", size=60, file=sys.stdout):
+    """
+    A (very) simple progressbar generator.
+
+    Parameters
+    ----------
+    it : iter
+        The iterator for which a progressbr should be shown.
+    prefix : str, optional
+        Prefix for the output. The default is "".
+    size : int, optional
+        The size of the progressbar (in characters). The default is 60.
+    file : filehandle, optional
+        The file-handle to write to. The default is sys.stdout.
+
+    Yields
+    ------
+    item :
+        Consecutive items from the iterator.
+
+    """
     count = len(it)
 
     def show(j):
         x = int(size * j / count)
         file.write("\r%s[%s%s] %i/%i\r" % (prefix, "#" * x, "." * (size - x), j, count))
         file.flush()
 
@@ -177,49 +241,51 @@
                         docsplit = (
                             docsplit[: (paramline + offset)]
                             + indent(val, " " * nspaces).split("\n")
                             + docsplit[(paramline + offset) :]
                         )
                         doc = "\n".join(docsplit)
                     except ValueError:
-                        print(f"EOmaps: Unable to update docstring for {f.__name__}")
+                        _log.debug(
+                            f"EOmaps: Unable to update docstring for {f.__name__}"
+                        )
 
             if prefix is not None:
                 doc = prefix + "\n" + doc
             if suffix is not None:
                 doc = doc + "\n" + suffix
 
             inner.__doc__ = doc
             return inner
         except Exception:
-            print(f"EOmaps: Unable to update docstring for {f.__name__}")
+            _log.debug(f"EOmaps: Unable to update docstring for {f.__name__}")
             return f
 
     return decorator
 
 
-class searchtree:
+class SearchTree:
+    """Class to perform fast nearest-neighbour queries."""
+
     def __init__(self, m):
         """
-        Nearest-neighbour search.
+        Class to perform fast nearest-neighbour queries.
 
         Parameters
         ----------
         m : eomaps.Maps
             The maps-object that provides the data.
         """
         self._m = m
         # set starting pick-distance to 50 times the radius
         self.set_search_radius("50")
 
-        self._misses = 0
-
     @property
     def d(self):
-        """Side-length of the search-rectangle (in units of the plot-crs)"""
+        """Side-length of the search-rectangle (in units of the plot-crs)."""
         return self._d
 
     def set_search_radius(self, r):
         """
         Set the rectangle side-length that is used to limit the query.
 
         (e.g. only points that are within a rectangle of the specified size
@@ -235,32 +301,36 @@
               The radius of the circle in units of the plot_crs
             - if `str`:
               A multiplication-factor for the estimated pixel-radius.
               (e.g. a circle with (`r=search_radius * m.shape.radius`) is
               used if possible and else np.inf is used.
 
             The default is "50" (e.g. 50 times the pixel-radius).
-        """
 
+        """
         self._search_radius = r
-
         if isinstance(r, str):
             # evaluate an appropriate pick-distance
-            if getattr(self._m.shape, "radius_crs", None) != "out":
+            if getattr(self._m.shape, "radius_crs", None) == "out":
+                radius = self._m.shape.radius
+            else:
                 try:
-                    radius = self._m.set_shape._estimate_radius(self._m, "out", np.max)
+                    if self._m.get_crs("in") == self._m.get_crs(self._m._crs_plot):
+                        radius = self._m.shape.radius
+                    else:
+                        radius = self._m.set_shape._estimate_radius(
+                            self._m, "out", np.max
+                        )
                 except AssertionError:
-                    print(
+                    _log.error(
                         "EOmaps: Unable to estimate search-radius based on data."
                         "Defaulting to `np.inf`. "
                         "See `m.cb.pick.set_props(search_radius=...)` for more details!"
                     )
                     radius = [np.inf]
-            else:
-                radius = self._m.shape.radius
 
             self._d = np.max(radius) * float(self._search_radius)
         elif isinstance(r, (int, float, np.number)):
             self._d = float(r)
         else:
             raise TypeError(
                 f"EOmaps: {r} is not a valid search-radius. "
@@ -434,39 +504,22 @@
                     )
                 i = idx[
                     ((x_rect - x[0]) ** 2 + (y_rect - x[1]) ** 2).argpartition(
                         range(min(k, x_rect.size))
                     )[:k]
                 ]
         else:
-            # show a warning if no points are found in the search area
-            if self._misses < 3:
-                self._misses += 1
-            else:
-                text = "Found no data here...\n Increase search_radius?"
-                # TODO fix cleanup of temporary artists!!
-                self._m.add_annotation(
-                    xy=x,
-                    permanent=False,
-                    text=text,
-                    xytext=(0.98, 0.98),
-                    textcoords=self._m.ax.transAxes,
-                    horizontalalignment="right",
-                    verticalalignment="top",
-                    arrowprops=None,
-                    fontsize=7,
-                    bbox=dict(ec="r", fc=(1, 0.9, 0.9, 0.5), lw=0.25, boxstyle="round"),
-                )
-
             i = None
 
         return i
 
 
 class LayoutEditor:
+    """Class to handle interactive re-positioning of figure-objects."""
+
     def __init__(self, m, modifier="alt+d", cb_modifier="control"):
         self.modifier = modifier
         self.cb_modifier = cb_modifier
 
         self.m = m
         self.f = self.m.parent.f
 
@@ -478,14 +531,15 @@
 
         self.cids = []
 
         # indicator if the pick-callback should be re-attached or not
         self._reattach_pick_cb = False
 
         self.f.canvas.mpl_connect("key_press_event", self.cb_key_press)
+        self.f.canvas.mpl_connect("resize_event", self._on_resize)
 
         # the snap-to-grid interval (0 means no snapping)
         self._snap_id = 5
 
         # an optional filepath that will be used to store the layout once the
         # editor exits
         self._filepath = None
@@ -496,14 +550,63 @@
         # indicator if multiple-axis select key is pressed or not (e.g. "shift")
         self._shift_pressed = False
 
         self._max_hist_steps = 1000
         self._history = list()
         self._history_undone = list()
 
+        self._current_bg = None
+
+        self._info_text = None
+        self._info_text_hidden = False
+
+    def add_info_text(self):
+        self._info_text_hidden = False
+
+        a = self.m.f.text(
+            0.72,
+            0.98,
+            (
+                "LayoutEditor Controls:\n\n"
+                "0 - 9:  Snap-grid spacing\n"
+                "SHIFT:  Multi-select\n"
+                "P:      Print to console\n"
+                "ESCAPE (or ALT + L): Exit\n"
+                "\n"
+                "ARROW-KEYS:   Move\n"
+                "SCROLL (+/-): Resize\n"
+                "  H:    horizontal\n"
+                "  V:    vertical\n"
+                "  ctrl: histogram"
+                "\n\n(right-click to hide info)"
+            ),
+            transform=self.m.f.transFigure,
+            ha="left",
+            va="top",
+            fontsize=min(self.m.f.bbox.width * 72 / self.m.f.dpi / 60, 12),
+            bbox=dict(
+                boxstyle="round", facecolor=".8", edgecolor="k", lw=0.5, alpha=0.9
+            ),
+            zorder=1e6,
+            fontfamily="monospace",
+        )
+        return a
+
+    def _update_info_text(self):
+        if getattr(self, "_info_text", None) is not None:
+            self._info_text.set_fontsize(
+                min(self.m.f.bbox.width * 72 / self.m.f.dpi / 60, 15)
+            )
+
+    def _on_resize(self, *args, **kwargs):
+        # update snap-grid on resize
+        if self.modifier_pressed:
+            self._add_snap_grid()
+            self._update_info_text()
+
     @property
     def modifier_pressed(self):
         return self._modifier_pressed
 
     @modifier_pressed.setter
     def modifier_pressed(self, val):
         self._modifier_pressed = val
@@ -690,35 +793,48 @@
             l = self._history_undone.pop(-1)
             self._history.append(l)
             self.m.apply_layout(l)
             self.m.redraw()
 
     def cb_release(self, event):
         self._set_startpos(event)
-        self._remove_snap_grid()
 
     def cb_pick(self, event):
         if not self.modifier_pressed:
             return
         if (self.f.canvas.toolbar is not None) and self.f.canvas.toolbar.mode != "":
             return False
 
+        # toggle info-text visibility on left-click
+        if event.button == 3:
+            if getattr(self, "_info_text", None) is not None:
+                vis = not self._info_text.get_visible()
+                self._info_text.set_visible(vis)
+                self._info_text_hidden = not vis
+
         eventax = event.inaxes
 
         if eventax not in self.axes:
             # if no axes is clicked "unpick" previously picked axes
             if len(self._ax_picked) + len(self._cb_picked) == 0:
-                # if there was nothing picked there's nothing to do...
+                # if there was nothing picked there's nothing to do
+                # except updating the info-text visibility
+
+                if getattr(self, "_info_text", None) is not None:
+                    self.blit_artists()
+
                 return
 
             self._ax_picked = []
             self._cb_picked = []
             self._m_picked = []
             self._color_axes()
-            self.m.redraw()
+            self._remove_snap_grid()
+            self.fetch_current_background()
+            self.blit_artists()
             return
 
         if self._shift_pressed:
             if eventax in self.maxes:
                 m = self.ms[self.maxes.index(eventax)]
                 if eventax in self._ax_picked:
                     self._ax_picked.remove(eventax)
@@ -759,22 +875,44 @@
                     elif eventax in self.cbaxes:
                         self._cb_picked.append(self.cbs[self.cbaxes.index(eventax)])
                     else:
                         self._m_picked = []
                         self._cb_picked = []
                         self._ax_picked.append(eventax)
 
-                    self._show_snap_grid()
+                    self._add_snap_grid()
 
             else:
-                self._show_snap_grid()
+                self._add_snap_grid()
 
-        self._color_axes()
         self._set_startpos(event)
-        self.m.redraw()
+        self._color_axes()
+        self.fetch_current_background()
+        self.blit_artists()
+
+    def fetch_current_background(self):
+        # make sure blank background has been fetched
+        self.m.BM._do_fetch_blank()
+
+        with ExitStack() as stack:
+            for ax in self._ax_picked:
+                stack.enter_context(ax._cm_set(visible=False))
+
+            for cb in self._cb_picked:
+                stack.enter_context(cb.ax_cb._cm_set(visible=False))
+                stack.enter_context(cb.ax_cb_plot._cm_set(visible=False))
+
+            self.m.BM.blit_artists(self.axes, self.m.BM._blank_bg, False)
+
+            grid = getattr(self, "_snap_grid_artist", None)
+            if grid is not None:
+                self.m.BM.blit_artists([grid], None, False)
+
+            self.m.BM.canvas.blit()
+            self._current_bg = self.m.BM.canvas.copy_from_bbox(self.m.f.bbox)
 
     def cb_move_with_key(self, event):
         if not self.modifier_pressed:
             return
         if (self.f.canvas.toolbar is not None) and self.f.canvas.toolbar.mode != "":
             return False
 
@@ -785,17 +923,17 @@
             bbox = self._get_move_with_key_bbox(ax, event.key)
             ax.set_position(bbox)
 
         for cb in self._cb_picked:
             bbox = self._get_move_with_key_bbox(cb._ax, event.key)
             cb.set_position(bbox)
 
-        self._color_axes()
-        self.m.redraw()
         self._add_to_history()
+        self._color_axes()
+        self.blit_artists()
 
     def cb_move(self, event):
         if (self.f.canvas.toolbar is not None) and self.f.canvas.toolbar.mode != "":
             return False
         if self.modifier is not None:
             if not self.modifier_pressed:
                 return False
@@ -813,16 +951,28 @@
         for cb in self._cb_picked:
             if cb is None:
                 return
 
             bbox = self._get_move_bbox(cb._ax, event.x, event.y)
             cb.set_position(bbox)
 
-        self.m.redraw()
         self._add_to_history()
+        self._color_axes()
+        self.blit_artists()
+
+    def blit_artists(self):
+        artists = [*self._ax_picked]
+        for cb in self._cb_picked:
+            artists.append(cb.ax_cb)
+            artists.append(cb.ax_cb_plot)
+
+        if getattr(self, "_info_text", None) is not None:
+            artists.append(self._info_text)
+
+        self.m.BM.blit_artists(artists, self._current_bg)
 
     def cb_scroll(self, event):
         if (self.f.canvas.toolbar is not None) and self.f.canvas.toolbar.mode != "":
             return False
         if self.modifier is not None:
             if not self.modifier_pressed:
                 return False
@@ -846,33 +996,37 @@
                 new_size = np.clip(start_size + event.step * 0.02, 0.0, 1.0)
                 cb.set_hist_size(new_size)
             else:
                 resize_bbox = self._get_resize_bbox(cb._ax, event.step)
                 if resize_bbox is not None:
                     cb.set_position(resize_bbox)
 
-        self._color_axes()
-        self.m.redraw()
         self._add_to_history()
+        # self._color_axes()
+        self.blit_artists()
 
     def cb_key_press(self, event):
         # release shift key on every keypress
         self._shift_pressed = False
 
-        if (self.f.canvas.toolbar is not None) and self.f.canvas.toolbar.mode != "":
-            return False
-
         if (event.key == self.modifier) and (not self.modifier_pressed):
             self._make_draggable()
             return
         elif (event.key == self.modifier or event.key == "escape") and (
             self.modifier_pressed
         ):
             self._undo_draggable()
             return
+        elif (event.key.lower() == "p") and (self.modifier_pressed):
+            s = "\nlayout = {\n    "
+            s += "\n    ".join(
+                f'"{key}": {val},' for key, val in self.get_layout().items()
+            )
+            s += "\n}\n"
+            print(s)
         elif (event.key.lower() == "q") and (self.modifier_pressed):
             print(
                 "\n##########################\n\n"
                 "EOmaps Layout Editor controls:\n\n"
                 "Click on axes to select them for editing.\n"
                 "(Hold 'shift' while clicking on axes to select multiple axes.)\n\n"
                 "Drag selected axes with the mouse or use the 'arrow-keys' to "
@@ -911,15 +1065,17 @@
 
         elif event.key == "shift":
             self._shift_pressed = True
 
         # assign snaps with keys 0-9
         if event.key in map(str, range(10)):
             self._snap_id = int(event.key)
-            self._show_snap_grid()
+            self._add_snap_grid()
+            self.fetch_current_background()
+            self.blit_artists()
 
         # assign snaps with keys 0-9
         if event.key in ["+", "-", "ctrl++", "ctrl+-"]:
 
             class dummyevent:
                 pass
 
@@ -945,17 +1101,32 @@
             n = (self.f.bbox.width / 400) * (self._snap_id)
 
             snap = (n, n)
 
         return snap
 
     def _make_draggable(self, filepath=None):
+        # Uncheck avtive pan/zoom actions of the matplotlib toolbar.
+        # use a try-except block to avoid issues with ipympl in jupyter notebooks
+        # (see https://github.com/matplotlib/ipympl/issues/530#issue-1780919042)
+        try:
+            toolbar = getattr(self.m.BM.canvas, "toolbar", None)
+            if toolbar is not None:
+                for key in ["pan", "zoom"]:
+                    val = toolbar._actions.get(key, None)
+                    if val is not None and val.isCheckable() and val.isChecked():
+                        val.trigger()
+        except AttributeError:
+            pass
+
         self._filepath = filepath
         self.modifier_pressed = True
-        print("EOmaps: Layout Editor activated! (press 'esc' to exit and 'q' for info)")
+        _log.info(
+            "EOmaps: Layout Editor activated! (press 'esc' to exit " "and 'q' for info)"
+        )
 
         self._history.clear()
         self._history_undone.clear()
         self._add_to_history()
 
         self._revert_props = []
         for ax in self.f.axes:
@@ -984,87 +1155,110 @@
             if not singularax:
                 ax.set_visible(True)
 
             ax.set_animated(False)
             ax.set_frame_on(True)
 
             for child in ax.get_children():
-                for prop in [
-                    "facecolor",
+                revert_props = [
                     "edgecolor",
                     "linewidth",
                     "linestyle",
                     "alpha",
                     "animated",
                     "visible",
-                ]:
-                    if hasattr(child, f"set_{prop}") and hasattr(child, f"get_{prop}"):
-                        self._revert_props.append(
-                            (
-                                getattr(child, f"set_{prop}"),
-                                getattr(child, f"get_{prop}")(),
-                            )
-                        )
+                ]
+                self._add_revert_props(child, *revert_props)
 
                 if isinstance(child, Spine) and not cbaxQ:
                     # make sure spines are visible (and re-drawn on draw)
                     child.set_animated(False)
                     child.set_visible(True)
+
                 elif (
                     ax not in self.maxes
                     and showXY
                     and isinstance(child, (XAxis, YAxis))
                 ):
                     # keep all tick labels etc. of normal axes and colorbars visible
                     child.set_animated(False)
                     child.set_visible(True)
+
                 elif child is ax.patch and not cbaxQ:
+                    # only reset facecolors for axes-patches to avoid issues with
+                    # black spines (TODO check why this happens!)
+                    self._add_revert_props(child, "facecolor")
+
                     # make sure patches are visible (and re-drawn on draw)
                     child.set_visible(True)
                     child.set_facecolor("w")
                     child.set_alpha(0.75)  # for overlapping axes
+
                 else:
                     # make all other childs invisible (to avoid drawing them)
                     child.set_visible(False)
                     child.set_animated(True)
 
+        # only re-draw if info-text is None
+        if getattr(self, "_info_text", None) is None:
+            self._info_text = self.add_info_text()
+
         self._color_axes()
         self._attach_callbacks()
+
+        self.m._emit_signal("layoutEditorActivated")
+
         self.m.redraw()
 
+    def _add_revert_props(self, child, *args):
+        for prop in args:
+            if hasattr(child, f"set_{prop}") and hasattr(child, f"get_{prop}"):
+                self._revert_props.append(
+                    (
+                        getattr(child, f"set_{prop}"),
+                        getattr(child, f"get_{prop}")(),
+                    )
+                )
+
     def _undo_draggable(self):
+        if getattr(self, "_info_text", None) not in (None, False):
+            self._info_text.remove()
+            # set to None to avoid crating the info-text again
+            self._info_text = None
 
         self._history.clear()
         self._history_undone.clear()
 
         toolbar = getattr(self.m.f, "toolbar", None)
         if toolbar is not None:
             # Reset the axes stack to make sure the "home" "back" and "forward" buttons
             # of the toolbar do not reset axis positions
             # see "matplotlib.backend_bases.NavigationToolbar2.update"
             if hasattr(toolbar, "update"):
                 try:
                     toolbar.update()
                 except Exception:
-                    print("EOmaps: Error while trying to reset the axes stack!")
+                    _log.exception(
+                        "EOmaps: Error while trying to reset the axes stack!"
+                    )
 
         # clear all picks on exit
         self._ax_picked = []
         self._cb_picked = []
         self._m_picked = []
 
-        print("EOmaps: Exiting layout-editor mode...")
+        _log.info("EOmaps: Exiting layout-editor mode...")
 
         # in case a filepath was provided, save the new layout
         if self._filepath:
             try:
                 self.m.get_layout(filepath=self._filepath, override=True)
             except Exception:
-                print(
-                    "EOmaps WARNING: The layout could not be saved to the provided "
+                _log.exception(
+                    "EOmaps: Layout could not be saved to the provided "
                     + f"filepath: '{self._filepath}'."
                 )
 
         self._reset_callbacks()
         # revert all changes to artists
         for p in self._revert_props:
             if isinstance(p, tuple):
@@ -1076,14 +1270,19 @@
 
         # reset the histogram-size of all colorbars to make sure previously hidden
         # axes (e.g. size=0) become visible if the size is now > 0.
         for m in self.ms:
             for cb in m._colorbars:
                 cb.set_hist_size()
 
+        # remove snap-grid (if it's still visible)
+        self._remove_snap_grid()
+
+        self.m._emit_signal("layoutEditorDeactivated")
+
         self.m.redraw()
 
     def _reset_callbacks(self):
         # disconnect all callbacks of the layout-editor
         while len(self.cids) > 0:
             cid = self.cids.pop(-1)
             self.f.canvas.mpl_disconnect(cid)
@@ -1100,15 +1299,15 @@
             ("key_press_event", self.cb_move_with_key),
             ("key_release_event", self.cb_key_release),
         )
 
         for event, cb in events:
             self.cids.append(self.f.canvas.mpl_connect(event, cb))
 
-    def _show_snap_grid(self, snap=None):
+    def _add_snap_grid(self, snap=None):
         # snap = (snapx, snapy)
 
         if snap is None:
             if self._snap_id == 0:
                 self._remove_snap_grid()
                 return
             else:
@@ -1127,30 +1326,25 @@
         ]
         g = t.transform(np.column_stack((gx.flat, gy.flat)))
 
         l = Line2D(
             *g.T,
             lw=0,
             marker=".",
-            markerfacecolor="k",
+            markerfacecolor="steelblue",
             markeredgecolor="none",
             ms=(snapx + snapy) / 6,
         )
         self._snap_grid_artist = self.m.f.add_artist(l)
 
-        self.f.draw_artist(self._snap_grid_artist)
-        self.f.canvas.blit()
-
     def _remove_snap_grid(self):
         if hasattr(self, "_snap_grid_artist"):
             self._snap_grid_artist.remove()
             del self._snap_grid_artist
 
-        self.m.redraw()
-
     def get_layout(self, filepath=None, override=False, precision=5):
         """
         Get the positions of all axes within the current plot.
 
         To re-apply a layout, use:
 
             >>> l = m.get_layout()
@@ -1220,15 +1414,15 @@
         if filepath is not None:
             filepath = Path(filepath)
             assert (
                 not filepath.exists() or override
             ), f"The file {filepath} already exists! Use override=True to relace it."
             with open(filepath, "w") as file:
                 json.dump(layout, file)
-            print("EOmaps: Layout saved to:\n       ", filepath)
+            _log.info(f"EOmaps: Layout saved to:\n       {filepath}")
 
         return layout
 
     def apply_layout(self, layout):
         """
         Set the positions of all axes within the current plot based on a previously
         defined layout.
@@ -1297,44 +1491,51 @@
                 axes[i].set_position(val)
 
         self.m.redraw()
 
 
 # taken from https://matplotlib.org/stable/tutorials/advanced/blitting.html#class-based-example
 class BlitManager:
+    """Manager used to schedule draw events, cache backgrounds, etc."""
+
+    _snapshot_on_update = None
+
     def __init__(self, m):
         """
+        Manager used to schedule draw events, cache backgrounds, etc.
+
         Parameters
         ----------
         canvas : FigureCanvasAgg
             The canvas to work with, this only works for sub-classes of the Agg
             canvas which have the `~FigureCanvasAgg.copy_from_bbox` and
             `~FigureCanvasAgg.restore_region` methods.
 
         animated_artists : Iterable[Artist]
             List of the artists to manage
-        """
 
+        """
         self._m = m
 
-        self._bg = None
         self._artists = dict()
 
         self._bg_artists = dict()
         self._bg_layers = dict()
 
+        self._pending_webmaps = dict()
+
         # the name of the layer at which all "unmanaged" artists are drawn
         self._unmanaged_artists_layer = "base"
 
         # grab the background on every draw
         self.cid = self.canvas.mpl_connect("draw_event", self.on_draw)
 
         self._after_update_actions = []
         self._after_restore_actions = []
-        self._bg_layer = 0
+        self._bg_layer = "base"
 
         self._artists_to_clear = dict()
 
         self._hidden_artists = set()
 
         self._refetch_bg = True
         self._layers_to_refetch = set()
@@ -1365,14 +1566,30 @@
         self._refetch_blank = True
         self._blank_bg = None
 
         self._managed_axes = set()
 
         self._clear_on_layer_change = False
 
+        self._on_layer_change_running = False
+
+    def _get_renderer(self):
+        # don't return the renderer if the figure is saved.
+        # in this case the normal draw-routines are used (see m.savefig) so there is
+        # no need to trigger updates (also `canvas.get_renderer` is undefined for
+        # pdf/svg exports since those canvas do not expose the renderer)
+        # ... this is required to support vektor format outputs!
+        if self.canvas.is_saving():
+            return None
+
+        try:
+            return self.canvas.get_renderer()
+        except Exception:
+            return None
+
     def _get_all_map_axes(self):
         maxes = {
             m.ax for m in (self._m.parent, *self._m.parent._children) if m._new_axis_map
         }
         return maxes
 
     def _get_managed_axes(self):
@@ -1387,65 +1604,87 @@
         allaxes = set(self._m.f.axes)
 
         unmanaged_axes = allaxes.difference(managed_axes)
         return unmanaged_axes
 
     @property
     def figure(self):
+        """The matplotlib figure instance."""
         return self._m.f
 
     @property
     def canvas(self):
+        """The figure canvas instance."""
         return self.figure.canvas
 
+    @contextmanager
+    def _cx_on_layer_change_running(self):
+        # a context-manager to avoid recursive on_layer_change calls
+        try:
+            self._on_layer_change_running = True
+            yield
+        finally:
+            self._on_layer_change_running = False
+
     def _do_on_layer_change(self, layer, new=False):
+        # avoid recursive calls to "_do_on_layer_change"
+        # This is required in case the executed functions trigger actions that would
+        # trigger "_do_on_layer_change" again which can result in a mixed-up order of
+        # the scheduled functions.
+        if self._on_layer_change_running is True:
+            return
+
         # do not execute layer-change callbacks on private layer activation!
         if layer.startswith("__"):
             return
 
-        # only execute persistent layer-change callbacks if the layer changed!
-        if new:
-            # general callbacks executed on any layer change
-            # persistent callbacks
-            for f in self._on_layer_change[True]:
-                f(layer=layer)
-
-        # single-shot callbacks
-        # (execute also if the layer is already active)
-        while len(self._on_layer_change[False]) > 0:
-            try:
-                f = self._on_layer_change[False].pop(-1)
-                f(layer=layer)
-            except Exception as ex:
-                print(
-                    "EOmaps: there was an issue while trying to execute a "
-                    f"layer-change action: {ex}"
-                )
-
-        if new:
-            for l in layer.split("|"):
-                # individual callables executed if a specific layer is activate
+        with self._cx_on_layer_change_running():
+            # only execute persistent layer-change callbacks if the layer changed!
+            if new:
+                # general callbacks executed on any layer change
                 # persistent callbacks
-                for f in self._on_layer_activation[True].get(layer, []):
-                    f(layer=l)
+                for f in reversed(self._on_layer_change[True]):
+                    f(layer=layer)
 
-        for l in layer.split("|"):
             # single-shot callbacks
-            single_shot_funcs = self._on_layer_activation[False].get(l, [])
-            while len(single_shot_funcs) > 0:
+            # (execute also if the layer is already active)
+            while len(self._on_layer_change[False]) > 0:
                 try:
-                    f = single_shot_funcs.pop(-1)
-                    f(layer=l)
+                    f = self._on_layer_change[False].pop(0)
+                    f(layer=layer)
                 except Exception as ex:
-                    raise (ex)
-                    print(
-                        "EOmaps: there was an issue while trying to execute a "
-                        f"layer-change action: {ex}"
+                    _log.error(
+                        "EOmaps: Issue while executing a layer-change action",
+                        exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
                     )
 
+            if new:
+                for l in layer.split("|"):
+                    # individual callables executed if a specific layer is activate
+                    # persistent callbacks
+                    for f in reversed(self._on_layer_activation[True].get(layer, [])):
+                        f(layer=l)
+
+            for l in layer.split("|"):
+                # single-shot callbacks
+                single_shot_funcs = self._on_layer_activation[False].get(l, [])
+                while len(single_shot_funcs) > 0:
+                    try:
+                        f = single_shot_funcs.pop(0)
+                        f(layer=l)
+                    except Exception as ex:
+                        _log.error(
+                            "EOmaps: Issue while executing a layer-change action",
+                            exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+                        )
+
+            # clear the list of pending webmaps once the layer has been activated
+            if layer in self._pending_webmaps:
+                self._pending_webmaps.pop(layer)
+
     @contextmanager
     def _without_artists(self, artists=None, layer=None):
         try:
             removed_artists = {layer: set(), "all": set()}
             if artists is None:
                 yield
             else:
@@ -1479,14 +1718,15 @@
                     )
                 bg = self.canvas.copy_from_bbox(self.figure.bbox)
 
         return bg
 
     @property
     def bg_layer(self):
+        """The currently visible layer-name."""
         return self._bg_layer
 
     @bg_layer.setter
     def bg_layer(self, val):
         if val == self._bg_layer:
             # in case the layer did not change, do nothing
             return
@@ -1551,29 +1791,32 @@
 
         Parameters
         ----------
         func : callable
             The callable to use.
             The call-signature is:
 
-            >>> def func(m, l):
-            >>>    # m... the Maps-object
-            >>>    # l... the name of the layer
+            >>> def func(m, layer):
+            >>>    # m     ... the Maps-object
+            >>>    # layer ... the name of the layer
 
 
         layer : str or None, optional
             - If str: The function will only be called if the specified layer is
               activated.
             - If None: The function will be called on any layer-change.
 
             The default is None.
         persistent : bool, optional
             Indicator if the function should be called only once (False) or if it
             should be called whenever a layer is activated.
             The default is False.
+        m : eomaps.Maps
+            The Maps-object to pass as argument to the function execution.
+            If None, the parent Maps-object is used.
 
         """
         if m is None:
             m = self._m
 
         def cb(*args, **kwargs):
             func(m=m, *args, **kwargs)
@@ -1604,14 +1847,29 @@
             else:
                 sortp.append(0)
 
         sortp.append(getattr(art, "zorder", -1))
         return sortp
 
     def get_bg_artists(self, layer):
+        """
+        Get all (sorted) background artists assigned to a given layer-name.
+
+        Parameters
+        ----------
+        layer : str
+            The layer name for which artists should be fetched.
+
+        Returns
+        -------
+        artists : list
+            A list of artists on the specified layer, sorted with respect to the
+            vertical stacking (layer-order / zorder).
+
+        """
         artists = list()
         for l in np.atleast_1d(layer):
             # get all relevant artists for combined background layers
             l = str(l)  # w make sure we convert non-string layer names to string!
 
             # get artists defined on the layer itself
             # Note: it's possible to create explicit multi-layers and attach
@@ -1624,71 +1882,141 @@
         # make the list unique but maintain order (dicts keep order for python>3.7)
         artists = dict.fromkeys(artists)
         # sort artists by zorder (respecting inset-map priority)
         artists = sorted(artists, key=self._bg_artists_sort)
 
         return artists
 
-    def _combine_bgs(self, layer):
+    def get_artists(self, layer):
+        """
+        Get all (sorted) dynamically updated artists assigned to a given layer-name.
+
+        Parameters
+        ----------
+        layer : str
+            The layer name for which artists should be fetched.
+
+        Returns
+        -------
+        artists : list
+            A list of artists on the specified layer, sorted with respect to the
+            vertical stacking (layer-order / zorder).
+
+        """
+
+        artists = list()
+        for l in np.atleast_1d(layer):
+            # get all relevant artists for combined background layers
+            l = str(l)  # w make sure we convert non-string layer names to string!
+
+            # get artists defined on the layer itself
+            # Note: it's possible to create explicit multi-layers and attach
+            # artists that are only visible if both layers are visible! (e.g. "l1|l2")
+            artists.extend(self._artists.get(l, []))
+
+        # make the list unique but maintain order (dicts keep order for python>3.7)
+        artists = dict.fromkeys(artists)
+        # sort artists by zorder (respecting inset-map priority)
+        artists = sorted(artists, key=self._bg_artists_sort)
+
+        return artists
+
+    def _get_layers_alphas(self, layer=None):
+        if layer is None:
+            layer = self.bg_layer
+
         layers, alphas = [], []
         for l in layer.split("|"):
             if l.endswith("}") and "{" in l:
                 try:
-                    name, a = l.split("{")
+                    name, a = l.split("{", maxsplit=1)
                     a = float(a.replace("}", ""))
 
                     layers.append(name)
                     alphas.append(a)
                 except Exception:
                     raise TypeError(
                         "EOmaps: unable to parse multilayer-transparency " f"for '{l}'"
                     )
             else:
                 layers.append(l)
                 alphas.append(1)
+        return layers, alphas
+
+    def _combine_bgs(self, layer):
+        layers, alphas = self._get_layers_alphas(layer)
 
         # make sure all layers are already fetched
         for l in layers:
             if l not in self._bg_layers:
                 # execute actions on layer-changes
                 # (to make sure all lazy WMS services are properly added)
                 self._do_on_layer_change(layer=l, new=False)
                 self._do_fetch_bg(l)
 
-        gc = self.canvas.renderer.new_gc()
-        gc.set_clip_rectangle(self.canvas.figure.bbox)
-
-        # switch to a blank background layer before merging backgrounds
-        # TODO is there a beter way to avoid drawing on initial backgrounds?
-        self.canvas.restore_region(self._blank_bg)
+        renderer = self._get_renderer()
+        if renderer:
+            gc = renderer.new_gc()
+            gc.set_clip_rectangle(self.canvas.figure.bbox)
 
-        x0, y0, w, h = self.figure.bbox.bounds
-        for l, a in zip(layers, alphas):
+            # switch to a blank background layer before merging backgrounds
+            # TODO is there a beter way to avoid drawing on initial backgrounds?
+            self.canvas.restore_region(self._blank_bg)
 
-            rgba = self._get_array(l, a=a)
-            self.canvas.renderer.draw_image(
-                gc,
-                int(x0),
-                int(y0),
-                rgba[int(y0) : int(y0 + h), int(x0) : int(x0 + w), :],
-            )
-        # cache the combined background
-        self._bg_layers[layer] = self._m.f.canvas.copy_from_bbox(self._m.f.bbox)
-        gc.restore()
+            x0, y0, w, h = self.figure.bbox.bounds
+            for l, a in zip(layers, alphas):
+                rgba = self._get_array(l, a=a)
+                if rgba is None:
+                    # to handle completely empty layers
+                    continue
+                renderer.draw_image(
+                    gc,
+                    int(x0),
+                    int(y0),
+                    rgba[int(y0) : int(y0 + h), int(x0) : int(x0 + w), :],
+                )
+            # cache the combined background
+            bg = self._m.f.canvas.copy_from_bbox(self._m.f.bbox)
+            # self._bg_layers[layer] = bg
+            gc.restore()
+            return bg
 
     def _get_array(self, l, a=1):
+        if l not in self._bg_layers:
+            return None
         rgba = np.array(self._bg_layers[l])[::-1, :, :]
         if a != 1:
             rgba = rgba.copy()
             rgba[..., -1] = (rgba[..., -1] * a).astype(rgba.dtype)
         return rgba
 
+    def _get_background(self, layer, bbox=None, cache=False):
+        if layer not in self._bg_layers:
+            current_bg = self.canvas.copy_from_bbox(self.figure.bbox)
+
+            if "|" in layer:
+                bg = self._combine_bgs(layer)
+            else:
+                self.fetch_bg(layer, bbox=bbox)
+                bg = self._bg_layers[layer]
+
+            self.canvas.restore_region(current_bg)
+        else:
+            bg = self._bg_layers[layer]
+
+        if cache is True:
+            # explicitly cache the layer
+            # (for peek-layer callbacks to avoid re-fetching the layers all the time)
+            self._bg_layers[layer] = bg
+
+        return bg
+
     def _do_fetch_bg(self, layer, bbox=None):
         cv = self.canvas
-        renderer = cv.get_renderer()
+        renderer = self._get_renderer()
 
         if bbox is None:
             bbox = self.figure.bbox
 
         if "|" in layer:
             if layer not in self._bg_layers:
                 self._combine_bgs(layer)
@@ -1728,22 +2056,23 @@
             # check if all artists are not stale
             no_stale_artists = all(not art.stale for art in allartists)
 
             # don't re-fetch the background if it is not necessary
             if no_stale_artists and (self._bg_layers.get(layer, None) is not None):
                 return
 
-            self.canvas.restore_region(self._blank_bg)
+            if renderer:
+                self.canvas.restore_region(self._blank_bg)
 
-            if not self._m.parent._layout_editor._modifier_pressed:
-                for art in allartists:
-                    if art not in self._hidden_artists:
-                        art.draw(renderer)
-                        art.stale = False
-                self._bg_layers[layer] = cv.copy_from_bbox(bbox)
+                if not self._m.parent._layout_editor._modifier_pressed:
+                    for art in allartists:
+                        if art not in self._hidden_artists:
+                            art.draw(renderer)
+                            art.stale = False
+                            self._bg_layers[layer] = cv.copy_from_bbox(bbox)
 
     def _do_fetch_blank(self):
         # fetch a blank background
         if self._refetch_blank is False and self._blank_bg is not None:
             # don't re-fetch the background if it is not necessary
             return
         try:
@@ -1752,33 +2081,48 @@
             self.canvas.draw()
             self._blank_bg = self.canvas.copy_from_bbox(self.figure.bbox)
             self._refetch_blank = False
         finally:
             self._m.f.set_visible(True)
 
     def fetch_bg(self, layer=None, bbox=None):
+        """
+        Trigger fetching (and caching) the background for a given layer-name.
+
+        Parameters
+        ----------
+        layer : str, optional
+            The layer for which the background should be fetched.
+            If None, the currently visible layer is fetched.
+            The default is None.
+        bbox : bbox, optional
+            The region-boundaries (in figure coordinates) for which the background
+            should be fetched (x0, y0, w, h). If None, the whole figure is fetched.
+            The default is None.
+
+        """
         if self._m.parent._layout_editor._modifier_pressed:
             return
 
-        initial_layer = self.bg_layer
-
         if layer is None:
-            layer = initial_layer
+            layer = self.bg_layer
+
+        initial_layer = self.canvas.copy_from_bbox(self.figure.bbox)
 
         if layer in self._bg_layers:
             # don't re-fetch existing layers
             # (layers get cleared automatically if re-draw is necessary)
             return
 
         with self._disconnect_draw():
             self._do_fetch_blank()
             self._do_fetch_bg(layer, bbox)
 
             if initial_layer in self._bg_layers:
-                self.canvas.restore_region(self._bg_layers[initial_layer])
+                self.canvas.restore_region(initial_layer)
 
     @contextmanager
     def _disconnect_draw(self):
         try:
             # temporarily disconnect draw-event callback to avoid recursion
             if self.cid is not None:
                 self.canvas.mpl_disconnect(self.cid)
@@ -1788,25 +2132,32 @@
             # reconnect draw event
             if self.cid is None:
                 self.cid = self.canvas.mpl_connect("draw_event", self.on_draw)
 
     def on_draw(self, event):
         """Callback to register with 'draw_event'."""
         cv = self.canvas
-
-        if "RendererBase._draw_disabled" in cv.get_renderer().draw_image.__qualname__:
-            # TODO this fixes issues when saving figues with a "tight" bbox, e.g.:
-            # m.savefig(bbox_inches='tight', pad_inches=0.1)
-
-            # This workaround is necessary but the implementation is suboptimal since
-            # it relies on the __qualname__ to identify if the
-            # `matplotlib.backend_bases.RendererBase._draw_disabled()` context is active
-            # The reason why the "_draw_disabled" context has to be handled explicitly
-            # is because otherwise empty backgrounds would be fetched (and cached) by
-            # the draw-event and the export would result in an empty figure.
+        _log.log(5, "draw")
+        try:
+            if (
+                "RendererBase._draw_disabled"
+                in cv.get_renderer().draw_image.__qualname__
+            ):
+                # TODO this fixes issues when saving figues with a "tight" bbox, e.g.:
+                # m.savefig(bbox_inches='tight', pad_inches=0.1)
+
+                # This workaround is necessary but the implementation is suboptimal since
+                # it relies on the __qualname__ to identify if the
+                # `matplotlib.backend_bases.RendererBase._draw_disabled()` context is active
+                # The reason why the "_draw_disabled" context has to be handled explicitly
+                # is because otherwise empty backgrounds would be fetched (and cached) by
+                # the draw-event and the export would result in an empty figure.
+                return
+        except AttributeError:
+            # return on AttributeError to handle backends that don't expose the renderer
             return
 
         if event is not None:
             if event.canvas != cv:
                 raise RuntimeError
         try:
             # reset all background-layers and re-fetch the default one
@@ -1891,32 +2242,34 @@
         else:
             art.set_animated(True)
             self._artists[layer].append(art)
 
             if isinstance(art, plt.Axes):
                 self._managed_axes.add(art)
 
-    def add_bg_artist(self, art, layer=None):
+    def add_bg_artist(self, art, layer=None, draw=True):
         """
         Add a background-artist to be managed.
         (Background artists are only updated on zoom-events... they are NOT animated!)
 
         Parameters
         ----------
         art : Artist
-
             The artist to be added.  Will be set to 'animated' (just
             to be safe).  *art* must be in the figure associated with
             the canvas this class is managing.
         layer : str or None, optional
             The layer name at which the artist should be drawn.
 
             - If "all": the corresponding feature will be added to ALL layers
 
             The default is None in which case the layer of the base-Maps object is used.
+        draw : bool, optional
+            If True, `figure.draw_idle()` is called after adding the artist.
+            The default is True.
         """
 
         if layer is None:
             layer = self._m.layer
 
         # make sure all layer names are converted to string
         layer = str(layer)
@@ -1928,32 +2281,53 @@
         if (
             getattr(art, "axes", None) is not None
             and art.axes.get_label() == "inset_map"
             and not layer.startswith("__inset_")
         ):
             layer = "__inset_" + str(layer)
         if layer in self._bg_artists and art in self._bg_artists[layer]:
-            print(f"EOmaps: Background-artist '{art}' already added")
+            _log.info(f"EOmaps: Background-artist '{art}' already added")
             return
 
         art.set_animated(True)
         self._bg_artists.setdefault(layer, []).append(art)
 
         if isinstance(art, plt.Axes):
             self._managed_axes.add(art)
 
         # tag all relevant layers for refetch
         self._refetch_layer(layer)
 
         for f in self._on_add_bg_artist:
             f()
 
-        self.canvas.draw_idle()
+        if draw:
+            self.canvas.draw_idle()
+
+    def remove_bg_artist(self, art, layer=None, draw=True):
+        """
+        Remove a (background) artist from the map.
 
-    def remove_bg_artist(self, art, layer=None):
+        Parameters
+        ----------
+        art : Artist
+            The artist that should be removed.
+        layer : str or None, optional
+            If provided, the artist is only searched on the provided layer, otherwise
+            all map layers are searched. The default is None.
+        draw : bool, optional
+            If True, `figure.draw_idle()` is called after removing the artist.
+            The default is True.
+
+        Note
+        ----
+        This only removes the artist from the blit-manager and does not call its
+        remove method!
+
+        """
         # handle the "__inset_" prefix of inset-map artists
         if (
             layer is not None
             and getattr(art, "axes", None) is not None
             and art.axes.get_label() == "inset_map"
             and not layer.startswith("__inset_")
         ):
@@ -1990,56 +2364,76 @@
         if removed:
             for f in self._on_remove_bg_artist:
                 f()
 
             # tag all relevant layers for refetch
             self._refetch_layer(layer)
 
-        self.canvas.draw_idle()
+        if draw:
+            self.canvas.draw_idle()
 
     def remove_artist(self, art, layer=None):
-        # this only removes the artist from the blit-manager,
-        # it does not clear it from the plot!
+        """
+        Remove a (dynamically updated) artist from the blit-manager.
+
+        Parameters
+        ----------
+        art : matpltolib.Artist
+            The artist to remove.
+        layer : str, optional
+            The layer to search for the artist. If None, all layers are searched.
+            The default is None.
 
+        Note
+        ----
+        This only removes the artist from the blit-manager and does not call its
+        remove method!
+
+        """
         if layer is None:
             for key, layerartists in self._artists.items():
                 if art in layerartists:
                     art.set_animated(False)
                     layerartists.remove(art)
 
                     # remove axes from the managed_axes set as well!
                     if art in self._managed_axes:
                         self._managed_axes.remove(art)
 
         else:
-            if art in self._artists[layer]:
+            if art in self._artists.get(layer, []):
                 art.set_animated(False)
                 self._artists[layer].remove(art)
 
                 # remove axes from the managed_axes set as well!
                 if art in self._managed_axes:
                     self._managed_axes.remove(art)
+            else:
+                _log.debug(f"The artist {art} is not on the layer '{layer}'")
 
     def _get_artist_zorder(self, a):
         try:
             return a.get_zorder()
         except Exception:
-            print(r"EOmaps: unalble to identify zorder of {a}... using 99")
+            _log.error(r"EOmaps: unalble to identify zorder of {a}... using 99")
             return 99
 
     def _draw_animated(self, layers=None, artists=None):
         """
         Draw animated artists
 
         - if layers is None and artists is None: active layer artists will be re-drawn
         - if layers is not None: all artists from the selected layers will be re-drawn
         - if artists is not None: all provided artists will be redrawn
 
         """
         fig = self.canvas.figure
+        renderer = self._get_renderer()
+        if renderer is None:
+            return
 
         # make sure to strip-off transparency-assignments (e.g. "layer1{0.5}")
         if layers is None:
             layers = [self.bg_layer]
             layers.extend(
                 (l.split("{", maxsplit=1)[0] for l in self.bg_layer.split("|"))
             )
@@ -2059,15 +2453,15 @@
 
         # draw all "unmanaged" axes (e.g. axes that are found in the figure but
         # not in the blit-manager)
         # TODO would be nice to find a better way to handle this!
         # - NOTE: this must be done before drawing managed artists to properly support
         #   temporary artists on unmanaged axes!
         for ax in self._get_unmanaged_axes():
-            ax.draw(self.canvas.renderer)
+            ax.draw(renderer)
 
         # redraw artists from the selected layers and explicitly provided artists
         # (sorted by zorder for each layer)
         layer_artists = list(
             sorted(self._artists.get(layer, []), key=self._get_artist_zorder)
             for layer in layers
         )
@@ -2086,23 +2480,29 @@
     def _get_unmanaged_artists(self):
         # return all artists not explicitly managed by the blit-manager
         # (e.g. any artist added via cartopy or matplotlib functions)
         managed_artists = set(
             chain(*self._bg_artists.values(), *self._artists.values())
         )
 
-        axes = {m.ax for m in (self._m, *self._m._children)}
+        axes = {m.ax for m in (self._m, *self._m._children) if m.ax is not None}
 
         allartists = set()
         for ax in axes:
+            # only include axes titles if they are actually set
+            # (otherwise empty artists appear in the widget)
+            titles = [
+                i
+                for i in (ax.title, ax._left_title, ax._right_title)
+                if len(i.get_text()) > 0
+            ]
+
             axartists = {
                 *ax._children,
-                ax.title,
-                ax._left_title,
-                ax._right_title,
+                *titles,
                 *([ax.legend_] if ax.legend_ is not None else []),
             }
 
             allartists.update(axartists)
 
         return allartists.difference(managed_artists)
 
@@ -2147,26 +2547,29 @@
 
                 try:
                     self._artists_to_clear.get("on_layer_change", []).remove(art)
                 except ValueError:
                     # ignore errors if the artist is not present in the list
                     pass
 
-    def _get_showlayer_name(self, layer=None):
+    def _get_showlayer_name(self, layer=None, transparent=False):
         # combine all layers that should be shown
         # (e.g. to add spines, backgrounds and inset-maps)
 
         if layer is None:
             layer = self.bg_layer
 
         # pass private layers through
         if layer.startswith("__"):
             return layer
 
-        show_layers = [layer, "__SPINES__"]
+        if transparent is True:
+            show_layers = [layer, "__SPINES__"]
+        else:
+            show_layers = ["__BG__", layer, "__SPINES__"]
 
         # show inset map layers and spines only if they contain at least 1 artist
         inset_Q = False
         for l in layer.split("|"):
             narts = len(self._bg_artists.get("__inset_" + l, []))
 
             if narts > 0:
@@ -2218,25 +2621,27 @@
 
         if clear:
             self._clear_temp_artists(clear)
 
         # restore the background
         # add additional layers (background, spines etc.)
         show_layer = self._get_showlayer_name()
+
         if show_layer not in self._bg_layers:
             # make sure the background is properly fetched
             self.fetch_bg(show_layer)
 
-        cv.restore_region(self._bg_layers[show_layer])
+        cv.restore_region(self._get_background(show_layer))
 
-        # draw all of the animated artists
+        # execute after restore actions (e.g. peek layer callbacks)
         while len(self._after_restore_actions) > 0:
             action = self._after_restore_actions.pop(0)
             action()
 
+        # draw all of the animated artists
         self._draw_animated(layers=layers, artists=artists)
         if blit:
             # workaround for nbagg backend to avoid glitches
             # it's slow but at least it works...
             # check progress of the following issuse
             # https://github.com/matplotlib/matplotlib/issues/19116
             if self._mpl_backend_force_full:
@@ -2257,14 +2662,21 @@
             action = self._after_update_actions.pop(0)
             action()
 
         # let the GUI event loop process anything it has to do
         # don't do this! it is causing infinite loops
         # cv.flush_events()
 
+        if (
+            blit
+            and not getattr(self._m, "_snapshotting", False)
+            and BlitManager._snapshot_on_update is True
+        ):
+            self._m.snapshot(clear=True)
+
     def blit_artists(self, artists, bg="active", blit=True):
         """
         Blit artists (optionally on top of a given background)
 
         Parameters
         ----------
         artists : iterable
@@ -2273,19 +2685,18 @@
             A fetched background that is restored before drawing the artists.
             The default is "active".
         blit : bool
             Indicator if canvas.blit() should be called or not.
             The default is True
         """
         cv = self.canvas
-
-        # paranoia in case we missed the first draw event
-        if getattr(self.figure, "_cachedRenderer", None) is None:
-            with self._disconnect_draw():
-                self.figure.canvas.draw()
+        renderer = self._get_renderer()
+        if renderer is None:
+            _log.error("EOmaps: encountered a problem while trying to blit artists...")
+            return
 
         # restore the background
         if bg is not None:
             if bg == "active":
                 bg = self._get_active_bg()
             cv.restore_region(bg)
 
@@ -2305,62 +2716,66 @@
     ):
         """
         Update a part of the screen with a different background
         (intended as after-restore action)
 
         bbox_bounds = (x, y, width, height)
         """
-
         if bbox_bounds is None:
             bbox = self.figure.bbox
         else:
             bbox = Bbox.from_bounds(*bbox_bounds)
 
         def action():
+            renderer = self._get_renderer()
+            if renderer is None:
+                return
+
             if self.bg_layer == layer:
                 return
 
             # make sure the background is fetched
             if layer not in self._bg_layers:
                 self.fetch_bg(layer)
                 # update to make sure spines etc. are properly displayed
                 self.update()
 
             x0, y0, w, h = bbox.bounds
 
             # convert the buffer to rgba so that we can add transparency
-            buffer = self._bg_layers[layer]
+            buffer = self._get_background(layer, cache=True)
 
             x = buffer.get_extents()
             ncols, nrows = x[2] - x[0], x[3] - x[1]
 
             argb = (
                 np.frombuffer(buffer, dtype=np.uint8).reshape((nrows, ncols, 4)).copy()
             )
             argb = argb[::-1, :, :]
 
             argb[:, :, -1] = (argb[:, :, -1] * alpha).astype(np.int8)
 
-            gc = self.canvas.renderer.new_gc()
+            gc = renderer.new_gc()
 
             gc.set_clip_rectangle(bbox)
             if set_clip_path is True:
                 gc.set_clip_path(clip_path)
 
-            self.canvas.renderer.draw_image(
+            renderer.draw_image(
                 gc,
                 int(x0),
                 int(y0),
                 argb[int(y0) : int(y0 + h), int(x0) : int(x0 + w), :],
             )
             gc.restore()
 
         return action
 
     def cleanup_layer(self, layer):
+        """Trigger cleanup methods for a given layer."""
         self._cleanup_bg_artists(layer)
         self._cleanup_artists(layer)
         self._cleanup_bg_layers(layer)
         self._cleanup_on_layer_activation(layer)
 
     def _cleanup_bg_artists(self, layer):
         if layer not in self._bg_artists:
@@ -2371,15 +2786,15 @@
             a = artists.pop()
             try:
                 self.remove_bg_artist(a, layer)
                 # no need to remove spines (to avoid NotImplementedErrors)!
                 if not isinstance(a, Spine):
                     a.remove()
             except Exception:
-                print(f"EOmaps-cleanup: Problem while clearing bg artist:\n {a}")
+                _log.debug(f"EOmaps-cleanup: Problem while clearing bg artist:\n {a}")
 
         del self._bg_artists[layer]
 
     def _cleanup_artists(self, layer):
         if layer not in self._artists:
             return
 
@@ -2388,28 +2803,34 @@
             a = artists.pop()
             try:
                 self.remove_artist(a)
                 # no need to remove spines (to avoid NotImplementedErrors)!
                 if not isinstance(a, Spine):
                     a.remove()
             except Exception:
-                print(f"EOmaps-cleanup: Problem while clearing dynamic artist:\n {a}")
+                _log.debug(
+                    f"EOmaps-cleanup: Problem while clearing dynamic artist:\n {a}"
+                )
 
         del self._artists[layer]
 
     def _cleanup_bg_layers(self, layer):
         try:
             # remove cached background-layers
             if layer in self._bg_layers:
                 del self._bg_layers[layer]
         except Exception:
-            print("EOmaps-cleanup: Problem while clearing cached background layers")
+            _log.debug(
+                "EOmaps-cleanup: Problem while clearing cached background layers"
+            )
 
     def _cleanup_on_layer_activation(self, layer):
 
         try:
             # remove not yet executed lazy-activation methods
             # (e.g. not yet fetched WMS services)
             if layer in self._on_layer_activation:
                 del self._on_layer_activation[layer]
         except Exception:
-            print("EOmaps-cleanup: Problem while clearing layer activation methods")
+            _log.debug(
+                "EOmaps-cleanup: Problem while clearing layer activation methods"
+            )
```

### Comparing `EOmaps-6.5/eomaps/logo.png` & `EOmaps-7.0/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/mapsgrid.py` & `EOmaps-7.0/eomaps/mapsgrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+"""Mapsgrid class definition (helper for initialization of regular Maps-grids)."""
+
 from functools import wraps, lru_cache
 
 import numpy as np
 from matplotlib.gridspec import GridSpec
 import matplotlib.pyplot as plt
 
-from ._shapes import shapes
+from .shapes import Shapes
 from .eomaps import Maps
 
 from .ne_features import NaturalEarth_features
 
 try:
-    from ._webmap_containers import wms_container
+    from .webmap_containers import WebMapContainer
 except ImportError:
-    wms_container = None
+    WebMapContainer = None
 
 
 class MapsGrid:
     """
     Initialize a grid of Maps objects
 
     Parameters
@@ -140,16 +142,16 @@
         f=None,
         **kwargs,
     ):
 
         self._Maps = []
         self._names = dict()
 
-        if wms_container is not None:
-            self._wms_container = wms_container(self)
+        if WebMapContainer is not None:
+            self._wms_container = WebMapContainer(self)
 
         gskwargs = dict(bottom=0.01, top=0.99, left=0.01, right=0.99)
         gskwargs.update(kwargs)
         self.gridspec = GridSpec(nrows=r, ncols=c, **gskwargs)
 
         if m_inits is None and ax_inits is None:
             if isinstance(crs, list):
@@ -370,29 +372,27 @@
         for m in self:
             m.plot_map(**kwargs)
 
     plot_map.__doc__ = _doc_prefix + plot_map.__doc__
 
     @property
     @lru_cache()
-    @wraps(shapes)
+    @wraps(Shapes)
     def set_shape(self):
-        s = shapes(self)
+        s = Shapes(self)
         s.__doc__ = self._doc_prefix + s.__doc__
 
         return s
 
-    @wraps(Maps.set_data_specs)
-    def set_data_specs(self, *args, **kwargs):
+    @wraps(Maps.set_data)
+    def set_data(self, *args, **kwargs):
         for m in self:
-            m.set_data_specs(*args, **kwargs)
-
-    set_data_specs.__doc__ = _doc_prefix + set_data_specs.__doc__
+            m.set_data(*args, **kwargs)
 
-    set_data = set_data_specs
+    set_data.__doc__ = _doc_prefix + set_data.__doc__
 
     @wraps(Maps.set_classify_specs)
     def set_classify_specs(self, scheme=None, **kwargs):
         for m in self:
             m.set_classify_specs(scheme=scheme, **kwargs)
 
     set_classify_specs.__doc__ = _doc_prefix + set_classify_specs.__doc__
@@ -441,14 +441,21 @@
     @wraps(Maps.add_scalebar)
     def add_scalebar(self, *args, **kwargs):
         for m in self:
             m.add_scalebar(*args, **kwargs)
 
     add_scalebar.__doc__ = _doc_prefix + add_scalebar.__doc__
 
+    @wraps(Maps.add_compass)
+    def add_compass(self, *args, **kwargs):
+        for m in self:
+            m.add_compass(*args, **kwargs)
+
+    add_compass.__doc__ = _doc_prefix + add_compass.__doc__
+
     @wraps(Maps.add_colorbar)
     def add_colorbar(self, *args, **kwargs):
         for m in self:
             m.add_colorbar(*args, **kwargs)
 
     add_colorbar.__doc__ = _doc_prefix + add_colorbar.__doc__
```

### Comparing `EOmaps-6.5/eomaps/ne_features.py` & `EOmaps-7.0/eomaps/ne_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,90 @@
+"""Classes to fetch and draw NaturalEarth features."""
+
+import logging
 from textwrap import dedent
-from warnings import warn
 from pathlib import Path
 import json
-from matplotlib.colors import rgb2hex
+
 from cartopy import crs as ccrs
 
-cfeature = None
-shapereader = None
+from .helpers import register_modules
 
+_log = logging.getLogger(__name__)
 
-def _register_cartopy_feature_io():
-    global cfeature
-    global shapereader
-    import cartopy.feature as cfeature
-    from cartopy.io import shapereader
 
+def combdoc(*args):
+    """Dedent and combine strings."""
+    return "\n".join(dedent(str(i)) for i in args)
 
-gpd = None
 
+class NaturalEarth_presets:
+    """
+    Feature presets.
 
-def _register_geopandas():
-    global gpd
-    try:
-        import geopandas as gpd
-    except ImportError:
-        return False
+    To add single preset-features (or customize the appearance), use:
 
-    return True
+    >>> m.add_feature.preset.coastline(ec="r", scale=50, ...)
 
+    To quickly add multiple features in one go, use:
 
-def combdoc(*args):
-    """Dedent and combine strings."""
-    return "\n".join(dedent(str(i)) for i in args)
+    >>> m.add_feature.preset("coastline", "ocean", "land")
 
+    """
 
-class _NaturalEarth_presets:
     def __init__(self, m):
-        _register_cartopy_feature_io()
         self._m = m
 
+    def __call__(self, *args, scale=50, layer=None):
+        """
+        Add multiple preset-features in one go.
+
+        >>> m.add_feature.preset("coastline", "ocean", "land")
+
+        Parameters
+        ----------
+        *args : str
+            The names of the features to add.
+        scale : int or str
+            Set the scale of the feature preset (10, 50, 110 or "auto")
+            The default is "auto"
+        layer : str or None, optional
+            The name of the layer at which map-features are plotted.
+
+            - If "all": the corresponding feature will be added to ALL layers
+            - If None, the layer of the parent object is used.
+
+            The default is None.
+
+        """
+        wrong_names = set(args).difference(self._feature_names)
+        assert len(wrong_names) == 0, (
+            f"EOmaps: {wrong_names} are not valid preset-feature names!\n"
+            f"Use one of: {self._feature_names}."
+        )
+
+        for a in args:
+            getattr(self, a)(scale=scale, layer=layer)
+
+    @property
+    def _feature_names(self):
+        return [i for i in self.__dir__() if not i.startswith("_")]
+
     @property
     def coastline(self):
         """
         Add a coastline to the map.
 
         All provided arguments are passed to `m.add_feature`
 
         The default args are:
 
         - fc="none", ec="k", zorder=100
         """
-        return self._feature(
+        return self._Feature(
             self._m,
             "physical",
             "coastline",
             facecolor="none",
             edgecolor="k",
             zorder=100,
         )
@@ -67,17 +97,17 @@
         All provided arguments are passed to `m.add_feature`
 
         The default args are:
 
         - fc=(0.59375, 0.71484375, 0.8828125), ec="none", zorder=-2, reproject="cartopy"
         """
         # convert color to hex to avoid issues with geopandas
-        color = rgb2hex(cfeature.COLORS["water"])
+        color = "#97b6e1"  # rgb2hex(cfeature.COLORS["water"])
 
-        return self._feature(
+        return self._Feature(
             self._m, "physical", "ocean", facecolor=color, edgecolor="none", zorder=-2
         )
 
     @property
     def land(self):
         """
         Add a land-coloring to the map.
@@ -86,17 +116,17 @@
 
         The default args are:
 
         - fc=(0.9375, 0.9375, 0.859375), ec="none", zorder=-1
 
         """
         # convert color to hex to avoid issues with geopandas
-        color = rgb2hex(cfeature.COLORS["land"])
+        color = "#efefdb"  # rgb2hex(cfeature.COLORS["land"])
 
-        return self._feature(
+        return self._Feature(
             self._m, "physical", "land", facecolor=color, edgecolor="none", zorder=-1
         )
 
     @property
     def countries(self):
         """
         Add country-boundaries to the map.
@@ -104,15 +134,15 @@
         All provided arguments are passed to `m.add_feature`
 
         The default args are:
 
         - fc="none", ec=".5", lw=0.5, zorder=99
 
         """
-        return self._feature(
+        return self._Feature(
             self._m,
             "cultural",
             "admin_0_countries",
             facecolor="none",
             edgecolor=".5",
             linewidth=0.5,
             zorder=99,
@@ -126,15 +156,15 @@
         All provided arguments are passed to `m.add_feature`
 
         The default args are:
 
         - fc="r", lw=0., zorder=100
 
         """
-        return self._feature(
+        return self._Feature(
             self._m,
             "cultural",
             "urban_areas",
             facecolor="r",
             linewidth=0.0,
             zorder=100,
         )
@@ -147,15 +177,15 @@
         All provided arguments are passed to `m.add_feature`
 
         The default args are:
 
         - fc="b", ec="none", lw=0., zorder=98
 
         """
-        return self._feature(
+        return self._Feature(
             self._m,
             "physical",
             "lakes",
             facecolor="b",
             linewidth=0,
             zorder=98,
         )
@@ -168,25 +198,25 @@
         All provided arguments are passed to `m.add_feature`
 
         The default args are:
 
         - fc="none", ec="b", lw=0.75, zorder=97
 
         """
-        return self._feature(
+        return self._Feature(
             self._m,
             "physical",
             "rivers_lake_centerlines",
             facecolor="none",
             edgecolor="b",
             linewidth=0.75,
             zorder=97,
         )
 
-    class _feature:
+    class _Feature:
         def __init__(self, m, category, name, **kwargs):
             self._m = m
             self.category = category
             self.name = name
             self.kwargs = kwargs
 
             self.feature = self._m.add_feature._get_feature(
@@ -207,42 +237,43 @@
 
         def _handle_synonyms(self, kwargs):
             # make sure to replace shortcuts with long names
             # (since "facecolor=..." will override "fc=..." if both are specified)
             subst = dict(fc="facecolor", ec="edgecolor", lw="linewidth", ls="linestyle")
             return {subst.get(key, key): val for key, val in kwargs.items()}
 
-        def __call__(self, scale=50, **kwargs):
+        def __call__(self, scale=50, layer=None, **kwargs):
             k = dict(**self.kwargs)
             k.update(kwargs)
 
             if scale != "auto":
                 self.feature = self._m.add_feature._get_feature(
                     category=self.category, name=self.name
                 )
 
             self.__doc__ = self.feature.__doc__
-            return self.feature(scale=scale, **self._handle_synonyms(k))
+            return self.feature(scale=scale, layer=layer, **self._handle_synonyms(k))
 
 
 _NE_features_path = Path(__file__).parent / "NE_features.json"
 
 try:
     with open(_NE_features_path, "r") as file:
         _NE_features = json.load(file)
 
         _NE_features_all = dict()
         for scale, scale_items in _NE_features.items():
             for category, category_items in scale_items.items():
                 _NE_features_all.setdefault(category, set()).update(category_items)
 
 except Exception:
-    print(
+    _log.error(
         "EOmaps: Could not load available NaturalEarth features from\n"
-        f"{_NE_features_path}"
+        f"{_NE_features_path}",
+        exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
     )
     _NE_features = dict()
     _NE_features_all = dict()
 
 
 class NaturalEarth_features(object):
     """
@@ -288,51 +319,26 @@
       >>> countries = m.add_feature.cultural.admin_0_countries.get_gdf(scale=10)
       >>> countries["area_rank"] = countries.area.rank()
       >>> m.add_gdf(countries, column="area_rank")
 
     """
 
     def __init__(self, m):
-        _register_cartopy_feature_io()
-
         self._m = m
-
-        self._depreciated_names = dict()
-
-        for scale, scale_items in _NE_features.items():
-            for category, category_items in scale_items.items():
-                ns = dict()
-                for name in category_items:
-                    ns[name] = self._get_feature(category, name)
-
-                c = self._category(scale, category, **ns)
-                self._depreciated_names[f"{category}_{scale}"] = c
-
         for category, names in _NE_features_all.items():
-            func = lambda name: self._feature(self._m, category, name)
+            func = lambda name: self._Feature(self._m, category, name)
             ns = dict(zip(names, map(func, names)))
 
-            c = self._category(scale, category, **ns)
+            c = self._Category(scale, category, **ns)
             setattr(self, category, c)
 
     def __call__(self, category, scale, name, **kwargs):
         feature = self._get_feature(category, name)
         return feature(**kwargs)
 
-    def __getattribute__(self, key):
-        if key != "_depreciated_names" and key in self._depreciated_names:
-            warn(
-                f"EOmaps: Using 'm.add_feature.{key}.< name >()' is depreciated! "
-                f"use 'm.add_feature.{key.split('_')[0]}.< name >(scale=...)' instead! ",
-                stacklevel=99,
-            )
-            return self._depreciated_names[key]
-        else:
-            return object.__getattribute__(self, key)
-
     def __getitem__(self, key):
         return getattr(self, key)
 
     def _get_feature(self, category, name):
         if category not in ["cultural", "physical"]:
             raise AssertionError(
                 "EOmaps: Use one of ['cultural', 'physical']" + " as category!"
@@ -345,29 +351,29 @@
 
             matches = get_close_matches(name, available_names, 3)
             raise AssertionError(
                 f"EOmaps: {name} is not a valid feature-name... "
                 + (f"did you mean one of {matches}?" if matches else "")
             )
 
-        return self._feature(self._m, category, name)
+        return self._Feature(self._m, category, name)
 
     @property
     def preset(self):
         """
         Access to commonly used NaturalEarth features with pre-defined styles.
 
         - "coastline" - black coastlines
         - "ocean" - blue ocean coloring
         - "land" - beige land coloring
         - "countries" - gray country boarder lines
         """
-        return _NaturalEarth_presets(self._m)
+        return NaturalEarth_presets(self._m)
 
-    class _category:
+    class _Category:
         def __init__(self, scale, category, **kwargs):
 
             self._s = scale
             self._c = category
 
             for key, val in kwargs.items():
                 setattr(self, key, val)
@@ -395,15 +401,15 @@
             self.__doc__ = combdoc(header, NaturalEarth_features.__doc__)
 
         def __repr__(self):
             return (
                 f"EOmaps interface for {self._s} {self._c} " + "NaturalEarth features"
             )
 
-    class _feature:
+    class _Feature:
         """
         Natural Earth Feature.
 
         Call this class like a function to add the feature to the map.
 
         By default, the scale of the feature is automatically adjusted based on the
         map-extent. Use `scale=...` to use a fixed scale.
@@ -424,15 +430,15 @@
             The (preferred) scale of the NaturalEarth feature.
 
             If the scale is not available for the selected feature, the next available
             scale will be used (and a warning is issued)!
 
             If 'auto' the scale is automatically adjusted based on the map-extent.
 
-        layer : int, str or None, optional
+        layer : str or None, optional
             The name of the layer at which map-features are plotted.
 
             - If "all": the corresponding feature will be added to ALL layers
             - If None, the layer of the parent object is used.
 
             The default is None.
 
@@ -483,27 +489,32 @@
             self.__doc__ = (
                 "NaturalEarth feature: "
                 f"{self._category} | {self._name}\n\n"
                 "----------------------------------------\n\n"
             ) + self.__doc__
 
         def __call__(self, layer=None, scale="auto", **kwargs):
+            _log.debug(f"EOmaps: Adding feature: {self._category}: {self._name}")
+
             self._set_scale(scale)
 
             from . import MapsGrid  # do this here to avoid circular imports!
 
             for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
                 if layer is None:
                     uselayer = m.layer
                 else:
                     uselayer = layer
 
                 feature = self._get_cartopy_feature(self._scale)
                 feature._kwargs.update(kwargs)
                 art = m.ax.add_feature(feature)
+                art.set_label(
+                    f"NaturalEarth feature: {feature.category}  |  {feature.name}"
+                )
                 m.BM.add_bg_artist(art, layer=uselayer)
 
         def _set_scale(self, scale):
             if scale == "auto":
                 self._scale = "auto"
                 return
 
@@ -516,23 +527,23 @@
                 "110m",
                 "auto",
             ], "scale must be one of  [10, 50, 110, 'auto']"
 
             self._scale = self._get_available_scale(scale)
 
             if self._scale != scale:
-                print(
+                _log.warning(
                     f"EOmaps: The NaturalEarth feature '{self._name}' is not "
                     f"available at 1:{scale} scale... using 1:{self._scale} instead!"
                 )
 
         def get_validated_scaler(self, *args, **kwargs):
-            _register_cartopy_feature_io()
+            from cartopy.feature import AdaptiveScaler
 
-            class AdaptiveValidatedScaler(cfeature.AdaptiveScaler):
+            class AdaptiveValidatedScaler(AdaptiveScaler):
                 # subclass of the AdaptiveScaler to make sure the dataset exists
                 def __init__(self, default_scale, limits, validator=None):
                     super().__init__(default_scale, limits)
 
                     self.validator = validator
 
                 def scale_from_extent(self, extent):
@@ -543,14 +554,16 @@
 
                     self._scale = scale
                     return self._scale
 
             return AdaptiveValidatedScaler(*args, **kwargs)
 
         def _get_cartopy_feature(self, scale):
+            from cartopy.feature import NaturalEarthFeature
+
             self._set_scale(scale)
 
             if (
                 self._cartopy_feature is not None
                 and self._scale == self._cartopy_feature.scale
             ):
 
@@ -562,15 +575,15 @@
                     (("50m", 50), ("10m", 15)),
                     validator=self._get_available_scale,
                 )
             else:
                 usescale = self._scale
 
             # get an instance of the corresponding cartopy-feature
-            self._cartopy_feature = cfeature.NaturalEarthFeature(
+            self._cartopy_feature = NaturalEarthFeature(
                 category=self._category, name=self._name, scale=usescale
             )
 
             return self._cartopy_feature
 
         def _get_available_scale(self, scale):
             # return the optimal scale for the selected feature
@@ -605,35 +618,35 @@
                 The default is False
 
             Returns
             -------
             gdf : geopandas.GeoDataFrame
                 A GeoDataFrame with all geometries of the feature
             """
-            assert (
-                _register_geopandas()
-            ), "EOmaps: Missing dependency `geopandas` for `feature.get_gdf()`"
+            (gpd,) = register_modules("geopandas")
 
             self._set_scale(scale)
 
             if what == "full":
+                from cartopy.io import shapereader
+
                 gdf = gpd.read_file(
                     shapereader.natural_earth(
                         resolution=self._scale, category=self._category, name=self._name
                     )
                 )
             elif what.startswith("geoms"):
                 feature = self._get_cartopy_feature(self._scale)
 
                 if what == "geoms_intersecting":
                     try:
                         extent = self._m.get_extent(feature.crs)
                         feature.scaler.scale_from_extent(extent)
                     except:
-                        print("EOmaps: unable to determine extent")
+                        _log.error("EOmaps: unable to determine extent")
                         pass
                     geoms = list(feature.geometries())
                 elif what == "geoms":
                     try:
                         extent = self._m.get_extent(feature.crs)
                         geoms = list(feature.intersecting_geometries(extent))
                     except ValueError:
```

### Comparing `EOmaps-6.5/eomaps/projections.py` & `EOmaps-7.0/eomaps/projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Projection definitions."""
+
 from cartopy import crs as ccrs
 from pyproj import CRS
 
 # fmt: off
 equi7_wkt = {
        'AF': 'PROJCS["Azimuthal_Equidistant",GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0],UNIT["Degree",0.0174532925199433]],PROJECTION["Azimuthal_Equidistant"],PARAMETER["latitude_of_center",8.5],PARAMETER["longitude_of_center",21.5],PARAMETER["false_easting",5621452.01998],PARAMETER["false_northing",5990638.42298],UNIT["metre",1,AUTHORITY["EPSG","9001"]],AXIS["Easting",EAST],AXIS["Northing",NORTH]]',
        'AN': 'PROJCS["Azimuthal_Equidistant",GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0],UNIT["Degree",0.0174532925199433]],PROJECTION["Azimuthal_Equidistant"],PARAMETER["latitude_of_center",-90],PARAMETER["longitude_of_center",0],PARAMETER["false_easting",3714266.97719],PARAMETER["false_northing",3402016.50625],UNIT["metre",1,AUTHORITY["EPSG","9001"]],AXIS["Easting",EAST],AXIS["Northing",NORTH]]',
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/app.py` & `EOmaps-7.0/eomaps/qtcompanion/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,187 +1,195 @@
 from PyQt5 import QtWidgets
-from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QSize
+from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QSize, QObject
 from PyQt5.QtGui import QKeySequence
 
-# TODO make sure a QApplication has been instantiated
-app = QtWidgets.QApplication.instance()
-if app is None:
-    # if it does not exist then a QApplication is created
-    app = QtWidgets.QApplication([])
-
-
-from .base import transparentWindow
+from .base import AlwaysOnTopWindow
 from .widgets.peek import PeekTabs
 from .widgets.editor import ArtistEditor
 from .widgets.wms import AddWMSMenuButton
 from .widgets.save import SaveFileWidget
-from .widgets.files import OpenFileTabs, OpenDataStartTab
+from .widgets.files import OpenFileTabs
 from .widgets.utils import get_cmap_pixmaps
 from .widgets.extent import SetExtentToLocation
 from .widgets.click_callbacks import ClickCallbacks
 
 from .widgets.editor import LayerTabBar
+from .widgets.layer import AutoUpdateLayerMenuButton
 
-
-class OpenFileButton(QtWidgets.QPushButton):
-    def enterEvent(self, e):
-        OpenDataStartTab.enterEvent(self, e)
+# TODO make sure a QApplication has been instantiated
+app = QtWidgets.QApplication.instance()
+if app is None:
+    # if it does not exist then a QApplication is created
+    app = QtWidgets.QApplication([])
 
 
-class Tab1(QtWidgets.QWidget):
+class CompareTab(QtWidgets.QWidget):
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.m = m
 
         peektabs = PeekTabs(m=self.m)
 
         setextent = SetExtentToLocation(m=self.m)
-        save = SaveFileWidget(m=self.m)
+        self.save_widget = SaveFileWidget(m=self.m)
 
         # -------------
         self.layer_tabs = LayerTabBar(self.m, populate=True)
         # make sure the tab-widget auto-expands properly
         self.layer_tabs.setSizePolicy(
             QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
         )
         self.layer_tabs.setTabsClosable(False)
         # -------------
 
-        click_cbs = ClickCallbacks(m=self.m)
+        self.click_cbs = ClickCallbacks(m=self.m)
 
+        # add wms button
         try:
             addwms = AddWMSMenuButton(m=self.m, new_layer=True)
             addwms.wmsLayerCreated.connect(
                 self.layer_tabs.repopulate_and_activate_current
             )
         except:
-            addwms = QtWidgets.QPushButton("WMS services unavailable")
+            addwms = None
 
-        self.open_file_button = OpenFileButton("Open File")
-        self.open_file_button.setFixedSize(self.open_file_button.sizeHint())
+        self.layer_button = AutoUpdateLayerMenuButton(m=self.m)
 
-        l2 = QtWidgets.QHBoxLayout()
-        l2.addWidget(addwms)
-        l2.addWidget(self.open_file_button)
-        l2.addStretch(1)
-        l2.addWidget(setextent)
+        options_layout = QtWidgets.QHBoxLayout()
+        if addwms:
+            options_layout.addWidget(addwms)
+        options_layout.addStretch(1)
+        options_layout.addWidget(setextent)
 
         layer_tab_layout = QtWidgets.QHBoxLayout()
         layer_tab_layout.setAlignment(Qt.AlignLeft)
-        layer_tab_layout.addWidget(QtWidgets.QLabel("<b>Layers: </b>"))
+        layer_tab_layout.addWidget(self.layer_button)
         layer_tab_layout.addWidget(self.layer_tabs)
 
         layout = QtWidgets.QVBoxLayout()
         layout.addWidget(peektabs)
-        layout.addStretch(1)
-        layout.addWidget(click_cbs)
-        layout.addStretch(1)
-        layout.addLayout(l2)
+        layout.addWidget(self.click_cbs)
+        layout.addLayout(options_layout)
         layout.addStretch(1)
         layout.addLayout(layer_tab_layout)
-        layout.addWidget(save)
+        layout.addWidget(self.save_widget)
 
         self.setLayout(layout)
 
 
 class ControlTabs(QtWidgets.QTabWidget):
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.m = m
 
-        self.tab1 = Tab1(m=self.m)
+        self.tab_compare = CompareTab(m=self.m)
         self.tab_open = OpenFileTabs(m=self.m)
-
-        # connect the open-file-button to the button from the "Open Files" tab
-        self.tab1.open_file_button.clicked.connect(self.trigger_open_file_button)
-
         self.tab_edit = ArtistEditor(m=self.m)
 
-        self.addTab(self.tab1, "Compare")
+        self.addTab(self.tab_compare, "Compare")
         self.addTab(self.tab_edit, "Edit")
-        self.addTab(self.tab_open, "Open Files")
+        self.addTab(self.tab_open, "Data")
 
         # re-populate artists on tab-change
         self.currentChanged.connect(self.tabchanged)
 
         self.setAcceptDrops(True)
 
-    @pyqtSlot()
-    def trigger_open_file_button(self):
-        self.tab_open.starttab.open_button.clicked.emit()
+        self.setStyleSheet(
+            """
+            ControlTabs {
+                font-size: 10pt;
+                font-weight: bold;
+            }
+
+            QTabWidget::pane {
+              border: 0px;
+              top:0px;
+              background: rgb(240, 240, 240);
+              border-radius: 10px;
+            }
+
+            QTabBar::tab {
+              background: rgb(240, 240, 240);
+              border: 0px;
+              padding: 3px;
+              padding-bottom: 6px;
+              padding-left: 6px;
+              padding-right: 6px;
+              margin-left: 10px;
+              margin-bottom: -2px;
+              border-radius: 4px;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(200, 200, 200);
+              border:1px solid rgb(150, 150, 150);
+              margin-bottom: 2px;
+            }
+            """
+        )
 
     @pyqtSlot()
     def tabchanged(self):
-        if self.currentWidget() == self.tab1:
-            self.tab1.layer_tabs.repopulate_and_activate_current()
+
+        if self.currentWidget() == self.tab_compare:
+            self.tab_compare.layer_tabs.repopulate_and_activate_current()
 
         elif self.currentWidget() == self.tab_edit:
             self.tab_edit.artist_tabs.repopulate_and_activate_current()
 
     def dragEnterEvent(self, e):
         self.tab_open.dragEnterEvent(e)
 
     def dragLeaveEvent(self, e):
         self.tab_open.dragLeaveEvent(e)
 
     def dropEvent(self, e):
         self.tab_open.dropEvent(e)
 
 
-class MenuWindow(transparentWindow):
-
-    cmapsChanged = pyqtSignal()
-
+class MenuWindow(AlwaysOnTopWindow):
     def __init__(self, *args, m=None, **kwargs):
 
-        # assign m before calling the init of the transparentWindow
+        # assign m before calling the init of the AlwaysOnTopWindow
         # to show the layer-selector!
         self.m = m
 
         # indicator if help-tooltips should be displayed or not
         # (toggled by a toolbar checkbox)
         self.showhelp = False
 
         super().__init__(*args, m=self.m, **kwargs)
 
-        # clear the colormaps-dropdown pixmap cache if the colormaps have changed
-        # (the pyqtSignal is emmited by Maps-objects if a new colormap is registered)
-        self.cmapsChanged.connect(self.clear_pixmap_cache)
-
         self.tabs = ControlTabs(m=self.m)
         self.tabs.setMouseTracking(True)
 
-        self.setStyleSheet(
-            """QToolTip {
-            font-family: "SansSerif";
-            font-size:10;
-            background-color: rgb(53, 53, 53);
-            color: white;
-            border: none;
-            }"""
-        )
-        self.cb_transparentQ()
-
         menu_layout = QtWidgets.QVBoxLayout()
         menu_layout.addWidget(self.tabs)
         menu_widget = QtWidgets.QWidget()
         menu_widget.setLayout(menu_layout)
 
         statusbar = QtWidgets.QStatusBar(self)
+        statusbar.addPermanentWidget(QtWidgets.QLabel(f"EOmaps v{self.m.__version__}"))
+
         self.setStatusBar(statusbar)
 
         # prevent context-menu's from appearing to avoid the "hide toolbar"
         # context menu when right-clicking the toolbar
         self.setContextMenuPolicy(Qt.NoContextMenu)
 
         self.setCentralWidget(menu_widget)
 
         # sh = self.sizeHint()
         # self.resize(int(sh.width() * 1.35), sh.height())
 
+        # clear the colormaps-dropdown pixmap cache if the colormaps have changed
+        # (the pyqtSignal is emmited by Maps-objects if a new colormap is registered)
+        self.m._connect_signal("cmapsChanged", self.clear_pixmap_cache)
+
     def show(self):
         super().show()
         # make sure show/hide shortcut also works if the widget is active
         # we need to re-assign this on show to make sure it is always assigned
         # when the window is shown
         self.shortcut = QtWidgets.QShortcut(QKeySequence("w"), self)
         self.shortcut.setContext(Qt.WindowShortcut)
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/icons/logo.png` & `EOmaps-7.0/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle.png` & `EOmaps-7.0/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle_active.png` & `EOmaps-7.0/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse.png` & `EOmaps-7.0/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `EOmaps-7.0/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/click_callbacks.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/click_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,16 +156,17 @@
 
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.setStyleSheet(
             """
             ClickCallbacks{
-                border: 1px solid rgb(200,200,200);
+                border: 0px solid rgb(200,200,200);
                 border-radius: 10px;
+                background-color: rgb(200,200,200);
                 };
             """
         )
 
         self.m = m
 
         self._pick_map = self.m
@@ -300,31 +301,29 @@
         self.widgetShown.connect(self.update_buttons)
 
         self.set_pick_map(0)
 
         # make sure we re-attach pick-callback on a layer change
         self.m.BM.on_layer(self.on_layer_change, persistent=True)
 
+        self.m._connect_signal("dataPlotted", self.populate_dropdown)
+        self.m._connect_signal("dataPlotted", self.update_buttons)
+
     def showEvent(self, event):
         self.widgetShown.emit()
 
     def identify_pick_map(self):
+        layers, _ = self.m.BM._get_layers_alphas()
+        layers.extend(("all", "inset_all"))
+
         pickm = list()
         for m in (self.m.parent, *self.m.parent._children):
-            if (
-                m.coll is not None
-                and m.ax == self.m.ax
-                and m.layer
-                in (
-                    "all",
-                    m.BM._bg_layer,
-                    *m.BM._bg_layer.split("|"),
-                )
-            ):
+            if m.coll is not None and m.ax == self.m.ax and m.layer in layers:
                 pickm.append(m)
+
         return pickm
 
     @pyqtSlot()
     def clear_annotations_and_markers(self):
         # clear all annotations and markers from this axis
         # (irrespective of the visible layer!)
         for m in (self.m.parent, *self.m.parent._children):
@@ -345,15 +344,15 @@
     def set_permanent(self):
         self.reattach_pick_callbacks()
         # re-attach click callbacks as well
         for key in ("annotate", "mark", "print"):
             if self.cids.get(key, None) is not None:
                 self.attach_callback(key)
 
-    def populate_dropdown(self):
+    def populate_dropdown(self, *args, **kwargs):
         self.map_dropdown.clear()
 
         # the QAbstractItemView object that holds the dropdown-items
         view = self.map_dropdown.view()
         view.setTextElideMode(Qt.ElideNone)
 
         for i, m in enumerate(self.identify_pick_map()):
@@ -416,22 +415,38 @@
                 # set pick-buttons to invisible if no pick_map is found
                 if self._pick_map is None or self._pick_map.coll is None:
                     val.setEnabled(False)
                 else:
                     val.setEnabled(True)
 
                 if self.cids.get(key, None) is not None:
-                    val.setStyleSheet("background-color : rgb(200,100,100);")
+                    val.setStyleSheet(
+                        "background-color : rgb(200,100,100);"
+                        "padding: 4px;"
+                        "border-radius : 4px;"
+                    )
                 else:
-                    val.setStyleSheet("background-color : rgba(200,100,100,50);")
+                    val.setStyleSheet(
+                        "background-color : rgba(200,100,100,50);"
+                        "padding: 4px;"
+                        "border-radius : 4px;"
+                    )
             else:
                 if self.cids.get(key, None) is not None:
-                    val.setStyleSheet("background-color : rgb(100,150,100);")
+                    val.setStyleSheet(
+                        "background-color : rgb(100,150,100);"
+                        "padding: 4px;"
+                        "border-radius : 4px;"
+                    )
                 else:
-                    val.setStyleSheet("background-color : rgba(100,150,100,50);")
+                    val.setStyleSheet(
+                        "background-color : rgba(100,150,100,50);"
+                        "padding: 4px;"
+                        "border-radius : 4px;"
+                    )
 
     def remove_callback(self, key):
         mcid = self.cids.get(key, None)
         if mcid is not None:
             m, cid = mcid
             if key.endswith("_pick"):
                 # explicitly check if the callback is attached to avoid warnings if
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/draw.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/draw.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-from PyQt5 import QtWidgets
-from PyQt5.QtCore import Qt, pyqtSlot
-
-from .utils import GetColorWidget, AlphaSlider
-
+import logging
 
-class TransparencySlider(AlphaSlider):
-    def enterEvent(self, e):
-        if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(),
-                "<h3>Transparency</h3> Set the transparency of the facecolor.",
-            )
+from PyQt5 import QtWidgets
+from PyQt5.QtCore import Qt, pyqtSlot, pyqtSignal
 
+from .utils import ColorWithSlidersWidget
 
-class LineWidthSlider(AlphaSlider):
-    def enterEvent(self, e):
-        if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(),
-                "<h3>Linewidth</h3> Set the linewidth of the shape boundary.",
-            )
+_log = logging.getLogger(__name__)
 
 
 class SaveButton(QtWidgets.QPushButton):
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
@@ -39,14 +25,45 @@
                 e.globalPos(),
                 "<h3>Remove Polygons</h3> Successivlely remove the most recently "
                 "created polygons from the map.",
             )
 
 
 class PolyButton(QtWidgets.QPushButton):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.setCheckable(True)
+
+        self.setStyleSheet(
+            """
+            PolyButton {
+                border-radius: 5px;
+                border-width: 1px;
+                border-style: solid;
+                border-color: rgb(100, 100, 100);
+                background-color: rgb(220, 220, 220);
+                padding: 3px
+                }
+
+            PolyButton:pressed {
+                background-color: rgb(150, 150, 150);
+                }
+
+            PolyButton:hover:!pressed {
+                background-color: rgb(180, 180, 180);
+                }
+
+            PolyButton:checked {
+                background-color: rgb(180, 0, 0);
+                border-color: rgb(100, 0, 0);
+                }
+            """
+        )
+
     def enterEvent(self, e):
         if self.window().showhelp is True:
             name = self.text()
             if name == "Polygon":
                 txt = (
                     "<h3>Draw a Polygon</h3>"
                     "Draw an arbitrary polygon on the map."
@@ -100,14 +117,15 @@
         self.m = m
 
         self.setTabsClosable(True)
         self.tabCloseRequested.connect(self.close_handler)
 
         w = self._get_new_drawer()
         self.addTab(w, "0")
+        self.update_tab_icon(w=w)
 
         # a tab that is used to create new tabs
         newtabwidget = QtWidgets.QWidget()
         newtablayout = QtWidgets.QHBoxLayout()
         l = QtWidgets.QLabel("Click on <b>+</b> to open a new drawer tab!")
         newtablayout.addWidget(l)
         newtabwidget.setLayout(newtablayout)
@@ -115,14 +133,45 @@
         self.addTab(newtabwidget, "+")
         # don't show the close button for this tab
         self.tabBar().setTabButton(self.count() - 1, self.tabBar().RightSide, None)
 
         self.tabBarClicked.connect(self.tabbar_clicked)
         self.setCurrentIndex(0)
 
+        self.setStyleSheet(
+            """
+            QTabWidget::pane {
+              border: 0px;
+              top:0px;
+              background: rgb(150, 150, 150);
+              border-radius: 10px;
+            }
+
+            QTabBar::tab {
+              background: rgb(185, 185, 185);
+              border: 0px;
+              padding: 3px;
+              padding-bottom: 6px;
+              padding-left: 6px;
+              padding-right: 6px;
+              margin-left: 10px;
+              margin-bottom: -2px;
+              border-radius: 4px;
+              font-weight: normal;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(150, 150, 150);
+              border: 0px;
+              margin-bottom: -2px;
+              font-weight: normal;
+            }
+            """
+        )
+
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
                 "<h3>Draw Shape Tabs</h3>"
                 "Each tab represents a ShapeDrawer that can be used to draw shapes "
                 "on the map."
@@ -135,25 +184,29 @@
             )
 
     @pyqtSlot(int)
     def tabbar_clicked(self, index):
         if self.tabText(index) == "+":
             w = self._get_new_drawer()
             self.insertTab(self.count() - 1, w, "0")
+            self.update_tab_icon(w=w)
 
     @pyqtSlot(int)
     def close_handler(self, index):
         curridx = self.currentIndex()
         drawerwidget = self.widget(index)
 
         try:
             while len(drawerwidget.drawer._artists) > 0:
                 drawerwidget.drawer.remove_last_shape()
         except Exception:
-            print("EOmaps: Encountered some problems while clearing the drawer!")
+            _log.error(
+                "EOmaps: Encountered some problems while clearing the drawer!",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
 
         self.m.BM.update()
 
         self.removeTab(index)
         if index == curridx:
             self.setCurrentIndex(index - 1)
 
@@ -163,85 +216,108 @@
         def cb():
             npoly = len(w.drawer._artists)
             idx = self.indexOf(w)
             self.setTabText(idx, str(npoly))
 
         w.drawer._on_new_poly.append(cb)
         w.drawer._on_poly_remove.append(cb)
-
+        w.colorSelected.connect(self.update_tab_icon)
         return w
 
     def set_layer(self, layer):
         for i in range(self.count()):
             if self.tabText(i) != "+":
                 self.widget(i).set_layer(layer)
 
+    @pyqtSlot()
+    def update_tab_icon(self, w=None):
+        if w is None:
+            w = self.sender()
+        self.setTabIcon(self.indexOf(w), w.get_tab_icon())
+
 
 class DrawerWidget(QtWidgets.QWidget):
 
+    colorSelected = pyqtSignal()
+
     _polynames = {
         "Polygon": "polygon",
         "Rectangle": "rectangle",
         "Circle": "circle",
     }
 
-    def __init__(self, m=None, *args, **kwargs):
+    def __init__(self, *args, m=None, **kwargs):
 
         super().__init__(*args, **kwargs)
 
         self.m = m
 
         self.save_button = SaveButton("  Save Polygons  ")
         self.save_button.setMaximumSize(self.save_button.sizeHint())
         self.save_button.setEnabled(False)
 
         self.remove_button = RemoveButton("Remove")
         self.remove_button.setMaximumSize(self.remove_button.sizeHint())
         self.remove_button.setEnabled(False)
 
+        self.cancel_button = RemoveButton("Cancel")
+        self.cancel_button.setMaximumSize(self.cancel_button.sizeHint())
+        self.cancel_button.setEnabled(False)
+
         self._new_drawer()
 
         self.save_button.clicked.connect(self.save_shapes)
         self.remove_button.clicked.connect(self.remove_last_shape)
+        self.cancel_button.clicked.connect(self.cancel_draw)
 
-        polybuttons = []
+        self.polybuttons = []
         for name, poly in self._polynames.items():
             poly_b = PolyButton(name)
             poly_b.clicked.connect(self.draw_shape_callback(poly=poly))
             poly_b.setMaximumWidth(100)
-            polybuttons.append(poly_b)
-
-        self.colorselector = GetColorWidget()
+            self.polybuttons.append(poly_b)
 
-        self.alphaslider = TransparencySlider(Qt.Horizontal)
-        self.alphaslider.valueChanged.connect(self.set_alpha_with_slider)
-        self.alphaslider.setValue(50)
+        b_layout = QtWidgets.QVBoxLayout()
+        b_layout.setContentsMargins(0, 0, 0, 0)
+        b_layout.setSpacing(2)
 
-        self.linewidthslider = LineWidthSlider(Qt.Horizontal)
-        self.linewidthslider.valueChanged.connect(self.set_linewidth_with_slider)
-        self.linewidthslider.setValue(20)
+        for b in self.polybuttons:
+            b_layout.addWidget(b)
 
         save_layout = QtWidgets.QVBoxLayout()
         save_layout.addWidget(self.save_button)
         save_layout.addWidget(self.remove_button)
+        save_layout.addWidget(self.cancel_button)
 
-        b_layout = QtWidgets.QVBoxLayout()
-        for b in polybuttons:
-            b_layout.addWidget(b)
-
-        layout = QtWidgets.QGridLayout()
-        layout.addWidget(self.colorselector, 0, 0, 2, 1)
-        layout.addWidget(self.alphaslider, 0, 1)
-        layout.addWidget(self.linewidthslider, 1, 1)
-        layout.addLayout(b_layout, 0, 2, 2, 1)
-        layout.addLayout(save_layout, 0, 3, 2, 1)
-
-        layout.setAlignment(Qt.AlignCenter | Qt.AlignTop)
+        self.colorselector = ColorWithSlidersWidget(linewidth=1)
+        self.colorselector.colorSelected.connect(lambda: self.colorSelected.emit())
+        self.colorselector.layout().setContentsMargins(0, 0, 0, 0)
+
+        layout = QtWidgets.QHBoxLayout()
+        layout.addLayout(b_layout)
+        layout.addLayout(save_layout)
+        layout.addWidget(self.colorselector)
+        layout.setAlignment(Qt.AlignLeft | Qt.AlignTop)
         self.setLayout(layout)
 
+        self.m._connect_signal("drawFinished", self.uncheck_polybuttons)
+        self.m._connect_signal("drawAborted", self.uncheck_polybuttons)
+        self.m._connect_signal("drawStarted", self.check_polybuttons)
+
+    def check_polybuttons(self, poly):
+        for b in self.polybuttons:
+            if b.text() == poly:
+                b.setChecked(True)
+        self.cancel_button.setEnabled(True)
+
+    def uncheck_polybuttons(self):
+        for b in self.polybuttons:
+            b.setChecked(False)
+        self.cancel_button.setEnabled(False)
+
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
                 "<h3>Draw Shapes on the Map</h3>"
                 "A widget to draw simple shapes on the map."
                 "<p>"
@@ -263,22 +339,25 @@
                 "For any shape, the added points can be undone by successively "
                 "clicking the right mouse button.",
             )
 
     def draw_shape_callback(self, poly):
         @pyqtSlot()
         def cb():
-            self.window().hide()
-            self.m.f.canvas.show()
-            self.m.f.canvas.activateWindow()
+            s = self.sender()
+            for b in self.polybuttons:
+                if s is b:
+                    b.setChecked(True)
+                else:
+                    b.setChecked(False)
 
             getattr(self.drawer, poly)(
                 facecolor=self.colorselector.facecolor.getRgbF(),
                 edgecolor=self.colorselector.edgecolor.getRgbF(),
-                linewidth=self.linewidthslider.alpha * 10,
+                linewidth=self.colorselector.linewidth,
             )
 
         return cb
 
     @pyqtSlot()
     def _new_poly_cb(self):
         # callback executed on creation of a new polygon
@@ -306,41 +385,77 @@
                 filter="Shapefiles (*.shp)",
             )
             if save_path is not None and len(save_path) > 0:
                 self.drawer.save_shapes(save_path)
                 # after saving the polygons, start with a new drawer
                 self._new_drawer()
         except Exception:
-            print(
-                "EOmaps: Encountered a problem while trying to save " "drawn shapes..."
+            _log.error(
+                "EOmaps: Encountered a problem while trying to save " "drawn shapes...",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
             )
 
     @pyqtSlot()
     def remove_last_shape(self):
         try:
             self.drawer.remove_last_shape()
             # update to make sure the changes are reflected on the map immediately
             self.m.BM.update()
         except Exception:
-            print(
+            _log.error(
                 "EOmaps: Encountered a problem while trying to remove "
-                "the last drawn shape..."
+                "the last drawn shape...",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
             )
 
-    @pyqtSlot(int)
-    def set_alpha_with_slider(self, i):
-        self.colorselector.set_alpha(i / 100)
-
-    @pyqtSlot(int)
-    def set_linewidth_with_slider(self, i):
-        self.colorselector.set_linewidth(i / 10)
+    @pyqtSlot()
+    def cancel_draw(self):
+        self.drawer._finish_drawing()
 
     def _new_drawer(self):
         self.drawer = self.m.draw.new_drawer()
         self.save_button.setEnabled(False)
         self.remove_button.setEnabled(False)
 
         self.drawer._on_new_poly.append(self._new_poly_cb)
         self.drawer._on_poly_remove.append(self._new_poly_cb)
 
     def set_layer(self, layer):
         self.drawer.set_layer(layer)
+
+    @pyqtSlot()
+    def get_tab_icon(self):
+        from PyQt5 import QtGui
+        from PyQt5.QtCore import QRectF
+
+        canvas = QtGui.QPixmap(20, 20)
+        canvas.fill(Qt.transparent)
+
+        painter = QtGui.QPainter(canvas)
+        painter.setRenderHints(QtGui.QPainter.HighQualityAntialiasing)
+
+        painter.setBrush(QtGui.QBrush(self.colorselector.facecolor, Qt.SolidPattern))
+
+        if self.colorselector.linewidth > 0.01:
+            painter.setPen(
+                QtGui.QPen(
+                    self.colorselector.edgecolor,
+                    0.5 * self.colorselector.linewidth,
+                    Qt.SolidLine,
+                )
+            )
+        else:
+            painter.setPen(
+                QtGui.QPen(
+                    self.colorselector.facecolor,
+                    0.5 * self.colorselector.linewidth,
+                    Qt.SolidLine,
+                )
+            )
+
+        rect = QRectF(2.5, 2.5, 15, 15)
+        painter.drawRoundedRect(rect, 5, 5)
+        painter.end()
+
+        icon = QtGui.QIcon(canvas)
+
+        return icon
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/editor.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/editor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+import logging
+
 from PyQt5 import QtCore, QtWidgets, QtGui
-from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QSize
+from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QPointF
+from PyQt5.QtGui import QFont
 
 from matplotlib.colors import to_rgba_array
 
-from ...eomaps import InsetMaps
+from ...inset_maps import InsetMaps
 from ..common import iconpath
+from ..base import BasicCheckableToolButton
 from .wms import AddWMSMenuButton
-from .utils import GetColorWidget, AlphaSlider
-from .annotate import AddAnnotationInput
+from .utils import ColorWithSlidersWidget, GetColorWidget, AlphaSlider
+from .annotate import AddAnnotationWidget
 from .draw import DrawerTabs
+from .files import OpenDataStartTab
+from .layer import AutoUpdateLayerMenuButton
+
+_log = logging.getLogger(__name__)
 
 
 class AddFeaturesMenuButton(QtWidgets.QPushButton):
     FeatureAdded = pyqtSignal(str)
 
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
@@ -60,16 +68,19 @@
                     if not i.startswith("_")
                 ]
                 for feature in sub_features:
                     action = sub_menu.addAction(str(feature))
                     action.triggered.connect(
                         self.menu_callback_factory(featuretype, feature)
                     )
-            except:
-                print("there was a problem with the NaturalEarth feature", featuretype)
+            except Exception:
+                _log.warning(
+                    f"There was a problem with the NaturalEarth feature: {featuretype}",
+                    exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+                )
                 continue
 
         self._menu_fetched = True
 
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
@@ -114,49 +125,33 @@
                     f(layer=layer, **f.kwargs)
                 else:
                     f(layer=layer, **self.props)
 
                 self.m.f.canvas.draw_idle()
                 self.FeatureAdded.emit(str(layer))
             except Exception:
-                import traceback
-
-                print(
-                    "---- adding the feature", featuretype, feature, "did not work----"
+                _log.error(
+                    "---- adding the feature",
+                    featuretype,
+                    feature,
+                    "did not work----",
+                    exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
                 )
-                print(traceback.format_exc())
 
         return cb
 
 
 class ZorderInput(QtWidgets.QLineEdit):
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
-                "<h3>Zorder</h3> Set the zorder of the artist (e.g. the vertical "
-                "stacking order with respect to other artists in the figure)",
-            )
-
-
-class TransparencySlider(AlphaSlider):
-    def enterEvent(self, e):
-        if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(),
-                "<h3>Facecolor Transparency</h3> "
-                "Set the transparency for the facecolor of the feature.",
-            )
-
-
-class LinewidthSlider(AlphaSlider):
-    def enterEvent(self, e):
-        if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(), "<h3>Linewidth</h3> Set the linewidth of the feature"
+                "<h3>Zorder</h3>"
+                "Set the zorder of the artist (e.g. the vertical stacking "
+                "order with respect to other artists on the same layer)",
             )
 
 
 class RemoveArtistToolButton(QtWidgets.QToolButton):
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
@@ -168,15 +163,16 @@
 
 class ShowHideToolButton(QtWidgets.QToolButton):
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
                 "<h3>Show/Hide Artist</h3>"
-                "Make the corresponding artist visible (eye open) or invisible (eye closed).",
+                "Make the corresponding artist visible (eye open) "
+                "or invisible (eye closed).",
             )
 
 
 class LineWidthInput(QtWidgets.QLineEdit):
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
@@ -194,90 +190,71 @@
             )
 
 
 class AddFeatureWidget(QtWidgets.QFrame):
     def __init__(self, m=None):
 
         super().__init__()
-        self.setFrameStyle(QtWidgets.QFrame.StyledPanel | QtWidgets.QFrame.Plain)
+        # self.setFrameStyle(QtWidgets.QFrame.StyledPanel | QtWidgets.QFrame.Plain)
 
         self.m = m
 
         self.selector = AddFeaturesMenuButton(m=self.m)
         self.selector.clicked.connect(self.update_props)
 
-        self.colorselector = GetColorWidget(facecolor="#aaaa7f")
-        self.colorselector.cb_colorselected = self.update_on_color_selection
+        self.selector.menu().aboutToShow.connect(self.update_props)
 
-        self.alphaslider = TransparencySlider(Qt.Horizontal)
-        self.alphaslider.valueChanged.connect(self.set_alpha_with_slider)
-        self.alphaslider.valueChanged.connect(self.update_props)
-
-        self.linewidthslider = LinewidthSlider(Qt.Horizontal)
-        self.linewidthslider.valueChanged.connect(self.set_linewidth_with_slider)
-        self.linewidthslider.valueChanged.connect(self.update_props)
-        self.set_linewidth_slider_stylesheet()
+        self.colorselector = ColorWithSlidersWidget(facecolor="#aaaa7f")
 
         self.zorder = ZorderInput("0")
         validator = QtGui.QIntValidator()
         self.zorder.setValidator(validator)
         self.zorder.setMaximumWidth(30)
+        self.zorder.setMaximumHeight(20)
         self.zorder.setSizePolicy(
             QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
         )
         self.zorder.textChanged.connect(self.update_props)
 
         zorder_label = QtWidgets.QLabel("zorder: ")
         zorder_label.setSizePolicy(
             QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
         )
 
         zorder_layout = QtWidgets.QHBoxLayout()
         zorder_layout.addWidget(zorder_label)
-        zorder_layout.addWidget(self.zorder)
+        zorder_layout.addWidget(self.zorder, 0)
         zorder_label.setAlignment(Qt.AlignRight | Qt.AlignCenter)
 
-        layout = QtWidgets.QGridLayout()
-        layout.addWidget(self.colorselector, 0, 0, 2, 1)
-        layout.addWidget(self.alphaslider, 0, 1)
-        layout.addWidget(self.linewidthslider, 1, 1)
-        layout.addLayout(zorder_layout, 0, 2)
-        layout.addWidget(self.selector, 1, 2)
-
-        # set stretch factor to expand the color-selector first
-        layout.setColumnStretch(0, 1)
-
-        layout.setAlignment(Qt.AlignCenter | Qt.AlignTop)
-        self.setLayout(layout)
-
-        # do this at the end to ensure everything has already been set up properly
-        self.alphaslider.setValue(100)
-        self.linewidthslider.setValue(20)
-
-        self.update_props()
+        layout_buttons = QtWidgets.QVBoxLayout()
+        layout_buttons.addWidget(self.selector)
+        layout_buttons.addLayout(zorder_layout)
+
+        layout = QtWidgets.QHBoxLayout()
+        layout.addLayout(layout_buttons)
+        layout.addWidget(self.colorselector)
+        layout.setAlignment(Qt.AlignLeft | Qt.AlignCenter)
+
+        layout_tight = QtWidgets.QVBoxLayout()
+        layout_tight.addStretch(1)
+        layout_tight.addLayout(layout)
+        layout_tight.addStretch(1)
 
-    @pyqtSlot(int)
-    def set_alpha_with_slider(self, i):
-        self.colorselector.set_alpha(i / 100)
-
-    @pyqtSlot(int)
-    def set_linewidth_with_slider(self, i):
-        self.colorselector.set_linewidth(i / 10)
+        self.setLayout(layout_tight)
 
     @pyqtSlot()
     def update_props(self):
-        self.set_alpha_slider_stylesheet()
-
+        # don't specify alpha! it interferes with the alpha of the colors!
         self.selector.props.update(
             dict(
                 facecolor=self.colorselector.facecolor.getRgbF(),
                 edgecolor=self.colorselector.edgecolor.getRgbF(),
-                linewidth=self.linewidthslider.alpha * 5,
+                linewidth=self.colorselector.linewidth,
                 zorder=int(self.zorder.text()),
-                # alpha = self.alphaslider.alpha,   # don't specify alpha! it interferes with the alpha of the colors!
+                # alpha = self.colorselector.alpha,
             )
         )
 
     def set_linewidth_slider_stylesheet(self):
         self.linewidthslider.setStyleSheet(
             """
             QSlider::handle:horizontal {
@@ -323,151 +300,95 @@
             }}
             QSlider::groove:horizontal:hover {{
                 background-color: rgba(0,0,0,255);
             }}
             """
         )
 
-    def update_on_color_selection(self):
-        self.update_alphaslider()
-        self.update_props()
-
     def update_alphaslider(self):
         # to always round up to closest int use -(-x//1)
         self.alphaslider.setValue(int(-(-self.colorselector.alpha * 100 // 1)))
 
 
-class NewLayerLineEdit(QtWidgets.QLineEdit):
+class OpenFileButton(QtWidgets.QPushButton):
     def enterEvent(self, e):
-        if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(),
-                "<h3>New Layer</h3>"
-                "Enter a layer-name and press <b>enter</b> to create "
-                "a new (empty) layer on the map!"
-                "<p>"
-                "NTOE: The tab of the new layer will be activated once the layer is "
-                "created, but it is NOT automatically set as the visible layer!",
-            )
-
-
-class NewLayerWidget(QtWidgets.QFrame):
-    NewLayerCreated = pyqtSignal(str)
+        OpenDataStartTab.enterEvent(self, e)
 
-    def __init__(self, *args, m=None, **kwargs):
 
+class PlusButton(BasicCheckableToolButton):
+    def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.m = m
-
-        new_layer_label = QtWidgets.QLabel("<b>Create a new layer:</b>")
-        self.new_layer_name = NewLayerLineEdit()
-        self.new_layer_name.setMaximumWidth(300)
-        self.new_layer_name.setPlaceholderText("my_layer")
-        self.new_layer_name.returnPressed.connect(self.new_layer)
-
-        try:
-            self.addwms = AddWMSMenuButton(m=self.m, new_layer=False)
-        except:
-            self.addwms = None
-
-        newlayer = QtWidgets.QHBoxLayout()
-        newlayer.setAlignment(Qt.AlignLeft)
-
-        if self.addwms is not None:
-            newlayer.addWidget(self.addwms)
-        newlayer.addStretch(1)
-        newlayer.addWidget(new_layer_label)
-        newlayer.addWidget(self.new_layer_name)
-
-        # addfeature = AddFeatureWidget(m=self.m)
-
-        layout = QtWidgets.QVBoxLayout()
-        # layout.addWidget(addfeature)
-        layout.addLayout(newlayer)
-        self.setLayout(layout)
-
-    @pyqtSlot()
-    def new_layer(self):
-        # use .strip() to make sure the layer does not start or end with whitespaces
-        layer = self.new_layer_name.text().strip()
-        if len(layer) == 0:
-            QtWidgets.QToolTip.showText(
-                self.mapToGlobal(self.new_layer_name.pos()),
-                "Type a layer-name and press return!",
-            )
-            return
+        self.set_icons(
+            normal_icon=str(iconpath / "plus.png"),
+            hoover_icon=str(iconpath / "plus_hoover.png"),
+        )
 
-        m2 = self.m.new_layer(layer)
-        self.NewLayerCreated.emit(layer)
-        self.new_layer_name.clear()
-        # self.m.show_layer(layer)
+        self.setFixedSize(30, 30)
+        self.setCheckable(False)
 
-        return m2
+        self.setStyleSheet("PlusButton {border: 0}")
 
 
 class LayerArtistTabs(QtWidgets.QTabWidget):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        stylesheet = """
-            QTabWidget::pane { /* The tab widget frame */
-                border-top: 0px solid rgb(100,100,100);
-            }
-
-            QTabWidget::tab-bar {
-                left: 5px; /* move to the right by 5px */
-            }
-
-            QTabBar::tab {
-                background: qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1,
-                                            stop: 0 #E1E1E1, stop: 0.4 #DDDDDD,
-                                            stop: 0.5 #D8D8D8, stop: 1.0 #D3D3D3);
-                border-bottom-color: none;
-                border-top-left-radius: 2px;
-                border-top-right-radius: 2px;
-                min-width: 50px;
-                padding: 1px;
-                margin: 1px;
-            }
+    plusClicked = pyqtSignal()
 
-            QTabBar::tab:selected, QTabBar::tab:hover {
-                border: 1px solid black;
-                background: qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1,
-                                            stop: 0 #fafafa, stop: 0.4 #f4f4f4,
-                                            stop: 0.5 #e7e7e7, stop: 1.0 #fafafa);
-            }
-
-            QTabBar::tab:selected {
-                padding: 0px;
-                border: 2px solid rgb(200,0,0);
-                border-top-left-radius: 4px;
-                border-top-right-radius: 4px;
-                border-bottom-color: rgb(100,100,100); /* same as pane color */
-            }
-
-            QTabBar::tab:!selected {
-                border: 1px solid rgb(200,200,200);
-                margin-top: 4px; /* make non-selected tabs look smaller */
-            }
-            """
+    def __init__(self, *args, m=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.m = m
+        self.margin_left = 25
+        self.margin_right = 60
 
-        self.setStyleSheet(stylesheet)
+        # Plus Button
+        self.plus_button = PlusButton(self)
+        self.plus_button.clicked.connect(self.plusClicked.emit)
+
+        self.layer_button = AutoUpdateLayerMenuButton(self, m=self.m)
+        self.layer_button.setFixedWidth(30)
+
+        self.move_plus_button()  # Move to the correct location
+        self.move_layer_button()  # Move to the correct location
+
+    def move_plus_button(self, *args, **kwargs):
+        """Move the plus button to the correct location."""
+        # Set the plus button location in a visible area
+        h = self.geometry().top()
+        w = self.window().width()
+
+        self.plus_button.move(w - self.margin_right, -3)
+
+    def move_layer_button(self, *args, **kwargs):
+        """Move the plus button to the correct location."""
+        # Set the plus button location in a visible area
+        h = self.geometry().top()
+
+        self.layer_button.move(-5, 2)
+
+    def paintEvent(self, *args, **kwargs):
+        # make some space for the + button
+        self.tabBar().setFixedWidth(
+            self.window().width() - self.margin_left - self.margin_right
+        )
+        self.tabBar().move(self.margin_left, 0)
+        self.move_plus_button()
+        self.move_layer_button()
+        super().paintEvent(*args, **kwargs)
 
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
                 "<h3>Background Layers and Artists</h3>"
                 "Each tab represents a layer of the map."
                 "<ul>"
                 "<li>The tab-order represents the stacking order of the layers.</li>"
                 "<li><b>drag</b> tabs to change the layer ordering!</li>"
                 "</ul>"
                 "<ul>"
-                "<li><b>click</b> on a tab to select it (e.g. to add/remove features)</li>"
+                "<li><b>click</b> on a tab to select it (to add/remove features)</li>"
                 "<li><b>control + click</b> on a tab to make it the visible layer.</li>"
                 "<li><b>shift + click</b> on tabs to make multiple layers visible.</li>"
                 "</ul>"
                 "The tab-entries show all individual <b>background</b> artists of the "
                 "selected layer. (background artists are static map-elements that are "
                 "only re-drawn on pan/zoom or resize events)"
                 "<br>"
@@ -491,16 +412,27 @@
                 "to the map.</li>"
                 "<li><b>Draw Shapes:</b> Draw basic shapes on the map and optionally "
                 "save the shapes as geo-coded shapefiles.</li>"
                 "</ul>",
             )
 
 
+class LayerTransparencySlider(AlphaSlider):
+    _alphas = dict()
+
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Layer Transparency</h3> Set the global layer transparency.",
+            )
+
+
 class LayerTabBar(QtWidgets.QTabBar):
-    _number_of_min_tabs_for_size = 8
+    _number_of_min_tabs_for_size = 6
     _n_layer_msg_shown = False
 
     def __init__(self, m=None, populate=False, *args, **kwargs):
         """
         Parameters
         ----------
         m : eomaps.Maps
@@ -543,21 +475,105 @@
             # NOTE this is done by the TabWidget if tabs have content!!
             self.populate()
             # re-populate on show to make sure currently active layers are shown
             self.m.BM.on_layer(self.populate_on_layer, persistent=True)
             self.m._after_add_child.append(self.populate)
             self.m._on_show_companion_widget.append(self.populate)
 
-    def sizeHint(self):
-        # make sure the TabBar does not expand the window width
+        # set font properties before the stylesheet to avoid clipping of bold text!
+        font = QFont("sans seriv", 8, QFont.Bold, False)
+        self.setFont(font)
 
-        hint = super().sizeHint()
-        width = self.window().width()
-        hint.setWidth(width)
-        return hint
+        self.setStyleSheet(
+            """
+            QTabWidget::pane {
+              border: 0px;
+              top:0px;
+              background: rgb(200, 200, 200);
+              border-radius: 10px;
+            }
+
+            QTabBar::tab {
+              background: rgb(245, 245, 245);
+              border: 1px solid black;
+              padding: 3px;
+              margin-left: 2px;
+              margin-bottom: 0px;
+              border-radius: 4px;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(245, 245, 245);
+              border: 1px solid black;
+              margin-bottom: 0px;
+            }
+            """
+        )
+
+    def event(self, event):
+        # don't show normal tooltips while showhelp is active
+        # (they would cause the help-popups to disappear after ~ 1 sec)
+        if event.type() == QtCore.QEvent.ToolTip and self.window().showhelp:
+            return
+
+        return super().event(event)
+
+    def mousePressEvent(self, event):
+        # TODO a more clean implementation of this would be nice
+        # explicitly handle control+click and shift+click events
+        # to avoid activating the currently clicked tab
+        # (we want to activate the currently active tab which is shifted to the
+        # start-position!)
+        modifiers = QtWidgets.QApplication.keyboardModifiers()
+        if (
+            modifiers == Qt.ControlModifier
+            and event.button() == Qt.MouseButton.LeftButton
+        ):
+
+            idx = self.tabAt(event.pos())
+            self.tabchanged(idx)
+        elif (
+            modifiers == Qt.ShiftModifier
+            and event.button() == Qt.MouseButton.LeftButton
+        ):
+            idx = self.tabAt(event.pos())
+            self.tabchanged(idx)
+        else:
+            super().mousePressEvent(event)
+
+    @pyqtSlot()
+    def get_tab_icon(self, color="red"):
+        if isinstance(color, str):
+            color = QtGui.QColor(color)
+        elif isinstance(color, (list, tuple)):
+            color = QtGui.QColor(*color)
+
+        canvas = QtGui.QPixmap(20, 20)
+        canvas.fill(Qt.transparent)
+
+        painter = QtGui.QPainter(canvas)
+        painter.setRenderHints(QtGui.QPainter.HighQualityAntialiasing)
+
+        pencolor = QtGui.QColor(color)
+        pencolor.setAlpha(100)
+        painter.setPen(QtGui.QPen(pencolor, 2, Qt.SolidLine))
+        painter.setBrush(QtGui.QBrush(color, Qt.SolidPattern))
+
+        painter.drawEllipse(QPointF(10, 12), 7, 7)
+        painter.end()
+
+        icon = QtGui.QIcon(canvas)
+        return icon
+
+    # def sizeHint(self):
+    #     # make sure the TabBar does not expand the window width
+    #     hint = super().sizeHint()
+    #     width = self.window().width()
+    #     hint.setWidth(width)
+    #     return hint
 
     def minimumTabSizeHint(self, index):
         # the minimum width of the tabs is determined such that at least
         # "_number_of_min_tabs_for_size"  tabs are visible.
         # (e.g. for the elide of long tab-names)
 
         hint = super().tabSizeHint(index)
@@ -568,17 +584,17 @@
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
                 "<h3>Layer Tabs</h3>"
                 "Select, combine and re-arrange layers of the map. "
                 "<ul>"
-                "<li><b>control + click</b> to make the selected layer visible.</li>"
-                "<li><b>shift + click</b> to select multiple layers. </li>"
-                "<li><b>drag</b> layers to change the stacking-order. "
+                "<li><b>ctrl + click:</b> make selected layer visible</li>"
+                "<li><b>shift + click:</b> select multiple layers </li>"
+                "<li><b>drag:</b> change the layer stacking-order. "
                 "</ul>",
             )
 
     def repopulate_and_activate_current(self, *args, **kwargs):
         self.populate()
 
         # activate the currently visible layer tab
@@ -588,40 +604,44 @@
             )
             self.setCurrentIndex(idx)
         except StopIteration:
             pass
 
     @pyqtSlot()
     def tab_moved(self):
-        currlayers = self.m.BM.bg_layer.split("|")
+        # get currently active layers
+        active_layers, alphas = self.m.BM._get_layers_alphas()
 
         # get the name of the layer that was moved
         layer = self.tabText(self.currentIndex())
-        if layer not in currlayers:
+        if layer not in active_layers:
             return
 
         # get the current ordering of visible layers
         ntabs = self.count()
         layer_order = []
         for i in range(ntabs):
-            l = self.tabText(i)
-            if l in currlayers:
-                layer_order.append(self.tabText(i))
+            txt = self.tabText(i)
+            if txt in active_layers:
+                layer_order.append(txt)
 
         # set the new layer-order
-        if currlayers != layer_order:  # avoid recursions
-            self.m.BM.bg_layer = "|".join(layer_order)
-            self.m.BM.update()
+        if active_layers != layer_order:  # avoid recursions
+            alpha_order = [alphas[active_layers.index(i)] for i in layer_order]
+            self.m.show_layer(*zip(layer_order, alpha_order))
 
     @pyqtSlot(int)
     def close_handler(self, index):
         layer = self.tabText(index)
 
         self._msg = QtWidgets.QMessageBox(self)
         self._msg.setIcon(QtWidgets.QMessageBox.Question)
+
+        self._msg.setWindowIcon(QtGui.QIcon(str(iconpath / "info.png")))
+
         self._msg.setText(f"Do you really want to delete the layer '{layer}'")
         self._msg.setWindowTitle(f"Delete layer: '{layer}'?")
 
         self._msg.setStandardButtons(
             QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No
         )
         self._msg.buttonClicked.connect(self.get_close_tab_cb(index))
@@ -639,50 +659,49 @@
 
         if self._msg.standardButton(self._msg.clickedButton()) != self._msg.Yes:
             return
 
         layer = self.tabText(index)
 
         if self.m.layer == layer:
-            print("can't delete the base-layer")
+            _log.error("EOmaps: The base-layer cannot be deleted!")
             return
 
         # get currently active layers
-        active_with_transp = self.m.BM.bg_layer.split("|")
-        # strip off transparency assignments
-        active_layers = [i.split("{")[0] for i in active_with_transp]
+        active_layers, alphas = self.m.BM._get_layers_alphas()
 
         # cleanup the layer and remove any artists etc.
         for m in list(self.m._children):
             if layer == m.layer:
                 m.cleanup()
                 m.BM._bg_layers.pop(layer, None)
 
         # in case the layer was visible, try to activate a suitable replacement
         if layer in active_layers:
             # if possible, show the currently active multi-layer but without
             # the deleted layer
             layer_idx = active_layers.index(layer)
-            active_with_transp.pop(layer_idx)
+            active_layers.pop(layer_idx)
+            alphas.pop(layer_idx)
 
-            if len(active_with_transp) > 0:
+            if len(active_layers) > 0:
                 try:
-                    self.m.show_layer(*active_with_transp)
+                    self.m.show_layer(*zip(active_layers, alphas))
                 except Exception:
                     pass
             else:
                 # otherwise switch to the first available layer
                 try:
                     switchlayer = next(
                         (i for i in self.m.BM._bg_artists if layer not in i.split("|"))
                     )
                     self.m.show_layer(switchlayer)
                 except StopIteration:
                     # don't allow deletion of last layer
-                    print("you cannot delete the last available layer!")
+                    _log.error("EOmaps: Unable to delete the last available layer!")
                     return
 
         if layer in list(self.m.BM._bg_artists):
             for a in self.m.BM._bg_artists[layer]:
                 self.m.BM.remove_bg_artist(a)
                 a.remove()
             del self.m.BM._bg_artists[layer]
@@ -699,80 +718,85 @@
 
         for permanent, d in self.m.BM._on_layer_change.items():
             if layer in d:
                 del d[layer]
 
         self.populate()
 
-    def color_active_tab(self, m=None, layer=None):
-        currlayers = self.m.BM.bg_layer.split("|")
-
-        defaultcolor = self.palette().color(self.foregroundRole())
-        activecolor = QtGui.QColor(50, 200, 50)
-        multicolor = QtGui.QColor(200, 50, 50)
+    def color_active_tab(self, m=None, layer=None, adjust_order=True):
+        # defaultcolor = self.palette().color(self.foregroundRole())
+        defaultcolor = QtGui.QColor(100, 100, 100)
+        activecolor = QtGui.QColor(50, 150, 50)  # QtGui.QColor(0, 128, 0)
+        multicolor = QtGui.QColor(50, 150, 50)  # QtGui.QColor(0, 128, 0)
 
-        active_layers = set(self.m.BM._bg_layer.split("|"))
-        active_layers.add(self.m.BM._bg_layer)
-
-        if "{" in self.m.BM._bg_layer:  # TODO support transparency
-            for i in range(self.count()):
-                self.setTabTextColor(i, defaultcolor)
-            return
+        # get currently active layers
+        active_layers, alphas = self.m.BM._get_layers_alphas()
 
         for i in range(self.count()):
-
             selected_layer = self.tabText(i)
-
             color = activecolor if len(active_layers) == 1 else multicolor
             if selected_layer in active_layers:
+                idx = active_layers.index(selected_layer)
                 self.setTabTextColor(i, color)
+
+                if alphas[idx] < 1:
+                    color = QtGui.QColor(color)
+                    color.setAlpha(int(alphas[idx] * 100))
+
+                self.setTabIcon(i, self.get_tab_icon(color))
             else:
                 self.setTabTextColor(i, defaultcolor)
+                self.setTabIcon(i, QtGui.QIcon())
 
             if layer == selected_layer:
                 self.setTabTextColor(i, activecolor)
 
-        # --- adjust the sort-order of the tabs to the order of the visible layers
-        # disconnect tab_moved callback to avoid recursions
-        self.tabMoved.disconnect(self.tab_moved)
-        # to avoid issues with non-existent and private layers (e.g. the background
-        # layer on savefig etc.) use the following strategy:
-        # go through the layers in reverse and move each found layer to the position 0
-        for cl in currlayers[::-1]:
-            for i in range(self.count()):
-                layer = self.tabText(i)
-                if layer == cl:
-                    self.moveTab(i, 0)
-        # re-connect tab_moved callback
-        self.tabMoved.connect(self.tab_moved)
+        if adjust_order:
+            # --- adjust the sort-order of the tabs to the order of the visible layers
+            # disconnect tab_moved callback to avoid recursions
+            self.tabMoved.disconnect(self.tab_moved)
+            # to avoid issues with non-existent and private layers (e.g. the background
+            # layer on savefig etc.) use the following strategy:
+            # - go through the layers in reverse
+            # - move each found layer to the position 0
+            for cl in active_layers[::-1]:
+                for i in range(self.count()):
+                    layer = self.tabText(i)
+                    if layer == cl:
+                        self.moveTab(i, 0)
+            # re-connect tab_moved callback
+            self.tabMoved.connect(self.tab_moved)
 
     @pyqtSlot()
     def populate_on_layer(self, *args, **kwargs):
         lastlayer = getattr(self, "_last_populated_layer", "")
         currlayer = self.m.BM.bg_layer
         # only populate if the current layer is not part of the last set of layers
         # (e.g. to allow show/hide of selected layers without removing the tabs)
         if not set(lastlayer.split("|")).issuperset(set(currlayer.split("|"))):
             self.populate(*args, **kwargs)
             self._last_populated_layer = currlayer
+        else:
+            # still update tab colors  (e.g. if layers are removed from multi)
+            self.color_active_tab()
 
     @pyqtSlot()
     def populate(self, *args, **kwargs):
         if not self.isVisible():
             return
 
         self._current_tab_idx = self.currentIndex()
         self._current_tab_name = self.tabText(self._current_tab_idx)
 
         alllayers = set(self.m._get_layers())
         nlayers = len(alllayers)
         max_n_layers = self.m._companion_widget_n_layer_tabs
         if nlayers > max_n_layers:
             if not LayerTabBar._n_layer_msg_shown:
-                print(
+                _log.info(
                     "EOmaps-companion: The map has more than "
                     f"{max_n_layers} layers... only last active layers "
                     "are shown in the layer-tabs!"
                 )
                 LayerTabBar._n_layer_msg_shown = True
 
             # if more than 200 layers are available, show only active tabs to
@@ -808,19 +832,19 @@
             self.addTab(layer)
             self.setTabToolTip(i, layer)
 
             if layer == "all" or layer == self.m.layer:
                 # don't show the close button for this tab
                 self.setTabButton(self.count() - 1, self.RightSide, None)
 
+        self.color_active_tab()
+
         # try to restore the previously opened tab
         self.set_current_tab_by_name(self._current_tab_name)
 
-        self.color_active_tab()
-
     @pyqtSlot(str)
     def set_current_tab_by_name(self, layer):
         if layer is None:
             layer = self.m.BM.bg_layer
 
         found = False
         ntabs = self.count()
@@ -835,68 +859,76 @@
                 self.setCurrentIndex(0)
 
     @pyqtSlot(int)
     def tabchanged(self, index):
         # TODO
         # modifiers are only released if the canvas has focus while the event happens!!
         # (e.g. button is released but event is not fired on the canvas)
-        # see https://stackoverflow.com/questions/60978379/why-alt-modifier-does-not-trigger-key-release-event-the-first-time-you-press-it
+        # see https://stackoverflow.com/q/60978379/9703451
 
         # simply calling  canvas.setFocus() does not work!
 
         # for w in QtWidgets.QApplication.topLevelWidgets():
         #     if w.inherits('QMainWindow'):
         #         w.canvas.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
         #         w.canvas.setFocus()
         #         w.raise_()
-        #         print("raising", w, w.canvas)
+        #         _log.debug("raising", w, w.canvas)
 
         layer = self.tabText(index)
+        if len(layer) == 0:
+            return
 
         modifiers = QtWidgets.QApplication.keyboardModifiers()
         if modifiers == Qt.ControlModifier:
             if layer != "":
-                self.m.show_layer(layer)
+                self.m.show_layer(
+                    (layer, LayerTransparencySlider._alphas.get(layer, 1))
+                )
                 # TODO this is a workaround since modifier-releases are not
                 # forwarded to the canvas if it is not in focus
                 self.m.f.canvas.key_release_event("control")
 
         elif modifiers == Qt.ShiftModifier:
             # The all layer should not be combined with other layers...
             # (it is already visible anyways)
-            if layer == "all" or "|" in layer:
+            if layer == "all" and "|" in layer:
                 return
-            currlayers = [i for i in self.m.BM._bg_layer.split("|") if i != "_"]
 
-            for l in (i for i in layer.split("|") if i != "_"):
-                if l not in currlayers:
-                    currlayers.append(l)
-                else:
-                    currlayers.remove(l)
+            # get currently active layers
+            active_layers, alphas = self.m.BM._get_layers_alphas()
 
-            if len(currlayers) > 1:
-                uselayer = "|".join(currlayers)
+            for x in (i for i in layer.split("|") if i != "_"):
+                if x not in active_layers:
+                    active_layers.append(x)
+                    alphas.append(LayerTransparencySlider._alphas.get(layer, 1))
+                else:
+                    idx = active_layers.index(x)
+                    active_layers.pop(idx)
+                    alphas.pop(idx)
 
-                self.m.show_layer(uselayer)
-            elif len(currlayers) == 1:
-                self.m.show_layer(currlayers[0])
+            if len(active_layers) >= 1:
+                self.m.show_layer(*zip(active_layers, alphas))
             else:
-                self.m.show_layer(layer)
+                self.m.show_layer(
+                    (layer, LayerTransparencySlider._alphas.get(layer, 1))
+                )
             # TODO this is a workaround since modifier-releases are not
             # forwarded to the canvas if it is not in focus
             self.m.f.canvas.key_release_event("shift")
 
         # make sure to reflect the layer-changes in the tab-colors (and positions)
         self.color_active_tab()
 
+        self.set_current_tab_by_name(layer)
+
 
 class ArtistEditorTabs(LayerArtistTabs):
     def __init__(self, m=None):
-        super().__init__()
-        self.m = m
+        super().__init__(m=m)
 
         self.setTabBar(LayerTabBar(m=self.m))
 
         # re-populate tabs if a new layer is created
         self.populate()
         self.m._after_add_child.append(self.populate)
         self.m.BM.on_layer(self.populate_on_layer, persistent=True)
@@ -904,43 +936,94 @@
         self.currentChanged.connect(self.populate_layer)
         self.m.BM._on_add_bg_artist.append(self.populate)
         self.m.BM._on_remove_bg_artist.append(self.populate)
 
         self.m._on_show_companion_widget.append(self.populate)
         self.m._on_show_companion_widget.append(self.populate_layer)
 
+        self.plusClicked.connect(self.new_layer_button_clicked)
+
+        self.setStyleSheet(
+            """
+            QTabWidget::pane {
+                border: 0px;
+                top:0px;
+                background: rgb(240, 240, 240);
+                border-radius: 10px;
+            }
+            QScrollArea {border:0px}
+            """
+        )
+
+    def new_layer_button_clicked(self, *args, **kwargs):
+        inp = QtWidgets.QInputDialog(self)
+        inp.setWindowIcon(QtGui.QIcon(str(iconpath / "plus.png")))
+        inp.setWindowFlags(inp.windowFlags() & ~Qt.WindowContextHelpButtonHint)
+        inp.setInputMode(QtWidgets.QInputDialog.TextInput)
+        inp.setFixedSize(200, 100)
+
+        inp.setWindowTitle("New Layer")
+        inp.setLabelText("Name:")
+
+        if inp.exec_() == QtWidgets.QDialog.Accepted:
+            # use .strip to remove any trailing spaces
+            layer = inp.textValue().strip()
+            # only create layers if at least 1 character has been provided
+            if len(layer) > 0:
+                self.m.new_layer(layer)
+
+        inp.deleteLater()
+
     def repopulate_and_activate_current(self, *args, **kwargs):
         self.populate()
 
         # activate the currently visible layer tab
         try:
             idx = next(
                 i for i in range(self.count()) if self.tabText(i) == self.m.BM._bg_layer
             )
             self.setCurrentIndex(idx)
+
         except StopIteration:
             pass
 
         self.populate_layer()
 
     def _get_artist_layout(self, a, layer):
         # label
-        name = str(a)
-        if len(name) > 50:
-            label = QtWidgets.QLabel(name[:46] + "... >")
+        try:
+            name = a.get_label()
+            if len(name) == 0:
+                name = str(a)
+
+        except Exception:
+            name = str(a)
+
+        # for artists that should not show up in the editor
+        if name.startswith("__EOmaps_exclude"):
+            return [(None, None)]
+        elif name.startswith("__EOmaps_deactivate"):
+            name = name[20:].strip()
+            deactivated = True
+        else:
+            deactivated = False
+
+        if len(name) > 80:
+            label = QtWidgets.QLabel(name[:76] + "... >")
             label.setToolTip(name)
         else:
             label = QtWidgets.QLabel(name)
         label.setStyleSheet(
             "border-radius: 5px;"
             "border-style: solid;"
             "border-width: 1px;"
             "border-color: rgba(0, 0, 0,100);"
+            "padding-left: 10px;"
         )
-        label.setAlignment(Qt.AlignCenter)
+        label.setAlignment(Qt.AlignLeft)
         label.setMaximumHeight(25)
 
         # remove
         b_r = RemoveArtistToolButton()
         b_r.setText("🞪")
         b_r.setAutoRaise(True)
         b_r.setStyleSheet("QToolButton {color: red;}")
@@ -955,16 +1038,16 @@
         else:
             b_sh.setIcon(QtGui.QIcon(str(iconpath / "eye_open.png")))
 
         b_sh.clicked.connect(self.show_hide(artist=a, layer=layer))
 
         # zorder
         b_z = ZorderInput()
-        b_z.setMinimumWidth(25)
-        b_z.setMaximumWidth(25)
+        b_z.setMinimumWidth(30)
+        b_z.setMaximumWidth(30)
         validator = QtGui.QIntValidator()
         b_z.setValidator(validator)
         b_z.setText(str(a.get_zorder()))
         b_z.returnPressed.connect(self.set_zorder(artist=a, layer=layer, widget=b_z))
 
         # alpha
         alpha = a.get_alpha()
@@ -1032,37 +1115,38 @@
             b_c.setFrameStyle(QtWidgets.QFrame.StyledPanel | QtWidgets.QFrame.Plain)
 
             b_c.setSizePolicy(
                 QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
             )
             b_c.setMaximumWidth(25)
 
-        except:
+        except Exception:
             b_c = None
             use_cmap = True
             pass
 
         # cmap
         from .utils import CmapDropdown
 
         if use_cmap is True:
             try:
                 cmap = a.get_cmap()
                 b_cmap = CmapDropdown(startcmap=cmap.name)
                 b_cmap.activated.connect(
                     self.set_cmap(artist=a, layer=layer, widget=b_cmap)
                 )
-            except:
+            except Exception:
                 b_cmap = None
                 pass
         else:
             b_cmap = None
 
         layout = []
-        layout.append((b_sh, 0))  # show hide
+        if not deactivated:
+            layout.append((b_sh, 0))  # show hide
 
         # if b_c is not None:
         #     layout.append((b_c, 1))  # color
 
         layout.append((b_z, 2))  # zorder
 
         layout.append((label, 3))  # title
@@ -1072,52 +1156,60 @@
 
         # if b_a is not None:
         #     layout.append((b_a, 5))  # alpha
 
         # if b_cmap is not None:
         #     layout.append((b_cmap, 6))  # cmap
 
-        layout.append((b_r, 7))  # remove
+        if not deactivated:
+            layout.append((b_r, 7))  # remove
+
+        if deactivated:
+            for w in layout:
+                w[0].setEnabled(False)
 
         return layout
 
     @pyqtSlot()
     def populate_on_layer(self, *args, **kwargs):
         lastlayer = getattr(self, "_last_populated_layer", "")
         currlayer = self.m.BM.bg_layer
+
+        # ignore global layer transparencies (no need to re-populate if global)
+        # transparency changes.
+        # NOTE: This is necessary to avoid recursions for multi-layers!
+        last_layers = set(self.m.BM._get_layers_alphas(lastlayer)[0])
+        curr_layers = set(self.m.BM._get_layers_alphas(currlayer)[0])
+
         # only populate if the current layer is not part of the last set of layers
         # (e.g. to allow show/hide of selected layers without removing the tabs)
-        if not set(lastlayer.split("|")).issuperset(set(currlayer.split("|"))):
+        if not last_layers.issuperset(curr_layers):
             self.populate(*args, **kwargs)
             self._last_populated_layer = currlayer
+        else:
+            # TODO check why adjusting the tab-order causes recursions if multiple
+            # layers are selected (and the transparency of a sub-layer is changed)
+            self.tabBar().color_active_tab(adjust_order=False)
 
     @pyqtSlot()
     def populate(self, *args, **kwargs):
         if not self.isVisible():
             return
 
         tabbar = self.tabBar()
         self._current_tab_idx = self.currentIndex()
         self._current_tab_name = self.tabText(self._current_tab_idx)
 
-        alllayers = sorted(list(self.m._get_layers()))
-
-        self._current_tab_idx = self.currentIndex()
-        self._current_tab_name = self.tabText(self._current_tab_idx)
-
-        alllayers = set(self.m._get_layers())
-
         # go through the layers in reverse and remove any no longer existing layers
-
         alllayers = set(self.m._get_layers())
         nlayers = len(alllayers)
         max_n_layers = self.m._companion_widget_n_layer_tabs
         if nlayers > max_n_layers:
             if not LayerTabBar._n_layer_msg_shown:
-                print(
+                _log.info(
                     "EOmaps-companion: The map has more than "
                     f"{max_n_layers} layers... only last active layers "
                     "are shown in the layer-tabs!"
                 )
                 LayerTabBar._n_layer_msg_shown = True
 
             # if more than max_n_layers layers are available, show only active tabs to
@@ -1155,17 +1247,32 @@
             self.addTab(scroll, layer)
             self.setTabToolTip(i, layer)
 
             if layer == "all" or layer == self.m.layer:
                 # don't show the close button for this tab
                 tabbar.setTabButton(self.count() - 1, tabbar.RightSide, None)
 
+        tabbar.color_active_tab()
+
         # try to restore the previously opened tab
         tabbar.set_current_tab_by_name(self._current_tab_name)
-        tabbar.color_active_tab()
+
+    def get_layer_alpha(self, layer):
+        layers, alphas = self.m.BM._get_layers_alphas()
+        if layer in layers:
+            idx = layers.index(layer)
+            alpha = alphas[idx]
+            LayerTransparencySlider._alphas[layer] = alpha
+
+        elif layer in LayerTransparencySlider._alphas:
+            # use last set alpha value for the layer
+            alpha = LayerTransparencySlider._alphas[layer]
+        else:
+            alpha = 1
+        return alpha
 
     @pyqtSlot()
     def populate_layer(self, layer=None):
         if not self.isVisible():
             return
 
         if layer is None:
@@ -1177,28 +1284,80 @@
             layer = "__inset_" + layer
         widget = self.currentWidget()
 
         if widget is None:
             # ignore events without tabs (they happen on re-population of the tabs)
             return
 
-        layout = QtWidgets.QGridLayout()
-        layout.setAlignment(Qt.AlignTop | Qt.AlignLeft)
+        edit_layout = QtWidgets.QGridLayout()
+        edit_layout.setAlignment(Qt.AlignTop | Qt.AlignLeft)
 
         # make sure that we don't create an empty entry !
-        if layer in self.m.BM._bg_artists:
+        # TODO the None check is to address possible race-conditions
+        # with Maps objects that have no axes defined.
+        if layer in self.m.BM._bg_artists and self.m.ax is not None:
             artists = [
                 a for a in self.m.BM.get_bg_artists(layer) if a.axes is self.m.ax
             ]
         else:
             artists = []
 
         for i, a in enumerate(artists):
             for art, pos in self._get_artist_layout(a, layer):
-                layout.addWidget(art, i, pos)
+                if art is not None:
+                    edit_layout.addWidget(art, i, pos)
+
+        # ------------------------ layer-actions menu
+        # button to add WebMap services to the currently selected layer
+        try:
+            self.addwms = AddWMSMenuButton(m=self.m, new_layer=False, layer=layer)
+            self.addwms.wmsLayerCreated.connect(self.populate_layer)
+        except Exception:
+            self.addwms = None
+
+        # slider to set the global layer transparency
+        self.layer_transparency_slider = LayerTransparencySlider(Qt.Horizontal)
+        self.layer_transparency_slider.set_alpha_stylesheet()
+        self.layer_transparency_slider.setValue(int(self.get_layer_alpha(layer) * 100))
+        layer_transparency_label = QtWidgets.QLabel("<b>Layer Transparency:</b>")
+
+        def update_layerslider(alpha):
+            self.set_layer_alpha(layer, alpha / 100)
+            LayerTransparencySlider._alphas[layer] = alpha / 100
+
+        self.layer_transparency_slider.valueChanged.connect(update_layerslider)
+
+        layer_actions_layout = QtWidgets.QHBoxLayout()
+        if self.addwms is not None:
+            layer_actions_layout.addWidget(self.addwms)
+
+        spacer = QtWidgets.QSpacerItem(50, 1)
+        layer_actions_layout.addItem(spacer)
+
+        layer_actions_layout.addWidget(layer_transparency_label)
+        layer_actions_layout.addWidget(self.layer_transparency_slider, 1)
+        # ------------------------
+
+        # a separator line
+        separator = QtWidgets.QFrame()
+        separator.setFrameShape(QtWidgets.QFrame.HLine)
+        separator.setFixedHeight(1)
+        separator.setStyleSheet("background-color: rgb(150,150,150)")
+
+        layout = QtWidgets.QVBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+
+        layout.addLayout(layer_actions_layout)
+        # layout.addWidget(separator)
+
+        for text in self.m.BM._pending_webmaps.get(layer, []):
+            layout.addWidget(QtWidgets.QLabel(f"<b>PENDING WebMap</b>: {text}"))
+
+        layout.addLayout(edit_layout)
+        layout.addStretch(1)
 
         tabwidget = QtWidgets.QWidget()
         tabwidget.setLayout(layout)
         widget.setWidget(tabwidget)
 
     # --------
 
@@ -1215,36 +1374,40 @@
     def _do_remove(self, artist, layer):
         if self._msg.standardButton(self._msg.clickedButton()) != self._msg.Yes:
             return
 
         self.m.BM.remove_bg_artist(artist, layer)
         try:
             artist.remove()
-        except Exception as ex:
-            print(f"EOmaps: There was an error while trying to remove the artist: {ex}")
+        except Exception:
+            _log.error(
+                "EOmaps: There was an error while trying to remove the artist",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
 
         # explicit treatment for gridlines
         grids = self.m.parent._grid._gridlines
         for g in grids:
             if artist == g._coll:
                 g.remove()
 
         self.populate_layer(layer)
         self.m.redraw(layer)
 
     def remove(self, artist, layer):
         @pyqtSlot()
         def cb():
             self._msg = QtWidgets.QMessageBox(self)
+
             self._msg.setIcon(QtWidgets.QMessageBox.Question)
             self._msg.setWindowTitle("Delete artist?")
             self._msg.setText(
-                "Do you really want to delete the following artist"
+                "Do you really want to delete the following artist "
                 + f"from the layer '{layer}'?\n\n"
-                + f"    '{artist}'"
+                + f"    '{artist.get_label()}'"
             )
 
             self._msg.setStandardButtons(
                 QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No
             )
             self._msg.buttonClicked.connect(lambda: self._do_remove(artist, layer))
             self._msg.show()
@@ -1306,60 +1469,137 @@
             if len(val) > 0:
                 artist.set_cmap(val)
 
             self.m.redraw(layer)
 
         return cb
 
+    @pyqtSlot()
+    def set_layer_alpha(self, layer, alpha):
+        layers, alphas = self.m.BM._get_layers_alphas()
+        if layer in layers:
+            idx = layers.index(layer)
+            alphas[idx] = alpha
+
+        self.m.show_layer(*zip(layers, alphas))
+
 
 class ArtistEditor(QtWidgets.QWidget):
-    def __init__(self, m=None, show_editor=False):
+    def __init__(self, *args, m=None, show_editor=False, **kwargs):
 
         super().__init__()
 
         self.m = m
 
         self.artist_tabs = ArtistEditorTabs(m=self.m)
 
-        self.newlayer = NewLayerWidget(m=self.m)
-        # # re-populate layers on new layer creation
-        self.newlayer.NewLayerCreated.connect(self.artist_tabs.populate)
-        # set active tab to the new tab on layer creation
-        # self.newlayer.NewLayerCreated[str].connect(self.artist_tabs.set_current_tab_by_name)
+        self.artist_tabs.tabBar().setStyleSheet(
+            """
+            QTabBar::tab {
+              background: rgb(220, 220, 220);
+              border: 0px solid black;
+              padding: 1px;
+              padding-bottom: 6px;
+              margin: 0px;
+              margin-left: 2px;
+              margin-bottom: -3px;
+              border-radius: 4px;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(150, 150, 150);
+              border: 2px solid darkred;
+              margin-bottom: -3px;
+            }
+            """
+        )
 
         self.addfeature = AddFeatureWidget(m=self.m)
-        self.addannotation = AddAnnotationInput(m=self.m)
+        self.addannotation = AddAnnotationWidget(m=self.m)
         self.draw = DrawerTabs(m=self.m)
 
+        # add a margin to the top of the drawer widget
+        d = QtWidgets.QWidget()
+        layout = QtWidgets.QVBoxLayout()
+        layout.addWidget(self.draw)
+        layout.setContentsMargins(0, 5, 0, 0)
+        d.setLayout(layout)
+
         # make sure the layer is properly set
         self.set_layer()
 
         self.option_tabs = OptionTabs()
         self.option_tabs.addTab(self.addfeature, "Add Features")
         self.option_tabs.addTab(self.addannotation, "Add Annotations")
-        self.option_tabs.addTab(self.draw, "Draw Shapes")
+        self.option_tabs.addTab(d, "Draw Shapes")
+
+        # set font properties before the stylesheet to avoid clipping of bold text!
+        font = QFont("sans seriv", 8, QFont.Bold, False)
+        self.option_tabs.setFont(font)
+
+        self.option_tabs.setStyleSheet(
+            """
+            QTabWidget::pane {
+              border: 0px;
+              top:0px;
+              background: rgb(200, 200, 200);
+              border-radius: 10px;
+            }
+
+            QTabBar::tab {
+              background: rgb(220, 220, 220);
+              border: 0px;
+              padding: 5px;
+              padding-bottom: 6px;
+              margin-left: 10px;
+              margin-bottom: -2px;
+              border-radius: 4px;
+              font-weight: normal;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(200, 200, 200);
+              border: 0px;
+              margin-bottom: -2px;
+              font-weight: bold;
+            }
+            """
+        )
 
         # repopulate the layer if features or webmaps are added
         self.addfeature.selector.FeatureAdded.connect(self.artist_tabs.populate_layer)
-        self.newlayer.addwms.wmsLayerCreated.connect(self.artist_tabs.populate_layer)
 
         option_widget = QtWidgets.QWidget()
         option_layout = QtWidgets.QVBoxLayout()
         option_layout.addWidget(self.option_tabs)
 
-        option_layout.addWidget(self.newlayer)
         option_widget.setLayout(option_layout)
 
         splitter = QtWidgets.QSplitter(Qt.Vertical)
         splitter.addWidget(option_widget)
         splitter.addWidget(self.artist_tabs)
 
         splitter.setStretchFactor(0, 0)
         splitter.setStretchFactor(1, 1)
 
+        splitter.setStyleSheet(
+            """
+            QSplitter::handle {
+                background: rgb(220,220,220);
+                margin: 1px;
+                margin-left: 20px;
+                margin-right: 20px;
+                height:1px;
+                }
+            QSplitter::handle:pressed {
+                background: rgb(180,180,180);
+            }
+            """
+        )
+
         layout = QtWidgets.QVBoxLayout()
         layout.addWidget(splitter)
 
         self.setLayout(layout)
 
         # connect a callback to update the layer of the feature-button
         # with respect to the currently selected layer-tab
@@ -1368,11 +1608,8 @@
     @pyqtSlot()
     def set_layer(self):
         layer = self.artist_tabs.tabText(self.artist_tabs.currentIndex())
         self.addfeature.selector.set_layer(layer)
         if self.draw is not None:
             self.draw.set_layer(layer)
 
-        if self.newlayer.addwms is not None:
-            self.newlayer.addwms.set_layer(layer)
-
         self.addannotation.set_layer(layer)
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/extent.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/extent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import logging
 from datetime import datetime
+
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import pyqtSlot
 
+_log = logging.getLogger(__name__)
+
 
 class SetExtentToLocation(QtWidgets.QWidget):
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.m = m
 
-        label = QtWidgets.QLabel("Set map-extent to location:")
+        label = QtWidgets.QLabel("<b>Query Location:</b>")
         self.inp = QtWidgets.QLineEdit()
         self.inp.returnPressed.connect(self.set_extent)
         layout = QtWidgets.QHBoxLayout()
         layout.addWidget(label)
         layout.addWidget(self.inp)
 
         self.setLayout(layout)
@@ -46,8 +50,11 @@
                     )
                     return
 
             txt = self.inp.text()
             self.m.set_extent_to_location(txt)
             self.m.redraw()
         except Exception as ex:
-            print("There was an error while trying to set the extent:", ex)
+            _log.error(
+                "There was an error while trying to set the extent.",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/files.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
+import logging
+
 from PyQt5 import QtWidgets, QtGui
-from PyQt5.QtCore import Qt, QLocale
+from PyQt5.QtCore import Qt, QLocale, pyqtSignal
 from pathlib import Path
 import io
+import numpy as np
+
+_log = logging.getLogger(__name__)
 
 from .utils import (
     LineEditComplete,
     InputCRS,
     CmapDropdown,
     show_error_popup,
     to_float_none,
     get_crs,
     str_to_bool,
     GetColorWidget,
     AlphaSlider,
 )
 
-from ..base import NewWindow
+from ..base import NewWindow, get_dummy_spacer
+from ..common import iconpath
 
 
 def _none_or_val(val):
     if val == "None":
         return None
     else:
         return val
@@ -37,14 +43,128 @@
             r = float(r)
             rx = ry = r
         return rx, ry
     except:
         return r
 
 
+def _get_gdf_file_endings():
+    try:
+        from fiona.drvsupport import vector_driver_extensions
+
+        file_endings = [f".{i}" for i in vector_driver_extensions()]
+    except Exception as ex:
+        file_endings = []
+
+    return file_endings
+
+
+class AddColorbarCheckbox(QtWidgets.QCheckBox):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Add Colorbar</h3>"
+                "If checked, a colorbar will be added for the data.",
+            )
+
+
+class LayerInput(LineEditComplete):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Layer</h3>"
+                "Set the layer at which the dataset should be plotted.",
+            )
+
+
+class XInput(LineEditComplete):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set X Coordinate</h3>"
+                "Set the variable that should be used as x-coordinate.",
+            )
+
+
+class YInput(LineEditComplete):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set Y Coordinate</h3>"
+                "Set the variable that should be used as Y-coordinate.",
+            )
+
+
+class ParameterInput(LineEditComplete):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set Parameter</h3>"
+                "Set the variable that should be used as data.",
+            )
+
+
+class IDInput(LineEditComplete):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set ID</h3>"
+                "Set the variable that should be used to identify datapoints.",
+            )
+
+
+class ZorderInput(QtWidgets.QLineEdit):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set zorder</h3>"
+                "Set the zorder (e.g. the vertical stacking order) that will be "
+                "assigned to the artist.",
+            )
+
+
+class VminInput(QtWidgets.QLineEdit):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set vmin</h3>"
+                "Set the lower boundary that is used for color scaling."
+                "(by default the minimal value of the dataset is used)",
+            )
+
+
+class VmaxInput(QtWidgets.QLineEdit):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set vmax</h3>"
+                "Set the upper boundary that is used for color scaling."
+                "(by default the maximal value of the dataset is used)",
+            )
+
+
+class MinMaxUpdateButton(QtWidgets.QPushButton):
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set vmin/vmax to data limits</h3>"
+                "Identify vmin/vmax from the selected dataset.",
+            )
+
+
 class ShapeSelector(QtWidgets.QFrame):
     _ignoreargs = ["shade_hook", "agg_hook"]
 
     # special treatment of arguments
     _argspecials = dict(
         aggregator=_none_or_val,
         mask_radius=_none_or_val,
@@ -86,14 +206,26 @@
         self.layout.addLayout(self.options)
 
         self.setLayout(self.layout)
 
         self.shape_selector.setCurrentIndex(self.shape_selector.findText(self.shape))
         self.shape_changed(self.shape)
 
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Set Plot Shape</h3>"
+                "Set the plot-shape that is used to visualize the dataset."
+                "<br><br>"
+                "<b>NOTE:</b> Some shapes require more computational effort than "
+                "others! Checkout the docs on how to choose the shape that fits "
+                "your needs!",
+            )
+
     def set_shape(self, shape):
         self.shape_selector.setCurrentIndex(self.shape_selector.findText(shape))
         self.shape_changed(shape)
 
     def argparser(self, key, val):
         special = self._argspecials.get(key, None)
         if special is not None:
@@ -105,15 +237,15 @@
             try:
                 convval = t(val)
             except ValueError:
                 continue
 
             return convval
 
-        print(f"WARNING value-conversion for {key} = {val} did not succeed!")
+        _log.warning(f"EOmaps: value-conversion for {key} = {val} did not succeed!")
         return val
 
     @property
     def shape_args(self):
 
         out = dict(shape=self.shape)
         for key, val in self.paraminputs.items():
@@ -186,28 +318,14 @@
         attach_tab_after_plot=True,
         tab=None,
         window_title="Plot File",
         **kwargs,
     ):
         """
         A widget to add a layer from a file
-
-        Parameters
-        ----------
-        *args : TYPE
-            DESCRIPTION.
-        m : TYPE, optional
-            DESCRIPTION. The default is None.
-        **kwargs : TYPE
-            DESCRIPTION.
-
-        Returns
-        -------
-        None.
-
         """
         super().__init__(*args, **kwargs)
 
         self.m = m
         self.tab = tab
         self.window_title = window_title
 
@@ -225,45 +343,52 @@
         scroll.setWidgetResizable(True)
         self.file_info = QtWidgets.QLabel()
         self.file_info.setWordWrap(True)
         self.file_info.setTextInteractionFlags(Qt.TextSelectableByMouse)
         scroll.setWidget(self.file_info)
 
         # add colorbar checkbox
-        self.cb_colorbar = QtWidgets.QCheckBox("Add colorbar")
+        self.cb_colorbar = AddColorbarCheckbox("Add colorbar")
 
         # layer
         self.layer_label = QtWidgets.QLabel("<b>Layer:</b>")
-        self.layer = LineEditComplete()
+        self.layer = LayerInput()
         self.layer.setPlaceholderText(str(self.m.BM.bg_layer))
 
         setlayername = QtWidgets.QWidget()
         layername = QtWidgets.QHBoxLayout()
         layername.addWidget(self.layer_label)
         layername.addWidget(self.layer)
         setlayername.setLayout(layername)
 
         # shape selector (with shape options)
         self.shape_selector = ShapeSelector(m=self.m, default_shape=self.default_shape)
-        self.setStyleSheet("ShapeSelector{border:1px dashed;}")
+
+        self.setStyleSheet(
+            """
+            ShapeSelector{
+                border:1px dashed;
+                }
+            """
+        )
 
         # colormaps
         self.cmaps = CmapDropdown()
 
         validator = QtGui.QDoubleValidator()
         # make sure the validator uses . as separator
         validator.setLocale(QLocale("en_US"))
 
         # vmin / vmax
         vminlabel, vmaxlabel = QtWidgets.QLabel("vmin="), QtWidgets.QLabel("vmax=")
-        self.vmin, self.vmax = QtWidgets.QLineEdit(), QtWidgets.QLineEdit()
+        self.vmin, self.vmax = VminInput(), VmaxInput()
         self.vmin.setValidator(validator)
         self.vmax.setValidator(validator)
 
-        self.minmaxupdate = QtWidgets.QPushButton("🗘")
+        self.minmaxupdate = MinMaxUpdateButton("🗘")
         self.minmaxupdate.clicked.connect(self.do_update_vals)
 
         minmaxlayout = QtWidgets.QHBoxLayout()
         minmaxlayout.setAlignment(Qt.AlignLeft)
         minmaxlayout.addWidget(vminlabel)
         minmaxlayout.addWidget(self.vmin)
         minmaxlayout.addWidget(vmaxlabel)
@@ -290,37 +415,43 @@
         options_split.addWidget(scroll)
         options_split.addWidget(optionscroll)
         options_split.setSizes((500, 300))
 
         self.options_layout = QtWidgets.QHBoxLayout()
         self.options_layout.addWidget(options_split)
 
-        self.x = LineEditComplete("x")
-        self.y = LineEditComplete("y")
-        self.parameter = LineEditComplete("param")
-        self.ID = LineEditComplete("ID")
+        self.x = XInput("x")
+        self.y = YInput("y")
+        self.parameter = ParameterInput("param")
+        self.ID = IDInput("ID")
         self.crs = InputCRS()
 
-        tx = QtWidgets.QLabel("x:")
-        ty = QtWidgets.QLabel("y:")
-        tparam = QtWidgets.QLabel("parameter:")
-        tcrs = QtWidgets.QLabel("crs:")
-        self.tID = QtWidgets.QLabel("ID:")
+        # update info-text with respect to the selected columns
+        self.x.textChanged.connect(self.update_info_text)
+        self.y.textChanged.connect(self.update_info_text)
+        self.parameter.textChanged.connect(self.update_info_text)
+        self.ID.textChanged.connect(self.update_info_text)
+
+        tx = QtWidgets.QLabel("<b>x:</b>")
+        ty = QtWidgets.QLabel("<b>y:</b>")
+        tparam = QtWidgets.QLabel("<b>parameter:</b>")
+        tcrs = QtWidgets.QLabel("<b>crs:</b>")
+        self.tID = QtWidgets.QLabel("<b>ID:</b>")
 
         plotargs = QtWidgets.QHBoxLayout()
+        plotargs.addWidget(self.tID)
+        plotargs.addWidget(self.ID)
         plotargs.addWidget(tx)
         plotargs.addWidget(self.x)
         plotargs.addWidget(ty)
         plotargs.addWidget(self.y)
         plotargs.addWidget(tparam)
         plotargs.addWidget(self.parameter)
         plotargs.addWidget(tcrs)
         plotargs.addWidget(self.crs)
-        plotargs.addWidget(self.tID)
-        plotargs.addWidget(self.ID)
 
         plotargs.addWidget(self.b_plot)
 
         self.title = QtWidgets.QLabel("<b>Set plot variables:</b>")
         withtitle = QtWidgets.QVBoxLayout()
         withtitle.addWidget(self.title)
         withtitle.addLayout(plotargs)
@@ -328,54 +459,74 @@
 
         self.layout = QtWidgets.QVBoxLayout()
         self.layout.addLayout(self.options_layout, stretch=1)
         self.layout.addLayout(withtitle)
 
         self.setLayout(self.layout)
 
+        self._file_handle = None
+
+    def get_info_text(self):
+        return "???"
+
+    def update_info_text(self):
+        try:
+            self.file_info.setText(self.get_info_text())
+        except Exception:
+            self.file_info.setText("???")
+
     def get_layer(self):
         layer = self.layer.text()
         if layer == "":
             layer = self.layer.placeholderText()
 
         return layer
 
     def open_file(self, file_path=None):
-        info = self.do_open_file(file_path)
+        self._open_filehandle(file_path)
+
+        if file_path is not None:
+            self.file_path = file_path
 
         if self.file_endings is not None:
             if file_path.suffix.lower() not in self.file_endings:
                 self.file_info.setText(
                     f"the file {self.file_path.name} is not a valid file"
                 )
                 self.file_path = None
                 return
 
-        if file_path is not None:
-            self.file_path = file_path
+        self.do_open_file(file_path)
 
-        if info is not None:
-            self.file_info.setText(info)
+        self.file_info.setText(self.get_info_text())
 
         self.layer.set_complete_vals(
             [file_path.name]
             + [i for i in self.m._get_layers() if not i.startswith("_")]
         )
 
-        self.newwindow = NewWindow(m=self.m, title=self.window_title)
+        self.newwindow = NewWindow(
+            m=self.m,
+            title=self.window_title,
+            on_close=self._close_filehandle,
+        )
+
         self.newwindow.statusBar().showMessage(str(self.file_path))
 
         self.newwindow.setWindowFlags(
-            Qt.FramelessWindowHint | Qt.Dialog | Qt.WindowStaysOnTopHint
+            Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint | Qt.Dialog
         )
 
         self.newwindow.layout.addWidget(self)
         self.newwindow.resize(800, 500)
+        # self.newwindow.setWindowModality(Qt.ApplicationModal) make the popup blocking
         self.newwindow.show()
 
+        self.newwindow.on_close
+
     def b_plot_file(self):
         try:
             self.do_plot_file()
 
             # fetch the min/max values if no explicit values were provided
             vmin, vmax = self.vmin.text(), self.vmax.text()
             if vmin != "" and vmax != "":
@@ -393,45 +544,69 @@
             show_error_popup(
                 text="There was an error while trying to plot the data!",
                 title="Error",
                 details=traceback.format_exc(),
             )
             return
 
-        if self.close_on_plot:
-            self.newwindow.close()
+        try:
+            if self.close_on_plot:
+                self.newwindow.close()
 
-        if self.attach_tab_after_plot:
-            self.attach_as_tab()
+            if self.attach_tab_after_plot:
+                self.attach_as_tab()
+        finally:
+            self._close_filehandle()
 
     def do_open_file(self):
         file_path = Path(QtWidgets.QFileDialog.getOpenFileName()[0])
 
         return (
             file_path,
             f"The file {file_path.stem} has\n {file_path.stat().st_size} bytes.",
         )
 
+    def _open_filehandle(self, file_path):
+        self._file_handle = open(file_path, "r")
+
+    def _close_filehandle(self):
+
+        if self._file_handle is not None:
+            try:
+                self._file_handle.close()
+            except Exception as ex:
+                _log.error(
+                    "EOmaps: encountered a problem while closing the file.",
+                    exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+                )
+
+        self._file_handle = None
+
     def do_plot_file(self):
         self.file_info.setText("Implement `.do_plot_file()` to plot the data!")
 
     def do_update_vals(self):
         return
 
     def attach_as_tab(self):
         if self.tab is None:
             return
 
         if self.file_path is not None:
-            name = self.file_path.stem
+            name = self.file_path.name
         else:
             return
 
-        if len(name) > 10:
-            name = name[:7] + "..."
+        if len(name) > 15:
+            name = (
+                self.file_path.stem[:6]
+                + "..."
+                + self.file_path.stem[-3:]
+                + self.file_path.suffix
+            )
         self.tab.addTab(self, name)
 
         tabindex = self.tab.indexOf(self)
 
         self.tab.setCurrentIndex(tabindex)
         self.tab.setTabToolTip(tabindex, str(self.file_path))
 
@@ -456,318 +631,307 @@
         self.shape_selector.setEnabled(False)
         self.layer.setEnabled(False)
         self.cb_colorbar.setEnabled(False)
 
         self.b_plot.close()
 
 
-class PlotGeoTIFFWidget(PlotFileWidget):
-
-    file_endings = (".tif", ".tiff")
-
+class PlotXarrayWidget(PlotFileWidget):
     def __init__(self, *args, window_title="Plot GeoTIFF FIle", **kwargs):
 
         super().__init__(*args, **kwargs)
 
         # hide ID inputs... not supported for GeoTIFF
         self.tID.hide()
         self.ID.hide()
 
+        self.default_sel_args = dict()
+
     def get_crs(self):
         return get_crs(self.crs.text())
 
-    def do_open_file(self, file_path):
+    def _open_filehandle(self, file_path):
         import xarray as xar
 
-        with xar.open_dataset(file_path, mask_and_scale=False) as f:
-            import io
-
-            info = io.StringIO()
-            f.info(info)
-
-            coords = list(f.coords)
-            variables = list(f.variables)
-
-            crs = f.rio.crs
-            if crs is not None:
-                self.crs.setText(crs.to_string())
-            self.parameter.setText(next((i for i in variables if i not in coords)))
-
-        self.x.setText("x")
-        self.y.setText("y")
-
-        # set layer-name to filename by default
-        self.layer.setPlaceholderText(file_path.stem)
-
-        # set values for autocompletion
-        cols = sorted(set(variables + coords))
-        self.x.set_complete_vals(cols)
-        self.y.set_complete_vals(cols)
-        self.parameter.set_complete_vals(cols)
+        self._file_handle = xar.open_dataset(file_path, mask_and_scale=False)
 
-        return info.getvalue()
+    def get_info_text(self):
+        f = self._file_handle
+        import xarray as xar
 
-    def do_plot_file(self):
-        if self.file_path is None:
-            return
+        try:
+            selargs = self.get_sel_args()
+            usef = f[self.parameter.text()].sel(**selargs)
+            s = usef.__repr__()
+            return s
+        except Exception:
+            return f.__repr__()
 
-        m2 = self.m.new_layer_from_file.GeoTIFF(
-            self.file_path,
-            shape=self.shape_selector.shape_args,
-            coastline=False,
-            layer=self.get_layer(),
-            cmap=self.cmaps.currentText(),
-            vmin=to_float_none(self.vmin.text()),
-            vmax=to_float_none(self.vmax.text()),
-            data_crs=self.get_crs(),
-        )
+    def attach_as_tab(self, *args, **kwargs):
+        super().attach_as_tab(*args, **kwargs)
 
-        if self.cb_colorbar.isChecked():
-            m2.add_colorbar()
+        for key, val in self.sel_inputs.items():
+            val["inp"].setEnabled(False)
 
-        m2.show_layer(m2.layer)
+    def get_sel_args(self):
+        # use isVisibleTo to avoid issues
+        # (see https://stackoverflow.com/a/40174748/9703451)
+        s = dict()
+        for key, val in self.sel_inputs.items():
+            sel = val["inp"].text()
+            if val["inp"].isVisibleTo(self) and sel != "":
+                # convert to the correct dtype
+                sel = np.array(sel).astype(val["dtype"])
 
-        self.m2 = m2
+                s[key] = sel
+        return s
 
     def do_update_vals(self):
-        import xarray as xar
+        f = self._file_handle
 
         try:
-            with xar.open_dataset(self.file_path) as f:
-                vmin = f[self.parameter.text()].min()
-                vmax = f[self.parameter.text()].max()
-
-                self.vmin.setText(str(float(vmin)))
-                self.vmax.setText(str(float(vmax)))
+            vmin = f[self.parameter.text()].min()
+            vmax = f[self.parameter.text()].max()
 
+            self.vmin.setText(str(float(vmin)))
+            self.vmax.setText(str(float(vmax)))
         except Exception:
             import traceback
 
             show_error_popup(
                 text="There was an error while trying to update the values.",
                 title="Unable to update values.",
                 details=traceback.format_exc(),
             )
 
+    def get_sel_layout(self, f):
+        self.sel_title = QtWidgets.QLabel("<b>Select index-labels to plot:</b>")
 
-class PlotNetCDFWidget(PlotFileWidget):
+        layout = QtWidgets.QHBoxLayout()
+        dims = list(f.dims)
 
-    file_endings = ".nc"
+        self.sel_inputs = dict()
+        # get completion values
+        for d in dims:
+            vals = f[d].values.astype(str)
 
-    def __init__(self, *args, **kwargs):
+            label = QtWidgets.QLabel(f"{d}:")
+            inp = LineEditComplete()
+            inp.set_complete_vals(vals)
 
-        super().__init__(*args, window_title="Plot NetCDF FIle", **kwargs)
+            if d in self.default_sel_args:
+                inp.setText(str(self.default_sel_args[d]))
 
-        # hide ID inputs... not (yet) supported for NetCDF
-        self.tID.hide()
-        self.ID.hide()
+            inp.textChanged.connect(self.update_info_text)
 
-        l = QtWidgets.QHBoxLayout()
+            layout.addWidget(label)
+            layout.addWidget(inp)
 
-        self.sel_title = QtWidgets.QLabel("<b>Select index-labels to plot:</b>")
+            self.sel_inputs[d] = dict(inp=inp, label=label, dtype=f[d].dtype)
 
-        l.addWidget(self.sel_title)
+        self.x.textEdited.connect(self.deactivate_sel_cb)
+        self.x.completer().activated.connect(self.deactivate_sel_cb)
+        self.y.textEdited.connect(self.deactivate_sel_cb)
+        self.y.completer().activated.connect(self.deactivate_sel_cb)
+        self.parameter.textEdited.connect(self.deactivate_sel_cb)
+        self.parameter.completer().activated.connect(self.deactivate_sel_cb)
+        self.deactivate_sel_cb()
+        layout.addWidget(get_dummy_spacer())
+
+        sel_layout = QtWidgets.QVBoxLayout()
+        sel_layout.addWidget(self.sel_title)
+        sel_layout.addLayout(layout)
 
-        withtitle = QtWidgets.QWidget()
-        withtitlelayout = QtWidgets.QVBoxLayout()
-        withtitlelayout.addLayout(l)
-        withtitle.setLayout(withtitlelayout)
+        return sel_layout
 
-        withtitle.setMaximumHeight(60)
+    def deactivate_sel_cb(self):
+        selected_dims = [self.x.text(), self.y.text()]
 
-        self.layout.addWidget(withtitle)
+        try:
+            param_dims = self._file_handle[self.parameter.text()].dims
+        except Exception:
+            param_dims = None
 
-    def _deactivate_sel_factory(self, d):
-        def cb():
-            selected_dims = [self.x.text(), self.y.text()]
-            if d in selected_dims:
+        for d in self.sel_inputs:
+            if d in selected_dims or (param_dims is not None and d not in param_dims):
                 self.sel_inputs[d]["label"].hide()
                 self.sel_inputs[d]["inp"].hide()
-
             else:
                 self.sel_inputs[d]["label"].show()
                 self.sel_inputs[d]["inp"].show()
 
-            if any(i["inp"].isVisible() for i in self.sel_inputs.values()):
+            if any(i["inp"].isVisibleTo(self) for i in self.sel_inputs.values()):
                 self.sel_title.show()
             else:
                 self.sel_title.hide()
 
-        return cb
+    def do_plot_file(self):
+        f = self._file_handle
 
-    def get_sel_layout(self, f):
+        if f is None:
+            return
 
-        layout = QtWidgets.QHBoxLayout()
-        dims = list(f.dims)
+        m2 = self.m.new_layer_from_file.NetCDF(
+            f,
+            shape=self.shape_selector.shape_args,
+            coastline=False,
+            layer=self.get_layer(),
+            coords=(self.x.text(), self.y.text()),
+            parameter=self.parameter.text(),
+            data_crs=self.get_crs(),
+            sel=self.get_sel_args(),
+            cmap=self.cmaps.currentText(),
+            vmin=to_float_none(self.vmin.text()),
+            vmax=to_float_none(self.vmax.text()),
+        )
 
-        self.sel_inputs = dict()
-        # get completion values
-        for d in dims:
-            vals = f[d].values.astype(str)
+        if self.cb_colorbar.isChecked():
+            m2.add_colorbar()
 
-            label = QtWidgets.QLabel(f"{d}:")
-            inp = LineEditComplete()
-            inp.set_complete_vals(vals)
+        m2.show_layer(m2.layer)
 
-            layout.addWidget(label)
-            layout.addWidget(inp)
+        self.m2 = m2
 
-            self.sel_inputs[d] = dict(inp=inp, label=label, dtype=f[d].dtype)
 
-            deactivate_func = self._deactivate_sel_factory(d)
-            deactivate_func()
+class PlotGeoTIFFWidget(PlotXarrayWidget):
 
-            self.x.textEdited.connect(deactivate_func)
-            self.x.completer().activated.connect(deactivate_func)
-            self.y.textEdited.connect(deactivate_func)
-            self.y.completer().activated.connect(deactivate_func)
+    file_endings = (".tif", ".tiff")
 
-        return layout
+    def __init__(self, *args, window_title="Plot GeoTIFF FIle", **kwargs):
 
-    def get_sel_args(self):
+        super().__init__(*args, **kwargs)
 
-        s = dict()
+        # hide ID inputs... not supported for GeoTIFF
+        self.tID.hide()
+        self.ID.hide()
+        self.default_sel_args = dict(band=1)
 
-        for key, val in self.sel_inputs.items():
-            sel = val["inp"].text()
-            if val["inp"].isVisible() and sel != "":
-                # convert to the correct dtype
-                import numpy as np
+    def do_open_file(self, file_path):
+        f = self._file_handle
 
-                sel = np.array(sel).astype(val["dtype"])
+        coords = list(f.coords)
+        variables = list(f.variables)
 
-                s[key] = sel
-        return s
+        crs = f.rio.crs
+        if crs is not None:
+            self.crs.setText(crs.to_string())
+        self.parameter.setText(next((i for i in variables if i not in coords)))
 
-    def get_crs(self):
-        return get_crs(self.crs.text())
+        self.x.setText("x")
+        self.y.setText("y")
 
-    def do_open_file(self, file_path):
-        import xarray as xar
+        # set default layer-name to current layer if a single layer is selected,
+        # else use the filename
+        use_layer = self.m.BM.bg_layer
+        if "|" in use_layer:
+            use_layer = self.file_path.stem
+        else:
+            use_layer = use_layer.split("{")[0].strip()
 
-        with xar.open_dataset(file_path, mask_and_scale=False) as f:
+        self.layer.setPlaceholderText(use_layer)
 
-            info = io.StringIO()
-            f.info(info)
+        # set values for autocompletion
+        cols = sorted(set(variables + coords))
+        self.x.set_complete_vals(cols)
+        self.y.set_complete_vals(cols)
+        self.parameter.set_complete_vals(cols)
 
-            coords = list(f.coords)
-            variables = list(f.variables)
+        sel_layout = self.get_sel_layout(f)
+        self.layout.addLayout(sel_layout)
 
-            if len(coords) >= 2:
-                self.x.setText(coords[0])
-                self.y.setText(coords[1])
-
-            # set values for autocompletion
-            cols = sorted(set(variables + coords))
-            self.x.set_complete_vals(cols)
-            self.y.set_complete_vals(cols)
+        # update info text
+        self.update_info_text()
 
-            if "lon" in cols:
-                self.x.setText("lon")
-            elif "x" in cols:
-                self.x.setText("x")
-            else:
-                self.x.setText(cols[0])
 
-            if "lat" in cols:
-                self.y.setText("lat")
-            elif "y" in cols:
-                self.y.setText("y")
-            else:
-                self.x.setText(cols[1])
+class PlotNetCDFWidget(PlotXarrayWidget):
 
-            self.parameter.set_complete_vals(cols)
-            self.parameter.setText(
-                next(
-                    (
-                        i
-                        for i in variables
-                        if (i != self.x.text() and i != self.y.text())
-                    )
-                )
-            )
+    file_endings = (".nc",)
 
-            sel_layout = self.get_sel_layout(f)
-            self.layout.addLayout(sel_layout)
+    def __init__(self, *args, **kwargs):
 
-        # set layer-name to filename by default
-        self.layer.setPlaceholderText(file_path.stem)
+        super().__init__(*args, window_title="Plot NetCDF FIle", **kwargs)
 
-        return info.getvalue()
+        # hide ID inputs... not (yet) supported for NetCDF
+        self.tID.hide()
+        self.ID.hide()
 
-    def do_update_vals(self):
-        import xarray as xar
+    def do_open_file(self, file_path):
+        f = self._file_handle
 
-        try:
-            with xar.open_dataset(self.file_path) as f:
-                vmin = f[self.parameter.text()].min()
-                vmax = f[self.parameter.text()].max()
+        coords = list(f.coords)
+        variables = list(f.variables)
 
-                self.vmin.setText(str(float(vmin)))
-                self.vmax.setText(str(float(vmax)))
+        if len(coords) >= 2:
+            self.x.setText(coords[0])
+            self.y.setText(coords[1])
 
-        except Exception:
-            import traceback
+        # set values for autocompletion
+        cols = sorted(set(variables + coords))
+        self.x.set_complete_vals(cols)
+        self.y.set_complete_vals(cols)
 
-            show_error_popup(
-                text="There was an error while trying to update the values.",
-                title="Unable to update values.",
-                details=traceback.format_exc(),
-            )
+        if "lon" in cols:
+            self.x.setText("lon")
+        elif "x" in cols:
+            self.x.setText("x")
+        else:
+            self.x.setText(cols[0])
 
-    def do_plot_file(self):
-        if self.file_path is None:
-            return
+        if "lat" in cols:
+            self.y.setText("lat")
+        elif "y" in cols:
+            self.y.setText("y")
+        else:
+            self.x.setText(cols[1])
 
-        import xarray as xar
+        self.parameter.set_complete_vals(cols)
+        self.parameter.setText(
+            next((i for i in variables if (i != self.x.text() and i != self.y.text())))
+        )
 
-        with xar.open_dataset(self.file_path) as f:
-            selargs = self.get_sel_args()
-            usef = f.sel(**self.get_sel_args())
-            if len(selargs) > 0:
-                self.file_info.setText(usef.__repr__())
-
-            m2 = self.m.new_layer_from_file.NetCDF(
-                usef,
-                shape=self.shape_selector.shape_args,
-                coastline=False,
-                layer=self.get_layer(),
-                coords=(self.x.text(), self.y.text()),
-                parameter=self.parameter.text(),
-                data_crs=self.get_crs(),
-                # sel=self.get_sel_args(),
-                cmap=self.cmaps.currentText(),
-                vmin=to_float_none(self.vmin.text()),
-                vmax=to_float_none(self.vmax.text()),
-            )
+        sel_layout = self.get_sel_layout(f)
+        self.layout.addLayout(sel_layout)
 
-        if self.cb_colorbar.isChecked():
-            m2.add_colorbar()
+        # set default layer-name to current layer if a single layer is selected,
+        # else use the filename
+        use_layer = self.m.BM.bg_layer
+        if "|" in use_layer:
+            use_layer = self.file_path.stem
+        else:
+            use_layer = use_layer.split("{")[0].strip()
 
-        m2.show_layer(m2.layer)
+        self.layer.setPlaceholderText(use_layer)
 
-        self.m2 = m2
+        # update info text
+        self.update_info_text()
 
 
 class PlotCSVWidget(PlotFileWidget):
 
     default_shape = "ellipses"
     file_endings = ".csv"
 
     def __init__(self, *args, **kwargs):
 
         super().__init__(*args, window_title="Plot CSV FIle", **kwargs)
 
     def get_crs(self):
         return get_crs(self.crs.text())
 
-    def do_open_file(self, file_path):
+    def _open_filehandle(self, file_path):
         import pandas as pd
 
-        df = pd.read_csv(file_path)
+        self._data = pd.read_csv(file_path)
+
+    def _close_filehandle(self):
+        del self._data
+        pass
+
+    def do_open_file(self, file_path):
+        df = self._data
 
         if len(df) > 50000:
             # use "shade_points" as default shape if more than 50000 columns are found
             self.shape_selector.set_shape("shade_points")
 
         cols = df.columns
 
@@ -777,55 +941,104 @@
         self.parameter.set_complete_vals(cols)
         self.ID.set_complete_vals(cols)
 
         if len(cols) == 3:
 
             if "lon" in cols:
                 self.x.setText("lon")
+            elif "x" in cols:
+                self.x.setText("x")
             else:
                 self.x.setText(cols[0])
 
             if "lat" in cols:
                 self.y.setText("lat")
+            elif "y" in cols:
+                self.y.setText("x")
             else:
-                self.x.setText(cols[1])
+                self.y.setText(cols[1])
 
             self.parameter.setText(cols[2])
 
             # if there are only 3 columns there is no column left to use as ID!
-            self.ID.hide()
-            self.tID.hide()
+            self.ID.setText("")
+            self.ID.setPlaceholderText("index")
+            self.ID.setEnabled(False)
+            # self.ID.hide()
+            # self.tID.hide()
 
         if len(cols) > 3:
-
-            self.ID.setText(cols[0])
+            self.ID.setText("")
+            self.ID.setPlaceholderText("index")
+            self.ID.setEnabled(True)
 
             if "lon" in cols:
                 self.x.setText("lon")
+            elif "x" in cols:
+                self.x.setText("x")
             else:
                 self.x.setText(cols[1])
 
             if "lat" in cols:
                 self.y.setText("lat")
+            elif "y" in cols:
+                self.y.setText("y")
             else:
-                self.x.setText(cols[2])
+                self.y.setText(cols[2])
 
             self.parameter.setText(cols[3])
 
-        # set layer-name to filename by default
-        self.layer.setPlaceholderText(file_path.stem)
+        # set default layer-name to current layer if a single layer is selected,
+        # else use the filename
+        use_layer = self.m.BM.bg_layer
+        if "|" in use_layer:
+            use_layer = self.file_path.stem
+        else:
+            use_layer = use_layer.split("{")[0].strip()
 
-        return df.__repr__()
+        self.layer.setPlaceholderText(use_layer)
+
+    def get_info_text(self):
+        import pandas as pd
+
+        cols = dict()
+
+        ID = self.ID.text()
+        if self.ID.isVisibleTo(self) and len(ID) > 0 and ID != "index":
+            cols["ID"] = ID
+            show_index = False
+        else:
+            show_index = True
+
+        cols["x"] = self.x.text()
+        cols["y"] = self.y.text()
+        cols["parameter"] = self.parameter.text()
+
+        try:
+            usecols = list(cols.keys())
+            usevals = list(cols.values())
+
+            df = self._data[usevals]
+            init_cols = df.columns
+            df.columns = [f"{usecols[i]}: {val}" for i, val in enumerate(usevals)]
+            info = df.to_html(index=show_index, max_rows=100, max_cols=10)
+            df.columns = init_cols
+            return info
+        except:
+            try:
+                return self._data._repr_html_()
+            except Exception:
+                return self._data.__repr__()
 
     def do_plot_file(self):
         if self.file_path is None:
             return
 
         ID = self.ID.text()
-        if self.ID.isVisible() and ID != "":
+        if self.ID.isVisibleTo(self) and len(ID) > 0 and ID != "index":
             read_kwargs = dict(index_col=ID)
         else:
             read_kwargs = dict()
 
         m2 = self.m.new_layer_from_file.CSV(
             self.file_path,
             shape=self.shape_selector.shape_args,
@@ -846,17 +1059,15 @@
 
         m2.show_layer(m2.layer)
 
         self.m2 = m2
 
     def do_update_vals(self):
         try:
-            import pandas as pd
-
-            df = pd.read_csv(self.file_path)
+            df = self._data
 
             vmin = df[self.parameter.text()].min()
             vmax = df[self.parameter.text()].max()
 
             self.vmin.setText(str(float(vmin)))
             self.vmax.setText(str(float(vmax)))
 
@@ -866,19 +1077,21 @@
             show_error_popup(
                 text="There was an error while trying to update the values.",
                 title="Unable to update values.",
                 details=traceback.format_exc(),
             )
 
 
-class PlotShapeFileWidget(QtWidgets.QWidget):
+class PlotGeoDataFrameWidget(QtWidgets.QWidget):
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
+
+        self.file_endings = _get_gdf_file_endings()
+
         self.m = m
-        self.file_endings = [".shp"]
 
         self.file_path = None
 
         self.plot_props = dict()
 
         scroll = QtWidgets.QScrollArea()
         scroll.setWidgetResizable(True)
@@ -893,28 +1106,31 @@
 
         # color
         self.colorselector = GetColorWidget()
         self.colorselector.cb_colorselected = self.update_on_color_selection
 
         # alpha of facecolor
         self.alphaslider = AlphaSlider(Qt.Horizontal)
+        self.alphaslider.set_alpha_stylesheet()
         self.alphaslider.valueChanged.connect(
             lambda i: self.colorselector.set_alpha(i / 100)
         )
         self.alphaslider.valueChanged.connect(self.update_props)
 
         # linewidth
         self.linewidthslider = AlphaSlider(Qt.Horizontal)
+        self.linewidthslider.set_linewidth_stylesheet()
+
         self.linewidthslider.valueChanged.connect(
             lambda i: self.colorselector.set_linewidth(i / 10)
         )
         self.linewidthslider.valueChanged.connect(self.update_props)
 
         # zorder
-        self.zorder = QtWidgets.QLineEdit("10")
+        self.zorder = ZorderInput("10")
         validator = QtGui.QIntValidator()
         self.zorder.setValidator(validator)
         self.zorder.setMaximumWidth(30)
         self.zorder.setSizePolicy(
             QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
         )
         self.zorder.textChanged.connect(self.update_props)
@@ -927,16 +1143,15 @@
         zorder_layout = QtWidgets.QHBoxLayout()
         zorder_layout.addWidget(zorder_label)
         zorder_layout.addWidget(self.zorder)
         zorder_layout.setAlignment(Qt.AlignRight | Qt.AlignCenter)
 
         # layer
         layerlabel = QtWidgets.QLabel("Layer:")
-        self.layer = LineEditComplete()
-        self.layer.setPlaceholderText(str(self.m.BM.bg_layer))
+        self.layer = LayerInput()
 
         setlayername = QtWidgets.QWidget()
         layername = QtWidgets.QHBoxLayout()
         layername.addWidget(layerlabel)
         layername.addWidget(self.layer)
         layername.addLayout(zorder_layout)
         setlayername.setLayout(layername)
@@ -979,24 +1194,37 @@
             self.file_path,
             **self.plot_props,
             layer=layer,
         )
         self.window().close()
 
     def do_open_file(self, file_path=None):
+        try:
+            import geopandas as gpd
+        except ImportError:
+            _log.error(
+                "EOmaps: missing required dependency 'geopandas' to open the file."
+            )
+            return
         self.file_path = file_path
-
-        import geopandas as gpd
-
         self.gdf = gpd.read_file(self.file_path)
 
         self.file_info.setText(self.gdf.__repr__())
 
-    def open_file(self, file_path=None):
+        # set default layer-name to current layer if a single layer is selected,
+        # else use the filename
+        use_layer = self.m.BM.bg_layer
+        if "|" in use_layer:
+            use_layer = self.file_path.stem
+        else:
+            use_layer = use_layer.split("{")[0].strip()
+
+        self.layer.setPlaceholderText(use_layer)
 
+    def open_file(self, file_path=None):
         if self.file_endings is not None:
             if file_path.suffix.lower() not in self.file_endings:
                 self.file_info.setText(
                     f"the file {self.file_path.name} is not a valid file"
                 )
                 self.file_path = None
                 return
@@ -1045,47 +1273,49 @@
 
 class OpenDataStartTab(QtWidgets.QWidget):
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.m = m
 
+        icon = iconpath / "open.png"
+        self.b_str = (
+            f"<img src={icon} height=20 "
+            "style='display: inline; vertical-align:bottom;'>"
+            "</img>"
+        )
         self.t1 = QtWidgets.QLabel()
         # self.t1.setAlignment(Qt.AlignBottom | Qt.AlignCenter)
         self.t1.setText(
-            "<h3>Open or DRAG & DROP files!</h3>"
+            f"<h3>Click on {self.b_str} or DRAG & DROP to plot data from files!</h3>"
             "<p>"
             "Supported filetypes:"
             "<ul>"
             "<li>NetCDF: <code>[.nc]<code></li>"
             "<li>GeoTIFF: <code>[.tif, .tiff]<code></li>"
             "<li>CSV: <code>[.csv]<code></li>"
             "<li>Shapefile: <code>[.shp]<code></li>"
             "</ul>"
         )
 
-        self.open_button = QtWidgets.QPushButton("Open File")
-
         layout = QtWidgets.QVBoxLayout()
         layout.addSpacing(10)
         layout.addWidget(self.t1)
-        layout.addSpacing(10)
-        layout.addWidget(self.open_button)
 
         layout.setAlignment(Qt.AlignCenter | Qt.AlignTop)
         self.setLayout(layout)
 
         self.setAcceptDrops(True)
 
     def enterEvent(self, e):
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
                 "<h3>Plot Data from Files</h3>"
-                "Click on the 'Open File' button or simply drag-and-drop one of the "
+                f"Click on {self.b_str} or simply drag-and-drop one of the "
                 "supported filetypes to get a popup window where you can specify how "
                 "you want to visualize the data."
                 "<p>"
                 "Supported filetypes:"
                 "<ul>"
                 "<li>NetCDF: <code>[.nc]<code></li>"
                 "<li>GeoTIFF: <code>[.tif, .tiff]<code></li>"
@@ -1103,40 +1333,74 @@
                 "<li>Be aware that re-projecting large datasets might take quite some "
                 "time and can require a lot of memory!</li>"
                 "</ul>",
             )
 
 
 class OpenFileTabs(QtWidgets.QTabWidget):
+    openNewFile = pyqtSignal()
+
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.m = m
+        self.openNewFile.connect(
+            lambda *args, **kwargs: self.new_file_tab(file_path=None)
+        )
+
+        self.gdf_file_endings = _get_gdf_file_endings()
 
         self.starttab = OpenDataStartTab(m=self.m)
-        self.starttab.open_button.clicked.connect(
-            lambda: self.new_file_tab(file_path=None)
-        )
 
         self.setTabsClosable(True)
         self.tabCloseRequested.connect(self.close_handler)
 
         self.addTab(self.starttab, "NEW")
         # don't show the close button for this tab
         self.tabBar().setTabButton(self.count() - 1, self.tabBar().RightSide, None)
 
+        self.setStyleSheet(
+            """
+            QTabWidget::pane {
+              border: 0px;
+              top:0px;
+              background: rgb(200, 200, 200);
+              border-radius: 10px;
+            }
+
+            QTabBar::tab {
+              background: rgb(220, 220, 220);
+              border: 0px;
+              padding: 3px;
+              padding-bottom: 6px;
+              margin-left: 10px;
+              margin-bottom: -2px;
+              border-radius: 4px;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(200, 200, 200);
+              border: 0px;
+              margin-bottom: -2px;
+            }
+            """
+        )
+
     def close_handler(self, index):
         widget = self.widget(index)
 
         path = widget.file_path
 
         self._msg = QtWidgets.QMessageBox(self)
         self._msg.setIcon(QtWidgets.QMessageBox.Question)
-        self._msg.setText(f"Do you really want to close the dataset \n\n '{path}'?")
-        self._msg.setWindowTitle("Close dataset?")
+        self._msg.setText(
+            f"Do you really want to REMOVE the dataset \n\n '{path}' \n\n"
+            "from the map?"
+        )
+        self._msg.setWindowTitle("Remove dataset?")
 
         self._msg.setStandardButtons(
             QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No
         )
         self._msg.buttonClicked.connect(lambda: self.do_close_tab(index))
 
         self._msg.show()
@@ -1148,27 +1412,29 @@
 
         widget = self.widget(index)
         try:
             if widget.m2.coll in self.m.BM._bg_artists[widget.m2.layer]:
                 self.m.BM.remove_bg_artist(widget.m2.coll, layer=widget.m2.layer)
                 widget.m2.coll.remove()
         except Exception:
-            print("EOmaps_companion: unable to remove dataset artist.")
+            _log.error("EOmaps_companion: unable to remove dataset artist.")
 
         widget.m2.cleanup()
 
-        # make sure all temporary pick-artists have been cleared
-        widget.m2.BM._clear_temp_artists("pick")
         # redraw if the layer was currently visible
-        self.m.redraw(widget.m2.layer)
+        if widget.m2.layer in self.m.BM.bg_layer:
+            self.m.redraw(widget.m2.layer)
 
         del widget.m2
 
         self.removeTab(index)
 
+        # emit a "dataPlotted" signal to update dropdowns etc.
+        self.m._emit_signal("dataPlotted")
+
     def dragEnterEvent(self, e):
         if e.mimeData().hasUrls():
             urls = e.mimeData().urls()
 
             if len(urls) > 1:
                 self.window().statusBar().showMessage(
                     "Dropping more than 1 file is not supported!"
@@ -1195,39 +1461,56 @@
             file_path = Path(
                 QtWidgets.QFileDialog.getOpenFileName(
                     filter=(
                         "Supported Files (*.nc *.tif *tiff *.csv *.shp);;" "all (*)"
                     )
                 )[0]
             )
+            # in case no file is selected, don't raise an error!
+            if len(file_path.name) == 0:
+                return
         elif isinstance(file_path, str):
             file_path = Path(file_path)
 
         global plc
         ending = file_path.suffix.lower()
         if ending in [".nc"]:
             plc = PlotNetCDFWidget(m=self.m, tab=self)
         elif ending in [".csv"]:
             plc = PlotCSVWidget(m=self.m, tab=self)
         elif ending in [".tif", ".tiff"]:
             plc = PlotGeoTIFFWidget(m=self.m, tab=self)
-        elif ending in [".shp"]:
-            plc = PlotShapeFileWidget(m=self.m)
+        elif ending in self.gdf_file_endings:
+            plc = PlotGeoDataFrameWidget(m=self.m)
         else:
+            _log.error(f"EOmaps: Unknown file extension '{ending}'")
             self.window().statusBar().showMessage(
-                f"Unknown file extension {ending}", 5000
+                f"ERROR: Unknown file extension {ending}", 5000
+            )
+            show_error_popup(
+                text=f"Unknown file extension {ending}.",
+                title="Unknown file extension.",
+                details=(
+                    "Supported file extensions: "
+                    f"{['.tiff', '.netcdf', *self.gdf_file_endings]}"
+                ),
             )
+
             return
 
         self.window().statusBar().clearMessage()
 
         try:
             plc.open_file(file_path)
         except Exception:
-            self.window().statusBar().showMessage("File could not be opened...", 5000)
             import traceback
 
+            _log.error(f"EOmaps Error: Unable to open file {file_path}")
+            self.window().statusBar().showMessage(
+                "ERROR: File could not be opened...", 5000
+            )
+
             show_error_popup(
                 text="There was an error while trying to open the file.",
                 title="Unable to open file.",
                 details=traceback.format_exc(),
             )
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/layer.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/layer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import Qt, pyqtSlot
+from ..common import iconpath
+from PyQt5 import QtGui
 
 
 class AutoUpdatePeekLayerDropdown(QtWidgets.QComboBox):
     def __init__(
         self,
         *args,
         m=None,
@@ -78,14 +80,16 @@
             self.addItem("")
 
         # the QAbstractItemView object that holds the dropdown-items
         view = self.view()
         view.setTextElideMode(Qt.ElideNone)
 
         for key in layers:
+            if key == "all":
+                continue
             self.addItem(str(key))
         # set the size of the dropdown to be 10 + the longest item
         view.setFixedWidth(view.sizeHintForColumn(0) + 10)
 
         if self._use_active:
             # set current index to active layer if _use_active
             currindex = self.findText(str(self.m.BM.bg_layer))
@@ -93,21 +97,65 @@
         elif self._last_active is not None:
             # set current index to last active layer otherwise
             idx = self.findText(self._last_active)
             if idx != -1:
                 self.setCurrentIndex(idx)
 
 
+class AutoUpdateLayerLabel(QtWidgets.QLabel):
+    def __init__(self, *args, m=None, max_length=100, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.m = m
+
+        self._max_length = max_length
+
+        # update layers on every change of the Maps-object background layer
+        self.m.BM.on_layer(self.update, persistent=True)
+        self.setText(self.get_text())
+
+        # turn text interaction off to "click through" the label
+        self.setTextInteractionFlags(Qt.NoTextInteraction)
+
+    def get_text(self):
+        layers, alphas = self.m.BM._get_layers_alphas()
+
+        prefix = "&nbsp;&nbsp;&nbsp;&nbsp;" "<font color=gray>"
+        suffix = "<\font>"
+
+        s = ""
+        for i, (l, a) in enumerate(zip(layers, alphas)):
+            if len(s) > self._max_length:
+                s = f"<b>( {len(layers)} layers visible )</b>"
+                break
+
+            if i > 0:
+                s += "  |  "
+
+            ls = f"<b>{l}</b>"
+            if a < 1:
+                ls += " {" + f"{a*100:.0f}%" + "}"
+
+            s += ls
+
+        return prefix + s + suffix
+
+    def update(self, *args, **kwargs):
+        self.setText(self.get_text())
+
+
 class AutoUpdateLayerMenuButton(QtWidgets.QPushButton):
-    def __init__(self, *args, m=None, layers=None, exclude=None, **kwargs):
+    def __init__(
+        self, *args, m=None, layers=None, exclude=None, auto_text=False, **kwargs
+    ):
         super().__init__(*args, **kwargs)
 
         self.m = m
         self._layers = layers
         self._exclude = exclude
+        self._auto_text = auto_text
 
         self._last_layers = []
 
         menu = QtWidgets.QMenu()
         menu.setStyleSheet("QMenu { menu-scrollable: 1;}")
         menu.aboutToShow.connect(self.update_layers)
         self.setMenu(menu)
@@ -116,28 +164,97 @@
         self.m.BM.on_layer(self.update_visible_layer, persistent=True)
         # update layers before the widget is shown to make sure they always
         # represent the currently visible layers on startup of the widget
         # (since "update_visible_layer" only triggers if the widget is actually visible)
         self.m._on_show_companion_widget.append(self.update_visible_layer)
         self.update_layers()
 
+        # set font properties before the stylesheet to avoid clipping of bold text!
+        font = QtGui.QFont("sans seriv", 8, QtGui.QFont.Bold, False)
+        self.setFont(font)
+        # self.setText("Layers:")
+        # self.layer_button.setText("")
+        # self.setIcon(QtGui.QIcon(str(iconpath / "layers.png")))
+
+        self.set_icons(str(iconpath / "layers.png"), str(iconpath / "layers_hover.png"))
+
+        self.setStyleSheet(
+            """
+            QPushButton {border: 0px;}
+            QPushButton::menu-indicator { width: 0; }
+            """
+        )
+
+        self.toggled.connect(self.swap_icon)
+
+    def set_icons(self, normal_icon=None, hoover_icon=None, checked_icon=None):
+        if normal_icon:
+            pm = QtGui.QPixmap(normal_icon)
+            self.normal_icon = QtGui.QIcon(
+                pm.scaled(
+                    self.size(),
+                    Qt.KeepAspectRatio,
+                    Qt.SmoothTransformation,
+                )
+            )
+            self.setIcon(self.normal_icon)
+            self.active_icon = self.normal_icon
+        if hoover_icon:
+            pm = QtGui.QPixmap(hoover_icon)
+            self.hoover_icon = QtGui.QIcon(
+                pm.scaled(
+                    self.size(),
+                    Qt.KeepAspectRatio,
+                    Qt.SmoothTransformation,
+                )
+            )
+        if checked_icon:
+            pm = QtGui.QPixmap(checked_icon)
+            self.checked_icon = QtGui.QIcon(
+                pm.scaled(
+                    self.size(),
+                    Qt.KeepAspectRatio,
+                    Qt.SmoothTransformation,
+                )
+            )
+        else:
+            self.checked_icon = self.hoover_icon
+
+    def swap_icon(self, *args, **kwargs):
+        if self.normal_icon and self.hoover_icon:
+            if self.isChecked():
+                self.active_icon = self.checked_icon
+            else:
+                self.active_icon = self.normal_icon
+            self.setIcon(self.active_icon)
+
+    def leaveEvent(self, event):
+        if self.active_icon:
+            self.setIcon(self.active_icon)
+
+        return super().enterEvent(event)
+
     def enterEvent(self, e):
+        if self.hoover_icon and not self.isChecked():
+            self.setIcon(self.hoover_icon)
+        else:
+            self.setIcon(self.normal_icon)
+
         if self.window().showhelp is True:
             QtWidgets.QToolTip.showText(
                 e.globalPos(),
-                "<h3>Visible Layer</h3>"
+                "<h3>Layer Dropdown Menu</h3>"
                 "Get a dropdown-list of all currently available map-layers."
                 "<p>"
                 "<ul>"
                 "<li><b>click</b> to switch to the selected layer</li>"
                 "<li><b>control+click</b> to overlay multiple layers</li>"
                 "</ul>"
-                "NOTE: The order at which you select layers will determine "
-                "the 'stacking' of the layers! (the number [n] in front "
-                " of the layer-name indicates the stack-order of the layer.",
+                "The number [n] in front of the layer-name indicates the "
+                "stack-order of the layer.",
             )
 
     def get_uselayer(self):
         active_layers = []
         for a in self.menu().actions():
             w = a.defaultWidget()
 
@@ -169,20 +286,22 @@
             return [
                 i
                 for i in self.m._get_layers(exclude=self._exclude)
                 if not str(i).startswith("_")
             ]
 
     def update_display_text(self, l):
+        if not self._auto_text:
+            return
         # make sure that we don't use too long labels as text
         if len(l) > 50:
             l = f"{len([1 for i in l.split('|') if len(i) > 0])} layers visible"
             # txt = txt[:50] + " ..."
 
-        if "{" in l:  # TODO support transparency
+        if "{" in l:
             l = "custom :   " + l
             self.setStyleSheet("QPushButton{color: rgb(200,50,50)}")
         elif "|" in l:
             l = "multi :   " + l
             self.setStyleSheet("QPushButton{color: rgb(200,50,50)}")
         else:
             self.setStyleSheet("QPushButton{color: rgb(50,200,50)}")
@@ -246,23 +365,20 @@
             if uselayer != "???":
                 self.m.show_layer(uselayer)
         else:
             self.m.show_layer(selected_layer)
 
     def update_checkstatus(self):
         currlayer = str(self.m.BM.bg_layer)
-
-        if "{" in currlayer:  # TODO support transparency
-            active_layers = []
+        layers, alphas = self.m.BM._get_layers_alphas(currlayer)
+        if "|" in currlayer:
+            active_layers = [i for i in layers if not i.startswith("_")]
+            active_layers.append(currlayer)
         else:
-            if "|" in currlayer:
-                active_layers = [i for i in currlayer.split("|") if i != "_"]
-                active_layers.append(currlayer)
-            else:
-                active_layers = [currlayer]
+            active_layers = [currlayer]
 
         for action in self.menu().actions():
             key = action.data()
             w = action.defaultWidget()
             if isinstance(w, QtWidgets.QCheckBox):
                 # temporarily disconnect triggering the action on state-changes
                 w.clicked.disconnect(action.trigger)
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/peek.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/peek.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         self.set_rectangle_slider_stylesheet()
 
     def set_rectangle_slider_stylesheet(self):
         s = 5 + self.rectangle_size * 15
         border = (
             "2px solid black"
             if self.rectangle_size < 0.99
-            else "2px solid rgb(200,200,200)"
+            else "2px solid rgb(140,140,140)"
         )
 
         self.rectangle_slider.setStyleSheet(
             f"""
             QSlider::handle:horizontal {{
                 background-color: rgb(200,200,200);
                 border: {border};
@@ -307,45 +307,39 @@
                 "Assign a keyboard-modifier to the peek-callback. "
                 "If used, the peek-callback will <b>only</b> be executed if the "
                 "corresponding button is pressed on the keyboard!",
             )
 
 
 class PeekLayerWidget(QtWidgets.QWidget):
-    def __init__(
-        self, *args, m=None, layers=None, exclude=None, how=(0.5, 0.5), **kwargs
-    ):
+    def __init__(self, *args, m=None, layers=None, exclude=None, **kwargs):
         """
         A dropdown-list that attaches a peek-callback to look at the selected layer
 
         Parameters
         ----------
         layers : list or None, optional
             If a list is provided, only layers in the list will be used.
             Otherwise the available layers are fetched from the given Maps-object.
             The default is None.
         exclude : list, optional
             A list of layer-names to exclude. The default is None.
 
-        Returns
-        -------
-        None.
-
         """
         super().__init__(*args, **kwargs)
 
         self.m = m
         self._layers = layers
         self._exclude = exclude
 
         self.cid = None
         self.current_layer = None
 
         self.layerselector = AutoUpdatePeekLayerDropdown(
-            m=self.m, layers=layers, exclude=exclude
+            m=self.m, layers=self._layers, exclude=exclude
         )
         self.layerselector.update_layers()  # do this before attaching the callback!
         self.layerselector.currentIndexChanged[str].connect(self.set_layer_callback)
         self.layerselector.setMinimumWidth(100)
 
         self.buttons = PeekMethodButtons()
         self.buttons.methodChanged.connect(self.method_changed)
@@ -423,14 +417,23 @@
             layer=self.current_layer,
             how=self.buttons.how,
             alpha=self.buttons.alpha,
             modifier=modifier,
             shape=self.buttons.shape,
         )
 
+        # execute the attached callback with the last available
+        # event of the click-move container (to get a dynamic update
+        # of the peek-region when the method changes)
+        if self.m.all.cb._click_move._event is not None:
+            self.m.all.cb._click_move._execute_cbs(
+                self.m.all.cb._click_move._event, [self.cid]
+            )
+            self.m.BM.update()
+
     def remove_peek_cb(self):
         if self.cid is not None:
             if self.cid in self.m.all.cb.click.get.attached_callbacks:
                 self.m.all.cb.click.remove(self.cid)
             self.cid = None
 
 
@@ -446,50 +449,90 @@
         self.setElideMode(Qt.ElideRight)
 
     def tabSizeHint(self, index):
         size = QtWidgets.QTabBar.tabSizeHint(self, index)
         return QSize(min(size.width(), 150), size.height())
 
 
+class NewPeekTabWidget(QtWidgets.QWidget):
+    def __init__(self, *args, peektabs=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.peektabs = peektabs
+
+    def mousePressEvent(self, e):
+        # create a new peek-tab if the base-tab of the peek-widget is clicked
+        self.peektabs.make_new_tab()
+        self.peektabs.setCurrentIndex(0)
+
+
 class PeekTabs(QtWidgets.QTabWidget):
     def __init__(self, *args, m=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.m = m
 
         self.setTabBar(TabBar())
 
         self.setTabsClosable(True)
         self.tabCloseRequested.connect(self.close_handler)
 
         w = PeekLayerWidget(m=self.m)
-        self.addTab(w, peek_icons[w.buttons._method], "    ")
+        # self.addTab(w, peek_icons[w.buttons._method], "    ")
+
         self.setIconSize(QSize(10, 10))
         # update the tab title with the modifier key
         cb = self.settxt_factory(w)
         w.modifier.textChanged.connect(cb)
         w.buttons.methodChanged.connect(cb)
         w.layerselector.currentIndexChanged[str].connect(cb)
 
         # emit pyqtSignal to set text
         w.buttons.methodChanged.emit(w.buttons._method)
 
         # a tab that is used to create new tabs
-        newtabwidget = QtWidgets.QWidget()
+        newtabwidget = NewPeekTabWidget(peektabs=self)
         newtablayout = QtWidgets.QHBoxLayout()
-        l = QtWidgets.QLabel("Click on <b>+</b> to open a new peek layer tab!")
+        l = QtWidgets.QLabel("Click to open a new <b>peek layer</b> tab!")
         newtablayout.addWidget(l)
         newtabwidget.setLayout(newtablayout)
 
         self.addTab(newtabwidget, "+")
         # don't show the close button for this tab
         self.tabBar().setTabButton(self.count() - 1, self.tabBar().RightSide, None)
 
         self.tabBarClicked.connect(self.tabbar_clicked)
         self.setCurrentIndex(0)
 
+        self.setTabPosition(0)
+        self.setStyleSheet(
+            """
+            QTabWidget::pane {
+              border: 0px;
+              top:0px;
+              background: rgb(200, 200, 200);
+              border-radius: 10px;
+            }
+
+            QTabBar::tab {
+              background: rgb(220, 220, 220);
+              border: 0px;
+              padding: 3px;
+              padding-bottom: 6px;
+              margin-left: 10px;
+              margin-bottom: -2px;
+              border-radius: 4px;
+            }
+
+            QTabBar::tab:selected {
+              background: rgb(200, 200, 200);
+              border: 0px;
+              margin-bottom: -2px;
+            }
+            """
+        )
+
     def setTabText(self, index, tip):
         # set ToolTip as well wenn setting the TabText
         super().setTabText(index, tip)
         self.setTabToolTip(index, tip)
 
     def enterEvent(self, e):
         if self.window().showhelp is True:
@@ -502,27 +545,32 @@
                 "to quickly compare several different layers."
                 "<p>"
                 "Assign <b>modifiers</b> to the individual peek-callbacks to "
                 "switch between the peek-callbacks by holding the corresponding keys"
                 "on the keyboard.",
             )
 
+    def make_new_tab(self):
+        w = PeekLayerWidget(m=self.m)
+        self.insertTab(self.count() - 1, w, "    ")
+
+        # update the tab title with the modifier key
+        cb = self.settxt_factory(w)
+        w.modifier.textChanged.connect(cb)
+        w.buttons.methodChanged.connect(cb)
+        w.layerselector.currentIndexChanged[str].connect(cb)
+        # emit pyqtSignal to set text
+        w.buttons.methodChanged.emit(w.buttons._method)
+
+        return w
+
     @pyqtSlot(int)
     def tabbar_clicked(self, index):
         if self.tabText(index) == "+":
-            w = PeekLayerWidget(m=self.m)
-            self.insertTab(self.count() - 1, w, "    ")
-
-            # update the tab title with the modifier key
-            cb = self.settxt_factory(w)
-            w.modifier.textChanged.connect(cb)
-            w.buttons.methodChanged.connect(cb)
-            w.layerselector.currentIndexChanged[str].connect(cb)
-            # emit pyqtSignal to set text
-            w.buttons.methodChanged.emit(w.buttons._method)
+            self.make_new_tab()
 
     @pyqtSlot(int)
     def close_handler(self, index):
         curridx = self.currentIndex()
         self.widget(index).remove_peek_cb()
         self.removeTab(index)
         if index == curridx:
@@ -530,16 +578,17 @@
 
     def settxt_factory(self, w):
         @pyqtSlot()
         def settxt():
             self.setTabIcon(self.indexOf(w), peek_icons[w.buttons._method])
             mod = w.modifier.text().strip()
 
-            txt = ""
             if mod != "":
-                txt += f"[{mod}] "
+                txt = f"[{mod}] "
+            else:
+                txt = "  "
 
             tabtext = txt + (w.current_layer if w.current_layer is not None else "")
 
             self.setTabText(self.indexOf(w), tabtext)
 
         return settxt
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/utils.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PyQt5 import QtWidgets, QtGui
-from PyQt5.QtCore import Qt, QRectF, QSize, pyqtSlot
+from PyQt5.QtCore import Qt, QRectF, QSize, pyqtSlot, pyqtSignal
 from eomaps import Maps
 from functools import lru_cache
 
 import matplotlib.pyplot as plt
 
 
 @lru_cache()
@@ -127,14 +127,27 @@
             t = self.placeholderText()
 
         if t in self.crs_options:
             t = "Maps.CRS." + t
 
         return t
 
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>CRS</h3>"
+                "Set the coordinate reference system of the coordinates (x, y)."
+                "<ul>"
+                "<li>A name of a crs accessible via <code>Maps.CRS</code></li>"
+                "<li>An EPSG code</li>"
+                "<li>A PROJ or WKT string</li>"
+                "</ul>",
+            )
+
 
 class CmapDropdown(QtWidgets.QComboBox):
     def __init__(self, *args, startcmap="viridis", **kwargs):
         super().__init__(*args, **kwargs)
 
         self.setIconSize(QSize(100, 15))
         self.view().setVerticalScrollBarPolicy(Qt.ScrollBarAsNeeded)
@@ -144,21 +157,37 @@
 
         self.setStyleSheet("combobox-popup: 0;")
         self.setMaxVisibleItems(10)
         idx = self.findText(startcmap)
         if idx != -1:
             self.setCurrentIndex(idx)
 
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            QtWidgets.QToolTip.showText(
+                e.globalPos(),
+                "<h3>Colormap</h3>"
+                "Set the colormap that should be used when plotting the data.",
+            )
+
     def wheelEvent(self, e):
         # ignore mouse-wheel events to disable changing the colormap with the mousewheel
         pass
 
 
 class GetColorWidget(QtWidgets.QFrame):
-    def __init__(self, facecolor="#ff0000", edgecolor="#000000", linewidth=1, alpha=1):
+    def __init__(
+        self,
+        facecolor="#ff0000",
+        edgecolor="#000000",
+        linewidth=1,
+        alpha=1,
+        tooltip=None,
+        helptext=None,
+    ):
         """
         A widget that indicates a selected color (and opens a popup to change the
         color on click)
 
         Parameters
         ----------
         facecolor : str
@@ -170,14 +199,30 @@
         -------
         facecolor, edgecolor:
             The QColor object of the currently assigned facecolor/edgecolor.
             To get the hex-string, use    the  ".name()" property.
 
         """
 
+        if tooltip is None:
+            self._tooltip = (
+                "<b>click</b>: set facecolor <br> <b>alt + click</b>: set edgecolor"
+            )
+        else:
+            self._tooltip = tooltip
+
+        if helptext is None:
+            self._helptext = (
+                "<h3>Facecolor / Edgecolor</h3>"
+                "<ul><li><b>click</b> to set the facecolor</li>"
+                "<li><b>alt+click</b> to set the edgecolor</li></ul>"
+            )
+        else:
+            self._helptext = helptext
+
         super().__init__()
 
         if isinstance(facecolor, str):
             self.facecolor = QtGui.QColor(facecolor)
         else:
             self.facecolor = QtGui.QColor(*facecolor)
         if isinstance(edgecolor, str):
@@ -191,37 +236,30 @@
         self.setMinimumSize(15, 15)
         self.setMaximumSize(100, 100)
 
         self.setSizePolicy(
             QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding
         )
 
-        self.setToolTip(
-            "<b>click</b>: set facecolor <br> <b>alt + click</b>: set edgecolor"
-        )
+        self.setToolTip(self._tooltip)
 
         self.setStyleSheet(
             """QToolTip {
             font-family: "SansSerif";
             font-size:10;
             background-color: rgb(53, 53, 53);
             color: white;
             border: none;
             }
             """
         )
 
     def enterEvent(self, e):
         if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(),
-                "<h3>Facecolor / Edgecolor</h3>"
-                "<ul><li><b>click</b> to set the facecolor</li>"
-                "<li><b>alt+click</b> to set the edgecolor</li></ul>",
-            )
+            QtWidgets.QToolTip.showText(e.globalPos(), self._helptext)
 
     def resizeEvent(self, e):
         # make frame rectangular
         self.setMaximumHeight(self.width())
 
     def paintEvent(self, e):
         super().paintEvent(e)
@@ -280,25 +318,29 @@
         self._dialog.colorSelected.connect(self.cb_colorselected)
         self._dialog.setCurrentColor(QtGui.QColor(self.edgecolor))
         self._dialog.open()
 
     def set_facecolor(self, color):
         if isinstance(color, str):
             color = QtGui.QColor(color)
+        elif isinstance(color, (list, tuple)):
+            color = QtGui.QColor(*color)
 
         self.alpha = color.alpha() / 255
 
         color = QtGui.QColor(*color.getRgb()[:3], int(self.alpha * 255))
 
         self.facecolor = color
         self.update()
 
     def set_edgecolor(self, color):
         if isinstance(color, str):
             color = QtGui.QColor(color)
+        elif isinstance(color, (list, tuple)):
+            color = QtGui.QColor(*color)
 
         self.edgecolor = color
         self.update()
 
     def set_linewidth(self, linewidth):
         self.linewidth = linewidth
         self.update()
@@ -306,68 +348,29 @@
     def set_alpha(self, alpha):
         self.alpha = alpha
         self.set_facecolor(
             QtGui.QColor(*self.facecolor.getRgb()[:3], int(self.alpha * 255))
         )
 
 
-class EditLayoutButton(QtWidgets.QPushButton):
-    def __init__(self, *args, m=None, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.m = m
-
-        self.clicked.connect(self.callback)
-
-    def enterEvent(self, e):
-        if self.window().showhelp is True:
-            QtWidgets.QToolTip.showText(
-                e.globalPos(),
-                "<h3>Layout Editor</h3>"
-                "Toggle the EOmaps LayoutEditor to re-arrange the position and size"
-                "of the axes in the figure."
-                "<ul>"
-                "<li><b>Right-click</b> on axes with the mouse to select them (hold "
-                "down 'shift' to select multiple axes).</li>"
-                "<li><b>Drag</b> selected axes (or the <b>arrow-keys</b>) to adjust "
-                "their position</li>"
-                "<li>Use the <b>scroll-wheel</b> (or the <b>+/- keys</b>) to scale "
-                "the size of selected axes</li>"
-                "<li>Hold down <b>'h'</b> or <b>'v'</b> key to adjust "
-                "horizontal/vertical size. "
-                "(maps always keep their aspect-ratio!)</li>"
-                "<li>Hold down <b>'control'</b> to adjust the colorbar/histogram size."
-                "<li>Press <b>control + z</b> to undo the last step</li>"
-                "<li>Press <b>control + y</b> to redo the last undone step</li>"
-                "<li>Press <b>escape</b> to exit the LayoutEditor</li>"
-                "</ul>",
-            )
-
-    @pyqtSlot()
-    def callback(self):
-        if not self.m.parent._layout_editor._modifier_pressed:
-            self.m.parent.edit_layout()
-        else:
-            self.m.parent._layout_editor._undo_draggable()
-
-
 class AlphaSlider(QtWidgets.QSlider):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.alpha = 1
+        self._style = ""
 
         self.setRange(0, 100)
         self.setSingleStep(1)
         self.setTickInterval(10)
         self.setTickPosition(QtWidgets.QSlider.TicksBothSides)
         self.setValue(100)
 
         # self.setMinimumWidth(50)
-        self.setMaximumWidth(300)
+        # self.setMaximumWidth(300)
         self.setSizePolicy(
             QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Minimum
         )
 
         self.valueChanged.connect(self.value_changed)
 
         s = 14
@@ -398,10 +401,155 @@
             QSlider::groove:horizontal:hover {{
                 background-color: rgba(0,0,0,255);
             }}
 
             """
         )
 
+    def enterEvent(self, e):
+        if self.window().showhelp is True:
+            if self._style == "linewidth":
+                QtWidgets.QToolTip.showText(
+                    e.globalPos(),
+                    "<h3>Linewidth</h3> Set the linewidth of the shape boundary.",
+                )
+            elif self._style == "alpha":
+                QtWidgets.QToolTip.showText(
+                    e.globalPos(),
+                    "<h3>Transparency</h3> Set the transparency of the facecolor.",
+                )
+
+    def set_stylesheet(self):
+        if self._style == "linewidth":
+            self.set_linewidth_stylesheet()
+        elif self._style == "alpha":
+            self.set_alpha_stylesheet()
+
     @pyqtSlot(int)
     def value_changed(self, i):
         self.alpha = i / 100
+        self.set_stylesheet()
+
+    def set_linewidth_stylesheet(self):
+        self._style = "linewidth"
+
+        self.setStyleSheet(
+            """
+            QSlider::handle:horizontal {
+                background-color: black;
+                border: none;
+                border-radius: 0px;
+                height: 10px;
+                width: 5px;
+                margin: -10px 0;
+                padding: -10px 0px;
+            }
+            QSlider::groove:horizontal {
+                border-radius: 1px;
+                height: 1px;
+                margin: 5px;
+                background-color: rgba(0,0,0,50);
+            }
+            QSlider::groove:horizontal:hover {
+                background-color: rgba(0,0,0,255);
+            }
+            """
+        )
+
+    def set_alpha_stylesheet(self):
+        self._style = "alpha"
+        a = self.alpha * 255
+        s = 12
+        self.setStyleSheet(
+            f"""
+            QSlider::handle:horizontal {{
+                background-color: rgba(0,0,0,{a});
+                border: 1px solid black;
+                border-radius: {s//2}px;
+                height: {s}px;
+                width: {s}px;
+                margin: -{s//2}px 0px;
+                padding: -{s//2}px 0px;
+            }}
+            QSlider::groove:horizontal {{
+                border-radius: 1px;
+                height: 1px;
+                margin: 5px;
+                background-color: rgba(0,0,0,50);
+            }}
+            QSlider::groove:horizontal:hover {{
+                background-color: rgba(0,0,0,255);
+            }}
+            """
+        )
+
+
+class ColorWithSlidersWidget(QtWidgets.QWidget):
+    colorSelected = pyqtSignal()
+    alpha_slider_scale = 100
+    linewidth_slider_scale = 10
+
+    def __init__(
+        self,
+        *args,
+        facecolor="red",
+        edgecolor="black",
+        linewidth=1,
+        alpha=0.5,
+        **kwargs,
+    ):
+
+        super().__init__(*args, **kwargs)
+
+        self.color = GetColorWidget(
+            facecolor=facecolor, edgecolor=edgecolor, linewidth=linewidth, alpha=alpha
+        )
+        self.color.cb_colorselected = self.color_selected
+        self.color.setMaximumWidth(60)
+
+        self.alphaslider = AlphaSlider(Qt.Horizontal)
+        self.alphaslider.set_alpha_stylesheet()
+        self.alphaslider.valueChanged.connect(self.set_alpha_with_slider)
+        self.alphaslider.setValue(int(alpha * self.alpha_slider_scale))
+
+        self.linewidthslider = AlphaSlider(Qt.Horizontal)
+        self.linewidthslider.set_linewidth_stylesheet()
+        self.linewidthslider.valueChanged.connect(self.set_linewidth_with_slider)
+        self.linewidthslider.setValue(int(linewidth * self.linewidth_slider_scale))
+
+        layout_sliders = QtWidgets.QVBoxLayout()
+        layout_sliders.addWidget(self.alphaslider)
+        layout_sliders.addWidget(self.linewidthslider)
+
+        layout = QtWidgets.QHBoxLayout()
+        layout.addWidget(self.color)
+        layout.addLayout(layout_sliders)
+        self.setLayout(layout)
+
+    @property
+    def facecolor(self):
+        return self.color.facecolor
+
+    @property
+    def edgecolor(self):
+        return self.color.edgecolor
+
+    @property
+    def linewidth(self):
+        return self.color.linewidth
+
+    @property
+    def alpha(self):
+        return self.color.alpha
+
+    @pyqtSlot(int)
+    def set_alpha_with_slider(self, i):
+        self.color.set_alpha(i / self.alpha_slider_scale)
+        self.colorSelected.emit()
+
+    @pyqtSlot(int)
+    def set_linewidth_with_slider(self, i):
+        self.color.set_linewidth(i / self.linewidth_slider_scale)
+        self.colorSelected.emit()
+
+    def color_selected(self):
+        self.colorSelected.emit()
```

### Comparing `EOmaps-6.5/eomaps/qtcompanion/widgets/wms.py` & `EOmaps-7.0/eomaps/qtcompanion/widgets/wms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+import logging
+
 from PyQt5 import QtWidgets
-from PyQt5.QtCore import Qt, QThread, QObject, pyqtSignal, pyqtSlot
+from PyQt5.QtCore import Qt, QThread, QObject, pyqtSignal, pyqtSlot, QTimer
 from PyQt5.QtGui import QStatusTipEvent
 
 from ... import Maps, _data_dir
 from pathlib import Path
 import json
 import os
 
+_log = logging.getLogger(__name__)
+
 # the path to which already fetched WebMap layers are stored
 # (to avoid fetching available layers on menu-population)
 wms_layers_dumppath = Path(_data_dir) / "_companion_wms_layers.json"
 
 
 def remove_prefix(text, prefix):
     if text.startswith(prefix):
         return text[len(prefix) :]
     return text
 
 
+def _log_problem(name):
+    _log.error(
+        f"EOmaps: Problem while fetching wmslayers for {name}",
+        exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+    )
+
+
 class WMSBase:
     def __init__(self):
         pass
 
     def ask_for_legend(self, wms, wmslayer):
         if hasattr(wms, "add_legend"):
             try:
@@ -62,17 +73,17 @@
         self.m = m
         try:
             self.wmslayers = [
                 key
                 for key in self.m.add_wms.GEBCO.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for GEBCO", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.GEBCO.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -84,17 +95,17 @@
         self.m = m
         try:
             self.wmslayers = [
                 key
                 for key in self.m.add_wms.GMRT.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for GMRT", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.GMRT.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -106,17 +117,17 @@
         self.m = m
         try:
             self.wmslayers = [
                 key
                 for key in self.m.add_wms.GLAD.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for GLAD", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.GLAD.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -128,17 +139,17 @@
         self.m = m
         try:
             self.wmslayers = [
                 key
                 for key in self.m.add_wms.GOOGLE.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for GOOGLE", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.GOOGLE.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -150,17 +161,17 @@
         self.m = m
         try:
             self.wmslayers = [
                 key
                 for key in self.m.add_wms.CAMS.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for CAMS", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.CAMS.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -184,17 +195,17 @@
 
         try:
             self.wmslayers = [
                 key
                 for key in self.usewms.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for NASA_GIBS", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.usewms.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -206,26 +217,26 @@
         self.m = m
 
         try:
             self._AT_layers = [
                 "Austria__" + key
                 for key in self.m.add_wms.Austria.AT_basemap.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._AT_layers = []
-            print("EOmaps: Problem while fetching wmslayers for AT_Austria", ex)
+            _log_problem(self.name)
 
         try:
             self._Wien_layers = [
                 "Wien__" + key
                 for key in self.m.add_wms.Austria.Wien_basemap.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._Wien_layers = []
-            print("EOmaps: Problem while fetching wmslayers for AT_Wien", ex)
+            _log_problem(self.name)
 
         self.wmslayers = [*self._AT_layers, *self._Wien_layers]
 
     def do_add_layer(self, wmslayer, layer):
         if wmslayer in self._AT_layers:
             wms = getattr(
                 self.m.add_wms.Austria.AT_basemap.add_layer,
@@ -273,18 +284,20 @@
             layers = [i for i in self.wmslayers if i.startswith(prefix)]
             if wmslayer in layers:
                 service = getattr(self.m.add_wms.ESRI_ArcGIS, servicename, None)
 
                 wms = getattr(
                     service, remove_prefix(wmslayer, prefix)
                 ).add_layer.xyz_layer
+
+                wms.name = f"{self.name}_{wmslayer}"
                 break
 
         if wms is None:
-            print(f"EOaps: WebMap layer {wmslayer}, {layer} not found")
+            _log.error(f"EOaps: WebMap layer {wmslayer}, {layer} not found")
             return
 
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
 class WMS_OSM(WMSBase):
@@ -295,89 +308,89 @@
         self.m = m
         try:
             self.wmslayers = [
                 key
                 for key in self.m.add_wms.OpenStreetMap.add_layer.__dict__.keys()
                 if not (key in ["m"] or key.startswith("_"))
             ]
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for OSM", ex)
+            _log_problem("OSM")
 
         try:
             self._terrestis = [
                 "Terrestis__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_terrestis.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._terrestis = []
-            print("EOmaps: Problem while fetching wmslayers for OSM_terrestis", ex)
+            _log_problem("OSM_terrestis")
 
         try:
             self._mundialis = [
                 "Mundialis__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_mundialis.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._mundialis = []
-            print("EOmaps: Problem while fetching wmslayers for OSM_mundialis", ex)
+            _log_problem("OSM_mundialis")
 
         try:
             self._OSM_landuse = [
                 "OSM_landuse__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_landuse.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._OSM_landuse = []
-            print("Problem while fetching wmslayers for OSM_landuse", ex)
+            _log_problem("OSM_landuse")
 
         try:
             self._OSM_wms = [
                 "OSM_wms__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_wms.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._OSM_wms = []
-            print("Problem while fetching wmslayers for OSM_wms", ex)
+            _log_problem("OSM_wms")
 
         try:
             self._OSM_wheregroup = [
                 "WhereGroup__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_wheregroup.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._OSM_wheregroup = []
-            print("Problem while fetching wmslayers for OSM_wheregroup", ex)
+            _log_problem("OSM_wheregroup")
 
         try:
             self._OSM_waymarkedtrails = [
                 "WaymarkedTrails__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_waymarkedtrails.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._OSM_waymarkedtrails = []
-            print("Problem while fetching wmslayers for OSM_waymarkedtrails", ex)
+            _log_problem("OSM_waymarkedtrails")
 
         try:
             self._OSM_openrailwaymap = [
                 "OpenRailwayMap__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_openrailwaymap.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._OSM_openrailwaymap = []
-            print("Problem while fetching wmslayers for OSM_openrailwaymap", ex)
+            _log_problem("OSM_openrailwaymap")
 
         try:
             self._OSM_cartodb = [
                 "CartoDB__" + i
                 for i in m.add_wms.OpenStreetMap.OSM_cartodb.add_layer.__dict__
             ]
-        except Exception as ex:
+        except Exception:
             self._OSM_cartodb = []
-            print("Problem while fetching wmslayers for OSM_cartodb", ex)
+            _log_problem("OSM_cartodb")
 
         self.wmslayers += self._terrestis
         self.wmslayers += self._mundialis
         self.wmslayers += self._OSM_landuse
         self.wmslayers += self._OSM_wms
         self.wmslayers += self._OSM_wheregroup
         self.wmslayers += self._OSM_waymarkedtrails
@@ -416,17 +429,17 @@
     layer_prefix = "S2_"
     name = "S2 cloudless"
 
     def __init__(self, m=None):
         self.m = m
         try:
             self.wmslayers = sorted(self.m.add_wms.S2_cloudless.layers)
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for S2_cloudless", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.S2_cloudless.add_layer, wmslayer)
         wms(layer=layer)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -434,17 +447,17 @@
     layer_prefix = ""
     name = "ESA WorldCover"
 
     def __init__(self, m=None):
         self.m = m
         try:
             self.wmslayers = self.m.add_wms.ESA_WorldCover.layers
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for ESA_WorldCover", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.ESA_WorldCover.add_layer, wmslayer)
         wms(layer=layer)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -479,20 +492,16 @@
                         key
                         for key in getattr(
                             self.m.add_wms.ISRIC_SoilGrids, l
                         ).add_layer.__dict__.keys()
                         if not (key in ["m"] or key.startswith("_"))
                     ]
                 )
-            except Exception as ex:
-                print(
-                    "EOmaps: Problem while fetching wmslayers for ISRIC_SoilGrids "
-                    f"{subs}",
-                    ex,
-                )
+            except Exception:
+                _log_problem(f"ISRIC_SoilGrids {subs}")
 
     def do_add_layer(self, wmslayer, layer):
 
         sub = wmslayer.split("_", 1)[0]
 
         wms = getattr(getattr(self.m.add_wms.ISRIC_SoilGrids, sub).add_layer, wmslayer)
         wms(layer=layer)
@@ -503,17 +512,17 @@
     layer_prefix = "DLR_bm_"
     name = "DLR basemaps"
 
     def __init__(self, m=None):
         self.m = m
         try:
             self.wmslayers = self.m.add_wms.DLR_basemaps.layers
-        except Exception as ex:
+        except Exception:
             self.wmslayers = []
-            print("EOmaps: Problem while fetching wmslayers for DLR_basemaps", ex)
+            _log_problem(self.name)
 
     def do_add_layer(self, wmslayer, layer):
         wms = getattr(self.m.add_wms.DLR_basemaps.add_layer, wmslayer)
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
@@ -529,25 +538,25 @@
             self._moon = [
                 "Moon__" + i
                 for i in m.add_wms.OpenPlanetary.Moon.add_layer.__dict__
                 if not i.startswith("_")
             ]
         except Exception as ex:
             self._moon = []
-            print("EOmaps: Problem while fetching wmslayers for OpenPlanetary", ex)
+            _log_problem(self.name)
 
         try:
             self._mars = [
                 "Mars__" + i
                 for i in m.add_wms.OpenPlanetary.Mars.add_layer.__dict__
                 if not i.startswith("_")
             ]
         except Exception as ex:
             self._mars = []
-            print("EOmaps: Problem while fetching wmslayers for OpenPlanetary", ex)
+            _log_problem(self.name)
 
         self.wmslayers += self._moon
         self.wmslayers += self._mars
 
     def do_add_layer(self, wmslayer, layer):
 
         wms = None
@@ -560,15 +569,15 @@
 
             if wmslayer in layers:
                 service = getattr(self.m.add_wms.OpenPlanetary, servicename, None)
                 wms = getattr(service.add_layer, remove_prefix(wmslayer, prefix))
                 break
 
         if wms is None:
-            print("EOmaps: the wms service {wmslayer} does not exist")
+            _log.error("EOmaps: the wms service {wmslayer} does not exist")
             return
 
         wms(layer=layer, transparent=True)
         self.ask_for_legend(wms, wmslayer)
 
 
 # an event-filter to catch StatusTipFilter events
@@ -579,20 +588,22 @@
             return True
         return super().eventFilter(watched, event)
 
 
 class AddWMSMenuButton(QtWidgets.QPushButton):
     wmsLayerCreated = pyqtSignal(str)
 
-    def __init__(self, *args, m=None, new_layer=False, show_layer=False, **kwargs):
+    def __init__(
+        self, *args, m=None, new_layer=False, show_layer=False, layer=None, **kwargs
+    ):
         super().__init__(*args, **kwargs)
         self.m = m
         self._new_layer = new_layer
         self._show_layer = show_layer
-        self.layer = None
+        self.layer = layer
 
         self.wms_dict = {
             "OpenStreetMap": WMS_OSM,
             "S2 Cloudless": WMS_S2_cloudless,
             "ESA WorldCover": WMS_ESA_WorldCover,
             "S1GBM": WMS_S1GBM,
             "GEBCO": WMS_GEBCO,
@@ -605,17 +616,17 @@
             "DLR Basemaps": WMS_DLR_basemaps,
             "ESRI_ArcGIS": ESRI_ArcGIS,
             "Austria Basemaps": WMS_Austria,
             "OpenPlanetary": WMS_OpenPlanetary,
         }
 
         if self._new_layer:
-            self.setText("Create new WebMap Layer")
+            self.setText("New WebMap Layer")
         else:
-            self.setText("Add WebMap Service")
+            self.setText("Add WebMap")
 
         width = self.fontMetrics().boundingRect(self.text()).width()
         self.setFixedWidth(width + 30)
 
         self.feature_menu = QtWidgets.QMenu()
         self.feature_menu.setStyleSheet("QMenu { menu-scrollable: 1;}")
         self.feature_menu.aboutToShow.connect(self.populate_menu)
@@ -627,25 +638,39 @@
         # The cache will be updated if a layer of the wms-service is added to the map!
         # (since then the layers are anyways re-fetched)
         if wms_layers_dumppath.exists():
             try:
                 with open(wms_layers_dumppath, "r") as file:
                     self._submenus = json.load(file)
             except Exception:
-                print(
-                    "EOmaps: Unable to load cached wms-layers from:\n    ",
-                    wms_layers_dumppath,
+                _log.error(
+                    f"EOmaps: Unable to load cached wms-layers from: \n"
+                    "{wms_layers_dumppath}",
                 )
                 self._submenus = dict()
         else:
             self._submenus = dict()
 
         # set event-filter to avoid showing tooltips on hovver over QMenu items
         self.installEventFilter(StatusTipFilter(self))
 
+        self.setStyleSheet(
+            """
+            QPushButton {
+                border: 0px;
+                border-radius: 4px;
+                padding: 4px;
+            }
+            QPushButton:hover {
+                background-color: rgb(210, 210, 210);
+            }
+
+            """
+        )
+
     def enterEvent(self, e):
         if self.window().showhelp is True:
             if self._new_layer:
                 QtWidgets.QToolTip.showText(
                     e.globalPos(),
                     "<h3>New WebMap Layer</h3>"
                     "Create a new layer (<i>''[wms service]_[wms layer]''</i>) and add "
@@ -723,89 +748,105 @@
     def fetch_submenu(self, wmsname):
         try:
             # disconnect callbacks to avoid recursions
             self.sub_menus[wmsname].aboutToShow.disconnect()
 
             self._fetch_submenu(wmsname)
         except Exception as ex:
-            print(f"EOmaps: problem while trying to fetch the submenu for {wmsname}")
+            _log.error(
+                f"EOmaps: problem while trying to fetch the submenu for {wmsname}",
+                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+            )
 
     def _fetch_submenu(self, wmsname):
         if wmsname in getattr(Maps, "_companion_wms_submenus", dict()):
             self._submenus[wmsname] = Maps._companion_wms_submenus[wmsname]
 
         if wmsname in self._submenus:
             return
 
-        print(f"EOmaps: Fetching WMS layers for {wmsname} ...")
+        _log.info(f"EOmaps: Fetching WMS layers for {wmsname} ...")
 
         wmsclass = self.wms_dict[wmsname]
         wms = wmsclass(m=self.m)
         sub_features = wms.wmslayers
         self._submenus[wmsname] = sub_features
 
         if not hasattr(Maps, "_companion_wms_submenus"):
             Maps._companion_wms_submenus = dict()
         Maps._companion_wms_submenus[wmsname] = sub_features
 
         self._update_layer_cache(wmsname, wms.wmslayers)
 
     def populate_submenu(self, wmsname=None):
         if wmsname not in self._submenus:
-            print("No layers found for the WMS: {wmsname}")
+            _log.info("No layers found for the WMS: {wmsname}")
             return
         else:
             sub_features = self.select_wmslayers(wmsname, self._submenus[wmsname])
 
         try:
             submenu = self.sub_menus[wmsname]
 
             for wmslayer in sub_features:
                 action = submenu.addAction(wmslayer)
                 action.triggered.connect(self.menu_callback_factory(wmsname, wmslayer))
 
         except Exception:
-            print("There was a problem with the WMS: " + wmsname)
+            _log.error(f"There was a problem with the WMS: {wmsname}")
 
     @pyqtSlot()
     def menu_callback_factory(self, wmsname, wmslayer):
         @pyqtSlot()
         def wms_cb():
+
+            self.window().statusBar().showMessage(
+                f"Adding WebMap service:   {wmsname} - {wmslayer}   . . ."
+            )
+            # trigger an immediate repaint of the statusbar to show the messge
+            # before fetching the service
+            self.window().statusBar().repaint()
+
             wmsclass = self.wms_dict[wmsname]
             wms = wmsclass(m=self.m)
 
             if self._new_layer:
                 layer = wms.layer_prefix + wmslayer
                 # indicate creation of new layer in statusbar
                 self.window().statusBar().showMessage(
                     f"New WebMap layer '{layer}' created!", 5000
                 )
 
             else:
-                layer = self.layer
+                layer = str(self.layer)
                 if layer.startswith("_") and "|" in layer:
                     self.window().statusBar().showMessage(
                         "Adding features to temporary multi-layers is not supported!",
                         5000,
                     )
                     return
 
+                self.window().statusBar().showMessage(
+                    f"WebMap service added!   {wmsname} - {wmslayer}   . . .", 2000
+                )
+            self.window().statusBar().repaint()
+
             wms.do_add_layer(wmslayer, layer=layer)
 
             # update the cached layer-names if necessary
             self._update_layer_cache(wmsname, wms.wmslayers)
 
-            # emit a signal that a new layer has been created
-            self.wmsLayerCreated.emit(str(layer))
-
             if self._show_layer:
                 self.m.show_layer(layer)
 
+            # emit a signal that a new layer has been created
+            self.wmsLayerCreated.emit(layer)
+
             # call draw to make sure the wms service is properly fetched
-            self.m.BM.canvas.draw_idle()
+            self.m.redraw(layer)
 
         return wms_cb
 
     def _update_layer_cache(self, wmsname, layers):
         """
         Update the layer-cache for the wms-menu-buttons
 
@@ -875,15 +916,15 @@
 
         Returns
         -------
         dict
             The cached webmap layer names.
 
         """
-        print("EOmaps: Fetching WMS layers for the companion widget...")
+        _log.info("EOmaps: Fetching WMS layers for the companion widget...")
 
         b = cls(m=m)
 
         if refetch is True:
             b._submenus = dict()
 
         for wmsname in b.wms_dict:
```

### Comparing `EOmaps-6.5/eomaps/reader.py` & `EOmaps-7.0/eomaps/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,19 @@
+"""Classes to read files (NetCDF, GeoTIFF, CSV etc.)"""
+
+import logging
 from functools import wraps
-import numpy as np
-from pyproj import CRS
 from pathlib import Path
 
-pd = None
-
-
-def _register_pandas():
-    global pd
-    try:
-        import pandas as pd
-    except ImportError:
-        return False
-
-    return True
-
-
-xar = None
-
-
-def _register_xarray():
-    global xar
-    try:
-        import xarray as xar
-    except ImportError:
-        return False
-    return True
-
+import numpy as np
+from pyproj import CRS
 
-rioxarray = None
+from .helpers import register_modules
 
-
-def _register_rioxarray():
-    global rioxarray
-    try:
-        import rioxarray
-    except ImportError:
-        return False
-    return True
+_log = logging.getLogger(__name__)
 
 
 def identify_geotiff_cmap(path, band=1):
     """
     Identify GeoTIFF colormap.
 
     Check if a GeoTiff file contains a color specification and return appropriate
@@ -73,30 +45,33 @@
             colors = np.array(list(c.values())) / 255
             bins = list(c)
 
             cmap = ListedColormap(colors)
 
             classify_specs = dict(scheme="UserDefined", bins=bins)
         except ValueError:
-            print(
-                f"EOmaps: No cmap found for GeoTIFF band {band}, defaulting to 'viridis'"
+            _log.info(
+                f"EOmaps: No cmap found for GeoTIFF band {band}, using: 'viridis'"
             )
             classify_specs = None
             cmap = "viridis"
         except IndexError:
-            print(
-                f"EOmaps: No cmap found for GeoTIFF band {band}, defaulting to 'viridis'"
+            _log.info(
+                f"EOmaps: No cmap found for GeoTIFF band {band}, using: 'viridis'"
             )
             classify_specs = None
             cmap = "viridis"
 
         return cmap, classify_specs
 
     except ImportError as ex:
-        print("EOmaps: Unable to identify cmap for GeoTIFF:", ex)
+        _log.info(
+            "EOmaps: Unable to identify cmap for GeoTIFF, using: 'viridis'",
+            exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
+        )
         return "viridis", None
 
 
 class read_file:
     """
     A collection of methods to read data from a file.
 
@@ -214,20 +189,15 @@
         >>>     data = m.read_file.GeoTIFF(file)
 
         # to assign the data directly to the Maps-object, use `set_data=<Maps object>`:
 
         >>> m.read_file.GeoTIFF(path, set_data=m)
 
         """
-
-        assert _register_xarray() and _register_rioxarray(), (
-            "EOmaps: missing dependency for read_GeoTIFF: 'xarray' 'rioxarray'\n"
-            + "To install, use 'conda install -c conda-forge xarray'"
-            + "To install, use 'conda install -c conda-forge rioxarray'"
-        )
+        xar, rioxarray = register_modules("xarray", "rioxarray")
 
         if isel is None and sel is None:
             isel = {"band": 0}
 
         opened = False  # just an indicator if we have to close the file in the end
         try:
             if isinstance(path_or_dataset, (str, Path)):
@@ -448,19 +418,15 @@
 
         # to assign the data directly to the Maps-object, use `set_data=<Maps object>`:
 
         >>> m.read_file.NetCDF(path, set_data=m)
 
 
         """
-
-        assert _register_xarray(), (
-            "EOmaps: missing dependency for read_GeoTIFF: 'xarray'\n"
-            + "To install, use 'conda install -c conda-forge xarray'"
-        )
+        (xar,) = register_modules("xarray")
 
         opened = False  # just an indicator if we have to close the file in the end
         try:
             if isinstance(path_or_dataset, (str, Path)):
                 # if a path is provided, open the file (and close it in the end)
                 ncfile = xar.open_dataset(
                     path_or_dataset, mask_and_scale=mask_and_scale
@@ -480,15 +446,15 @@
             elif isel is not None:
                 usencfile = ncfile.isel(**isel)
             else:
                 usencfile = ncfile
 
             if parameter is None:
                 parameter = next(iter(ncfile))
-                print(f"EOmaps: Using NetCDF variable '{parameter}' as parameter.")
+                _log.info(f"EOmaps: Using NetCDF variable '{parameter}' as parameter.")
             else:
                 assert parameter in ncfile, (
                     f"EOmaps: The provided parameter-name '{parameter}' is not valid."
                     + f"Available parameters are {list(ncfile)}"
                 )
 
             data = usencfile[parameter]
@@ -499,15 +465,15 @@
                         "EOmaps: could not identify the coordinate-dimensions! "
                         + "Please provide coordinate-names explicitly via the "
                         + "'coords' kwarg.\n"
                         + f"Available coordinates: {list(usencfile.coords)}\n"
                         + f"Available variables: {list(ncfile)}"
                     )
                 else:
-                    print(f"EOmaps: Using NetCDF coordinates: {coords}")
+                    _log.info(f"EOmaps: Using NetCDF coordinates: {coords}")
 
             if data_crs is None:
                 for crskey in ["spatial_ref", "crs", "crs_wkt"]:
                     if crskey in usencfile.attrs:
                         data_crs = usencfile.attrs[crskey]
 
             assert data_crs is not None, (
@@ -643,38 +609,39 @@
 
         Returns
         -------
         dict (if set_data is False) or None (if set_data is True)
             A dict that contains the data required for plotting.
 
         """
-        assert _register_pandas(), (
-            "EOmaps: missing dependency for read_csv: 'pandas'\n"
-            + "To install, use 'conda install -c conda-forge pandas'"
-        )
+        (pd,) = register_modules("pandas")
 
         data = pd.read_csv(path, **kwargs)
 
         for key in [parameter, x, y]:
             assert key in data, (
                 f"EOmaps: the parameter-name {key} is not a column of the csv-file!\n"
                 + f"Available columns are: {list(data)}"
             )
 
+        # make sure only unique columns are selected
+        # (multiple columns with the same name cause problems!)
+        usecols = list(dict.fromkeys([parameter, x, y]))
+
         if set_data is not None:
             set_data.set_data(
-                data=data[[parameter, x, y]],
+                data=data[usecols],
                 x=x,
                 y=y,
                 crs=crs,
                 parameter=parameter,
             )
         else:
             return dict(
-                data=data[[parameter, x, y]],
+                data=data[usecols],
                 x=x,
                 y=y,
                 crs=crs,
                 parameter=parameter,
             )
 
 
@@ -785,15 +752,17 @@
             crs = Maps._get_cartopy_crs(crs=crs)
         except Exception:
             try:
                 crs = Maps._get_cartopy_crs(crs=CRS.from_user_input(crs))
 
             except Exception:
                 crs = 4326
-                print(f"EOmaps: could not use native crs... defaulting to epsg={crs}.")
+                _log.warning(
+                    f"EOmaps: could not use native crs... defaulting to epsg={crs}."
+                )
 
         m = Maps(crs=crs, figsize=figsize, layer=layer)
 
     if coastline:
         m.add_feature.preset.coastline()
 
     m.set_data(**data)
@@ -812,22 +781,22 @@
     if extent is not None:
         if isinstance(extent, tuple):
             if len(extent) == 2 and len(extent[0]) == 4:
                 m.set_extent(extent[0], crs=extent[1])
             elif len(extent) == 4:
                 m.set_extent(extent)
             else:
-                print(
+                _log.warning(
                     "EOmaps: unable to identify the provided extent"
                     f"{extent}... defaulting to global"
                 )
         elif isinstance(extent, str):
             m.set_extent_to_location(extent)
         else:
-            print(
+            _log.warning(
                 "EOmaps: unable to identify the provided extent"
                 f"{extent}... defaulting to global"
             )
 
     m.plot_map(**kwargs)
     return m
 
@@ -1026,19 +995,14 @@
         >>> m = Maps.from_file.NetCDF(file)
 
         >>> with xar.open_dataset(path) as file:
         >>>     m = Maps.from_file.NetCDF(file)
 
         """
 
-        assert _register_xarray(), (
-            "EOmaps: missing dependency for read_NetCDF: 'xarray'\n"
-            + "To install, use 'conda install -c conda-forge xarray'"
-        )
-
         # read data
         data = read_file.NetCDF(
             path_or_dataset,
             parameter=parameter,
             coords=coords,
             crs_key=data_crs_key,
             data_crs=data_crs,
@@ -1227,21 +1191,14 @@
         >>> file = xar.open_dataset(path)
         >>> m = Maps.from_file.GeoTIFF(file)
 
         >>> with xar.open_dataset(path) as file:
         >>>     m = Maps.from_file.GeoTIFF(file)
 
         """
-
-        assert _register_xarray() and _register_rioxarray(), (
-            "EOmaps: missing dependency for read_GeoTIFF: 'xarray' 'rioxarray'\n"
-            + "To install, use 'conda install -c conda-forge xarray'"
-            + "To install, use 'conda install -c conda-forge rioxarray'"
-        )
-
         # read data
         data = read_file.GeoTIFF(
             path_or_dataset,
             sel=sel,
             isel=isel,
             set_data=None,
             data_crs=data_crs,
@@ -1260,14 +1217,16 @@
         ):
 
             # try to identify used band
             if sel is not None and "band" in sel:
                 band = sel.get("band", 1)
 
             elif isel is not None and "band" in isel:
+                (xar,) = register_modules("xarray")
+
                 with xar.open_dataset(path_or_dataset) as ncfile:
                     band = np.atleast_1d(ncfile.isel(**isel).band.values)[0]
             else:
                 band = 1
 
             cmap, classify_specs = identify_geotiff_cmap(path_or_dataset, band=band)
             kwargs["cmap"] = cmap
```

### Comparing `EOmaps-6.5/eomaps/scalebar.py` & `EOmaps-7.0/eomaps/scalebar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from .helpers import pairwise
+"""Interactive scalebar."""
+
+import logging
 from collections import OrderedDict
 from functools import lru_cache
-import warnings
 
 import numpy as np
 
 from matplotlib.collections import LineCollection
 from matplotlib.textpath import TextPath
 from matplotlib.patches import Polygon, PathPatch
 from matplotlib.transforms import Affine2D
 from matplotlib.font_manager import FontProperties
 from matplotlib.colors import to_hex
 
+from .helpers import pairwise
+
 _picked_scalebars = set()
 
+_log = logging.getLogger(__name__)
+
 
 class ScaleBar:
     """Base class for EOmaps scalebars."""
 
     def __init__(
         self,
         m,
@@ -280,14 +285,15 @@
             import black
 
             code = black.format_str(s, mode=black.Mode())
             print(code)
             if return_str:
                 return s
         except ImportError:
+            _log.debug("Error during code formatting", exc_info=True)
             print(s)
             if return_str:
                 return s
 
     def _get_code(self, fixed=True, precision=10):
         """
         Return a string that can be used to reproduce the scalebar in its current state.
@@ -499,15 +505,15 @@
         scale  : float, optional
             The length (in meters) of the individual line-segments.
             If None, the scale will be determined automatically based on the currently
             visible plot-extent. The default is None.
 
         See Also
         --------
-        set_n : Set the number of segments to use.
+        ScaleBar.set_n : Set the number of segments to use.
 
         """
         self._scale = scale
         self._update(BM_update=True)
 
     def set_n(self, n=None):
         """
@@ -516,15 +522,15 @@
         Parameters
         ----------
         n  : int, optional
             The number of segments. The default is None.
 
         See Also
         --------
-        set_scale : Set the length of the scalebar segments.
+        ScaleBar.set_scale : Set the length of the scalebar segments.
 
         """
         self._n = n
 
         # if the number of segments changed, re-draw labels completely!
         self._redraw_minitxt()
         self._update(BM_update=True)
@@ -541,54 +547,26 @@
         colors : tuple, optional
             A sequence of colors that will be repeated to color the individual
             line-fragments of the scalebar. (you can provide more than 2 colors!)
             The default is ("k", "w").
 
         See Also
         --------
-        set_scale : Set a fixed length of the scalebar segments.
-
-        set_n : Set the number of segments to use.
-
-        set_patch_props : Set style properties of the scalebar frame.
-
-        set_label_props : Set style properties of the labels.
-
-        set_line_props : Set style properties of the lines between scalebar and labels.
+        ScaleBar.set_scale : Set a fixed length of the scalebar segments.
+        ScaleBar.set_n : Set the number of segments to use.
+        ScaleBar.set_patch_props : Set style properties of the scalebar frame.
+        ScaleBar.set_label_props : Set style properties of the labels.
+        ScaleBar.set_line_props : Set style of the lines between scalebar and labels.
 
         """
         self._set_scale_props(width=width, colors=colors, **kwargs)
 
         self._update(BM_update=True)
 
     def _set_scale_props(self, width=None, colors=None, **kwargs):
-        if "n" in kwargs:
-            warnings.warn(
-                "EOmaps: Setting the number of scalebar segments ('n') via the "
-                "`scale_props` is depreciated and will raise an error in the next "
-                "major release! \n"
-                "Use `s = m.add_scalebar(n=...)` or `s.set_n(...)` instead! ",
-                FutureWarning,
-                stacklevel=4,
-            )
-            self._n = kwargs.pop("n")
-            if hasattr(self, "_lon"):
-                self._redraw_minitxt()
-
-        if "scale" in kwargs:
-            warnings.warn(
-                "EOmaps: Setting the length of the scalebar segments ('scale') via the "
-                "`scale_props` is depreciated and will raise an error in the next major "
-                " release! \n"
-                "Use `s = m.add_scalebar(scale=...)` or `s.set_scale(...)` instead! ",
-                FutureWarning,
-                stacklevel=4,
-            )
-            self._scale = kwargs.pop("scale")
-
         if len(kwargs) > 0:
             raise TypeError(f"{list(kwargs)} are not allowed as 'scale_props' kwargs.")
 
         if width is not None:
             self._scale_props["width"] = width
         if colors is not None:
             self._scale_props["colors"] = colors
@@ -610,19 +588,17 @@
 
             Possible values are:
 
             - "facecolor", "edgecolor", "linewidth", "linestyle", "alpha" ...
 
         See Also
         --------
-        set_scale_props : Set style properties of the scale.
-
-        set_label_props : Set style properties of the labels.
-
-        set_line_props : Set style properties of the lines between scalebar and labels.
+        ScaleBar.set_scale_props : Set style of the scale.
+        ScaleBar.set_label_props : Set style of the labels.
+        ScaleBar.set_line_props : Set style of the lines between scalebar and labels.
 
         """
         for key in kwargs:
             if not hasattr(self._artists["patch"], f"set_{key}"):
                 raise AttributeError(f"EOmaps: '{key}' is not a valid patch property!")
 
         self._set_patch_props(offsets=offsets, **kwargs)
@@ -658,19 +634,17 @@
 
             Possible values are:
 
             - "edgecolor" (or "ec"), "linewidth" (or "lw"), "linestyle" (or "ls") ...
 
         See Also
         --------
-        set_scale_props : Set style properties of the scale.
-
-        set_patch_props : Set style properties of the scalebar frame.
-
-        set_label_props : Set style properties of the labels.
+        ScaleBar.set_scale_props : Set style of the scale.
+        ScaleBar.set_patch_props : Set style of the scalebar frame.
+        ScaleBar.set_label_props : Set style of the labels.
 
         """
         for key in kwargs:
             if not hasattr(self._artists["patch_lines"], f"set_{key}"):
                 raise AttributeError(f"EOmaps: '{key}' is not a valid line property!")
 
         self._set_line_props(**kwargs)
@@ -731,19 +705,17 @@
               - "family", "style", "variant", "stretch", and "weight"
 
             For example:
                 >>> dict(family="Helvetica", style="italic").
 
         See Also
         --------
-        set_scale_props : Set style properties of the scale.
-
-        set_patch_props : Set style properties of the scalebar frame.
-
-        set_line_props : Set style properties of the lines between scalebar and labels.
+        ScaleBar.set_scale_props : Set style of the scale.
+        ScaleBar.set_patch_props : Set style of the scalebar frame.
+        ScaleBar.set_line_props : Set style of the lines between scalebar and labels.
 
         """
         for key in kwargs:
             if not hasattr(FontProperties, f"set_{key}"):
                 raise AttributeError(f"EOmaps: '{key}' is not a valid font property!")
 
         self._set_label_props(
@@ -1439,15 +1411,15 @@
 
         ox, oy = self._pick_start_offset
         try:
             lon, lat = self._m._transf_plot_to_lonlat.transform(
                 event.xdata, event.ydata
             )
         except Exception:
-            print("EOmaps: Unable to position scalebar.")
+            _log.info("EOmaps: Unable to position scalebar.")
             return
 
         self._update(lon=lon + ox, lat=lat + oy, BM_update=True)
 
     def _cb_scroll(self, event):
         if not self._picked:
             return
@@ -1468,15 +1440,15 @@
             if self._scale is None:
                 self._autoscale = np.clip(
                     self._autoscale + multip * event.step / self._scale_factor_base,
                     0.01,
                     0.99,
                 )
             else:
-                print(
+                _log.warning(
                     "EOmaps: The scale of the scalebar is fixed! "
                     "Use s.set_scale(None) to use autoscaling!"
                 )
 
         self._update(BM_update=True)
 
     def _cb_keypress(self, event):
```

### Comparing `EOmaps-6.5/eomaps/utilities.py` & `EOmaps-7.0/eomaps/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Collection of utility classes (layer sliders, layer selectors etc.)"""
+
 from matplotlib.legend import DraggableLegend
 from matplotlib.lines import Line2D
 from matplotlib.widgets import Slider
 from functools import wraps
 from matplotlib.pyplot import Artist, rcParams
 
 
@@ -220,17 +222,16 @@
 
         To remove the widget (`s`), simply use:
 
         >>> s.remove()
 
         See Also
         --------
-
-        - m.util.layer_slider() : A slider widget to switch between layers.
-        - m.show_layer(): Set the currently visible layer.
+        utilities.layer_slider : A slider widget to switch between layers.
+        Maps.show_layer: Set the currently visible layer.
 
         """
 
         self._init_args = {
             "layers": layers,
             "draggable": draggable,
             "exclude_layers": exclude_layers,
@@ -566,15 +567,14 @@
 class utilities:
     """
     A collection of utility tools that can be added to EOmaps plots.
 
     Methods
     -------
     layer_selector: A legend-like widget to switch between layers
-
     layer_slider: A slider widget to switch between layers
 
     """
 
     def __init__(self, m):
         self._m = m
```

### Comparing `EOmaps-6.5/setup.py` & `EOmaps-7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         "pyepsg",
         "geopandas",
         "owslib",
         "requests",
         "xmltodict",
         "cairosvg",
         "packaging",
+        "click",
     ],
+    entry_points={"console_scripts": ["eomaps = eomaps.scripts.open:cli"]},
     keywords=["visualization", "plotting", "maps", "geographical data"],
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Visualization",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         # Pick your license as you wish (should match "license" above)
```

