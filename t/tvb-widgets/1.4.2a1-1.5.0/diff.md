# Comparing `tmp/tvb-widgets-1.4.2a1.tar.gz` & `tmp/tvb-widgets-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-widgets-1.4.2a1.tar", last modified: Thu May 11 21:19:47 2023, max compression
+gzip compressed data, was "tvb-widgets-1.5.0.tar", last modified: Tue Jul 11 10:37:28 2023, max compression
```

## Comparing `tvb-widgets-1.4.2a1.tar` & `tvb-widgets-1.5.0.tar`

### file list

```diff
@@ -1,62 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.467730 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.467730 tvb-widgets-1.4.2a1/tvbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/ini_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/pse_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/toml_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/model_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_phase_plane_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_pse_stage_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_tvb_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    36150 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/phase_plane_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_launcher_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/storage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/ts_widget_help.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/widget_with_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.469625 tvb-widgets-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-11 10:37:28.469625 tvb-widgets-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:37:28.469625 tvb-widgets-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.461625 tvb-widgets-1.5.0/tvb_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-11 10:37:28.000000 tvb-widgets-1.5.0/tvb_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-11 10:37:28.000000 tvb-widgets-1.5.0/tvb_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:37:28.000000 tvb-widgets-1.5.0/tvb_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 10:37:28.000000 tvb-widgets-1.5.0/tvb_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 10:37:28.000000 tvb-widgets-1.5.0/tvb_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.461625 tvb-widgets-1.5.0/tvbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.461625 tvb-widgets-1.5.0/tvbwidgets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.461625 tvb-widgets-1.5.0/tvbwidgets/core/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/hpc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/hpc/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/ini_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.461625 tvb-widgets-1.5.0/tvbwidgets/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.465625 tvb-widgets-1.5.0/tvbwidgets/core/pse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/pse/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/pse/pse_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/pse/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/pse/toml_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.465625 tvb-widgets-1.5.0/tvbwidgets/core/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/simulator/model_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/core/simulator/tvb_integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.465625 tvb-widgets-1.5.0/tvbwidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_phase_plane_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_pse_stage_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/test_tvb_integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.465625 tvb-widgets-1.5.0/tvbwidgets/tests/ts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/ts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/ts/test_data_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/ts/test_mne_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/ts/test_plotly_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/tests/ts/ts_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.465625 tvb-widgets-1.5.0/tvbwidgets/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/phase_plane_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/pse_launcher_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/pse_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/storage_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.469625 tvb-widgets-1.5.0/tvbwidgets/ui/ts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/base_ts_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:28.469625 tvb-widgets-1.5.0/tvbwidgets/ui/ts/data_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/data_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/mne_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/plotly_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/ts/ts_widget_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-11 10:37:20.000000 tvb-widgets-1.5.0/tvbwidgets/ui/widget_with_browser.py
```

### Comparing `tvb-widgets-1.4.2a1/LICENSE` & `tvb-widgets-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/PKG-INFO` & `tvb-widgets-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.4.2a1
+Version: 1.5.0
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.4.2a1/README.md` & `tvb-widgets-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/setup.py` & `tvb-widgets-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvb_widgets.egg-info/PKG-INFO` & `tvb-widgets-1.5.0/tvb_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.4.2a1
+Version: 1.5.0
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.4.2a1/tvb_widgets.egg-info/SOURCES.txt` & `tvb-widgets-1.5.0/tvb_widgets.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -18,33 +18,44 @@
 tvbwidgets/core/hpc/launcher.py
 tvbwidgets/core/logger/__init__.py
 tvbwidgets/core/logger/builder.py
 tvbwidgets/core/logger/logging.conf
 tvbwidgets/core/pse/__init__.py
 tvbwidgets/core/pse/parameters.py
 tvbwidgets/core/pse/pse_data.py
+tvbwidgets/core/pse/storage.py
 tvbwidgets/core/pse/toml_storage.py
 tvbwidgets/core/simulator/__init__.py
 tvbwidgets/core/simulator/model_exporters.py
 tvbwidgets/core/simulator/tvb_integrators.py
 tvbwidgets/tests/__init__.py
 tvbwidgets/tests/constants.py
 tvbwidgets/tests/test_base.py
 tvbwidgets/tests/test_drive_widget.py
 tvbwidgets/tests/test_exporters.py
 tvbwidgets/tests/test_head_widget.py
 tvbwidgets/tests/test_phase_plane_export.py
 tvbwidgets/tests/test_pse_stage_in.py
