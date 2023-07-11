# Comparing `tmp/python-djangogql-1.0.1.tar.gz` & `tmp/python-djangogql-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-djangogql-1.0.1.tar", last modified: Mon Jul 10 00:18:46 2023, max compression
+gzip compressed data, was "python-djangogql-1.1.1.tar", last modified: Tue Jul 11 00:28:56 2023, max compression
```

## Comparing `python-djangogql-1.0.1.tar` & `python-djangogql-1.1.1.tar`

### file list

```diff
@@ -1,61 +1,59 @@
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.0.1/LICENSE
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.0.1/MANIFEST.in
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.0.1/README.md
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.896037 python-djangogql-1.0.1/djangogql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.0.1/djangogql/__init__.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.896037 python-djangogql-1.0.1/djangogql/account/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.0.1/djangogql/account/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.0.1/djangogql/account/mixins.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.0.1/djangogql/auth_backend.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.0.1/djangogql/context.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/core/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.0.1/djangogql/core/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.0.1/djangogql/core/connection.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.0.1/djangogql/core/context.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.0.1/djangogql/core/dataloaders.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-07 18:32:47.000000 python-djangogql-1.0.1/djangogql/core/enums.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-08 20:10:49.000000 python-djangogql-1.0.1/djangogql/core/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-03-17 18:31:22.000000 python-djangogql-1.0.1/djangogql/core/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 15:24:41.000000 python-djangogql-1.0.1/djangogql/core/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17511 2023-07-08 20:10:37.000000 python-djangogql-1.0.1/djangogql/core/mutations.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/core/types/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/core/types/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.0.1/djangogql/core/types/base.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/core/types/common.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.0.1/djangogql/core/types/converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.0.1/djangogql/core/types/filter_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1632 2022-09-20 01:45:56.000000 python-djangogql-1.0.1/djangogql/core/types/model.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.0.1/djangogql/core/types/sort_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/core/types/upload.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     4774 2023-05-12 21:38:04.000000 python-djangogql-1.0.1/djangogql/core/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.0.1/djangogql/core/validators.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/db/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.0.1/djangogql/db/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.0.1/djangogql/db/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.0.1/djangogql/decorators.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.0.1/djangogql/exceptions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.0.1/djangogql/jwt.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.0.1/djangogql/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.0.1/djangogql/permissions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.0.1/djangogql/settings.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.892037 python-djangogql-1.0.1/djangogql/templates/
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/templates/graphql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.0.1/djangogql/templates/graphql/playground.html
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/utils/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5931 2023-07-08 20:50:37.000000 python-djangogql-1.0.1/djangogql/utils/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/utils/files.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.0.1/djangogql/utils/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3643 2023-05-04 18:55:50.000000 python-djangogql-1.0.1/djangogql/utils/sorting.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.0.1/djangogql/views.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.0.1/pyproject.toml
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/python_djangogql.egg-info/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1328 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/SOURCES.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/dependency_links.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.0.1/python_djangogql.egg-info/not-zip-safe
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      144 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/requires.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/top_level.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/setup.cfg
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1540 2023-07-10 00:18:15.000000 python-djangogql-1.0.1/setup.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.1.1/LICENSE
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.1.1/MANIFEST.in
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.1.1/README.md
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.007465 python-djangogql-1.1.1/djangogql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.1.1/djangogql/__init__.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/account/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.1.1/djangogql/account/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.1.1/djangogql/account/mixins.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.1.1/djangogql/auth_backend.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.1.1/djangogql/context.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/core/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.1.1/djangogql/core/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.1.1/djangogql/core/connection.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.1.1/djangogql/core/context.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.1.1/djangogql/core/dataloaders.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.1.1/djangogql/core/enums.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.1.1/djangogql/core/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.1.1/djangogql/core/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.1.1/djangogql/core/mutations.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/core/types/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/core/types/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.1.1/djangogql/core/types/base.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/core/types/common.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.1.1/djangogql/core/types/converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.1.1/djangogql/core/types/filter_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1632 2022-09-20 01:45:56.000000 python-djangogql-1.1.1/djangogql/core/types/model.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.1.1/djangogql/core/types/sort_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/core/types/upload.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.1.1/djangogql/core/validators.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/db/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.1.1/djangogql/db/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.1.1/djangogql/db/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.1.1/djangogql/decorators.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.1.1/djangogql/exceptions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.1.1/djangogql/jwt.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.1.1/djangogql/middleware.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.1.1/djangogql/permissions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.1.1/djangogql/settings.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.007465 python-djangogql-1.1.1/djangogql/templates/
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.011465 python-djangogql-1.1.1/djangogql/templates/graphql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.1.1/djangogql/templates/graphql/playground.html
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/djangogql/utils/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.1.1/djangogql/utils/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.1.1/djangogql/utils/files.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.1.1/djangogql/utils/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.1.1/djangogql/utils/sorting.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.1.1/djangogql/views.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.1.1/pyproject.toml
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/python_djangogql.egg-info/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1275 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.1.1/python_djangogql.egg-info/not-zip-safe
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      144 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/requires.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-11 00:28:55.000000 python-djangogql-1.1.1/python_djangogql.egg-info/top_level.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-11 00:28:56.015465 python-djangogql-1.1.1/setup.cfg
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1540 2023-07-11 00:28:37.000000 python-djangogql-1.1.1/setup.py
```

### Comparing `python-djangogql-1.0.1/LICENSE` & `python-djangogql-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/PKG-INFO` & `python-djangogql-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.0.1
+Version: 1.1.1
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.0.1/djangogql/account/mixins.py` & `python-djangogql-1.1.1/djangogql/account/mixins.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/auth_backend.py` & `python-djangogql-1.1.1/djangogql/auth_backend.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/context.py` & `python-djangogql-1.1.1/djangogql/context.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/connection.py` & `python-djangogql-1.1.1/djangogql/core/connection.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/dataloaders.py` & `python-djangogql-1.1.1/djangogql/core/dataloaders.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/enums.py` & `python-djangogql-1.1.1/djangogql/core/enums.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/fields.py` & `python-djangogql-1.1.1/djangogql/core/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/filters.py` & `python-djangogql-1.1.1/djangogql/core/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/mutations.py` & `python-djangogql-1.1.1/djangogql/core/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from itertools import chain
 from typing import Iterable, Union
 
 import graphene
