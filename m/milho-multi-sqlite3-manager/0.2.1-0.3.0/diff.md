# Comparing `tmp/milho_multi_sqlite3_manager-0.2.1.tar.gz` & `tmp/milho_multi_sqlite3_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milho_multi_sqlite3_manager-0.2.1.tar", max compression
+gzip compressed data, was "milho_multi_sqlite3_manager-0.3.0.tar", max compression
```

## Comparing `milho_multi_sqlite3_manager-0.2.1.tar` & `milho_multi_sqlite3_manager-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      310 2023-06-27 15:07:00.576002 milho_multi_sqlite3_manager-0.2.1/multisqlite3manager/__init__.py
--rw-r--r--   0        0        0     7228 2023-06-25 16:18:49.573958 milho_multi_sqlite3_manager-0.2.1/multisqlite3manager/db_manager.py
--rw-r--r--   0        0        0        0 2023-06-16 03:42:12.550884 milho_multi_sqlite3_manager-0.2.1/multisqlite3manager/tests/__init__.py
--rw-r--r--   0        0        0     4243 2023-06-25 07:07:37.088310 milho_multi_sqlite3_manager-0.2.1/multisqlite3manager/tests/db_manager_test.py
--rw-r--r--   0        0        0      453 2023-06-27 15:38:11.287908 milho_multi_sqlite3_manager-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1185 2023-06-25 17:47:20.995550 milho_multi_sqlite3_manager-0.2.1/README.md
--rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.2.1/setup.py
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2023-07-01 18:48:26.038198 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/__init__.py
+-rw-r--r--   0        0        0       35 2023-07-11 01:06:13.985060 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/file_manager/__init__.py
+-rw-r--r--   0        0        0     2348 2023-07-11 02:04:32.602447 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/file_manager/file_manager.py
+-rw-r--r--   0        0        0       41 2023-07-11 01:05:11.426535 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/__init__.py
+-rw-r--r--   0        0        0     9847 2023-07-11 01:52:34.227736 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/sqlite3_manager.py
+-rw-r--r--   0        0        0     6479 2023-07-11 02:03:43.934491 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/sqlite3_manager_test.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:42:12.550884 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/tests/__init__.py
+-rw-r--r--   0        0        0      453 2023-07-11 02:12:24.012409 milho_multi_sqlite3_manager-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-06-25 17:47:20.995550 milho_multi_sqlite3_manager-0.3.0/README.md
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.3.0/setup.py
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.3.0/PKG-INFO
```

### Comparing `milho_multi_sqlite3_manager-0.2.1/README.md` & `milho_multi_sqlite3_manager-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `milho_multi_sqlite3_manager-0.2.1/setup.py` & `milho_multi_sqlite3_manager-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['multisqlite3manager', 'multisqlite3manager.tests']
+['multisqlite3manager',
+ 'multisqlite3manager.file_manager',
+ 'multisqlite3manager.sqlite3_manager',
+ 'multisqlite3manager.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas>=2.0.2,<3.0.0', 'sqlalchemy>=2.0.16,<3.0.0', 'sqlglot>=16.3.1,<17.0.0']
 
 setup_kwargs = {
     'name': 'milho-multi-sqlite3-manager',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# milho-multi-sqlite3-manager\n\n## Description\n\nThe idea is to have an environment with multiple SQLITE3 files, aiming at ease of access and use.\nThe inspiration for creating this module came from the ease of working with Spark in BigData environments where, generally, everything is integrated, without the need to make several explicit connections in the code.\n\nIf you want an integrated environment on your machine, create an environment variable called "MULTISQLITE3MANAGER_FOLDER_PATH" with the directory of your folder. You will need to make sure that all files in this folder are SQLITE3 databases.\n\nWhen "to_dataframe" is used, the result is a Pandas DataFrame. The query is previously parsed to map all the databases used in the SQL. Then the module create a sqlalchemy connection and attach that databases to the connection. After that, the query is executed and the result is a Pandas DataFrame. \n\n## Code Samples\n\n```python\n\nfrom multisqlite3manager import print_databases, print_tables, to_dataframe\n\nprint_databases()\nprint_tables("DB_NAME")\n\ndf = to_dataframe("SELECT * FROM db_1.tMisto")\ndf2 = to_dataframe("SELECT * FROM db_2_copy.tMisto")\n\n```\n',
     'author': 'Guilherme S. Magalhães',
     'author_email': '40049979+Guisilcol@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `milho_multi_sqlite3_manager-0.2.1/PKG-INFO` & `milho_multi_sqlite3_manager-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milho-multi-sqlite3-manager
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: Guilherme S. Magalhães
 Author-email: 40049979+Guisilcol@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

