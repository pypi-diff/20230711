# Comparing `tmp/python-djangogql-1.1.1.tar.gz` & `tmp/python-djangogql-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-djangogql-1.1.1.tar", last modified: Tue Jul 11 00:28:56 2023, max compression
+gzip compressed data, was "python-djangogql-1.2.0.tar", last modified: Tue Jul 11 01:10:14 2023, max compression
```

## Comparing `python-djangogql-1.1.1.tar` & `python-djangogql-1.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.1.1/LICENSE
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.1.1/MANIFEST.in
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.1.1/README.md
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.007465 python-djangogql-1.1.1/djangogql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.1.1/djangogql/__init__.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/account/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.1.1/djangogql/account/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.1.1/djangogql/account/mixins.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.1.1/djangogql/auth_backend.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.1.1/djangogql/context.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/core/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.1.1/djangogql/core/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.1.1/djangogql/core/connection.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.1.1/djangogql/core/context.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.1.1/djangogql/core/dataloaders.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.1.1/djangogql/core/enums.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.1.1/djangogql/core/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.1.1/djangogql/core/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.1.1/djangogql/core/mutations.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/core/types/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/core/types/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.1.1/djangogql/core/types/base.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/core/types/common.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.1.1/djangogql/core/types/converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.1.1/djangogql/core/types/filter_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1632 2022-09-20 01:45:56.000000 python-djangogql-1.1.1/djangogql/core/types/model.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.1.1/djangogql/core/types/sort_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/core/types/upload.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.1.1/djangogql/core/validators.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/db/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.1.1/djangogql/db/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.1.1/djangogql/db/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.1.1/djangogql/decorators.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.1.1/djangogql/exceptions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.1.1/djangogql/jwt.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.1.1/djangogql/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.1.1/djangogql/permissions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.1.1/djangogql/settings.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.007465 python-djangogql-1.1.1/djangogql/templates/
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/templates/graphql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.1.1/djangogql/templates/graphql/playground.html
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/djangogql/utils/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.1.1/djangogql/utils/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/utils/files.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.1.1/djangogql/utils/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.1.1/djangogql/utils/sorting.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.1.1/djangogql/views.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.1.1/pyproject.toml
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/python_djangogql.egg-info/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1275 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/SOURCES.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/dependency_links.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.1.1/python_djangogql.egg-info/not-zip-safe
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      144 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/requires.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/top_level.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/setup.cfg
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1540 2023-07-11 00:28:37.000000 python-djangogql-1.1.1/setup.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.2.0/LICENSE
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.2.0/MANIFEST.in
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.2.0/README.md
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.335418 python-djangogql-1.2.0/djangogql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.2.0/djangogql/__init__.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.335418 python-djangogql-1.2.0/djangogql/account/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.2.0/djangogql/account/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.2.0/djangogql/account/mixins.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.2.0/djangogql/auth_backend.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.2.0/djangogql/context.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/core/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.2.0/djangogql/core/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.2.0/djangogql/core/connection.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.2.0/djangogql/core/context.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.2.0/djangogql/core/dataloaders.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.2.0/djangogql/core/enums.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.2.0/djangogql/core/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.2.0/djangogql/core/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.2.0/djangogql/core/mutations.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/core/types/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/core/types/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.2.0/djangogql/core/types/base.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/core/types/common.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.2.0/djangogql/core/types/converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.2.0/djangogql/core/types/filter_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2236 2023-07-11 01:08:37.000000 python-djangogql-1.2.0/djangogql/core/types/model.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.2.0/djangogql/core/types/sort_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/core/types/upload.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.2.0/djangogql/core/validators.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/db/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.2.0/djangogql/db/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.2.0/djangogql/db/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.2.0/djangogql/decorators.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.2.0/djangogql/exceptions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.2.0/djangogql/jwt.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.2.0/djangogql/middleware.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.2.0/djangogql/permissions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.2.0/djangogql/settings.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.335418 python-djangogql-1.2.0/djangogql/templates/
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/templates/graphql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.2.0/djangogql/templates/graphql/playground.html
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/djangogql/utils/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.2.0/djangogql/utils/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.2.0/djangogql/utils/files.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.2.0/djangogql/utils/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.2.0/djangogql/utils/sorting.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.2.0/djangogql/views.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.2.0/pyproject.toml
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/python_djangogql.egg-info/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1275 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.2.0/python_djangogql.egg-info/not-zip-safe
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      171 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/requires.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-11 01:10:14.000000 python-djangogql-1.2.0/python_djangogql.egg-info/top_level.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-11 01:10:14.339418 python-djangogql-1.2.0/setup.cfg
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1582 2023-07-11 01:09:52.000000 python-djangogql-1.2.0/setup.py
```

### Comparing `python-djangogql-1.1.1/LICENSE` & `python-djangogql-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/PKG-INFO` & `python-djangogql-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
@@ -25,7 +25,8 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DjangoGQL
 
 DjangoGQL is an open-source library that provides seamless integration between Django, a high-level Python web framework, and Graphene, a library for building GraphQL APIs. The library allows developers to create GraphQL APIs in Django quickly and efficiently while maintaining a high level of performance.
