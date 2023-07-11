# Comparing `tmp/python-djangogql-1.0.0.tar.gz` & `tmp/python-djangogql-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-djangogql-1.0.0.tar", last modified: Sun Jul  9 23:00:28 2023, max compression
+gzip compressed data, was "python-djangogql-1.0.1.tar", last modified: Mon Jul 10 00:18:46 2023, max compression
```

## Comparing `python-djangogql-1.0.0.tar` & `python-djangogql-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.0.0/LICENSE
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.0.0/MANIFEST.in
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.0.0/README.md
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.107018 python-djangogql-1.0.0/djangogql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.0.0/djangogql/__init__.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.111018 python-djangogql-1.0.0/djangogql/account/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.0.0/djangogql/account/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.0.0/djangogql/account/mixins.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.0.0/djangogql/auth_backend.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1471 2023-07-08 20:10:10.000000 python-djangogql-1.0.0/djangogql/context.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.111018 python-djangogql-1.0.0/djangogql/core/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      180 2023-04-29 23:33:17.000000 python-djangogql-1.0.0/djangogql/core/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15899 2023-07-08 20:11:19.000000 python-djangogql-1.0.0/djangogql/core/connection.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      517 2023-07-08 15:35:13.000000 python-djangogql-1.0.0/djangogql/core/context.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.0.0/djangogql/core/dataloaders.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-07 18:32:47.000000 python-djangogql-1.0.0/djangogql/core/enums.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-08 20:10:49.000000 python-djangogql-1.0.0/djangogql/core/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-03-17 18:31:22.000000 python-djangogql-1.0.0/djangogql/core/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 15:24:41.000000 python-djangogql-1.0.0/djangogql/core/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17511 2023-07-08 20:10:37.000000 python-djangogql-1.0.0/djangogql/core/mutations.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.111018 python-djangogql-1.0.0/djangogql/core/types/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.0.0/djangogql/core/types/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.0.0/djangogql/core/types/base.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.0.0/djangogql/core/types/common.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.0.0/djangogql/core/types/converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.0.0/djangogql/core/types/filter_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1632 2022-09-20 01:45:56.000000 python-djangogql-1.0.0/djangogql/core/types/model.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.0.0/djangogql/core/types/sort_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.0.0/djangogql/core/types/upload.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     4774 2023-05-12 21:38:04.000000 python-djangogql-1.0.0/djangogql/core/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.0.0/djangogql/core/validators.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/djangogql/db/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.0.0/djangogql/db/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.0.0/djangogql/db/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.0.0/djangogql/decorators.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.0.0/djangogql/exceptions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.0.0/djangogql/jwt.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.0.0/djangogql/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.0.0/djangogql/permissions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.0.0/djangogql/settings.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.107018 python-djangogql-1.0.0/djangogql/templates/
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/djangogql/templates/graphql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.0.0/djangogql/templates/graphql/playground.html
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/djangogql/utils/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5931 2023-07-08 20:50:37.000000 python-djangogql-1.0.0/djangogql/utils/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.0.0/djangogql/utils/files.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.0.0/djangogql/utils/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3643 2023-05-04 18:55:50.000000 python-djangogql-1.0.0/djangogql/utils/sorting.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.0.0/djangogql/views.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.0.0/pyproject.toml
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/python_djangogql.egg-info/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-09 23:00:28.000000 python-djangogql-1.0.0/python_djangogql.egg-info/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1328 2023-07-09 23:00:28.000000 python-djangogql-1.0.0/python_djangogql.egg-info/SOURCES.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.0.0/python_djangogql.egg-info/dependency_links.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.0.0/python_djangogql.egg-info/not-zip-safe
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      144 2023-07-09 23:00:28.000000 python-djangogql-1.0.0/python_djangogql.egg-info/requires.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-09 23:00:28.000000 python-djangogql-1.0.0/python_djangogql.egg-info/top_level.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-09 23:00:28.115018 python-djangogql-1.0.0/setup.cfg
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1540 2023-07-09 23:00:23.000000 python-djangogql-1.0.0/setup.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.0.1/LICENSE
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.0.1/MANIFEST.in
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.0.1/README.md
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.896037 python-djangogql-1.0.1/djangogql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.0.1/djangogql/__init__.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.896037 python-djangogql-1.0.1/djangogql/account/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.0.1/djangogql/account/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.0.1/djangogql/account/mixins.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.0.1/djangogql/auth_backend.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.0.1/djangogql/context.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/core/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.0.1/djangogql/core/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.0.1/djangogql/core/connection.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.0.1/djangogql/core/context.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.0.1/djangogql/core/dataloaders.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-07 18:32:47.000000 python-djangogql-1.0.1/djangogql/core/enums.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-08 20:10:49.000000 python-djangogql-1.0.1/djangogql/core/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-03-17 18:31:22.000000 python-djangogql-1.0.1/djangogql/core/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 15:24:41.000000 python-djangogql-1.0.1/djangogql/core/middleware.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17511 2023-07-08 20:10:37.000000 python-djangogql-1.0.1/djangogql/core/mutations.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/core/types/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/core/types/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.0.1/djangogql/core/types/base.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/core/types/common.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2022-09-20 01:45:56.000000 python-djangogql-1.0.1/djangogql/core/types/converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3656 2023-04-29 23:33:17.000000 python-djangogql-1.0.1/djangogql/core/types/filter_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1632 2022-09-20 01:45:56.000000 python-djangogql-1.0.1/djangogql/core/types/model.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.0.1/djangogql/core/types/sort_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/core/types/upload.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     4774 2023-05-12 21:38:04.000000 python-djangogql-1.0.1/djangogql/core/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.0.1/djangogql/core/validators.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/db/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.0.1/djangogql/db/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.0.1/djangogql/db/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.0.1/djangogql/decorators.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.0.1/djangogql/exceptions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.0.1/djangogql/jwt.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.0.1/djangogql/middleware.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.0.1/djangogql/permissions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.0.1/djangogql/settings.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.892037 python-djangogql-1.0.1/djangogql/templates/
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/templates/graphql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.0.1/djangogql/templates/graphql/playground.html
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.900037 python-djangogql-1.0.1/djangogql/utils/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5931 2023-07-08 20:50:37.000000 python-djangogql-1.0.1/djangogql/utils/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.0.1/djangogql/utils/files.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.0.1/djangogql/utils/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3643 2023-05-04 18:55:50.000000 python-djangogql-1.0.1/djangogql/utils/sorting.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.0.1/djangogql/views.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.0.1/pyproject.toml
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/python_djangogql.egg-info/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1352 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1328 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.0.1/python_djangogql.egg-info/not-zip-safe
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      144 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/requires.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-10 00:18:46.000000 python-djangogql-1.0.1/python_djangogql.egg-info/top_level.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-10 00:18:46.904037 python-djangogql-1.0.1/setup.cfg
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1540 2023-07-10 00:18:15.000000 python-djangogql-1.0.1/setup.py
```

### Comparing `python-djangogql-1.0.0/LICENSE` & `python-djangogql-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/PKG-INFO` & `python-djangogql-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.0.0/djangogql/account/mixins.py` & `python-djangogql-1.0.1/djangogql/account/mixins.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/auth_backend.py` & `python-djangogql-1.0.1/djangogql/auth_backend.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/context.py` & `python-djangogql-1.0.1/djangogql/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 from django.contrib.auth import authenticate, get_user_model
 from django.contrib.auth.models import AnonymousUser
 from django.http import HttpRequest
 from django.utils import timezone
 from django.utils.functional import SimpleLazyObject
 
