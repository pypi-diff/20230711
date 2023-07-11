# Comparing `tmp/pgsu-0.2.3.tar.gz` & `tmp/pgsu-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgsu-0.2.3.tar", last modified: Tue Nov 15 15:54:31 2022, max compression
+gzip compressed data, was "pgsu-0.2.4.tar", last modified: Tue Jul 11 04:17:02 2023, max compression
```

## Comparing `pgsu-0.2.3.tar` & `pgsu-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 15:54:31.434657 pgsu-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-11-15 15:54:22.000000 pgsu-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-15 15:54:22.000000 pgsu-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-11-15 15:54:31.434657 pgsu-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-11-15 15:54:22.000000 pgsu-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 15:54:31.430657 pgsu-0.2.3/pgsu/
--rw-r--r--   0 runner    (1001) docker     (121)    14250 2022-11-15 15:54:22.000000 pgsu-0.2.3/pgsu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-11-15 15:54:22.000000 pgsu-0.2.3/pgsu/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 15:54:31.434657 pgsu-0.2.3/pgsu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-11-15 15:54:31.000000 pgsu-0.2.3/pgsu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-11-15 15:54:31.000000 pgsu-0.2.3/pgsu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 15:54:31.000000 pgsu-0.2.3/pgsu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 15:54:31.000000 pgsu-0.2.3/pgsu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-15 15:54:31.000000 pgsu-0.2.3/pgsu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-15 15:54:31.000000 pgsu-0.2.3/pgsu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-15 15:54:22.000000 pgsu-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-15 15:54:31.434657 pgsu-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-15 15:54:22.000000 pgsu-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 04:16:52.000000 pgsu-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 04:16:52.000000 pgsu-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-11 04:17:02.484777 pgsu-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-11 04:16:52.000000 pgsu-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/pgsu/
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-07-11 04:16:52.000000 pgsu-0.2.4/pgsu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 04:16:52.000000 pgsu-0.2.4/pgsu/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/pgsu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 04:16:52.000000 pgsu-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-11 04:17:02.484777 pgsu-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 04:16:52.000000 pgsu-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-11 04:16:52.000000 pgsu-0.2.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-11 04:16:52.000000 pgsu-0.2.4/tests/test_pgtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-11 04:16:52.000000 pgsu-0.2.4/tests/test_sql.py
```

### Comparing `pgsu-0.2.3/LICENSE` & `pgsu-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgsu-0.2.3/PKG-INFO` & `pgsu-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsu
-Version: 0.2.3
+Version: 0.2.4
 Summary: Connect to an existing PostgreSQL cluster as a postgres superuser and execute SQL commands.
 Home-page: https://github.com/aiidateam/pgsu
 Author: AiiDA Team
 Author-email: aiidateam@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pgsu-0.2.3/README.md` & `pgsu-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pgsu-0.2.3/pgsu/__init__.py` & `pgsu-0.2.4/pgsu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 import logging
 import traceback
 import os
 from enum import IntEnum
 import subprocess
 
-import click
-
 # By default, try "sudo" only when 'postgres' user exists
 DEFAULT_POSTGRES_UNIX_USER = 'postgres'
 try:
     import pwd
     pwd.getpwnam(DEFAULT_POSTGRES_UNIX_USER)
     DEFAULT_TRY_SUDO = True
 except (KeyError, ModuleNotFoundError):
@@ -199,14 +197,15 @@
 
 def prompt_for_dsn(dsn):
     """
     Prompt interactively for postgres database connection details.
 
     :return: dictionary with the keys: host, port, database, user, password
     """
+    import click  # pylint: disable=import-outside-toplevel
     click.echo('Please provide PostgreSQL connection info:')
 
     # Note: Using '' as the prompt default is necessary to allow users to leave the field empty.
     #       Using `None` in the dictionary is necessary in order for psycopg2 to interpret the value as not provided.
     dsn_new = {}
     dsn_new['host'] = click.prompt(
         'postgres host', default=dsn.get('host') or '', type=str) or None
```

### Comparing `pgsu-0.2.3/pgsu.egg-info/PKG-INFO` & `pgsu-0.2.4/pgsu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsu
-Version: 0.2.3
+Version: 0.2.4
 Summary: Connect to an existing PostgreSQL cluster as a postgres superuser and execute SQL commands.
 Home-page: https://github.com/aiidateam/pgsu
 Author: AiiDA Team
 Author-email: aiidateam@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pgsu-0.2.3/setup.cfg` & `pgsu-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pgsu
-version = 0.2.3
+version = 0.2.4
 description = Connect to an existing PostgreSQL cluster as a postgres superuser and execute SQL commands.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aiidateam/pgsu
 author = AiiDA Team
 author_email = aiidateam@gmail.com
 license = MIT
```