-tvbwidgets/tests/test_ts_widget.py
 tvbwidgets/tests/test_tvb_integrators.py
-tvbwidgets/tests/ts_generator.py
+tvbwidgets/tests/ts/__init__.py
+tvbwidgets/tests/ts/test_data_wrappers.py
+tvbwidgets/tests/ts/test_mne_widget.py
+tvbwidgets/tests/ts/test_plotly_widget.py
+tvbwidgets/tests/ts/ts_generator.py
 tvbwidgets/ui/__init__.py
 tvbwidgets/ui/base_widget.py
 tvbwidgets/ui/drive_widget.py
 tvbwidgets/ui/head_widget.py
 tvbwidgets/ui/phase_plane_widget.py
 tvbwidgets/ui/pse_launcher_widget.py
 tvbwidgets/ui/pse_widget.py
 tvbwidgets/ui/storage_widget.py
-tvbwidgets/ui/ts_widget.py
-tvbwidgets/ui/ts_widget_help.ini
-tvbwidgets/ui/widget_with_browser.py
+tvbwidgets/ui/widget_with_browser.py
+tvbwidgets/ui/ts/__init__.py
+tvbwidgets/ui/ts/base_ts_widget.py
+tvbwidgets/ui/ts/mne_ts_widget.py
+tvbwidgets/ui/ts/plotly_ts_widget.py
+tvbwidgets/ui/ts/ts_widget_browser.py
+tvbwidgets/ui/ts/data_wrappers/__init__.py
+tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py
+tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py
+tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/__init__.py` & `tvb-widgets-1.5.0/tvbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/api.py` & `tvb-widgets-1.5.0/tvbwidgets/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 #
 # (c) 2022-2023, TVB Widgets Team
 #
 
 from .ui.phase_plane_widget import PhasePlaneWidget
 from .ui.storage_widget import StorageWidget
 from .ui.head_widget import HeadBrowser, HeadWidget, HeadWidgetConfig
-from .ui.ts_widget import TimeSeriesWidget, TimeSeriesBrowser
+from .ui.ts.mne_ts_widget import TimeSeriesWidgetMNE
+from .ui.ts.plotly_ts_widget import TimeSeriesWidgetPlotly
+from .ui.ts.ts_widget_browser import TimeSeriesBrowser
 from .ui.pse_widget import PSEWidget
 from .ui.pse_launcher_widget import PSELauncher
 from tvbwidgets.core.hpc.config import HPCConfig
 from IPython.core.display_functions import display
 from tvb.datatypes.time_series import TimeSeries
 
 
