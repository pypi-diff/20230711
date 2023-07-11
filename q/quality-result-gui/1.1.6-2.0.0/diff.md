# Comparing `tmp/quality-result-gui-1.1.6.tar.gz` & `tmp/quality-result-gui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quality-result-gui-1.1.6.tar", last modified: Tue May 23 07:22:42 2023, max compression
+gzip compressed data, was "quality-result-gui-2.0.0.tar", last modified: Tue Jul 11 10:47:36 2023, max compression
```

## Comparing `quality-result-gui-1.1.6.tar` & `quality-result-gui-2.0.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.049575 quality-result-gui-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-23 07:22:42.049575 quality-result-gui-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-23 07:22:42.049575 quality-result-gui-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.037576 quality-result-gui-1.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/api/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/quality_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/api/types/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/types/quality_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/layer_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_data_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_error_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29049 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_fatal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_result_gui.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/style/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/style/default_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/style/quality_layer_error_symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_error_tree_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/utils/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/utils/styling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/example_quality_errors/
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/mock_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/metadata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/i18n/fi.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.278218 quality-result-gui-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.282218 quality-result-gui-2.0.0/src/quality_result_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/quality_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/api/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/types/quality_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/layer_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_data_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_error_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_fatal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_result_gui.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/style/default_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/style/quality_layer_error_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_error_tree_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/utils/styling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/example_quality_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/mock_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/metadata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/i18n/fi.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg
```

### Comparing `quality-result-gui-1.1.6/CHANGELOG.md` & `quality-result-gui-2.0.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## [2.0.0] - 2023-07-11
+
+- Refactor!: replace hierachical representation of quality errors with a flat quality error list
+
 ## [1.1.6] - 2023-05-23
 
 - Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
 
 ## [1.1.5] - 2023-03-29
 
 - Fix: Do not zoom to error when geometry is null geometry
