# Comparing `tmp/python-djangogql-1.2.0.tar.gz` & `tmp/python-djangogql-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-djangogql-1.2.0.tar", last modified: Tue Jul 11 01:10:14 2023, max compression
+gzip compressed data, was "python-djangogql-1.3.0.tar", last modified: Tue Jul 11 18:09:52 2023, max compression
```

## Comparing `python-djangogql-1.2.0.tar` & `python-djangogql-1.3.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.2.0/LICENSE
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.2.0/MANIFEST.in
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.2.0/README.md
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.335418 python-djangogql-1.2.0/djangogql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.2.0/djangogql/__init__.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.335418 python-djangogql-1.2.0/djangogql/account/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.2.0/djangogql/account/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.2.0/djangogql/account/mixins.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.2.0/djangogql/auth_backend.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.2.0/djangogql/context.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/core/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.2.0/djangogql/core/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.2.0/djangogql/core/connection.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.2.0/djangogql/core/context.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.2.0/djangogql/core/dataloaders.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.2.0/djangogql/core/enums.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.2.0/djangogql/core/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.2.0/djangogql/core/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.2.0/djangogql/core/mutations.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/core/types/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/core/types/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.2.0/djangogql/core/types/base.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/core/types/common.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.2.0/djangogql/core/types/converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.2.0/djangogql/core/types/filter_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2236 2023-07-11 01:08:37.000000 python-djangogql-1.2.0/djangogql/core/types/model.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.2.0/djangogql/core/types/sort_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/core/types/upload.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.2.0/djangogql/core/validators.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/db/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.2.0/djangogql/db/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.2.0/djangogql/db/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.2.0/djangogql/decorators.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.2.0/djangogql/exceptions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.2.0/djangogql/jwt.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.2.0/djangogql/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.2.0/djangogql/permissions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.2.0/djangogql/settings.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.335418 python-djangogql-1.2.0/djangogql/templates/
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/templates/graphql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.2.0/djangogql/templates/graphql/playground.html
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/utils/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.2.0/djangogql/utils/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/utils/files.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.2.0/djangogql/utils/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.2.0/djangogql/utils/sorting.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.2.0/djangogql/views.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.2.0/pyproject.toml
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/python_djangogql.egg-info/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1275 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/SOURCES.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/dependency_links.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.2.0/python_djangogql.egg-info/not-zip-safe
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      171 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/requires.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/top_level.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/setup.cfg
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1582 2023-07-11 01:09:52.000000 python-djangogql-1.2.0/setup.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.3.0/LICENSE
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.3.0/MANIFEST.in
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.3.0/README.md
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.029632 python-djangogql-1.3.0/djangogql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.3.0/djangogql/__init__.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.029632 python-djangogql-1.3.0/djangogql/account/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.3.0/djangogql/account/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.3.0/djangogql/account/mixins.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.3.0/djangogql/auth_backend.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.3.0/djangogql/context.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/core/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.3.0/djangogql/core/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.3.0/djangogql/core/connection.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.3.0/djangogql/core/context.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.3.0/djangogql/core/dataloaders.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.3.0/djangogql/core/enums.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.3.0/djangogql/core/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.3.0/djangogql/core/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.3.0/djangogql/core/mutations.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/core/types/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/core/types/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.3.0/djangogql/core/types/base.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/core/types/common.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/filter_converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3663 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/filter_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3857 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/model.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7466 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/model_converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1193 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/registry.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.3.0/djangogql/core/types/sort_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/core/types/upload.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.3.0/djangogql/core/validators.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/db/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.3.0/djangogql/db/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.3.0/djangogql/db/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.3.0/djangogql/decorators.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.3.0/djangogql/exceptions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.3.0/djangogql/jwt.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.3.0/djangogql/middleware.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.3.0/djangogql/permissions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.3.0/djangogql/settings.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.029632 python-djangogql-1.3.0/djangogql/templates/
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/templates/graphql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.3.0/djangogql/templates/graphql/playground.html
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/utils/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.3.0/djangogql/utils/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1227 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/utils/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/utils/files.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.3.0/djangogql/utils/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.3.0/djangogql/utils/sorting.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.3.0/djangogql/views.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.3.0/pyproject.toml
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/python_djangogql.egg-info/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1381 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.3.0/python_djangogql.egg-info/not-zip-safe
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      164 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/requires.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/top_level.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/setup.cfg
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1573 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/setup.py
```

### Comparing `python-djangogql-1.2.0/LICENSE` & `python-djangogql-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/PKG-INFO` & `python-djangogql-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.2.0/djangogql/account/mixins.py` & `python-djangogql-1.3.0/djangogql/account/mixins.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/auth_backend.py` & `python-djangogql-1.3.0/djangogql/auth_backend.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/context.py` & `python-djangogql-1.3.0/djangogql/context.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/connection.py` & `python-djangogql-1.3.0/djangogql/core/connection.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/dataloaders.py` & `python-djangogql-1.3.0/djangogql/core/dataloaders.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/enums.py` & `python-djangogql-1.3.0/djangogql/core/enums.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/fields.py` & `python-djangogql-1.3.0/djangogql/core/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/filters.py` & `python-djangogql-1.3.0/djangogql/core/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/mutations.py` & `python-djangogql-1.3.0/djangogql/core/mutations.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/types/base.py` & `python-djangogql-1.3.0/djangogql/core/types/base.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/types/common.py` & `python-djangogql-1.3.0/djangogql/core/types/common.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/types/converter.py` & `python-djangogql-1.3.0/djangogql/core/types/filter_converter.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/types/filter_input.py` & `python-djangogql-1.3.0/djangogql/core/types/filter_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django_filters.filterset import FILTER_FOR_DBFIELD_DEFAULTS, BaseFilterSet
 from graphene import Argument, InputField, InputObjectType, String
 from graphene.types.inputobjecttype import InputObjectTypeOptions
 from graphene.types.utils import yank_fields_from_attrs
 
 from ..filters import GlobalIDFilter, GlobalIDMultipleChoiceFilter
 from .common import NonNullList