-from django.core.exceptions import (NON_FIELD_ERRORS, ImproperlyConfigured,
-                                    ValidationError)
+from django.core.exceptions import (
+    NON_FIELD_ERRORS,
+    ImproperlyConfigured,
+    ValidationError,
+)
 from django.db.models.fields.files import FileField
 from graphene import ObjectType
 from graphene.types.mutation import MutationOptions
 from graphql import GraphQLError
 
 from ..exceptions import PermissionDenied
-from ..utils import get_nodes, resolve_global_ids_to_primary_keys
+from ..utils import (
+    from_global_id_or_error,
+    get_error_code_from_error,
+    get_nodes,
+    resolve_global_ids_to_primary_keys,
+    snake_to_camel_case,
+)
 from .types import Error
-from .utils import (from_global_id_or_error, get_error_code_from_error,
-                    snake_to_camel_case)
 
 
 def get_model_name(model):
     model_name = model.__name__
     return model_name[:1].lower() + model_name[1:]
```

### Comparing `python-djangogql-1.0.1/djangogql/core/types/base.py` & `python-djangogql-1.1.1/djangogql/core/types/base.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/types/common.py` & `python-djangogql-1.1.1/djangogql/core/types/common.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/types/converter.py` & `python-djangogql-1.1.1/djangogql/core/types/converter.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/types/filter_input.py` & `python-djangogql-1.1.1/djangogql/core/types/filter_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/types/model.py` & `python-djangogql-1.1.1/djangogql/core/types/model.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/types/sort_input.py` & `python-djangogql-1.1.1/djangogql/core/types/sort_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/types/upload.py` & `python-djangogql-1.1.1/djangogql/core/types/upload.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/core/validators.py` & `python-djangogql-1.1.1/djangogql/core/validators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/decorators.py` & `python-djangogql-1.1.1/djangogql/decorators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/jwt.py` & `python-djangogql-1.1.1/djangogql/jwt.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/middleware.py` & `python-djangogql-1.1.1/djangogql/middleware.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/permissions.py` & `python-djangogql-1.1.1/djangogql/permissions.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/settings.py` & `python-djangogql-1.1.1/djangogql/settings.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/templates/graphql/playground.html` & `python-djangogql-1.1.1/djangogql/templates/graphql/playground.html`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/utils/__init__.py` & `python-djangogql-1.1.1/djangogql/utils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import binascii
 import logging
 import traceback
+from enum import Enum
 from typing import Any, Dict, Union
 from uuid import UUID
 
 import graphene
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db.models import Q
-from graphql.error import GraphQLError
+from graphene import ObjectType
+from graphql import GraphQLError
 from graphql.error import format_error as format_graphql_error
 from jwt import InvalidTokenError
 
-from ..core.utils import from_global_id_or_error
 from ..exceptions import PermissionDenied, ReadOnlyException
 
 ERROR_COULD_NO_RESOLVE_GLOBAL_ID = (
     "Could not resolve to a node with the global id list of '%s'."
 )
 REVERSED_DIRECTION = {
     "-": "",
@@ -30,14 +32,38 @@
     InvalidTokenError,
     PermissionDenied,
     ReadOnlyException,
     ValidationError,
 ]
 
 
+def from_global_id_or_error(
+    id: str, only_type: Union[ObjectType, str, None] = None, field: str = "id"
+):
+    try:
+        _type, _id = graphene.Node.from_global_id(id)
+    except (binascii.Error, UnicodeDecodeError, ValueError):
+        raise GraphQLError(f"Couldn't resolve id: {id}.")
+
+    if only_type and str(_type) != str(only_type):
+        raise GraphQLError(f"Must receive a {only_type} id.")
+    return _type, _id
+
+
+def from_global_id_or_none(
+    global_id,
+    only_type: Union[graphene.ObjectType, str, None] = None,
+    raise_error: bool = False,
+):
+    if not global_id:
+        return None
+
+    return from_global_id_or_error(global_id, only_type, raise_error)[1]
+
+
 def resolve_global_ids_to_primary_keys(
     ids, graphene_type=None, raise_error: bool = False
 ):
     pks = []
     invalid_ids = []
     used_type = graphene_type
 
@@ -179,7 +205,55 @@
         lines = []
 
         if isinstance(exc, BaseException):
             for line in traceback.format_exception(type(exc), exc, exc.__traceback__):
                 lines.extend(line.rstrip().splitlines())
         result["extensions"]["exception"]["stacktrace"] = lines
     return result
+
+
+def snake_to_camel_case(name):
+    if isinstance(name, str):
+        split_name = name.split("_")
+        return split_name[0] + "".join(map(str.capitalize, split_name[1:]))
+    return name
+
+
+DJANGO_VALIDATORS_ERROR_CODES = [
+    "invalid",
+    "invalid_extension",
+    "limit_value",
+    "max_decimal_places",
+    "max_digits",
+    "max_length",
+    "max_value",
+    "max_whole_digits",
+    "min_length",
+    "min_value",
+    "null_characters_not_allowed",
+]
+
+DJANGO_FORM_FIELDS_ERROR_CODES = [
+    "contradiction",
+    "empty",
+    "incomplete",
+    "invalid_choice",
+    "invalid_date",
+    "invalid_image",
+    "invalid_list",
+    "invalid_time",
+    "missing",
+    "overflow",
+]
+
+
+def get_error_code_from_error(error) -> str:
+    code = error.code
+    if code in ["required", "blank", "null"]:
+        return "required"
+    if code in ["unique", "unique_for_date"]:
+        return "unique"
+    if code in DJANGO_VALIDATORS_ERROR_CODES or code in DJANGO_FORM_FIELDS_ERROR_CODES:
+        return "invalid"
+    if isinstance(code, Enum):
+        code = code.value
+    return code
```