@@ -68,7 +72,8 @@
 [1.1.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.0
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
 [1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
+[2.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.0
```

### Comparing `quality-result-gui-1.1.6/LICENSE` & `quality-result-gui-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/PKG-INFO` & `quality-result-gui-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quality-result-gui
-Version: 1.1.6
+Version: 2.0.0
 Summary: QGIS plugin for visualizing quality check results.
 Home-page: https://github.com/nlsfi/quality-result-gui
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/quality-result-gui/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -38,37 +38,37 @@
 
 ```python
 import json
 
 from qgis.utils import iface
 
 from quality_result_gui.api.quality_api_client import QualityResultClient
-from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
+from quality_result_gui.api.types.quality_error import QualityError
 from quality_result_gui_plugin.dev_tools.response_parser import QualityErrorResponse
 from quality_result_gui.quality_error_manager import QualityResultManager
 
 
 class ExampleQualityResultClient(QualityResultClient):
 
-    def get_results(self) -> Optional[List[QualityErrorsByPriority]]:
+    def get_results(self) -> Optional[List[QualityError]]:
         """
         Retrieve latest quality errors from API
 
         Returns:
             None: if no results available
-            List[QualityErrorsByPriority]: if results available
+            List[QualityError]: if results available
 
         Raises:
             QualityResultClientError: if request fails
             QualityResultServerError: if check failed in backend
         """
         full_path_to_json = "some-path/example_quality_errors.json"
         example_response = json.loads(Path(full_path_to_json).read_text())
 
-        return QualityErrorResponse(example_response).errors_by_priority
+        return QualityErrorResponse(example_response).quality_results
 
     def get_crs(self) -> QgsCoordinateReferenceSystem:
         return QgsCoordinateReferenceSystem("EPSG:3067")
 
 
 
 api_client = ExampleQualityResultClient()
@@ -95,14 +95,18 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [2.0.0] - 2023-07-11
+
+- Refactor!: replace hierachical representation of quality errors with a flat quality error list
+
 ## [1.1.6] - 2023-05-23
 
 - Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
 
 ## [1.1.5] - 2023-03-29
 
 - Fix: Do not zoom to error when geometry is null geometry
@@ -167,7 +171,8 @@
 [1.1.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.0
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
 [1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
+[2.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.0
```

### Comparing `quality-result-gui-1.1.6/README.md` & `quality-result-gui-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,37 +18,37 @@
 
 ```python
 import json
 
 from qgis.utils import iface
 
 from quality_result_gui.api.quality_api_client import QualityResultClient
-from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
+from quality_result_gui.api.types.quality_error import QualityError
 from quality_result_gui_plugin.dev_tools.response_parser import QualityErrorResponse
 from quality_result_gui.quality_error_manager import QualityResultManager
 
 
 class ExampleQualityResultClient(QualityResultClient):
 
-    def get_results(self) -> Optional[List[QualityErrorsByPriority]]:
+    def get_results(self) -> Optional[List[QualityError]]:
         """
         Retrieve latest quality errors from API
 
         Returns:
             None: if no results available
-            List[QualityErrorsByPriority]: if results available
+            List[QualityError]: if results available
 
         Raises:
             QualityResultClientError: if request fails
             QualityResultServerError: if check failed in backend
         """
         full_path_to_json = "some-path/example_quality_errors.json"
         example_response = json.loads(Path(full_path_to_json).read_text())
 
-        return QualityErrorResponse(example_response).errors_by_priority
+        return QualityErrorResponse(example_response).quality_results
 
     def get_crs(self) -> QgsCoordinateReferenceSystem:
         return QgsCoordinateReferenceSystem("EPSG:3067")
 
 
 
 api_client = ExampleQualityResultClient()
```

### Comparing `quality-result-gui-1.1.6/setup.cfg` & `quality-result-gui-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with quality-result-gui. If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "1.1.6"
+__version__ = "2.0.0"
 
 
 from enum import Enum, auto
 
 
 class SelectionType(Enum):
     LeftClick = auto()
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/api/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/api/quality_api_client.py` & `quality-result-gui-2.0.0/src/quality_result_gui/api/quality_api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 #  along with quality-result-gui. If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
 from qgis.core import QgsCoordinateReferenceSystem
 
-from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
+from quality_result_gui.api.types.quality_error import QualityError
 
 
 class QualityResultClient(ABC):
     @abstractmethod
-    def get_results(self) -> Optional[List[QualityErrorsByPriority]]:
+    def get_results(self) -> Optional[List[QualityError]]:
         """
         Retrieve latest quality errors from API
 
         Returns:
             None: if no results available
-            List[QualityErrorsByPriority]: if results available
+            List[QualityError]: if results available
 
         Raises:
             QualityResultClientError: if request fails
             QualityResultServerError: if check failed in backend
         """
 
     @abstractmethod
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/api/types/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/api/types/quality_error.py` & `quality-result-gui-2.0.0/src/quality_result_gui/api/types/quality_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with quality-result-gui. If not, see <https://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 from qgis.core import QgsGeometry
 from qgis_plugin_tools.tools.i18n import tr
 
 
 class QualityErrorType(Enum):
     ATTRIBUTE = 1
@@ -65,37 +65,7 @@
     error_description: str
     error_extra_info: str
     geometry: QgsGeometry
     is_user_processed: bool
 
     def __getitem__(self, item: str) -> Any:
         return getattr(self, item)
-
-
-@dataclass
-class QualityErrorsByFeature:
-    feature_type: str
-    feature_id: str
-    errors: List[QualityError]
-
-
-@dataclass
-class QualityErrorsByFeatureType:
-    feature_type: str
-    errors: List[QualityErrorsByFeature]
-
-    def get_all_errors(self) -> List[QualityError]:
-        errors = [errors_by_feature.errors for errors_by_feature in self.errors]
-        return [item for sub_list in errors for item in sub_list]
-
-
-@dataclass
-class QualityErrorsByPriority:
-    priority: QualityErrorPriority
-    errors: List[QualityErrorsByFeatureType]
-
-    def get_all_errors(self) -> List[QualityError]:
-        errors = [
-            errors_by_feature_type.get_all_errors()
-            for errors_by_feature_type in self.errors
-        ]
-        return [item for sub_list in errors for item in sub_list]
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/configuration/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/layer_mapping.py` & `quality-result-gui-2.0.0/src/quality_result_gui/layer_mapping.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_data_fetcher.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_data_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from quality_result_gui.api.quality_api_client import (
     QualityResultClient,
     QualityResultClientError,
     QualityResultServerError,
 )
 
 if TYPE_CHECKING:
-    from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
+    from quality_result_gui.api.types.quality_error import QualityError
 
 BACKGROUND_POLL_INTERVAL = 10 * 1000
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CheckStatus(Enum):
@@ -125,17 +125,15 @@
             self.stop()
 
     @pyqtSlot(CheckStatus)
     def _worker_status_changed(self, status: CheckStatus) -> None:
         self.status_changed.emit(status)
 
     @pyqtSlot(list)
-    def _worker_results_received(
-        self, results: List["QualityErrorsByPriority"]
-    ) -> None:
+    def _worker_results_received(self, results: List["QualityError"]) -> None:
         self.results_received.emit(results)
 
     @pyqtSlot()
     def start(self) -> None:
         self.stop()
         self._thread = QThread(self)
         self._worker = PollingWorker(self._api_client, None, self._poll_interval)
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager_settings.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager_settings.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_error_visualizer.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_error_visualizer.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_filters.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,14 @@
     QualityResultManagerSettings,
 )
 from quality_result_gui.quality_errors_tree_model import QualityErrorTreeItemType
 
 if TYPE_CHECKING:
     from qgis.PyQt.QtWidgets import QWidget
 
-    from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
-
 FEATURE_TYPE_FILTER_MENU_LABEL = tr("Feature type")
 ERROR_TYPE_FILTER_MENU_LABEL = tr("Error type")
 ATTRIBUTE_NAME_FILTER_MENU_LABEL = tr("Attribute Filter")
 
 
 class FilterMenu(QMenu):
     """A QMenu for checkable filter actions with support for select all section and
@@ -242,23 +240,21 @@
             NotImplementedError: Should be implemented by inherited classes
 
         Returns:
             bool: Is the item accepted by the filter
         """
         raise NotImplementedError()
 
-    def update_filter_from_errors(
-        self, quality_errors: List["QualityErrorsByPriority"]
-    ) -> None:
+    def update_filter_from_errors(self, quality_errors: List["QualityError"]) -> None:
         """Updates filters dynamically from a given list of quality errors.
 
         Should be implemented in inherited classes if feature is wanted.
 
         Args:
-            quality_errors (List[&quot;QualityErrorsByPriority&quot;]): List of errors
+            quality_errors (List[&quot;QualityError&quot;]): List of errors
               to use to update filters
 
         Raises:
             NotImplementedError: Should be implemented in inherited classes
         """
         raise NotImplementedError()
 
@@ -373,26 +369,23 @@
 
     def accept_row(self, item_type: QualityErrorTreeItemType, item_value: Any) -> bool:
         if item_type == QualityErrorTreeItemType.FEATURE_TYPE:
             return cast(str, item_value) in self._accepted_values
 
         return True
 
-    def update_filter_from_errors(
-        self, quality_errors: List["QualityErrorsByPriority"]
-    ) -> None:
+    def update_filter_from_errors(self, quality_errors: List["QualityError"]) -> None:
         """
 
         Args:
-            quality_errors (List[&quot;QualityErrorsByPriority&quot;]): _description_
+            quality_errors (List[&quot;QualityError&quot;]): _description_
         """
         feature_types_in_errors = {  # Dict[filter_value, filter_label]
-            errors.feature_type: self._get_label_value(errors.feature_type)
-            for errors_by_feature_type in quality_errors
-            for errors in errors_by_feature_type.errors
+            error.feature_type: self._get_label_value(error.feature_type)
+            for error in quality_errors
         }
 
         self._refresh_filters(feature_types_in_errors)
 
     def _get_label_value(self, feature_type: str) -> str:
         return QualityResultManagerSettings.get().layer_mapping.get_layer_alias(
             feature_type
@@ -418,25 +411,20 @@
         if item_type == QualityErrorTreeItemType.ERROR:
             attribute_name = cast(QualityError, item_value).attribute_name
             if attribute_name:
                 return attribute_name in self._accepted_values
 
         return True
 
-    def update_filter_from_errors(
-        self, quality_errors: List["QualityErrorsByPriority"]
-    ) -> None:
+    def update_filter_from_errors(self, quality_errors: List["QualityError"]) -> None:
         attribute_names_in_errors = {  # Dict[filter_value, filter_label]
             error.attribute_name: self._get_label_value(
                 error.feature_type, error.attribute_name
             )
-            for errors_by_priority in quality_errors
-            for errors_by_feature_type in errors_by_priority.errors
-            for errors_by_feature in errors_by_feature_type.errors
-            for error in errors_by_feature.errors
+            for error in quality_errors
             if error.attribute_name
         }
 
         self._refresh_filters(attribute_names_in_errors)
 
     def _get_label_value(self, feature_type: str, attribute_name: str) -> str:
         return QualityResultManagerSettings.get().layer_mapping.get_field_alias(
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_tree_model.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_tree_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 from qgis_plugin_tools.tools.i18n import tr
 
 from quality_result_gui.api.types.quality_error import (
     ERROR_PRIORITY_LABEL,
     ERROR_TYPE_LABEL,
     QualityError,
     QualityErrorPriority,
-    QualityErrorsByPriority,
 )
 from quality_result_gui.quality_error_manager_settings import (
     QualityResultManagerSettings,
 )
 
 if TYPE_CHECKING:
     from qgis.core import QgsRectangle
@@ -81,32 +80,23 @@
 COLUMN_HEADERS = {
     ModelColumn.TYPE_OR_ID: tr("Errors"),
     ModelColumn.ERROR_DESCRIPTION: tr("Error description"),
 }
 
 
 def get_error_feature_types(
-    errors_by_priority: List[QualityErrorsByPriority],
+    quality_results: List[QualityError],
 ) -> Set[str]:
-    return {
-        errors.feature_type
-        for errors_by_feature_type in errors_by_priority
-        for errors in errors_by_feature_type.errors
-    }
+    return {errors.feature_type for errors in quality_results}
 
 
 def get_error_feature_attributes(
-    quality_errors: List[QualityErrorsByPriority],
+    quality_errors: List[QualityError],
 ) -> Set[str]:
-    return {
-        error.attribute_name
-        for errors_by_priority in quality_errors
-        for error in errors_by_priority.get_all_errors()
-        if error.attribute_name
-    }
+    return {error.attribute_name for error in quality_errors if error.attribute_name}
 
 
 def _get_quality_errors_indexes(
     model: QAbstractItemModel, index: QModelIndex
 ) -> Iterator[QModelIndex]:
     """Get quality all error indexes from index."""
     if not index.isValid():
@@ -299,18 +289,18 @@
 
         self._root_item = QualityErrorTreeItem(
             len(COLUMN_HEADERS) * [None],
             "header",
             QualityErrorTreeItemType.HEADER,
         )
         # Show error priority rows always
-        for priority in list(QualityErrorPriority):
+        for priority in [1, 2, 3]:
             priority_item = QualityErrorTreeItem(
-                [priority, None],
-                str(priority.value),
+                [QualityErrorPriority(priority), None],
+                str(QualityErrorPriority(priority).value),
                 QualityErrorTreeItemType.PRIORITY,
                 self._root_item,
             )
             self._add_item_to_model(priority_item, self._root_item)
 
     def index(self, row: int, column: int, parent: QModelIndex) -> QModelIndex:
         if not self.hasIndex(row, column, parent):
@@ -446,19 +436,17 @@
             column == ModelColumn.TYPE_OR_ID
             and item.item_type == QualityErrorTreeItemType.ERROR
         ):
             return super().flags(index) | Qt.ItemIsUserCheckable
 
         return super().flags(index)
 
-    def refresh_model(self, quality_errors: List[QualityErrorsByPriority]) -> None:
+    def refresh_model(self, quality_errors: List[QualityError]) -> None:
         updated_quality_error_ids = {
-            error.unique_identifier
-            for errors_by_priority in quality_errors
-            for error in errors_by_priority.get_all_errors()
+            error.unique_identifier for error in quality_errors
         }
 
         current_quality_error_ids = set()
         for i in range(self.rowCount(QModelIndex())):
             for index in _get_quality_errors_indexes(
                 self, self.index(i, 0, QModelIndex())
             ):
@@ -472,16 +460,15 @@
 
         # Nothing changed
         if not deleted_error_ids and not new_error_ids:
             return
 
         errors_to_be_added = (
             error
-            for errors_by_priority in quality_errors
-            for error in errors_by_priority.get_all_errors()
+            for error in quality_errors
             if error.unique_identifier in new_error_ids
         )
 
         errors_to_be_deleted: List[Tuple[QualityErrorTreeItem, QModelIndex]] = []
 
         for i in range(self.rowCount(QModelIndex())):
             for index in _get_quality_errors_indexes(
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/quality_layer.py` & `quality-result-gui-2.0.0/src/quality_result_gui/quality_layer.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/resources/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_fatal.svg` & `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_fatal.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_info.svg` & `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_info.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_warning.svg` & `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_warning.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_result_gui.svg` & `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_result_gui.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/style/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/style/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/style/default_style.py` & `quality-result-gui-2.0.0/src/quality_result_gui/style/default_style.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/style/quality_layer_error_symbol.py` & `quality-result-gui-2.0.0/src/quality_result_gui/style/quality_layer_error_symbol.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_error_tree_view.py` & `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_error_tree_view.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.py` & `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.ui` & `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.ui`

 * *Files 0% similar despite different names*

#### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.ui` & `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.ui`

```diff
@@ -14,14 +14,21 @@
       <string>Quality errors</string>
     </property>
     <widget class="QWidget" name="quality_errors_dock_contents">
       <layout class="QVBoxLayout" name="verticalLayout">
         <item>
           <layout class="QHBoxLayout" name="tree_filters_layout">
             <item>
+              <widget class="QLabel" name="info_label">
+                <property name="text">
+                  <string>No errors received yet</string>
+                </property>
+              </widget>
+            </item>
+            <item>
               <spacer name="horizontalSpacer">
                 <property name="orientation">
                   <enum>Qt::Horizontal</enum>
                 </property>
                 <property name="sizeHint" stdset="0">
                   <size>
                     <width>40</width>
@@ -42,21 +49,14 @@
                   <enum>Qt::ToolButtonTextBesideIcon</enum>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
         <item>
-          <widget class="QLabel" name="info_label">
-            <property name="text">
-              <string>No errors received yet</string>
-            </property>
-          </widget>
-        </item>
-        <item>
           <layout class="QVBoxLayout" name="error_tree_layout">
             <item>
               <widget class="QualityErrorTreeView" name="error_tree_view"/>
             </item>
           </layout>
         </item>
         <item>
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py` & `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/utils/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/utils/layer_utils.py` & `quality-result-gui-2.0.0/src/quality_result_gui/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui/utils/styling_utils.py` & `quality-result-gui-2.0.0/src/quality_result_gui/utils/styling_utils.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui.egg-info/PKG-INFO` & `quality-result-gui-2.0.0/src/quality_result_gui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quality-result-gui
-Version: 1.1.6
+Version: 2.0.0
 Summary: QGIS plugin for visualizing quality check results.
 Home-page: https://github.com/nlsfi/quality-result-gui
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/quality-result-gui/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -38,37 +38,37 @@
 
 ```python
 import json
 
 from qgis.utils import iface
 
 from quality_result_gui.api.quality_api_client import QualityResultClient
-from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
+from quality_result_gui.api.types.quality_error import QualityError
 from quality_result_gui_plugin.dev_tools.response_parser import QualityErrorResponse
 from quality_result_gui.quality_error_manager import QualityResultManager
 
 
 class ExampleQualityResultClient(QualityResultClient):
 
-    def get_results(self) -> Optional[List[QualityErrorsByPriority]]:
+    def get_results(self) -> Optional[List[QualityError]]:
         """
         Retrieve latest quality errors from API
 
         Returns:
             None: if no results available
-            List[QualityErrorsByPriority]: if results available
+            List[QualityError]: if results available
 
         Raises:
             QualityResultClientError: if request fails
             QualityResultServerError: if check failed in backend
         """
         full_path_to_json = "some-path/example_quality_errors.json"
         example_response = json.loads(Path(full_path_to_json).read_text())
 
-        return QualityErrorResponse(example_response).errors_by_priority
+        return QualityErrorResponse(example_response).quality_results
 
     def get_crs(self) -> QgsCoordinateReferenceSystem:
         return QgsCoordinateReferenceSystem("EPSG:3067")
 
 
 
 api_client = ExampleQualityResultClient()
@@ -95,14 +95,18 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [2.0.0] - 2023-07-11
+
+- Refactor!: replace hierachical representation of quality errors with a flat quality error list
+
 ## [1.1.6] - 2023-05-23
 
 - Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
 
 ## [1.1.5] - 2023-03-29
 
 - Fix: Do not zoom to error when geometry is null geometry
@@ -167,7 +171,8 @@
 [1.1.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.0
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
 [1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
+[2.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.0
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui.egg-info/SOURCES.txt` & `quality-result-gui-2.0.0/src/quality_result_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.019230769230769232%*

 * *Differences: {'12': "{'feature_type': 'road_link', 'feature_id': '7c2f-16df-4a5e-98d8-1c0d00c1196b', "*

 * *       "'error_id': 206, 'unique_identifier': '206', 'error_type': 2, 'attribute_name': None, "*

 * *       "'error_description': 'Self-intersection', 'extra_info': None, 'is_user_processed': False, "*

 * *       "'wkt_geom': 'PointZ (235297.14400000000023283 6712758.16299999970942736 "*

 * *       "-999.99900000000002365)', delete: ['errors']}",*

 * * '4': "{'feature_type': 'chimney_point', 'feature_id': '978d7670-5107-495f-a033-82c22f71 […]*

```diff
@@ -1,237 +1,171 @@
 [
     {
-        "errors": [
-            {
-                "errors": [
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": null,
-                                "error_description": "Invalid geometry",
-                                "error_id": 1,
-                                "error_type": 2,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "1",
-                                "wkt_geom": "PointZ (232503.85464823010261171 6712176.46128087863326073 3.81499999999999995)"
-                            },
-                            {
-                                "attribute_name": "vtj_prt",
-                                "error_description": "Invalid value",
-                                "error_id": 2,
-                                "error_type": 1,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "2",
-                                "wkt_geom": "MULTIPOLYGON Z (((232185.359 6711951.654 3.815,232139.885 6711993.324 3.815,232106.09100000001 6712024.05 3.815,232175.045 6712099.295 3.815,232188.708 6712086.809 3.815,232248.937 6712152.562 3.815,232269.228 6712133.942 3.815,232249.074 6712111.949 3.815,232270.633 6712092.193 3.815,232330.42 6712156.979 3.815,232255.603 6712225.5370000005 3.815,232298.354 6712272.191000001 3.815,232396.85700000002 6712181.931 3.815,232487.172 6712280.254 3.815,232510.547 6712258.783 3.815,232516.28100000002 6712265.027 3.815,232553.96600000001 6712230.411 3.815,232374.337 6712037.023 3.815,232371.835 6712039.321 3.815,232334.242 6711998.129 3.815,232342.173 6711990.891 3.815,232365.93600000002 6712017.396 3.815,232383.372 6712001.345 3.815,232376.35 6711993.716 3.815,232388.434 6711982.59 3.815,232380.883 6711974.249 3.815,232389.347 6711965.5370000005 3.815,232387.198 6711963.193 3.815,232394.642 6711956.371 3.815,232405.324 6711967.964 3.815,232432.628 6711943.028 3.815,232412.771 6711921.284 3.815,232416.9 6711917.512 3.815,232385.806 6711883.277 3.815,232368.77300000002 6711898.745 3.815,232355.869 6711884.6620000005 3.815,232373.956 6711868.089 3.815,232331.753 6711822.138 3.815,232329.44400000002 6711819.624 3.815,232185.359 6711951.654 3.815)))"
-                            },
-                            {
-                                "attribute_name": null,
-                                "error_description": "Overlapping geometry",
-                                "error_id": 3,
-                                "error_type": 3,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "3",
-                                "wkt_geom": "PolygonZ ((232237.78700000001117587 6712152.30400000046938658 3.875, 232247.94500000000698492 6712143.11799999978393316 0, 232253.35300000000279397 6712148.50900000054389238 3.81499999999999995, 232248.9370000000053551 6712152.56199999991804361 3.81499999999999995, 232243.10899999999674037 6712158.15400000009685755 3.875, 232237.78700000001117587 6712152.30400000046938658 3.875))"
-                            }
-                        ],
-                        "feature_id": "aa4a7f24-595a-44c9-9f5b-e5cbb9b459c4"
-                    },
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": "height_absolute",
-                                "error_description": "Invalid value",
-                                "error_id": 4,
-                                "error_type": 1,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "4",
-                                "wkt_geom": "MULTIPOLYGON Z (((233875.045 6712248.234 22.173,233868.598 6712259.0540000005 22.173,233869.63 6712259.669 22.173,233857.364 6712280.163 22.173,233864.051 6712284.2360000005 22.173,233882.763 6712252.832 22.173,233875.045 6712248.234 22.173)))"
-                            }
-                        ],
-                        "feature_id": "f93fd550-7677-4998-b7a6-ca2936494fe6"
-                    },
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": null,
-                                "error_description": "Overlapping geometry",
-                                "error_id": 5,
-                                "error_type": 3,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "5",
-                                "wkt_geom": "PolygonZ ((232237.78700000001117587 6712152.30400000046938658 3.875, 232247.94500000000698492 6712143.11799999978393316 0, 232253.35300000000279397 6712148.50900000054389238 3.81499999999999995, 232248.9370000000053551 6712152.56199999991804361 3.81499999999999995, 232243.10899999999674037 6712158.15400000009685755 3.875, 232237.78700000001117587 6712152.30400000046938658 3.875))"
-                            }
-                        ],
-                        "feature_id": "c0c8b4dc-3e5a-432a-8aa1-6b01a3c8273c"
-                    }
-                ],
-                "feature_type": "building_part_area"
-            },
-            {
-                "errors": [
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": "height_relative",
-                                "error_description": "Invalid value",
-                                "error_id": 6,
-                                "error_type": 1,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "6",
-                                "wkt_geom": "PointZ (232641.0456 6711924.7397 0)"
-                            }
-                        ],
-                        "feature_id": "978d7670-5107-495f-a033-82c22f713c90"
-                    }
-                ],
-                "feature_type": "chimney_point"
-            }
-        ],
-        "priority": 1
-    },
-    {
-        "errors": [
-            {
-                "errors": [
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": "floors_above_ground",
-                                "error_description": "Missing value",
-                                "error_id": 102,
-                                "error_type": 1,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "102",
-                                "wkt_geom": "MULTIPOLYGON Z (((232237.787 6712152.3040000005 3.875,232230.717 6712158.782000001 3.875,232250.563 6712180.600000001 3.875,232257.657 6712174.148 3.875,232237.787 6712152.3040000005 3.875)))"
-                            }
-                        ],
-                        "feature_id": "c0c8b4dc-3e5a-432a-8aa1-6b01a3c8273c"
-                    }
-                ],
-                "feature_type": "building_part_area"
-            },
-            {
-                "errors": [
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": "road_number",
-                                "error_description": "Missing value",
-                                "error_id": 103,
-                                "error_type": 1,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "103",
-                                "wkt_geom": "LINESTRING Z (232795.054 6712623.9120000005 5.69,232801.918 6712616.459 -999.999,232803.173 6712615.144 6.115,232827.047 6712590.955 -999.999,232827.382 6712590.603 7.239,232846.19400000002 6712569.879 -999.999,232847.412 6712568.518 7.975,232877.812 6712536.741 -999.999,232878.603 6712535.957 8.531,232897.011 6712517.614 -999.999,232905.044 6712508.706 -999.999,232906.334 6712507.1790000005 -999.999,232906.846 6712506.564 8.921,232921.481 6712487.557 -999.999,232922.035 6712486.822 9.024,232935.489 6712469.428 -999.999,232936.651 6712467.8 -999.999,232937.43 6712466.681 8.806,232942.84100000001 6712458.277 -999.999,232952.554 6712440.805 -999.999,232952.704 6712440.525 8.112,232963.74 6712419.225000001 -999.999,232964.221 6712418.229 7.355,232970.912 6712403.432 7.014,232993.552 6712345.744 -999.999,232993.76200000002 6712345.19 6.795,233008.103 6712307.692 4.998,233012.19700000001 6712296.4180000005 -999.999,233013.392 6712292.602 -999.999,233014.40600000002 6712288.735 -999.999,233014.89500000002 6712286.536 3.966,233015.92 6712280.627 -999.999,233016.73500000002 6712274.6850000005 -999.999,233016.978 6712272.934 3.532,233018.113 6712265.018 -999.999,233018.32700000002 6712263.031 -999.999,233018.389 6712262.343 3.366,233018.623 6712258.352 -999.999,233018.621 6712248.357 -999.999,233018.614 6712247.501 3.255,233018.508 6712237.507 -999.999,233018.405 6712235.51 -999.999,233018.29200000002 6712233.968 3.161,233017.847 6712229.995 -999.999,233017.19700000001 6712226.05 -999.999,233016.836 6712224.229 3.059,233013.956 6712212.587 -999.999,233013.581 6712211.157000001 2.993,233011.552 6712203.422 -999.999,233010.32200000001 6712199.619 -999.999,233009.616 6712197.748000001 -999.999,233009.26 6712196.87 2.914,233008.453 6712195.041 -999.999,233006.655 6712191.47 -999.999,233000.469 6712181.195 -999.999,233000.055 6712180.515000001 2.776,232992.93600000002 6712168.466 -999.999,232992.08000000002 6712167.116 2.668,232988.68300000002 6712162.174000001 -999.999,232983.797 6712155.8440000005 -999.999,232983.057 6712154.937 2.601,232977.84 6712148.877 -999.999,232973.7 6712144.538 -999.999,232972.268 6712143.144 -999.999,232971.901 6712142.796 2.483,232967.429 6712138.801 -999.999,232961.209 6712133.776000001 -999.999,232960.198 6712132.991 2.359,232943.923 6712120.951 2.225,232914.187 6712100.688 -999.999,232913.043 6712099.933 1.966,232877.856 6712077.034 -999.999,232876.878 6712076.408 1.98,232851.764 6712060.023 -999.999,232850.45200000002 6712059.124 2.179,232834.142 6712047.563 -999.999,232832.582 6712046.463 2.301,232796.081 6712021.927 -999.999,232795.633 6712021.626 2.245,232761.073 6711997.79 -999.999,232759.486 6711996.697 1.941,232734.592 6711979.978 -999.999,232734.05800000002 6711979.6280000005 1.764,232695.309 6711954.466 1.706,232644.005 6711919.701 -999.999,232642.77000000002 6711918.901000001 2.455,232621 6711904.71 -999.999,232619.365 6711903.557 -999.999,232618.23200000002 6711902.744 2.799,232608.729 6711895.428 -999.999,232604.13700000002 6711891.571 -999.999,232603.158 6711890.721 2.983,232597.272 6711885.3100000005 -999.999,232595.866 6711883.889 -999.999,232594.549 6711882.491 3.088,232591.92500000002 6711879.475000001 -999.999,232589.461 6711876.325 -999.999,232586.03900000002 6711871.401000001 -999.999,232583.91 6711868.017 -999.999,232583.426 6711867.213 3.258,232580.494 6711861.982 -999.999,232578.706 6711858.405 -999.999,232577.089 6711854.75 -999.999,232576.363 6711852.886 -999.999,232575.69700000001 6711851.002 -999.999,232575.09100000001 6711849.097 -999.999,232574.76200000002 6711847.957 3.278,232573.807 6711844.075 -999.999,232572.677 6711838.1850000005 -999.999,232572.58000000002 6711837.646 3.162)"
-                            },
-                            {
-                                "attribute_name": null,
-                                "error_description": "Self-intersection",
-                                "error_id": 104,
-                                "error_type": 2,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "104",
-                                "wkt_geom": "PointZ (232621.0456 6711904.7397 0)"
-                            }
-                        ],
-                        "feature_id": "43ad7fd2-6996-4c07-89c0-9ffd138fbcb6"
-                    },
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": null,
-                                "error_description": "Self-intersection",
-                                "error_id": 105,
-                                "error_type": 2,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "105",
-                                "wkt_geom": "LineStringZ (234877.73099999999976717 6711974.97400000039488077 0, 234826.9280000000144355 6711932.34700000006705523 0, 234850.86999999999534339 6711893.223000000230968 0, 234866.05199999999604188 6711934.09900000039488077 0, 234832.1840000000083819 6711950.44900000002235174 0)"
-                            },
-                            {
-                                "attribute_name": "road_link_road_class_id",
-                                "error_description": "Attribute value does match value of connecting feature",
-                                "error_id": 106,
-                                "error_type": 4,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "106",
-                                "wkt_geom": "LineStringZ (234877.73099999999976717 6711974.97400000039488077 0, 234826.9280000000144355 6711932.34700000006705523 0, 234850.86999999999534339 6711893.223000000230968 0, 234866.05199999999604188 6711934.09900000039488077 0, 234832.1840000000083819 6711950.44900000002235174 0)"
-                            }
-                        ],
-                        "feature_id": "54cf75b7-d203-4555-8849-506ff159a9e1"
-                    }
-                ],
-                "feature_type": "road_link"
-            }
-        ],
-        "priority": 2
-    },
-    {
-        "errors": [
-            {
-                "errors": [
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": "floors_above_ground",
-                                "error_description": "Missing value",
-                                "error_id": 202,
-                                "error_type": 1,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "202",
-                                "wkt_geom": "MULTIPOLYGON Z (((234793.35700000002 6711820.886 9.193,234790.483 6711823.535 9.193,234793.31900000002 6711826.612 9.193,234789.935 6711829.731 9.193,234785.9 6711825.353 9.193,234779.316 6711831.422 9.193,234776.56900000002 6711828.443 9.193,234769.875 6711834.613 9.193,234767.19700000001 6711831.708000001 9.193,234760.525 6711837.858 9.193,234757.813 6711834.915 9.193,234751.149 6711841.059 9.193,234748.437 6711838.116 9.193,234741.241 6711844.748000001 9.193,234749.37900000002 6711853.576 9.193,234756.044 6711847.432 9.193,234758.75 6711850.368 9.193,234765.43 6711844.211 9.193,234768.128 6711847.138 9.193,234774.821 6711840.9690000005 9.193,234777.52000000002 6711843.897 9.193,234784.23 6711837.713 9.193,234787.776 6711841.631 9.193,234794.9 6711835.161 9.193,234794.092 6711834.273 9.193,234800.352 6711828.589 9.193,234793.35700000002 6711820.886 9.193)))"
-                            }
-                        ],
-                        "feature_id": "925018e6-7f2b-4657-81ab-634338b66d3c"
-                    }
-                ],
-                "feature_type": "building_part_area"
-            },
-            {
-                "errors": [
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": null,
-                                "error_description": "Self-intersection",
-                                "error_id": 205,
-                                "error_type": 2,
-                                "extra_info": null,
-                                "is_user_processed": true,
-                                "unique_identifier": "205",
-                                "wkt_geom": "PointZ (235297.14400000000023283 6712758.16299999970942736 -999.99900000000002365)"
-                            }
-                        ],
-                        "feature_id": "59af7c2f-16df-4a5e-98d8-1c0d00c1196b"
-                    },
-                    {
-                        "errors": [
-                            {
-                                "attribute_name": null,
-                                "error_description": "Self-intersection",
-                                "error_id": 206,
-                                "error_type": 2,
-                                "extra_info": null,
-                                "is_user_processed": false,
-                                "unique_identifier": "206",
-                                "wkt_geom": "PointZ (235297.14400000000023283 6712758.16299999970942736 -999.99900000000002365)"
-                            }
-                        ],
-                        "feature_id": "7c2f-16df-4a5e-98d8-1c0d00c1196b"
-                    }
-                ],
-                "feature_type": "road_link"
-            }
-        ],
-        "priority": 3
+        "attribute_name": "vtj_prt",
+        "error_description": "Invalid value",
+        "error_id": 2,
+        "error_type": 1,
+        "extra_info": null,
+        "feature_id": "aa4a7f24-595a-44c9-9f5b-e5cbb9b459c4",
+        "feature_type": "building_part_area",
+        "is_user_processed": false,
+        "priority": 1,
+        "unique_identifier": "2",
+        "wkt_geom": "MULTIPOLYGON Z (((232185.359 6711951.654 3.815,232139.885 6711993.324 3.815,232106.09100000001 6712024.05 3.815,232175.045 6712099.295 3.815,232188.708 6712086.809 3.815,232248.937 6712152.562 3.815,232269.228 6712133.942 3.815,232249.074 6712111.949 3.815,232270.633 6712092.193 3.815,232330.42 6712156.979 3.815,232255.603 6712225.5370000005 3.815,232298.354 6712272.191000001 3.815,232396.85700000002 6712181.931 3.815,232487.172 6712280.254 3.815,232510.547 6712258.783 3.815,232516.28100000002 6712265.027 3.815,232553.96600000001 6712230.411 3.815,232374.337 6712037.023 3.815,232371.835 6712039.321 3.815,232334.242 6711998.129 3.815,232342.173 6711990.891 3.815,232365.93600000002 6712017.396 3.815,232383.372 6712001.345 3.815,232376.35 6711993.716 3.815,232388.434 6711982.59 3.815,232380.883 6711974.249 3.815,232389.347 6711965.5370000005 3.815,232387.198 6711963.193 3.815,232394.642 6711956.371 3.815,232405.324 6711967.964 3.815,232432.628 6711943.028 3.815,232412.771 6711921.284 3.815,232416.9 6711917.512 3.815,232385.806 6711883.277 3.815,232368.77300000002 6711898.745 3.815,232355.869 6711884.6620000005 3.815,232373.956 6711868.089 3.815,232331.753 6711822.138 3.815,232329.44400000002 6711819.624 3.815,232185.359 6711951.654 3.815)))"
+    },
+    {
+        "attribute_name": null,
+        "error_description": "Overlapping geometry",
+        "error_id": 3,
+        "error_type": 3,
+        "extra_info": null,
+        "feature_id": "aa4a7f24-595a-44c9-9f5b-e5cbb9b459c4",
+        "feature_type": "building_part_area",
+        "is_user_processed": false,
+        "priority": 1,
+        "unique_identifier": "3",
+        "wkt_geom": "PolygonZ ((232237.78700000001117587 6712152.30400000046938658 3.875, 232247.94500000000698492 6712143.11799999978393316 0, 232253.35300000000279397 6712148.50900000054389238 3.81499999999999995, 232248.9370000000053551 6712152.56199999991804361 3.81499999999999995, 232243.10899999999674037 6712158.15400000009685755 3.875, 232237.78700000001117587 6712152.30400000046938658 3.875))"
+    },
+    {
+        "attribute_name": "height_absolute",
+        "error_description": "Invalid value",
+        "error_id": 4,
+        "error_type": 1,
+        "extra_info": null,
+        "feature_id": "f93fd550-7677-4998-b7a6-ca2936494fe6",
+        "feature_type": "building_part_area",
+        "is_user_processed": false,
+        "priority": 1,
+        "unique_identifier": "4",
+        "wkt_geom": "MULTIPOLYGON Z (((233875.045 6712248.234 22.173,233868.598 6712259.0540000005 22.173,233869.63 6712259.669 22.173,233857.364 6712280.163 22.173,233864.051 6712284.2360000005 22.173,233882.763 6712252.832 22.173,233875.045 6712248.234 22.173)))"
+    },
+    {
+        "attribute_name": null,
+        "error_description": "Overlapping geometry",
+        "error_id": 5,
+        "error_type": 3,
+        "extra_info": null,
+        "feature_id": "c0c8b4dc-3e5a-432a-8aa1-6b01a3c8273c",
+        "feature_type": "building_part_area",
+        "is_user_processed": false,
+        "priority": 1,
+        "unique_identifier": "5",
+        "wkt_geom": "PolygonZ ((232237.78700000001117587 6712152.30400000046938658 3.875, 232247.94500000000698492 6712143.11799999978393316 0, 232253.35300000000279397 6712148.50900000054389238 3.81499999999999995, 232248.9370000000053551 6712152.56199999991804361 3.81499999999999995, 232243.10899999999674037 6712158.15400000009685755 3.875, 232237.78700000001117587 6712152.30400000046938658 3.875))"
+    },
+    {
+        "attribute_name": "height_relative",
+        "error_description": "Invalid value",
+        "error_id": 6,
+        "error_type": 1,
+        "extra_info": null,
+        "feature_id": "978d7670-5107-495f-a033-82c22f713c90",
+        "feature_type": "chimney_point",
+        "is_user_processed": false,
+        "priority": 1,
+        "unique_identifier": "6",
+        "wkt_geom": "PointZ (232641.0456 6711924.7397 0)"
+    },
+    {
+        "attribute_name": "floors_above_ground",
+        "error_description": "Missing value",
+        "error_id": 102,
+        "error_type": 1,
+        "extra_info": null,
+        "feature_id": "c0c8b4dc-3e5a-432a-8aa1-6b01a3c8273c",
+        "feature_type": "building_part_area",
+        "is_user_processed": false,
+        "priority": 2,
+        "unique_identifier": "102",
+        "wkt_geom": "MULTIPOLYGON Z (((232237.787 6712152.3040000005 3.875,232230.717 6712158.782000001 3.875,232250.563 6712180.600000001 3.875,232257.657 6712174.148 3.875,232237.787 6712152.3040000005 3.875)))"
+    },
+    {
+        "attribute_name": "road_number",
+        "error_description": "Missing value",
+        "error_id": 103,
+        "error_type": 1,
+        "extra_info": null,
+        "feature_id": "43ad7fd2-6996-4c07-89c0-9ffd138fbcb6",
+        "feature_type": "road_link",
+        "is_user_processed": false,
+        "priority": 2,
+        "unique_identifier": "103",
+        "wkt_geom": "LINESTRING Z (232795.054 6712623.9120000005 5.69,232801.918 6712616.459 -999.999,232803.173 6712615.144 6.115,232827.047 6712590.955 -999.999,232827.382 6712590.603 7.239,232846.19400000002 6712569.879 -999.999,232847.412 6712568.518 7.975,232877.812 6712536.741 -999.999,232878.603 6712535.957 8.531,232897.011 6712517.614 -999.999,232905.044 6712508.706 -999.999,232906.334 6712507.1790000005 -999.999,232906.846 6712506.564 8.921,232921.481 6712487.557 -999.999,232922.035 6712486.822 9.024,232935.489 6712469.428 -999.999,232936.651 6712467.8 -999.999,232937.43 6712466.681 8.806,232942.84100000001 6712458.277 -999.999,232952.554 6712440.805 -999.999,232952.704 6712440.525 8.112,232963.74 6712419.225000001 -999.999,232964.221 6712418.229 7.355,232970.912 6712403.432 7.014,232993.552 6712345.744 -999.999,232993.76200000002 6712345.19 6.795,233008.103 6712307.692 4.998,233012.19700000001 6712296.4180000005 -999.999,233013.392 6712292.602 -999.999,233014.40600000002 6712288.735 -999.999,233014.89500000002 6712286.536 3.966,233015.92 6712280.627 -999.999,233016.73500000002 6712274.6850000005 -999.999,233016.978 6712272.934 3.532,233018.113 6712265.018 -999.999,233018.32700000002 6712263.031 -999.999,233018.389 6712262.343 3.366,233018.623 6712258.352 -999.999,233018.621 6712248.357 -999.999,233018.614 6712247.501 3.255,233018.508 6712237.507 -999.999,233018.405 6712235.51 -999.999,233018.29200000002 6712233.968 3.161,233017.847 6712229.995 -999.999,233017.19700000001 6712226.05 -999.999,233016.836 6712224.229 3.059,233013.956 6712212.587 -999.999,233013.581 6712211.157000001 2.993,233011.552 6712203.422 -999.999,233010.32200000001 6712199.619 -999.999,233009.616 6712197.748000001 -999.999,233009.26 6712196.87 2.914,233008.453 6712195.041 -999.999,233006.655 6712191.47 -999.999,233000.469 6712181.195 -999.999,233000.055 6712180.515000001 2.776,232992.93600000002 6712168.466 -999.999,232992.08000000002 6712167.116 2.668,232988.68300000002 6712162.174000001 -999.999,232983.797 6712155.8440000005 -999.999,232983.057 6712154.937 2.601,232977.84 6712148.877 -999.999,232973.7 6712144.538 -999.999,232972.268 6712143.144 -999.999,232971.901 6712142.796 2.483,232967.429 6712138.801 -999.999,232961.209 6712133.776000001 -999.999,232960.198 6712132.991 2.359,232943.923 6712120.951 2.225,232914.187 6712100.688 -999.999,232913.043 6712099.933 1.966,232877.856 6712077.034 -999.999,232876.878 6712076.408 1.98,232851.764 6712060.023 -999.999,232850.45200000002 6712059.124 2.179,232834.142 6712047.563 -999.999,232832.582 6712046.463 2.301,232796.081 6712021.927 -999.999,232795.633 6712021.626 2.245,232761.073 6711997.79 -999.999,232759.486 6711996.697 1.941,232734.592 6711979.978 -999.999,232734.05800000002 6711979.6280000005 1.764,232695.309 6711954.466 1.706,232644.005 6711919.701 -999.999,232642.77000000002 6711918.901000001 2.455,232621 6711904.71 -999.999,232619.365 6711903.557 -999.999,232618.23200000002 6711902.744 2.799,232608.729 6711895.428 -999.999,232604.13700000002 6711891.571 -999.999,232603.158 6711890.721 2.983,232597.272 6711885.3100000005 -999.999,232595.866 6711883.889 -999.999,232594.549 6711882.491 3.088,232591.92500000002 6711879.475000001 -999.999,232589.461 6711876.325 -999.999,232586.03900000002 6711871.401000001 -999.999,232583.91 6711868.017 -999.999,232583.426 6711867.213 3.258,232580.494 6711861.982 -999.999,232578.706 6711858.405 -999.999,232577.089 6711854.75 -999.999,232576.363 6711852.886 -999.999,232575.69700000001 6711851.002 -999.999,232575.09100000001 6711849.097 -999.999,232574.76200000002 6711847.957 3.278,232573.807 6711844.075 -999.999,232572.677 6711838.1850000005 -999.999,232572.58000000002 6711837.646 3.162)"
+    },
+    {
+        "attribute_name": null,
+        "error_description": "Self-intersection",
+        "error_id": 104,
+        "error_type": 2,
+        "extra_info": null,
+        "feature_id": "43ad7fd2-6996-4c07-89c0-9ffd138fbcb6",
+        "feature_type": "road_link",
+        "is_user_processed": false,
+        "priority": 2,
+        "unique_identifier": "104",
+        "wkt_geom": "PointZ (232621.0456 6711904.7397 0)"
+    },
+    {
+        "attribute_name": null,
+        "error_description": "Self-intersection",
+        "error_id": 105,
+        "error_type": 2,
+        "extra_info": null,
+        "feature_id": "54cf75b7-d203-4555-8849-506ff159a9e1",
+        "feature_type": "road_link",
+        "is_user_processed": false,
+        "priority": 2,
+        "unique_identifier": "105",
+        "wkt_geom": "LineStringZ (234877.73099999999976717 6711974.97400000039488077 0, 234826.9280000000144355 6711932.34700000006705523 0, 234850.86999999999534339 6711893.223000000230968 0, 234866.05199999999604188 6711934.09900000039488077 0, 234832.1840000000083819 6711950.44900000002235174 0)"
+    },
+    {
+        "attribute_name": "road_link_road_class_id",
+        "error_description": "Attribute value does match value of connecting feature",
+        "error_id": 106,
+        "error_type": 4,
+        "extra_info": null,
+        "feature_id": "54cf75b7-d203-4555-8849-506ff159a9e1",
+        "feature_type": "road_link",
+        "is_user_processed": false,
+        "priority": 2,
+        "unique_identifier": "106",
+        "wkt_geom": "LineStringZ (234877.73099999999976717 6711974.97400000039488077 0, 234826.9280000000144355 6711932.34700000006705523 0, 234850.86999999999534339 6711893.223000000230968 0, 234866.05199999999604188 6711934.09900000039488077 0, 234832.1840000000083819 6711950.44900000002235174 0)"
+    },
+    {
+        "attribute_name": "floors_above_ground",
+        "error_description": "Missing value",
+        "error_id": 202,
+        "error_type": 1,
+        "extra_info": null,
+        "feature_id": "925018e6-7f2b-4657-81ab-634338b66d3c",
+        "feature_type": "building_part_area",
+        "is_user_processed": false,
+        "priority": 3,
+        "unique_identifier": "202",
+        "wkt_geom": "MULTIPOLYGON Z (((234793.35700000002 6711820.886 9.193,234790.483 6711823.535 9.193,234793.31900000002 6711826.612 9.193,234789.935 6711829.731 9.193,234785.9 6711825.353 9.193,234779.316 6711831.422 9.193,234776.56900000002 6711828.443 9.193,234769.875 6711834.613 9.193,234767.19700000001 6711831.708000001 9.193,234760.525 6711837.858 9.193,234757.813 6711834.915 9.193,234751.149 6711841.059 9.193,234748.437 6711838.116 9.193,234741.241 6711844.748000001 9.193,234749.37900000002 6711853.576 9.193,234756.044 6711847.432 9.193,234758.75 6711850.368 9.193,234765.43 6711844.211 9.193,234768.128 6711847.138 9.193,234774.821 6711840.9690000005 9.193,234777.52000000002 6711843.897 9.193,234784.23 6711837.713 9.193,234787.776 6711841.631 9.193,234794.9 6711835.161 9.193,234794.092 6711834.273 9.193,234800.352 6711828.589 9.193,234793.35700000002 6711820.886 9.193)))"
+    },
+    {
+        "attribute_name": null,
+        "error_description": "Self-intersection",
+        "error_id": 205,
+        "error_type": 2,
+        "extra_info": null,
+        "feature_id": "59af7c2f-16df-4a5e-98d8-1c0d00c1196b",
+        "feature_type": "road_link",
+        "is_user_processed": true,
+        "priority": 3,
+        "unique_identifier": "205",
+        "wkt_geom": "PointZ (235297.14400000000023283 6712758.16299999970942736 -999.99900000000002365)"
+    },
+    {
+        "attribute_name": null,
+        "error_description": "Self-intersection",
+        "error_id": 206,
+        "error_type": 2,
+        "extra_info": null,
+        "feature_id": "7c2f-16df-4a5e-98d8-1c0d00c1196b",
+        "feature_type": "road_link",
+        "is_user_processed": false,
+        "priority": 3,
+        "unique_identifier": "206",
+        "wkt_geom": "PointZ (235297.14400000000023283 6712758.16299999970942736 -999.99900000000002365)"
     }
 ]
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/mock_api_client.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/mock_api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,33 +21,33 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
 from qgis.core import QgsCoordinateReferenceSystem
 
 from quality_result_gui.api.quality_api_client import QualityResultClient
-from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
+from quality_result_gui.api.types.quality_error import QualityError
 from quality_result_gui_plugin.dev_tools.response_parser import QualityErrorResponse
 
 
 @dataclass
 class MockQualityResultClient(QualityResultClient):
     json_file_path: Path
 
-    def get_results(self) -> Optional[List[QualityErrorsByPriority]]:
+    def get_results(self) -> Optional[List[QualityError]]:
         """
         Retrieve latest quality errors from API
 
         Returns:
             None: if no results available
-            List[QualityErrorsByPriority]: if results available
+            List[QualityError]: if results available
 
         Raises:
             QualityResultClientError: if request fails
             QualityResultServerError: if check failed in backend
         """
         return QualityErrorResponse(
             json.loads(self.json_file_path.read_text())
-        ).errors_by_priority
+        ).quality_results
 
     def get_crs(self) -> QgsCoordinateReferenceSystem:
         return QgsCoordinateReferenceSystem("EPSG:3067")
```

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/env.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/env.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/metadata.txt` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/metadata.txt`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/plugin.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/__init__.py` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg` & `quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg`

 * *Files identical despite different names*