-from .converter import convert_form_field
+from .filter_converter import convert_form_field
 
 GLOBAL_ID_FILTERS = {
     models.AutoField: {"filter_class": GlobalIDFilter},
     models.OneToOneField: {"filter_class": GlobalIDFilter},
     models.ForeignKey: {"filter_class": GlobalIDFilter},
     models.ManyToManyField: {"filter_class": GlobalIDMultipleChoiceFilter},
     models.ManyToOneRel: {"filter_class": GlobalIDMultipleChoiceFilter},
```

### Comparing `python-djangogql-1.2.0/djangogql/core/types/sort_input.py` & `python-djangogql-1.3.0/djangogql/core/types/sort_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/types/upload.py` & `python-djangogql-1.3.0/djangogql/core/types/upload.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/core/validators.py` & `python-djangogql-1.3.0/djangogql/core/validators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/decorators.py` & `python-djangogql-1.3.0/djangogql/decorators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/jwt.py` & `python-djangogql-1.3.0/djangogql/jwt.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/middleware.py` & `python-djangogql-1.3.0/djangogql/middleware.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/permissions.py` & `python-djangogql-1.3.0/djangogql/permissions.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/settings.py` & `python-djangogql-1.3.0/djangogql/settings.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/templates/graphql/playground.html` & `python-djangogql-1.3.0/djangogql/templates/graphql/playground.html`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/utils/__init__.py` & `python-djangogql-1.3.0/djangogql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/utils/files.py` & `python-djangogql-1.3.0/djangogql/utils/files.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/utils/filters.py` & `python-djangogql-1.3.0/djangogql/utils/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/utils/sorting.py` & `python-djangogql-1.3.0/djangogql/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/djangogql/views.py` & `python-djangogql-1.3.0/djangogql/views.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.2.0/python_djangogql.egg-info/PKG-INFO` & `python-djangogql-1.3.0/python_djangogql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.2.0/python_djangogql.egg-info/SOURCES.txt` & `python-djangogql-1.3.0/python_djangogql.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,26 @@
 djangogql/core/fields.py
 djangogql/core/filters.py
 djangogql/core/mutations.py
 djangogql/core/validators.py
 djangogql/core/types/__init__.py
 djangogql/core/types/base.py
 djangogql/core/types/common.py
-djangogql/core/types/converter.py
+djangogql/core/types/filter_converter.py
 djangogql/core/types/filter_input.py
 djangogql/core/types/model.py
+djangogql/core/types/model_converter.py
+djangogql/core/types/registry.py
 djangogql/core/types/sort_input.py
 djangogql/core/types/upload.py
 djangogql/db/__init__.py
 djangogql/db/utils.py
 djangogql/templates/graphql/playground.html
 djangogql/utils/__init__.py
+djangogql/utils/fields.py
 djangogql/utils/files.py
 djangogql/utils/filters.py
 djangogql/utils/sorting.py
 python_djangogql.egg-info/PKG-INFO
 python_djangogql.egg-info/SOURCES.txt
 python_djangogql.egg-info/dependency_links.txt
 python_djangogql.egg-info/not-zip-safe
```

### Comparing `python-djangogql-1.2.0/setup.py` & `python-djangogql-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="python-djangogql",
-    version="1.2.0",
+    version="1.3.0",
     description="A Django app to build graphql APIs",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/felipevisu/djangogql",
     author="Felipe Faria",
     author_email="felipevisu@gmail.com",
     license="MIT",
@@ -28,18 +28,18 @@
     ],
     keywords="api graphql graphene django",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "Django >= 3.2",
         "django-filter >= 23.2",
         "graphene >= 2.1.9, < 3",
-        "graphene-django >= 2.16.0, < 3",
         "graphql-core >= 2.3.2, < 3",
         "graphql-relay >= 2.0.1, < 3",
         "promise >= 2.3",
         "PyJWT >= 2.7.0",
+        "text-unidecode >= 1.3",
     ],
     extras_require={"dev": ["twine >= 4.0.2"]},
     include_package_data=True,
     zip_safe=False,
     platforms="any",
 )
```