### Comparing `python-djangogql-1.0.1/djangogql/utils/files.py` & `python-djangogql-1.1.1/djangogql/utils/files.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/utils/filters.py` & `python-djangogql-1.1.1/djangogql/utils/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/djangogql/utils/sorting.py` & `python-djangogql-1.1.1/djangogql/utils/sorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Tuple
 
 from django.db.models import QuerySet
 from graphql.error import GraphQLError
 
 from ..core.enums import OrderDirection
 from ..core.types import SortInputObjectType
-from ..core.utils import from_global_id_or_error
+from . import from_global_id_or_error
 
 REVERSED_DIRECTION = {
     "-": "",
     "": "-",
 }
```

### Comparing `python-djangogql-1.0.1/djangogql/views.py` & `python-djangogql-1.1.1/djangogql/views.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.1/python_djangogql.egg-info/PKG-INFO` & `python-djangogql-1.1.1/python_djangogql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.0.1
+Version: 1.1.1
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.0.1/python_djangogql.egg-info/SOURCES.txt` & `python-djangogql-1.1.1/python_djangogql.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 djangogql/core/__init__.py
 djangogql/core/connection.py
 djangogql/core/context.py
 djangogql/core/dataloaders.py
 djangogql/core/enums.py
 djangogql/core/fields.py
 djangogql/core/filters.py
-djangogql/core/middleware.py
 djangogql/core/mutations.py
-djangogql/core/utils.py
 djangogql/core/validators.py
 djangogql/core/types/__init__.py
 djangogql/core/types/base.py
 djangogql/core/types/common.py
 djangogql/core/types/converter.py
 djangogql/core/types/filter_input.py
 djangogql/core/types/model.py
```

### Comparing `python-djangogql-1.0.1/setup.py` & `python-djangogql-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="python-djangogql",
-    version="1.0.1",
+    version="1.1.1",
     description="A Django app to build graphql APIs",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/felipevisu/djangogql",
     author="Felipe Faria",
     author_email="felipevisu@gmail.com",
     license="MIT",
```