+
```

### Comparing `python-djangogql-1.1.1/djangogql/account/mixins.py` & `python-djangogql-1.2.0/djangogql/account/mixins.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/auth_backend.py` & `python-djangogql-1.2.0/djangogql/auth_backend.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/context.py` & `python-djangogql-1.2.0/djangogql/context.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/connection.py` & `python-djangogql-1.2.0/djangogql/core/connection.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/dataloaders.py` & `python-djangogql-1.2.0/djangogql/core/dataloaders.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/enums.py` & `python-djangogql-1.2.0/djangogql/core/enums.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/fields.py` & `python-djangogql-1.2.0/djangogql/core/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/filters.py` & `python-djangogql-1.2.0/djangogql/core/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/mutations.py` & `python-djangogql-1.2.0/djangogql/core/mutations.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/types/base.py` & `python-djangogql-1.2.0/djangogql/core/types/base.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/types/common.py` & `python-djangogql-1.2.0/djangogql/core/types/common.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/types/converter.py` & `python-djangogql-1.2.0/djangogql/core/types/converter.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/types/filter_input.py` & `python-djangogql-1.2.0/djangogql/core/types/filter_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/types/model.py` & `python-djangogql-1.2.0/djangogql/core/types/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+import graphene
 from django.db.models import Model, Q
 from graphene.types.objecttype import ObjectType, ObjectTypeOptions
+from graphene.types.utils import yank_fields_from_attrs
+from graphene_django.registry import get_global_registry
+from graphene_django.types import construct_fields
+
+ALL_FIELDS = "__all__"
 
 
 class ModelObjectOptions(ObjectTypeOptions):
     model = None
 
 
 class ModelObjectType(ObjectType):
     @classmethod
     def __init_subclass_with_meta__(
         cls,
         interfaces=(),
         possible_types=(),
         default_resolver=None,
+        fields=None,
+        exclude=None,
+        convert_choices_to_enum=True,
         _meta=None,
         **options,
     ):
         if not _meta:
             _meta = ModelObjectOptions(cls)
 
         if not getattr(_meta, "model", None):
@@ -29,14 +38,24 @@
                     "ModelObjectType was declared with invalid 'model' option value "
                     "in it's Meta. Expected subclass of django.db.models.Model, "
                     f"received '{type(options['model'])}' type."
                 )
 
             _meta.model = options.pop("model")
 
+        registry = get_global_registry()
+        model = _meta.model
+
+        django_fields = yank_fields_from_attrs(
+            construct_fields(model, registry, fields, exclude, convert_choices_to_enum),
+            _as=graphene.Field,
+        )
+
+        _meta.fields = django_fields
+
         super(ModelObjectType, cls).__init_subclass_with_meta__(
             interfaces=interfaces,
             possible_types=possible_types,
             default_resolver=default_resolver,
             _meta=_meta,
             **options,
         )
@@ -50,7 +69,8 @@
             return model.objects.get(lookup)
         except model.DoesNotExist:
             return None
 
     @classmethod
     def get_model(cls):
         return cls._meta.model
+        return cls._meta.model
```

### Comparing `python-djangogql-1.1.1/djangogql/core/types/sort_input.py` & `python-djangogql-1.2.0/djangogql/core/types/sort_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/types/upload.py` & `python-djangogql-1.2.0/djangogql/core/types/upload.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/core/validators.py` & `python-djangogql-1.2.0/djangogql/core/validators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/decorators.py` & `python-djangogql-1.2.0/djangogql/decorators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/jwt.py` & `python-djangogql-1.2.0/djangogql/jwt.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/middleware.py` & `python-djangogql-1.2.0/djangogql/middleware.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/permissions.py` & `python-djangogql-1.2.0/djangogql/permissions.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/settings.py` & `python-djangogql-1.2.0/djangogql/settings.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/templates/graphql/playground.html` & `python-djangogql-1.2.0/djangogql/templates/graphql/playground.html`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/utils/__init__.py` & `python-djangogql-1.2.0/djangogql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/utils/files.py` & `python-djangogql-1.2.0/djangogql/utils/files.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/utils/filters.py` & `python-djangogql-1.2.0/djangogql/utils/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/utils/sorting.py` & `python-djangogql-1.2.0/djangogql/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/djangogql/views.py` & `python-djangogql-1.2.0/djangogql/views.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/python_djangogql.egg-info/PKG-INFO` & `python-djangogql-1.2.0/python_djangogql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
@@ -25,7 +25,8 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DjangoGQL
 
 DjangoGQL is an open-source library that provides seamless integration between Django, a high-level Python web framework, and Graphene, a library for building GraphQL APIs. The library allows developers to create GraphQL APIs in Django quickly and efficiently while maintaining a high level of performance.
+
```

### Comparing `python-djangogql-1.1.1/python_djangogql.egg-info/SOURCES.txt` & `python-djangogql-1.2.0/python_djangogql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.1.1/setup.py` & `python-djangogql-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="python-djangogql",
-    version="1.1.1",
+    version="1.2.0",
     description="A Django app to build graphql APIs",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/felipevisu/djangogql",
     author="Felipe Faria",
     author_email="felipevisu@gmail.com",
     license="MIT",
@@ -28,14 +28,15 @@
     ],
     keywords="api graphql graphene django",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "Django >= 3.2",
         "django-filter >= 23.2",
         "graphene >= 2.1.9, < 3",
+        "graphene-django >= 2.16.0, < 3",
         "graphql-core >= 2.3.2, < 3",
         "graphql-relay >= 2.0.1, < 3",
         "promise >= 2.3",
         "PyJWT >= 2.7.0",
     ],
     extras_require={"dev": ["twine >= 4.0.2"]},
     include_package_data=True,
```

