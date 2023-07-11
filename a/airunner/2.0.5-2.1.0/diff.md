# Comparing `tmp/airunner-2.0.5.tar.gz` & `tmp/airunner-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-2.0.5.tar", last modified: Mon Jul 10 08:20:37 2023, max compression
+gzip compressed data, was "airunner-2.1.0.tar", last modified: Tue Jul 11 01:08:54 2023, max compression
```

## Comparing `airunner-2.0.5.tar` & `airunner-2.1.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.367770 airunner-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 08:20:25.000000 airunner-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-10 08:20:37.367770 airunner-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-10 08:20:25.000000 airunner-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:20:37.367770 airunner-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-10 08:20:25.000000 airunner-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.359770 airunner-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.359770 airunner-2.0.5/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.359770 airunner-2.0.5/src/airunner/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.363770 airunner-2.0.5/src/airunner/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/brushes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_active_grid_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_brushes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_grid_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_image_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_selectionbox_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/canvas_widgets_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/comic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/embedding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/extension_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    48995 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/generator_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/history_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/lora_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/menubar_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/mixins/toolbar_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.363770 airunner-2.0.5/src/airunner/pyqt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/base_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/embedding_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/generate_form_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/lora_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/main_window_new_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/model_merger_model_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/model_merger_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/noise_filter_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/prompt_browser_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/saturation_window_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.367770 airunner-2.0.5/src/airunner/pyqt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/canvas_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/embedding_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/generator_tab_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/grid_preferences_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/header_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/layer_container_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/layer_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/lora_container_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/lora_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/prompt_builder_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/slider_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/tool_menu_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/pyqt/widgets/toolbar_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-10 08:20:25.000000 airunner-2.0.5/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:20:37.359770 airunner-2.0.5/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-10 08:20:37.000000 airunner-2.0.5/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-10 08:20:37.000000 airunner-2.0.5/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:20:37.000000 airunner-2.0.5/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 08:20:37.000000 airunner-2.0.5/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 08:20:37.000000 airunner-2.0.5/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.850991 airunner-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 01:08:44.000000 airunner-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 01:08:54.850991 airunner-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-11 01:08:44.000000 airunner-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:08:54.850991 airunner-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 01:08:44.000000 airunner-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.830991 airunner-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.834991 airunner-2.1.0/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.838991 airunner-2.1.0/src/airunner/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.842991 airunner-2.1.0/src/airunner/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_active_grid_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_grid_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_image_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_selectionbox_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/canvas_widgets_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/comic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/embedding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/extension_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32391 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/generator_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/history_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/lora_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/menubar_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/mixins/toolbar_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.846991 airunner-2.1.0/src/airunner/pyqt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/base_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/generate_form_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/main_window_new_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/model_merger_model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/model_merger_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/noise_filter_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/prompt_browser_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/saturation_window_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.850991 airunner-2.1.0/src/airunner/pyqt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/canvas_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/generator_tab_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/grid_preferences_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/header_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/layer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/lora_container_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/slider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/tool_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/pyqt/widgets/toolbar_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-11 01:08:44.000000 airunner-2.1.0/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:08:54.838991 airunner-2.1.0/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 01:08:54.000000 airunner-2.1.0/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-2.0.5/LICENSE` & `airunner-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/PKG-INFO` & `airunner-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 2.0.5
+Version: 2.1.0
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-2.0.5/README.md` & `airunner-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/setup.py` & `airunner-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="2.0.5",
+    version="2.1.0",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `airunner-2.0.5/src/airunner/balloon.py` & `airunner-2.1.0/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/canvas.py` & `airunner-2.1.0/src/airunner/canvas.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/extensions.py` & `airunner-2.1.0/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/main.py` & `airunner-2.1.0/src/airunner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import pickle
 import sys
+import traceback
 from functools import partial
 import psutil
 import torch
 from PyQt6 import uic, QtCore
 from PyQt6.QtWidgets import QApplication, QFileDialog, QSplashScreen, QMainWindow, QSplitter, QTabWidget
 from PyQt6.QtCore import pyqtSlot, Qt, QThread, pyqtSignal, QObject, QTimer
 from PyQt6.QtGui import QGuiApplication, QPixmap, QShortcut, QKeySequence
@@ -206,20 +207,20 @@
     @pyqtSlot(int, int, str, object, object)
     def tqdm_callback(self, step, total, action, image=None, data=None):
         if step == 0 and total == 0:
             current = 0
         else:
             if self.progress_bar_started and not self.tqdm_callback_triggered:
                 self.tqdm_callback_triggered = True
-                self.tabs[action].progressBar.setRange(0, 100)
+                self.generator_tab_widget.data[action]["progressBar"].setRange(0, 100)
             try:
                 current = (step / total)
             except ZeroDivisionError:
                 current = 0
-        self.tabs[action].progressBar.setValue(int(current * 100))
+        self.generator_tab_widget.set_progress_bar_value(action, int(current * 100))
 
     @property
     def is_windows(self):
         return sys.platform.startswith("win") or sys.platform.startswith("cygwin") or sys.platform.startswith("msys")
 
     @property
     def is_maximized(self):
@@ -359,15 +360,15 @@
         self.set_status_label(f"New version available: {self.latest_version}")
 
     def show_update_popup(self):
         self.update_popup = UpdateWindow(self.settings_manager, app=self)
 
     def reset_settings(self):
         logger.info("Resetting settings...")
-        GeneratorMixin.reset_settings(self)
+        # GeneratorMixin.reset_settings(self)
         self.canvas.reset_settings()
 
     def on_state_changed(self, state):
         if state == Qt.ApplicationState.ApplicationActive:
             self.canvas.pos_x = int(self.x() / 4)
             self.canvas.pos_y = int(self.y() / 2)
             self.canvas.update()
@@ -382,17 +383,17 @@
         self.header_widget.set_stylesheet()
         self.canvas_widget.set_stylesheet()
         self.tool_menu_widget.set_stylesheet()
         self.toolbar_widget.set_stylesheet()
         self.footer_widget.set_stylesheet()
 
     def initialize(self):
+        self.initialize_settings_manager()
         self.instantiate_widgets()
         self.initialize_saved_prompts()
-        self.initialize_settings_manager()
         self.initialize_tqdm()
         self.initialize_handlers()
         self.initialize_window()
         self.initialize_widgets()
         self.initialize_mixins()
         self.header_widget.initialize()
         self.header_widget.set_size_increment_levels()
@@ -751,14 +752,26 @@
         splash.showMessage(f"Loading AI Runner v{get_version()}", QtCore.Qt.AlignmentFlag.AlignBottom | QtCore.Qt.AlignmentFlag.AlignCenter, QtCore.Qt.GlobalColor.white)
         app.processEvents()
         return splash
 
     splash = display_splash_screen(app)
 
     def show_main_application(splash):
-        window = MainWindow()
+        try:
+            window = MainWindow()
+        except Exception as e:
+            # print a stacktrace to see where the original error occurred
+            # we want to see the original error path using the traceback
+            traceback.print_exc()
+
+            print(e)
+            splash.finish(None)
+            sys.exit("""
+                An error occurred while initializing the application. 
+                Please report this issue on GitHub or Discord."
+            """)
         splash.finish(window)
         window.raise_()
 
     QTimer.singleShot(50, partial(show_main_application, splash))
 
     sys.exit(app.exec())
```