@@ -22,17 +24,15 @@
     :param data: timeseries data as numpy array or TimeSeries object
     :param sample_freq: float
     :param ch_idx: Channels Index from the max 4D of the data. We assume time is on 0
     :param backend: plotting backend ('matplotlib' or 'plotly'), currently only matplotlib is supported (string)
     """
 
     if backend == 'matplotlib':
-        tsw = TimeSeriesWidget()
-        if isinstance(data, TimeSeries):
-            tsw.add_datatype(data)
-        else:
-            tsw.add_data_array(data, sample_freq, ch_idx)
-        display(tsw)
+        tsw = TimeSeriesWidgetMNE()
     elif backend == 'plotly':
-        raise NotImplementedError('Plotly is not currently supported')
+        tsw = TimeSeriesWidgetPlotly()
     else:
         raise ValueError('The chose backend is not supported, please choose between: "matplotlib" and "plotly"')
+
+    tsw.add_data(data=data, sample_freq=sample_freq, ch_idx=ch_idx)
+    display(tsw)
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/auth.py` & `tvb-widgets-1.5.0/tvbwidgets/core/auth.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/exceptions.py` & `tvb-widgets-1.5.0/tvbwidgets/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/config.py` & `tvb-widgets-1.5.0/tvbwidgets/core/hpc/config.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/launcher.py` & `tvb-widgets-1.5.0/tvbwidgets/core/hpc/launcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pyunicore.credentials import AuthenticationFailedException
 from pkg_resources import get_distribution, DistributionNotFound
 from tvbwidgets.core.auth import get_current_token
 from tvbwidgets.core.hpc.config import HPCConfig
 from tvbwidgets.core.logger.builder import get_logger
 from tvbwidgets.core.pse.parameters import PROGRESS_STATUS
 from tvb.simulator.simulator import Simulator
+from tvbwidgets.core.pse.storage import StoreObj
 from tvbwidgets.core.pse.toml_storage import TOMLStorage
 
 LOGGER = get_logger(__name__)
 
 
 class HPCLaunch(object):
     pip_libraries = 'tvb-widgets tvb-data'
@@ -61,33 +62,17 @@
 
     @property
     def _install_dependencies_command(self):
         return f'pip install -U pip && pip install {self.pip_libraries}'
 
     def _serialize_configuration(self, sim):
         # type: (Simulator) -> Path
-        if self.param1 == "connectivity":
-            param1_values = self.get_connectivity_files(self.param1_values)
-            param2_values = self.param2_values
-        elif self.param2 == "connectivity":
-            param1_values = self.param1_values
-            param2_values = self.get_connectivity_files(self.param2_values)
-        else:
-            param1_values = self.param1_values
-            param2_values = self.param2_values
-
-        return TOMLStorage.write_pse_in_file(sim, self.param1, self.param2, param1_values, param2_values,
-                                             self.metrics, self.config.n_threads, self.file_name)
-
-    def get_connectivity_files(self, values):
-        connectivity_files = []
-        for connectivity in values:
-            connectivity_files.append(f"connectivity_{connectivity.tract_lengths.shape[0]}.zip")
-
-        return connectivity_files
+        return TOMLStorage.write_pse_in_file(StoreObj(sim, self.param1, self.param2, self.param1_values,
+                                                      self.param2_values, self.metrics, self.config.n_threads,
+                                                      self.file_name))
 
     def connect_client(self):
         LOGGER.info(f"Connecting to {self.config.site}...")
         token = get_current_token()
         transport = pyunicore.client.Transport(token)
         registry = pyunicore.client.Registry(transport, pyunicore.client._HBP_REGISTRY_URL)
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/ini_parser.py` & `tvb-widgets-1.5.0/tvbwidgets/core/ini_parser.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/logger/builder.py` & `tvb-widgets-1.5.0/tvbwidgets/core/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/logger/logging.conf` & `tvb-widgets-1.5.0/tvbwidgets/core/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/pse/parameters.py` & `tvb-widgets-1.5.0/tvbwidgets/core/pse/parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -386,20 +386,21 @@
     )
     exe = JobLibExec(seq=seq, post=pp, backend=None, checkpoint_dir=None, update_progress=update_progress)
     exe(n_jobs=n_threads)
 
 
 if __name__ == '__main__':
     in_file = sys.argv[1]
-    name_param1, vals_param1, name_param2, vals_param2, \
-        metrics_list, result_file, n_th, sim_obj = TOMLStorage.read_pse_from_file(in_file)
+    stored_obj = TOMLStorage.read_pse_from_file(in_file)
 
-    LOGGER.info(f"We are now starting PSE for '{name_param1}' x '{name_param2}' on {n_th} threads\n"
-                f"Expect the result in '{result_file}' \n"
-                f"Metrics {metrics_list} \n"
-                f"Simulator {sim_obj}")
+    LOGGER.info(f"We are now starting PSE for '{stored_obj.param1}' x '{stored_obj.param2}' on "
+                f"{stored_obj.n_threads} threads\n"
+                f"Expect the result in '{stored_obj.file_name}' \n"
+                f"Metrics {stored_obj.metrics} \n"
+                f"Simulator {stored_obj.sim}")
 
     with open(PROGRESS_STATUS, "w+") as f:
         f.write("0")
 
-    launch_local_param(sim_obj, name_param1, name_param2, vals_param1, vals_param2, metrics_list, result_file,
-                       n_threads=n_th)
+    launch_local_param(stored_obj.sim, stored_obj.param1, stored_obj.param2, stored_obj.param1_values,
+                       stored_obj.param2_values, stored_obj.metrics, stored_obj.file_name,
+                       n_threads=stored_obj.n_threads)
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/pse/pse_data.py` & `tvb-widgets-1.5.0/tvbwidgets/core/pse/pse_data.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/pse/toml_storage.py` & `tvb-widgets-1.5.0/tvbwidgets/core/pse/toml_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import importlib
 import numpy as np
 from pathlib import Path
 from datetime import datetime
 from tvb.basic.neotraits._attr import NArray
 from tvb.datatypes.connectivity import Connectivity
 from tvb.simulator.simulator import Simulator
+from tvbwidgets.core.pse.storage import StoreObj
 
 
 class TOMLStorage:
 
     @staticmethod
     def read_pse_from_file(file_name):
 
@@ -34,15 +35,15 @@
         else:
             param2_values = [Connectivity.from_file(elem) for elem in obj["connectivity"]["param2_values"]]
         metrics = obj["parameters"]["metrics"]
         file_name = obj["parameters"]["file_name"]
         n_threads = obj["parameters"]["n_threads"]
 
         simulator = TOMLStorage._stage_out_simulator(obj["simulator"])
-        return param1, param1_values, param2, param2_values, metrics, file_name, n_threads, simulator
+        return StoreObj(simulator, param1, param2, param1_values, param2_values, metrics, n_threads, file_name)
 
     @staticmethod
     def _stage_out_simulator(simulator_data):
         simulator = Simulator()
 
         model = simulator_data["model_class"]
         models = importlib.import_module("tvb.simulator.models")
@@ -73,39 +74,61 @@
             from_file = simulator_data["connectivity_from_file"]
             simulator.connectivity = Connectivity.from_file(from_file)
         else:
             simulator.connectivity = Connectivity.from_file()
         return simulator
 
     @staticmethod
-    def write_pse_in_file(simulator, param1, param2, param1_values, param2_values, metrics, n_threads, file_name):
+    def write_pse_in_file(store_obj):
         data = {}
+        param1_values, param2_values = TOMLStorage.serialize_params_values(store_obj.param1, store_obj.param2,
+                                                                           store_obj.param1_values,
+                                                                           store_obj.param2_values)
         stage_in_obj = Path(f"pse_{datetime.now().strftime('%Y%m%d_%H%M%S')}.toml")
         if not stage_in_obj.exists():
             stage_in_obj.touch()
 
         with open(stage_in_obj, "w") as f:
-            data["parameters"] = {"param1": param1, "param2": param2, "metrics": metrics,
-                                  "file_name": file_name, "n_threads": n_threads}
+            data["parameters"] = {"param1": store_obj.param1, "param2": store_obj.param2,
+                                  "metrics": store_obj.metrics, "file_name": store_obj.file_name,
+                                  "n_threads": store_obj.n_threads}
 
-            if param1 == "connectivity":
+            if store_obj.param1 == "connectivity":
                 data["parameters"].update({"param2_values": param2_values})
                 data["connectivity"] = {"param1_values": param1_values}
 
-            elif param2 == "connectivity":
+            elif store_obj.param2 == "connectivity":
                 data["parameters"].update({"param1_values": param1_values})
                 data["connectivity"] = {"param2_values": param2_values}
             else:
-                data["parameters"].update({"param1_values": param1_values, "param2_values": param2_values})
+                data["parameters"].update({"param1_values": param1_values,
+                                           "param2_values": param2_values})
 
-            data_sim = TOMLStorage._stage_in_simulator(data, simulator)
+            data_sim = TOMLStorage._stage_in_simulator(data, store_obj.sim)
             toml.dump(data_sim, f)
         return stage_in_obj
 
     @staticmethod
+    def serialize_params_values(param1, param2, param1_values, param2_values):
+        if param1 == "connectivity":
+            return TOMLStorage.get_connectivity_files(param1_values), param2_values
+        elif param2 == "connectivity":
+            return param1_values, TOMLStorage.get_connectivity_files(param2_values)
+        else:
+            return param1_values, param2_values
+
+    @staticmethod
+    def get_connectivity_files(values):
+        connectivity_files = []
+        for connectivity in values:
+            connectivity_files.append(f"connectivity_{connectivity.tract_lengths.shape[0]}.zip")
+
+        return connectivity_files
+
+    @staticmethod
     def _stage_in_simulator(data, simulator):
         # type (dict, Simulator) -> dict
         # TODO add the 'stvar' attribute to stage-in simulator, if needed
         data["simulator"] = {"model_parameters": {}, "attributes": {"state_variable_range": {}}}
 
         simulator.configure()
         data["simulator"]["model_class"] = simulator.model.__class__.__name__
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/model_exporters.py` & `tvb-widgets-1.5.0/tvbwidgets/core/simulator/model_exporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
 class PythonCodeExporter(ABCModelExporter):
     """
     Exporter class to export a model configuration as python code in
     a python file
     """
     file_name = 'model_instances'
-    file_extension = 'json'
+    file_extension = 'py'
     numpy_import = 'import numpy'
     module_name = 'models'
     models_import = f'from tvb.simulator import {module_name}'
     instance_var_name = 'model_instance'
 
     def __init__(self, model_instance, keys, file_name=None):
         # type: (Model, list[str], str) -> None
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/tvb_integrators.py` & `tvb-widgets-1.5.0/tvbwidgets/core/simulator/tvb_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_base.py` & `tvb-widgets-1.5.0/tvbwidgets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_drive_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/tests/test_drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_exporters.py` & `tvb-widgets-1.5.0/tvbwidgets/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_head_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/tests/test_head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_phase_plane_export.py` & `tvb-widgets-1.5.0/tvbwidgets/tests/test_phase_plane_export.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/tests/ts_generator.py` & `tvb-widgets-1.5.0/tvbwidgets/tests/ts/ts_generator.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/base_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/base_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/drive_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/head_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/phase_plane_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/phase_plane_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,17 @@
         self.box_layout = widgets.Layout(border='solid 1px black',
                                          margin='0px 5px 5px 0px',
                                          padding='2px 2px 2px 2px')
 
         # Toggle variable for trajectory
         self.traj_out = None
 
+        # Create message area
+        self.message_area = widgets.HTML(value="", layout=widgets.Layout(margin="0px 0px 0px 22px"))
+
     def plotter(self, **plot_params):
         """
         Main plotter function, (re)drawing the main Phase Plane canvases.
         """
         if self.plot_main_axes is None:
             self.plot_main_axes, self.plot_bellow = self._init_plot()
         else:
@@ -112,19 +115,20 @@
 
         # Set Model Parameters
         for k, v in plot_params.items():
             setattr(self.model, k, np.r_[v])
 
         noise_element_exists = 'noise_slider_' + str(self.model.state_variables[0])
         if noise_element_exists in plot_params:
-            # Update integrator noise based on the noise slider value, for stohastic integrators
+            # Update integrator noise based on the noise slider value, for stochastic integrators
             noise_sliders = []
             for state_variable in self.model.state_variables:
                 noise_sliders.append([[plot_params.pop('noise_slider_' + str(state_variable))]])
-            self.integrator.noise.nsig = np.array(noise_sliders)
+            if hasattr(self.integrator, 'noise'):
+                self.integrator.noise.nsig = np.array(noise_sliders)
 
         # Set State Vector
         sv_mean = np.array([plot_params[key] for key in self.model.state_variables])
         sv_mean = sv_mean.reshape((self.model.nvar, 1, 1))
         default_sv = sv_mean.repeat(self.model.number_of_modes, axis=2)
         no_coupling = np.zeros((self.model.nvar, 1, self.model.number_of_modes))
 
@@ -303,16 +307,16 @@
                                        layout=self.box_layout)
 
         # Widget Group "Model"
         self._add_model_selector()
         self._add_integrator_selector()
         widgets_integrator = self.add_integrator_widgets()
         self.param_widgets = widgets.VBox([self.model_selector] + list(self.param_sliders.values()) +
-                                          [self.reset_param_button, self.integrator_selector] + widgets_integrator,
-                                          layout=self.box_layout)
+                                          [self.reset_param_button, self.integrator_selector, self.message_area] +
+                                          widgets_integrator, layout=self.box_layout)
 
         # Exports
         self.build_export_section()
 
         # Group all Widgets in tabs
         return self._build_top_tabs()
 
@@ -684,27 +688,30 @@
                                                     description='Integrator',
                                                     value=self.integrator.__class__.__name__)
 
         def on_change_callback(change):
             if change['type'] != 'change' or change['name'] != 'value':
                 return
             self.integrator = integrators_dict[change['new']]()
-            self.noise_slider_valinit = self.integrator.noise.nsig[0]
-            self._rebuild_widget()
-
+            if hasattr(self.integrator, 'noise'):
+                self.noise_slider_valinit = self.integrator.noise.nsig[0]
+                self._rebuild_widget()
+            else:
+                self.message_area.value = f"{self.integrator.__class__.__name__} integrator has no noise parameter."
         self.integrator_selector.observe(on_change_callback)
 
     def _rebuild_widget(self):
         # type: () -> None
         """
         rebuilds widget. Used when changing model or integrator
         """
         for wid in self.hbox.children:
             wid.close()
 
+        self.message_area.value = ""
         self.model.configure()
         self.ui = self.create_ui()
         self.clear_traj.value = True
         self.out = widgets.interactive_output(self.plotter, self.params)
         self.hbox.children = (self.ui, self.out)
 
     # -----------------------------------------------------------#
```

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_launcher_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/pse_launcher_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/pse_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/storage_widget.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/storage_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.2a1/tvbwidgets/ui/widget_with_browser.py` & `tvb-widgets-1.5.0/tvbwidgets/ui/widget_with_browser.py`

 * *Files identical despite different names*

