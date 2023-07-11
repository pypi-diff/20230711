# Comparing `tmp/peek-plugin-gis-diagram-3.4.7.tar.gz` & `tmp/peek-plugin-gis-diagram-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-gis-diagram-3.4.7.tar", last modified: Mon Jul  3 08:34:53 2023, max compression
+gzip compressed data, was "peek-plugin-gis-diagram-3.4.8.tar", last modified: Tue Jul 11 02:53:56 2023, max compression
```

## Comparing `peek-plugin-gis-diagram-3.4.7.tar` & `peek-plugin-gis-diagram-3.4.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.531370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/
--rw-r--r--   0 root         (0) root         (0)      680 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.531370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.531370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.531370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1483 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.ts
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.component.html
--rw-r--r--   0 root         (0) root         (0)      221 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.component.ts
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.532370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.532370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      943 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/versions/0b12f40fadba_added_stringint_table.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/versions/450e040742f8_added_setting_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.532370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/gisDiagram.component.ts
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/gisDiagram.component.web.html
--rw-r--r--   0 root         (0) root         (0)     2891 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/gisDiagram.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.532370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/show-diagram/
--rw-r--r--   0 root         (0) root         (0)     4139 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/show-diagram/show-diagram.component.ts
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/show-diagram/show-diagram.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.532370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    23560 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.532370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2126 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/
--rw-r--r--   0 root         (0) root         (0)      360 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/GisDiagramApi.py
--rw-r--r--   0 root         (0) root         (0)     3782 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/admin_backend/StringIntTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     3584 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/tuple_providers/CoordSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     7721 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/StringIntTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      365 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/tuples/AddIntValueActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/tuples/GisDiagramTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/tuples/StringCapToggleActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.533371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/both-doc/
--rw-r--r--   0 root         (0) root         (0)    23560 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/both-doc/icon.png
--rw-r--r--   0 root         (0) root         (0)      366 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/GisDiagramPositionService.ts
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/GisDiagramToolbarService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      547 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      161 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/services/PrivateGisDiagramPositionService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      476 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/tuples/GisDiagramTuple.ts
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/tuples/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/package.json
--rw-r--r--   0 root         (0) root         (0)     2540 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/server/
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/server/GisDiagramApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/tuples/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-03 08:32:07.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:34:53.531370 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3994 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 08:34:53.534371 peek-plugin-gis-diagram-3.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2503 2023-07-03 08:34:53.000000 peek-plugin-gis-diagram-3.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.817890 peek-plugin-gis-diagram-3.4.8/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-11 02:53:56.817890 peek-plugin-gis-diagram-3.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.component.html
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.component.ts
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      943 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/versions/0b12f40fadba_added_stringint_table.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/versions/450e040742f8_added_setting_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/gisDiagram.component.ts
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/gisDiagram.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/gisDiagram.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/show-diagram/
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/show-diagram/show-diagram.component.ts
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/show-diagram/show-diagram.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    23560 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/GisDiagramApi.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/admin_backend/StringIntTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.815890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/tuple_providers/CoordSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     7721 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/StringIntTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/tuples/AddIntValueActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/tuples/GisDiagramTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/tuples/StringCapToggleActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/both-doc/
+-rw-r--r--   0 root         (0) root         (0)    23560 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/both-doc/icon.png
+-rw-r--r--   0 root         (0) root         (0)      366 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/GisDiagramPositionService.ts
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/GisDiagramToolbarService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.816890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/services/PrivateGisDiagramPositionService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.817890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/tuples/GisDiagramTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/tuples/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/package.json
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.817890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/server/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/server/GisDiagramApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.817890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/tuples/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-11 02:51:13.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:56.814890 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 02:53:56.817890 peek-plugin-gis-diagram-3.4.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-07-11 02:53:56.000000 peek-plugin-gis-diagram-3.4.8/setup.py
```

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/__init__.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 
-__version__ = '3.4.7'
+__version__ = '3.4.8'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.component.html` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.module.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/admin-app/gisDiagram.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/script.py.mako` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/versions/0b12f40fadba_added_stringint_table.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/versions/0b12f40fadba_added_stringint_table.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/alembic/versions/450e040742f8_added_setting_table.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/alembic/versions/450e040742f8_added_setting_table.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/gisDiagram.module.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/gisDiagram.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-app/show-diagram/show-diagram.component.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-app/show-diagram/show-diagram.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/both-assets/icon.png` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/ClientEntryHook.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/DeviceTupleDataObservableProxy.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/DeviceTupleDataObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/client/DeviceTupleProcessorActionProxy.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/client/DeviceTupleProcessorActionProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/LogicEntryHook.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/TupleActionProcessor.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/TupleDataObservable.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/admin_backend/StringIntTableHandler.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/admin_backend/StringIntTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/controller/MainController.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/server/tuple_providers/CoordSetTupleProvider.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/server/tuple_providers/CoordSetTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/DeclarativeBase.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/Setting.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/storage/StringIntTuple.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/storage/StringIntTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/_private/tuples/GisDiagramTuple.py` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/_private/tuples/GisDiagramTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/both-doc/icon.png` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/both-doc/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/GisDiagramPositionService.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/GisDiagramPositionService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/GisDiagramToolbarService.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/GisDiagramToolbarService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/PluginNames.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/PluginNames.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/services/PrivateGisDiagramPositionService.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/services/PrivateGisDiagramPositionService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin-module/_private/tuples/SettingPropertyTuple.ts` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin-module/_private/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram/plugin_package.json` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram/plugin_package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285716%*

 * *Differences: {"'plugin'": "{'version': '3.4.8'}"}*

```diff
@@ -61,15 +61,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_gis_diagram",
         "title": "GIS Diagram",
-        "version": "3.4.7",
+        "version": "3.4.8",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "field",
         "office",
```

### Comparing `peek-plugin-gis-diagram-3.4.7/peek_plugin_gis_diagram.egg-info/SOURCES.txt` & `peek-plugin-gis-diagram-3.4.8/peek_plugin_gis_diagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-gis-diagram-3.4.7/setup.py` & `peek-plugin-gis-diagram-3.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_gis_diagram"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.7"
+package_version = "3.4.8"
 description = "Peek Plugin GisDiagram - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

