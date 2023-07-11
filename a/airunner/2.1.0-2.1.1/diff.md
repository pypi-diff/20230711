# Comparing `tmp/airunner-2.1.0.tar.gz` & `tmp/airunner-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-2.1.0.tar", last modified: Tue Jul 11 01:08:54 2023, max compression
+gzip compressed data, was "airunner-2.1.1.tar", last modified: Tue Jul 11 03:10:51 2023, max compression
```

## Comparing `airunner-2.1.0.tar` & `airunner-2.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.850991 airunner-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 01:08:44.000000 airunner-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 01:08:54.850991 airunner-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-11 01:08:44.000000 airunner-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:08:54.850991 airunner-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 01:08:44.000000 airunner-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.830991 airunner-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.834991 airunner-2.1.0/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.838991 airunner-2.1.0/src/airunner/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.842991 airunner-2.1.0/src/airunner/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/brushes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_active_grid_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_brushes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_grid_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_image_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_selectionbox_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_widgets_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/comic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/embedding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/extension_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    32391 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/generator_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/history_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/lora_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/menubar_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/toolbar_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.846991 airunner-2.1.0/src/airunner/pyqt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/base_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/embedding_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/generate_form_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/lora_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/main_window_new_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/model_merger_model_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/model_merger_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/noise_filter_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/prompt_browser_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/saturation_window_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.850991 airunner-2.1.0/src/airunner/pyqt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/canvas_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/embedding_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/generator_tab_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/grid_preferences_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/header_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/layer_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/lora_container_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/lora_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/slider_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/tool_menu_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/toolbar_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.838991 airunner-2.1.0/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.571689 airunner-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 03:10:42.000000 airunner-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 03:10:51.571689 airunner-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-11 03:10:42.000000 airunner-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 03:10:51.571689 airunner-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 03:10:42.000000 airunner-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.563689 airunner-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.563689 airunner-2.1.1/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.563689 airunner-2.1.1/src/airunner/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27986 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.567690 airunner-2.1.1/src/airunner/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_active_grid_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_grid_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_image_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_selectionbox_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/canvas_widgets_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/comic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/embedding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/extension_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32361 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/generator_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/history_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/lora_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/menubar_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/mixins/toolbar_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.567690 airunner-2.1.1/src/airunner/pyqt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/base_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/generate_form_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/main_window_new_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/model_merger_model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/model_merger_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/noise_filter_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/prompt_browser_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/saturation_window_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.571689 airunner-2.1.1/src/airunner/pyqt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/canvas_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/generator_tab_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/grid_preferences_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/header_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/layer_container_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/layer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/lora_container_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/prompt_builder_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/slider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/tool_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/pyqt/widgets/toolbar_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-11 03:10:42.000000 airunner-2.1.1/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:10:51.563689 airunner-2.1.1/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 03:10:51.000000 airunner-2.1.1/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-11 03:10:51.000000 airunner-2.1.1/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:10:51.000000 airunner-2.1.1/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 03:10:51.000000 airunner-2.1.1/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 03:10:51.000000 airunner-2.1.1/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-2.1.0/LICENSE` & `airunner-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/PKG-INFO` & `airunner-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-2.1.0/README.md` & `airunner-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/setup.py` & `airunner-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="2.1.0",
+    version="2.1.1",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.18.1",
+        "aihandler==1.18.2",
     ]
 )
```

### Comparing `airunner-2.1.0/src/airunner/balloon.py` & `airunner-2.1.1/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/canvas.py` & `airunner-2.1.1/src/airunner/canvas.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/extensions.py` & `airunner-2.1.1/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/main.py` & `airunner-2.1.1/src/airunner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,17 @@
 
     def handle_bottom_splitter_moved(self, pos, index):
         top_height = self.center_splitter.widget(0).height()
         bottom_height = self.center_splitter.widget(1).height()
         self.settings_manager.settings.bottom_splitter_sizes.set([top_height, bottom_height])
 
     def initialize_saved_prompts(self):
+        print("INITIALZING PROMPTS")
         self.prompts_manager = PromptManager()
+        print(self.prompts_manager.settings.prompts)
         self.prompts_manager.enable_save()
 
     def initialize_settings_manager(self):
         self.settings_manager = SettingsManager()
         self.settings_manager.disable_save()
         # self.get_extensions_from_path()  TODO: Extensions
         self.settings_manager.settings.size.my_signal.connect(self.set_size_form_element_step_values)