-from .core.context import PortalContext
+from .core.context import Context
 from .jwt import get_token_from_request, jwt_decode_with_exception_handler
 
 User = get_user_model()
 
 
-def get_context_value(request: HttpRequest) -> PortalContext:
-    request = cast(PortalContext, request)
+def get_context_value(request: HttpRequest) -> Context:
+    request = cast(Context, request)
     request.dataloaders = {}
     request.allow_replica = getattr(request, "allow_replica", True)
     request.request_time = timezone.now()
     set_auth_on_context(request)
     set_decoded_auth_token(request)
     return request
 
 
 class RequestWithUser(HttpRequest):
     _cached_user: Optional[User]
 
 
-def set_decoded_auth_token(request: PortalContext):
+def set_decoded_auth_token(request: Context):
     auth_token = get_token_from_request(request)
     if auth_token:
         request.decoded_auth_token = jwt_decode_with_exception_handler(auth_token)
     else:
         request.decoded_auth_token = None
 
 
-def get_user(request: PortalContext) -> Optional[User]:
+def get_user(request: Context) -> Optional[User]:
     if not hasattr(request, "_cached_user"):
         request._cached_user = cast(Optional[User], authenticate(request=request))
     return request._cached_user
 
 
-def set_auth_on_context(request: PortalContext):
+def set_auth_on_context(request: Context):
     def user():
         return get_user(request) or AnonymousUser()
 
     request.user = SimpleLazyObject(user)  # type: ignore