### Comparing `airunner-2.0.5/src/airunner/mixins/brushes_mixin.py` & `airunner-2.1.0/src/airunner/mixins/brushes_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/canvas_active_grid_area_mixin.py` & `airunner-2.1.0/src/airunner/mixins/canvas_active_grid_area_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             self.active_grid_area_rect.x() + size,
             self.active_grid_area_rect.y() + size,
             self.settings_manager.settings.working_width.get() - (size * 2),
             self.settings_manager.settings.working_height.get() - (size * 2)
         )
         painter.drawRect(rect)
 
-        # draw a thirder black border in the center of the two rectangles
+        # draw a third black border in the center of the two rectangles
         pen = QPen(
             QColor(0, 0, 0),
             self.settings_manager.settings.line_width.get() + 1
         )
         painter.setPen(pen)
         size = 2
         rect = QRect(
```

### Comparing `airunner-2.0.5/src/airunner/mixins/canvas_brushes_mixin.py` & `airunner-2.1.0/src/airunner/mixins/canvas_brushes_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/canvas_grid_mixin.py` & `airunner-2.1.0/src/airunner/mixins/canvas_grid_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/canvas_image_mixin.py` & `airunner-2.1.0/src/airunner/mixins/canvas_image_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/canvas_selectionbox_mixin.py` & `airunner-2.1.0/src/airunner/mixins/canvas_selectionbox_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/comic_mixin.py` & `airunner-2.1.0/src/airunner/mixins/comic_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/embedding_mixin.py` & `airunner-2.1.0/src/airunner/mixins/embedding_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/extension_mixin.py` & `airunner-2.1.0/src/airunner/mixins/extension_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/history_mixin.py` & `airunner-2.1.0/src/airunner/mixins/history_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/lora_mixin.py` & `airunner-2.1.0/src/airunner/mixins/lora_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/menubar_mixin.py` & `airunner-2.1.0/src/airunner/mixins/menubar_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/mixins/toolbar_mixin.py` & `airunner-2.1.0/src/airunner/mixins/toolbar_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/base_window_ui.py` & `airunner-2.1.0/src/airunner/pyqt/base_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/embedding_ui.py` & `airunner-2.1.0/src/airunner/pyqt/embedding_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/generate_form_ui.py` & `airunner-2.1.0/src/airunner/pyqt/generate_form_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/lora_ui.py` & `airunner-2.1.0/src/airunner/pyqt/lora_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/main_window_new_ui.py` & `airunner-2.1.0/src/airunner/pyqt/main_window_new_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/main_window_ui.py` & `airunner-2.1.0/src/airunner/pyqt/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/model_merger_model_ui.py` & `airunner-2.1.0/src/airunner/pyqt/model_merger_model_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/model_merger_ui.py` & `airunner-2.1.0/src/airunner/pyqt/model_merger_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/noise_filter_ui.py` & `airunner-2.1.0/src/airunner/pyqt/noise_filter_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py` & `airunner-2.1.0/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/prompt_browser_ui.py` & `airunner-2.1.0/src/airunner/pyqt/prompt_browser_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/saturation_window_ui.py` & `airunner-2.1.0/src/airunner/pyqt/saturation_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/canvas_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/canvas_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/embedding_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/embedding_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/generator_tab_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/generator_tab_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/grid_preferences_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/grid_preferences_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/header_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/header_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/layer_container_widget_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/layer_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/layer_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/lora_container_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/lora_container_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/lora_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/lora_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/prompt_builder_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/slider_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/slider_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/tool_menu_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/tool_menu_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/pyqt/widgets/toolbar_ui.py` & `airunner-2.1.0/src/airunner/pyqt/widgets/toolbar_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/runai_client.py` & `airunner-2.1.0/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/themes.py` & `airunner-2.1.0/src/airunner/themes.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner/utils.py` & `airunner-2.1.0/src/airunner/utils.py`

 * *Files identical despite different names*

### Comparing `airunner-2.0.5/src/airunner.egg-info/PKG-INFO` & `airunner-2.1.0/src/airunner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 2.0.5
+Version: 2.1.0
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-2.0.5/src/airunner.egg-info/SOURCES.txt` & `airunner-2.1.0/src/airunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