```

### Comparing `airunner-2.1.0/src/airunner/mixins/brushes_mixin.py` & `airunner-2.1.1/src/airunner/mixins/brushes_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/canvas_active_grid_area_mixin.py` & `airunner-2.1.1/src/airunner/mixins/canvas_active_grid_area_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/canvas_brushes_mixin.py` & `airunner-2.1.1/src/airunner/mixins/canvas_brushes_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/canvas_grid_mixin.py` & `airunner-2.1.1/src/airunner/mixins/canvas_grid_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/canvas_image_mixin.py` & `airunner-2.1.1/src/airunner/mixins/canvas_image_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/canvas_selectionbox_mixin.py` & `airunner-2.1.1/src/airunner/mixins/canvas_selectionbox_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/comic_mixin.py` & `airunner-2.1.1/src/airunner/mixins/comic_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/embedding_mixin.py` & `airunner-2.1.1/src/airunner/mixins/embedding_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/extension_mixin.py` & `airunner-2.1.1/src/airunner/mixins/extension_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/generator_mixin.py` & `airunner-2.1.1/src/airunner/mixins/generator_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,18 +290,18 @@
         self.do_upscale_full_image_var.set(val)
 
     @property
     def image_to_new_layer(self):
         return self.settings_manager.settings.image_to_new_layer.get()
 
     def update_prompt(self, prompt):
-        self.tabs[self.current_section].prompt.setPlainText(prompt)
+        self.generator_tab_widget.set_prompt(prompt)
 
     def update_negative_prompt(self, prompt):
-        self.tabs[self.current_section].negative_prompt.setPlainText(prompt)
+        self.generator_tab_widget.set_negative_prompt(prompt)
 
     def initialize(self):
         self.tool_menu_widget.initialize()
         self.initialize_lora()
 
         # listen to F5 keypress and call self.generate_callback
         self.generate_shortcut = QShortcut(QKeySequence(Qt.Key.Key_F5), self)
```

### Comparing `airunner-2.1.0/src/airunner/mixins/history_mixin.py` & `airunner-2.1.1/src/airunner/mixins/history_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/lora_mixin.py` & `airunner-2.1.1/src/airunner/mixins/lora_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/menubar_mixin.py` & `airunner-2.1.1/src/airunner/mixins/menubar_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/mixins/toolbar_mixin.py` & `airunner-2.1.1/src/airunner/mixins/toolbar_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/base_window_ui.py` & `airunner-2.1.1/src/airunner/pyqt/base_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/embedding_ui.py` & `airunner-2.1.1/src/airunner/pyqt/embedding_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/generate_form_ui.py` & `airunner-2.1.1/src/airunner/pyqt/generate_form_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/lora_ui.py` & `airunner-2.1.1/src/airunner/pyqt/lora_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/main_window_new_ui.py` & `airunner-2.1.1/src/airunner/pyqt/main_window_new_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/main_window_ui.py` & `airunner-2.1.1/src/airunner/pyqt/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/model_merger_model_ui.py` & `airunner-2.1.1/src/airunner/pyqt/model_merger_model_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/model_merger_ui.py` & `airunner-2.1.1/src/airunner/pyqt/model_merger_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/noise_filter_ui.py` & `airunner-2.1.1/src/airunner/pyqt/noise_filter_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py` & `airunner-2.1.1/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/prompt_browser_ui.py` & `airunner-2.1.1/src/airunner/pyqt/prompt_browser_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/saturation_window_ui.py` & `airunner-2.1.1/src/airunner/pyqt/saturation_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/canvas_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/canvas_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/embedding_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/embedding_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/generator_tab_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/generator_tab_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/grid_preferences_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/grid_preferences_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/header_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/header_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/layer_container_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/layer_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/layer_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/lora_container_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/lora_container_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/lora_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/lora_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/prompt_builder_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/slider_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/slider_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/tool_menu_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/tool_menu_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/pyqt/widgets/toolbar_ui.py` & `airunner-2.1.1/src/airunner/pyqt/widgets/toolbar_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/runai_client.py` & `airunner-2.1.1/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/themes.py` & `airunner-2.1.1/src/airunner/themes.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner/utils.py` & `airunner-2.1.1/src/airunner/utils.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.0/src/airunner.egg-info/PKG-INFO` & `airunner-2.1.1/src/airunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-2.1.0/src/airunner.egg-info/SOURCES.txt` & `airunner-2.1.1/src/airunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