```

### Comparing `python-djangogql-1.0.0/djangogql/core/connection.py` & `python-djangogql-1.0.1/djangogql/core/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         pageinfo_type or graphene.relay.PageInfo,
     )
 
     return slice
 
 
 def _validate_slice_args(
-    info: ResolveInfo,
+    info: "ResolveInfo",
     args: dict,
     max_limit: Optional[int] = None,
 ):
     enforce_first_or_last = _is_first_or_last_required(info)
 
     first = args.get("first")
     last = args.get("last")
```

### Comparing `python-djangogql-1.0.0/djangogql/core/dataloaders.py` & `python-djangogql-1.0.1/djangogql/core/dataloaders.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/enums.py` & `python-djangogql-1.0.1/djangogql/core/enums.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/fields.py` & `python-djangogql-1.0.1/djangogql/core/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/filters.py` & `python-djangogql-1.0.1/djangogql/core/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/mutations.py` & `python-djangogql-1.0.1/djangogql/core/mutations.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/base.py` & `python-djangogql-1.0.1/djangogql/core/types/base.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/common.py` & `python-djangogql-1.0.1/djangogql/core/types/common.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/converter.py` & `python-djangogql-1.0.1/djangogql/core/types/converter.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/filter_input.py` & `python-djangogql-1.0.1/djangogql/core/types/filter_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/model.py` & `python-djangogql-1.0.1/djangogql/core/types/model.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/sort_input.py` & `python-djangogql-1.0.1/djangogql/core/types/sort_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/types/upload.py` & `python-djangogql-1.0.1/djangogql/core/types/upload.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/utils.py` & `python-djangogql-1.0.1/djangogql/core/utils.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/core/validators.py` & `python-djangogql-1.0.1/djangogql/core/validators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/decorators.py` & `python-djangogql-1.0.1/djangogql/decorators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/jwt.py` & `python-djangogql-1.0.1/djangogql/jwt.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/middleware.py` & `python-djangogql-1.0.1/djangogql/middleware.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/permissions.py` & `python-djangogql-1.0.1/djangogql/permissions.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/settings.py` & `python-djangogql-1.0.1/djangogql/settings.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/templates/graphql/playground.html` & `python-djangogql-1.0.1/djangogql/templates/graphql/playground.html`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/utils/__init__.py` & `python-djangogql-1.0.1/djangogql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/utils/files.py` & `python-djangogql-1.0.1/djangogql/utils/files.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/utils/filters.py` & `python-djangogql-1.0.1/djangogql/utils/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/utils/sorting.py` & `python-djangogql-1.0.1/djangogql/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/djangogql/views.py` & `python-djangogql-1.0.1/djangogql/views.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/python_djangogql.egg-info/PKG-INFO` & `python-djangogql-1.0.1/python_djangogql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.0.0/python_djangogql.egg-info/SOURCES.txt` & `python-djangogql-1.0.1/python_djangogql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.0.0/setup.py` & `python-djangogql-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="python-djangogql",
-    version="1.0.0",
+    version="1.0.1",
     description="A Django app to build graphql APIs",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/felipevisu/djangogql",
     author="Felipe Faria",
     author_email="felipevisu@gmail.com",
     license="MIT",
```

