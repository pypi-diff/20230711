# Comparing `tmp/sqlalchemy-bigquery-1.6.1.tar.gz` & `tmp/sqlalchemy-bigquery-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-bigquery-1.6.1.tar", last modified: Wed Feb  1 20:04:55 2023, max compression
+gzip compressed data, was "sqlalchemy-bigquery-1.7.0.tar", last modified: Tue Jul 11 21:09:15 2023, max compression
```

## Comparing `sqlalchemy-bigquery-1.6.1.tar` & `sqlalchemy-bigquery-1.7.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.148858 sqlalchemy-bigquery-1.6.1/
--rw-rw-r--   0 root         (0)     1003      622 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/AUTHORS
--rw-rw-r--   0 root         (0)     1003     1064 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003    11513 2023-02-01 20:04:55.148858 sqlalchemy-bigquery-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    10381 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/README.rst
--rw-rw-r--   0 root         (0)     1003      300 2023-02-01 20:04:55.148858 sqlalchemy-bigquery-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3990 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.140857 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/
--rw-rw-r--   0 root         (0)     1003     2238 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     2412 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/_helpers.py
--rw-rw-r--   0 root         (0)     1003     5062 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/_struct.py
--rw-rw-r--   0 root         (0)     1003     4677 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/_types.py
--rw-rw-r--   0 root         (0)     1003    38532 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/base.py
--rw-rw-r--   0 root         (0)     1003     8638 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/geography.py
--rw-rw-r--   0 root         (0)     1003     9854 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/parse_url.py
--rw-rw-r--   0 root         (0)     1003     7361 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/requirements.py
--rw-rw-r--   0 root         (0)     1003     1131 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.140857 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/
--rw-r--r--   0 root         (0)     1003    11513 2023-02-01 20:04:55.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1615 2023-02-01 20:04:55.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-01 20:04:55.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       69 2023-02-01 20:04:55.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003      369 2023-02-01 20:04:55.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-01 20:04:55.000000 sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.140857 sqlalchemy-bigquery-1.6.1/tests/
--rw-rw-r--   0 root         (0)     1003        0 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1574 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.144857 sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/README.rst
--rw-rw-r--   0 root         (0)     1003     3368 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/conftest.py
--rw-rw-r--   0 root         (0)     1003    10371 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.144857 sqlalchemy-bigquery-1.6.1/tests/system/
--rw-rw-r--   0 root         (0)     1003     1108 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     5884 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.144857 sqlalchemy-bigquery-1.6.1/tests/system/data/
--rw-rw-r--   0 root         (0)     1003   200036 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/data/sample.json
--rw-rw-r--   0 root         (0)     1003      340 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/data/sample_one_row.json
--rw-rw-r--   0 root         (0)     1003     1481 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/data/schema.json
--rw-rw-r--   0 root         (0)     1003     6219 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/test__struct.py
--rw-rw-r--   0 root         (0)     1003     6248 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/test_alembic.py
--rw-rw-r--   0 root         (0)     1003     8790 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/test_geography.py
--rw-rw-r--   0 root         (0)     1003     3231 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/test_helpers.py
--rw-rw-r--   0 root         (0)     1003    26710 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/system/test_sqlalchemy_bigquery.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-01 20:04:55.148858 sqlalchemy-bigquery-1.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003        0 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003     3648 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/conftest.py
--rw-rw-r--   0 root         (0)     1003    16729 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/fauxdbi.py
--rw-rw-r--   0 root         (0)     1003     5231 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test__struct.py
--rw-rw-r--   0 root         (0)     1003    10392 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_catalog_functions.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_comments.py
--rw-rw-r--   0 root         (0)     1003     4263 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_compiler.py
--rw-rw-r--   0 root         (0)     1003     7047 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_compliance.py
--rw-rw-r--   0 root         (0)     1003     1632 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_dialect_types.py
--rw-rw-r--   0 root         (0)     1003     2815 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_engine.py
--rw-rw-r--   0 root         (0)     1003     5749 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_geography.py
--rw-rw-r--   0 root         (0)     1003     7821 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_helpers.py
--rw-rw-r--   0 root         (0)     1003     1963 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_like_reescape.py
--rw-rw-r--   0 root         (0)     1003     8633 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_parse_url.py
--rw-rw-r--   0 root         (0)     1003    15861 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_select.py
--rw-rw-r--   0 root         (0)     1003     8283 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_sqlalchemy_bigquery.py
--rw-rw-r--   0 root         (0)     1003     1386 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_version.py
--rw-rw-r--   0 root         (0)     1003     1647 2023-02-01 20:02:18.000000 sqlalchemy-bigquery-1.6.1/tests/unit/test_view.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.700960 sqlalchemy-bigquery-1.7.0/
+-rw-rw-r--   0 root         (0)     1003      622 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/AUTHORS
+-rw-rw-r--   0 root         (0)     1003     1064 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003    12530 2023-07-11 21:09:15.700960 sqlalchemy-bigquery-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    11372 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/README.rst
+-rw-rw-r--   0 root         (0)     1003      300 2023-07-11 21:09:15.700960 sqlalchemy-bigquery-1.7.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     4671 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.692959 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/
+-rw-rw-r--   0 root         (0)     1003     2258 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2412 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4943 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/_struct.py
+-rw-rw-r--   0 root         (0)     1003     4717 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/_types.py
+-rw-rw-r--   0 root         (0)     1003    39824 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/base.py
+-rw-rw-r--   0 root         (0)     1003     8638 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/geography.py
+-rw-rw-r--   0 root         (0)     1003     9854 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/parse_url.py
+-rw-rw-r--   0 root         (0)     1003     7361 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/requirements.py
+-rw-rw-r--   0 root         (0)     1003     1131 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.692959 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/
+-rw-r--r--   0 root         (0)     1003    12530 2023-07-11 21:09:15.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1615 2023-07-11 21:09:15.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-11 21:09:15.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       69 2023-07-11 21:09:15.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003      599 2023-07-11 21:09:15.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-11 21:09:15.000000 sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.692959 sqlalchemy-bigquery-1.7.0/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1574 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.696959 sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/README.rst
+-rw-rw-r--   0 root         (0)     1003     3368 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/conftest.py
+-rw-rw-r--   0 root         (0)     1003    10371 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.696959 sqlalchemy-bigquery-1.7.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003     1108 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5884 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.696959 sqlalchemy-bigquery-1.7.0/tests/system/data/
+-rw-rw-r--   0 root         (0)     1003   200036 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/data/sample.json
+-rw-rw-r--   0 root         (0)     1003      340 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/data/sample_one_row.json
+-rw-rw-r--   0 root         (0)     1003     1481 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/data/schema.json
+-rw-rw-r--   0 root         (0)     1003     6219 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/test__struct.py
+-rw-rw-r--   0 root         (0)     1003     6542 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/test_alembic.py
+-rw-rw-r--   0 root         (0)     1003     8790 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/test_geography.py
+-rw-rw-r--   0 root         (0)     1003     3231 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003    29215 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/system/test_sqlalchemy_bigquery.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 21:09:15.700960 sqlalchemy-bigquery-1.7.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3648 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/conftest.py
+-rw-rw-r--   0 root         (0)     1003    16729 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/fauxdbi.py
+-rw-rw-r--   0 root         (0)     1003     5231 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test__struct.py
+-rw-rw-r--   0 root         (0)     1003    10392 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_catalog_functions.py
+-rw-rw-r--   0 root         (0)     1003     3578 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_comments.py
+-rw-rw-r--   0 root         (0)     1003     4263 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_compiler.py
+-rw-rw-r--   0 root         (0)     1003     7047 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_compliance.py
+-rw-rw-r--   0 root         (0)     1003     1632 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_dialect_types.py
+-rw-rw-r--   0 root         (0)     1003     2815 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_engine.py
+-rw-rw-r--   0 root         (0)     1003     5838 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_geography.py
+-rw-rw-r--   0 root         (0)     1003     7821 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003     1963 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_like_reescape.py
+-rw-rw-r--   0 root         (0)     1003     8633 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_parse_url.py
+-rw-rw-r--   0 root         (0)     1003    17303 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_select.py
+-rw-rw-r--   0 root         (0)     1003     8283 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_sqlalchemy_bigquery.py
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_version.py
+-rw-rw-r--   0 root         (0)     1003     1647 2023-07-11 21:06:27.000000 sqlalchemy-bigquery-1.7.0/tests/unit/test_view.py
```

### Comparing `sqlalchemy-bigquery-1.6.1/AUTHORS` & `sqlalchemy-bigquery-1.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/LICENSE` & `sqlalchemy-bigquery-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/MANIFEST.in` & `sqlalchemy-bigquery-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/PKG-INFO` & `sqlalchemy-bigquery-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bigquery
-Version: 1.6.1
+Version: 1.7.0
 Summary: SQLAlchemy dialect for BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-sqlalchemy
 Author: The Sqlalchemy-Bigquery Authors
 Author-email: googleapis-packages@google.com
 Keywords: bigquery,sqlalchemy
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Obsoletes: pybigquery
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: geography
 Provides-Extra: alembic
 Provides-Extra: tests
+Provides-Extra: bqstorage
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS
 
 SQLAlchemy Dialect for BigQuery
 ===============================
 
@@ -108,14 +109,28 @@
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install sqlalchemy-bigquery
 
+
+Installations when processing large datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+When handling large datasets, you may see speed increases by also installing the
+`bqstorage` dependencies. See the instructions above about creating a virtual 
+environment and then install `sqlalchemy-bigquery` using the `bqstorage` extras:
+
+.. code-block:: console
+
+    source <your-env>/bin/activate
+    <your-env>/bin/pip install sqlalchemy-bigquery[bqstorage]
+
+
 Usage
 -----
 
 SQLAlchemy
 ^^^^^^^^^^
 
 .. code-block:: python
@@ -131,20 +146,35 @@
 ^^^^^^^
 
 ``project`` in ``bigquery://project`` is used to instantiate BigQuery client with the specific project ID. To infer project from the environment, use ``bigquery://`` – without ``project``
 
 Authentication
 ^^^^^^^^^^^^^^
 
-Follow the `Google Cloud library guide <https://google-cloud-python.readthedocs.io/en/latest/core/auth.html>`_ for authentication. Alternatively, you can provide the path to a service account JSON file in ``create_engine()``:
+Follow the `Google Cloud library guide <https://google-cloud-python.readthedocs.io/en/latest/core/auth.html>`_ for authentication. 
+
+Alternatively, you can choose either of the following approaches:
+
+* provide the path to a service account JSON file in ``create_engine()`` using the ``credentials_path`` parameter:
 
 .. code-block:: python
 
+    # provide the path to a service account JSON file
     engine = create_engine('bigquery://', credentials_path='/path/to/keyfile.json')
 
+* pass the credentials in ``create_engine()`` as a Python dictionary using the ``credentials_info`` parameter:
+
+.. code-block:: python
+    
+    # provide credentials as a Python dictionary
+    credentials_info = {
+        "type": "service_account", 
+        "project_id": "your-service-account-project-id"
+    },
+    engine = create_engine('bigquery://', credentials_info=credentials_info)
 
 Location
 ^^^^^^^^
 
 To specify location of your datasets pass ``location`` to ``create_engine()``:
 
 .. code-block:: python
```

### Comparing `sqlalchemy-bigquery-1.6.1/README.rst` & `sqlalchemy-bigquery-1.7.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -77,14 +77,28 @@
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install sqlalchemy-bigquery
 
+
+Installations when processing large datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+When handling large datasets, you may see speed increases by also installing the
+`bqstorage` dependencies. See the instructions above about creating a virtual 
+environment and then install `sqlalchemy-bigquery` using the `bqstorage` extras:
+
+.. code-block:: console
+
+    source <your-env>/bin/activate
+    <your-env>/bin/pip install sqlalchemy-bigquery[bqstorage]
+
+
 Usage
 -----
 
 SQLAlchemy
 ^^^^^^^^^^
 
 .. code-block:: python
@@ -100,20 +114,35 @@
 ^^^^^^^
 
 ``project`` in ``bigquery://project`` is used to instantiate BigQuery client with the specific project ID. To infer project from the environment, use ``bigquery://`` – without ``project``
 
 Authentication
 ^^^^^^^^^^^^^^
 
-Follow the `Google Cloud library guide <https://google-cloud-python.readthedocs.io/en/latest/core/auth.html>`_ for authentication. Alternatively, you can provide the path to a service account JSON file in ``create_engine()``:
+Follow the `Google Cloud library guide <https://google-cloud-python.readthedocs.io/en/latest/core/auth.html>`_ for authentication. 
+
+Alternatively, you can choose either of the following approaches:
+
+* provide the path to a service account JSON file in ``create_engine()`` using the ``credentials_path`` parameter:
 
 .. code-block:: python
 
+    # provide the path to a service account JSON file
     engine = create_engine('bigquery://', credentials_path='/path/to/keyfile.json')
 
+* pass the credentials in ``create_engine()`` as a Python dictionary using the ``credentials_info`` parameter:
+
+.. code-block:: python
+    
+    # provide credentials as a Python dictionary
+    credentials_info = {
+        "type": "service_account", 
+        "project_id": "your-service-account-project-id"
+    },
+    engine = create_engine('bigquery://', credentials_info=credentials_info)
 
 Location
 ^^^^^^^^
 
 To specify location of your datasets pass ``location`` to ``create_engine()``:
 
 .. code-block:: python
```

### Comparing `sqlalchemy-bigquery-1.6.1/setup.py` & `sqlalchemy-bigquery-1.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,19 +41,34 @@
 
 
 def readme():
     with io.open("README.rst", "r", encoding="utf8") as f:
         return f.read()
 
 
-extras = dict(
-    geography=["GeoAlchemy2", "shapely"],
-    alembic=["alembic"],
-    tests=["packaging", "pytz"],
-)
+extras = {
+    "geography": ["GeoAlchemy2", "shapely"],
+    "alembic": ["alembic"],
+    "tests": ["packaging", "pytz"],
+    # Keep the no-op bqstorage extra for backward compatibility.
+    # See: https://github.com/googleapis/python-bigquery/issues/757
+    "bqstorage": [
+        "google-cloud-bigquery-storage >= 2.0.0, <3.0.0dev",
+        # Due to an issue in pip's dependency resolver, the `grpc` extra is not
+        # installed, even though `google-cloud-bigquery-storage` specifies it
+        # as `google-api-core[grpc]`. We thus need to explicitly specify it here.
+        # See: https://github.com/googleapis/python-bigquery/issues/83 The
+        # grpc.Channel.close() method isn't added until 1.32.0.
+        # https://github.com/grpc/grpc/pull/15254
+        "grpcio >= 1.47.0, < 2.0dev",
+        "grpcio >= 1.49.1, < 2.0dev; python_version>='3.11'",
+        "pyarrow >= 3.0.0",
+    ],
+}
+
 extras["all"] = set(itertools.chain.from_iterable(extras.values()))
 
 setup(
     name=name,
     version=version,
     description=description,
     long_description=readme(),
@@ -81,19 +96,16 @@
     install_requires=[
         "google-api-core >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
         # NOTE: Maintainers, please do not require google-auth>=2.x.x
         # Until this issue is closed
         # https://github.com/googleapis/google-cloud-python/issues/10566
         "google-auth>=1.25.0,<3.0.0dev",  # Work around pip wack.
         "google-cloud-bigquery>=2.25.2,<4.0.0dev",
-        "google-cloud-bigquery-storage>=2.0.0,<3.0.0dev",
         "packaging",
-        "pyarrow>=3.0.0",
         "sqlalchemy>=1.2.0,<2.0.0dev",
-        "future",
     ],
     extras_require=extras,
     python_requires=">=3.7, <3.12",
     tests_require=["packaging", "pytz"],
     entry_points={
         "sqlalchemy.dialects": ["bigquery = sqlalchemy_bigquery:BigQueryDialect"]
     },
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/__init__.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     "STRUCT",
     "TIME",
     "TIMESTAMP",
 ]
 
 try:
     from .geography import GEOGRAPHY, WKB, WKT  # noqa
-except ImportError:
+except ImportError:  # pragma: NO COVER
     pass
 else:
     __all__.extend(["GEOGRAPHY", "WKB", "WKT"])
 
 try:
     import pybigquery  # noqa
 except ImportError:
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/_helpers.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/_struct.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/_struct.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-from typing import Mapping, Tuple
-
 import packaging.version
 import sqlalchemy.sql.default_comparator
 import sqlalchemy.sql.sqltypes
 import sqlalchemy.types
 
 from . import base
 
@@ -50,16 +48,16 @@
     See https://googleapis.dev/python/sqlalchemy-bigquery/latest/struct.html
     """
 
     # See https://docs.sqlalchemy.org/en/14/core/custom_types.html#creating-new-types
 
     def __init__(
         self,
-        *fields: Tuple[str, sqlalchemy.types.TypeEngine],
-        **kwfields: Mapping[str, sqlalchemy.types.TypeEngine],
+        *fields,
+        **kwfields,
     ):
         # Note that because:
         # https://docs.python.org/3/whatsnew/3.6.html#pep-468-preserving-keyword-argument-order
         # We know that `kwfields` preserves order.
         self._STRUCT_fields = tuple(
             (
                 name,
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/_types.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import sqlalchemy.types
 import sqlalchemy.util
 
 from google.cloud.bigquery.schema import SchemaField
 
 try:
     from .geography import GEOGRAPHY
-except ImportError:
+except ImportError:  # pragma: NO COVER
     pass
 
 from ._struct import STRUCT
 
 _type_map = {
     "ARRAY": sqlalchemy.types.ARRAY,
     "BIGNUMERIC": sqlalchemy.types.Numeric,
@@ -65,15 +65,15 @@
 RECORD = _type_map["RECORD"]
 STRING = _type_map["STRING"]
 TIMESTAMP = _type_map["TIMESTAMP"]
 TIME = _type_map["TIME"]
 
 try:
     _type_map["GEOGRAPHY"] = GEOGRAPHY
-except NameError:
+except NameError:  # pragma: NO COVER
     pass
 
 STRUCT_FIELD_TYPES = "RECORD", "STRUCT"
 
 
 def _get_transitive_schema_fields(fields):
     """
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/base.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """Integration between SQLAlchemy and BigQuery."""
 
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
 from decimal import Decimal
 import random
 import operator
 import uuid
 
 from google import auth
 import google.api_core.exceptions
@@ -36,14 +33,15 @@
 import sqlalchemy
 import sqlalchemy.sql.expression
 import sqlalchemy.sql.functions
 import sqlalchemy.sql.sqltypes
 import sqlalchemy.sql.type_api
 from sqlalchemy.exc import NoSuchTableError
 from sqlalchemy import util
+from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.sql.compiler import (
     SQLCompiler,
     GenericTypeCompiler,
     DDLCompiler,
     IdentifierPreparer,
 )
 from sqlalchemy.sql.sqltypes import Integer, String, NullType, Numeric
@@ -259,14 +257,15 @@
     def _known_tables(self):
         known_tables = set()
 
         for from_ in self.compile_state.froms:
             if isinstance(from_, Table):
                 known_tables.add(from_.name)
             elif isinstance(from_, CTE):
+                known_tables.add(from_.name)
                 for column in from_.original.selected_columns:
                     table = getattr(column, "table", None)
                     if table is not None:
                         known_tables.add(table.name)
 
         return known_tables
 
@@ -549,14 +548,26 @@
         return param
 
     def visit_getitem_binary(self, binary, operator_, **kw):
         left = self.process(binary.left, **kw)
         right = self.process(binary.right, **kw)
         return f"{left}[OFFSET({right})]"
 
+    def _get_regexp_args(self, binary, kw):
+        string = self.process(binary.left, **kw)
+        pattern = self.process(binary.right, **kw)
+        return string, pattern
+
+    def visit_regexp_match_op_binary(self, binary, operator, **kw):
+        string, pattern = self._get_regexp_args(binary, kw)
+        return "REGEXP_CONTAINS(%s, %s)" % (string, pattern)
+
+    def visit_not_regexp_match_op_binary(self, binary, operator, **kw):
+        return "NOT %s" % self.visit_regexp_match_op_binary(binary, operator, **kw)
+
 
 class BigQueryTypeCompiler(GenericTypeCompiler):
     def visit_INTEGER(self, type_, **kw):
         return "INT64"
 
     visit_BIGINT = visit_SMALLINT = visit_INTEGER
 
@@ -770,14 +781,15 @@
     ):
         super(BigQueryDialect, self).__init__(*args, **kwargs)
         self.arraysize = arraysize
         self.credentials_path = credentials_path
         self.credentials_info = credentials_info
         self.credentials_base64 = credentials_base64
         self.location = location
+        self.identifier_preparer = self.preparer(self)
         self.dataset_id = None
         self.list_tables_page_size = list_tables_page_size
 
     @classmethod
     def dbapi(cls):
         return dbapi
 
@@ -1051,14 +1063,27 @@
         super().__init__(*args, **kwargs)
 
 
 dialect = BigQueryDialect
 
 try:
     import alembic  # noqa
-except ImportError:
+except ImportError:  # pragma: NO COVER
     pass
 else:
     from alembic.ddl import impl
+    from alembic.ddl.base import ColumnType, format_type, alter_table, alter_column
 
     class SqlalchemyBigqueryImpl(impl.DefaultImpl):
         __dialect__ = "bigquery"
+
+    @compiles(ColumnType, "bigquery")
+    def visit_column_type(element: ColumnType, compiler: DDLCompiler, **kw) -> str:
+        """Replaces the visit_column_type() function in alembic/alembic/ddl/base.py.
+        The alembic version ends in TYPE <element type>, but bigquery requires this syntax:
+        SET DATA TYPE <element type>"""
+
+        return "%s %s %s" % (  # pragma: NO COVER
+            alter_table(compiler, element.table_name, element.schema),
+            alter_column(compiler, element.column_name),
+            "SET DATA TYPE %s" % format_type(compiler, element.type_),
+        )
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/geography.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/geography.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/parse_url.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/parse_url.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/requirements.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery/version.py` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-__version__ = "1.6.1"
+__version__ = "1.7.0"
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/PKG-INFO` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bigquery
-Version: 1.6.1
+Version: 1.7.0
 Summary: SQLAlchemy dialect for BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-sqlalchemy
 Author: The Sqlalchemy-Bigquery Authors
 Author-email: googleapis-packages@google.com
 Keywords: bigquery,sqlalchemy
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Obsoletes: pybigquery
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: geography
 Provides-Extra: alembic
 Provides-Extra: tests
+Provides-Extra: bqstorage
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS
 
 SQLAlchemy Dialect for BigQuery
 ===============================
 
@@ -108,14 +109,28 @@
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install sqlalchemy-bigquery
 
+
+Installations when processing large datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+When handling large datasets, you may see speed increases by also installing the
+`bqstorage` dependencies. See the instructions above about creating a virtual 
+environment and then install `sqlalchemy-bigquery` using the `bqstorage` extras:
+
+.. code-block:: console
+
+    source <your-env>/bin/activate
+    <your-env>/bin/pip install sqlalchemy-bigquery[bqstorage]
+
+
 Usage
 -----
 
 SQLAlchemy
 ^^^^^^^^^^
 
 .. code-block:: python
@@ -131,20 +146,35 @@
 ^^^^^^^
 
 ``project`` in ``bigquery://project`` is used to instantiate BigQuery client with the specific project ID. To infer project from the environment, use ``bigquery://`` – without ``project``
 
 Authentication
 ^^^^^^^^^^^^^^
 
-Follow the `Google Cloud library guide <https://google-cloud-python.readthedocs.io/en/latest/core/auth.html>`_ for authentication. Alternatively, you can provide the path to a service account JSON file in ``create_engine()``:
+Follow the `Google Cloud library guide <https://google-cloud-python.readthedocs.io/en/latest/core/auth.html>`_ for authentication. 
+
+Alternatively, you can choose either of the following approaches:
+
+* provide the path to a service account JSON file in ``create_engine()`` using the ``credentials_path`` parameter:
 
 .. code-block:: python
 
+    # provide the path to a service account JSON file
     engine = create_engine('bigquery://', credentials_path='/path/to/keyfile.json')
 
+* pass the credentials in ``create_engine()`` as a Python dictionary using the ``credentials_info`` parameter:
+
+.. code-block:: python
+    
+    # provide credentials as a Python dictionary
+    credentials_info = {
+        "type": "service_account", 
+        "project_id": "your-service-account-project-id"
+    },
+    engine = create_engine('bigquery://', credentials_info=credentials_info)
 
 Location
 ^^^^^^^^
 
 To specify location of your datasets pass ``location`` to ``create_engine()``:
 
 .. code-block:: python
```

### Comparing `sqlalchemy-bigquery-1.6.1/sqlalchemy_bigquery.egg-info/SOURCES.txt` & `sqlalchemy-bigquery-1.7.0/sqlalchemy_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/conftest.py` & `sqlalchemy-bigquery-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/README.rst` & `sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/conftest.py` & `sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py` & `sqlalchemy-bigquery-1.7.0/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/__init__.py` & `sqlalchemy-bigquery-1.7.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/conftest.py` & `sqlalchemy-bigquery-1.7.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/data/sample.json` & `sqlalchemy-bigquery-1.7.0/tests/system/data/sample.json`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/data/schema.json` & `sqlalchemy-bigquery-1.7.0/tests/system/data/schema.json`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/test__struct.py` & `sqlalchemy-bigquery-1.7.0/tests/system/test__struct.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/test_alembic.py` & `sqlalchemy-bigquery-1.7.0/tests/system/test_alembic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import contextlib
 
 import pytest
-from sqlalchemy import Column, DateTime, Integer, String
+from sqlalchemy import Column, DateTime, Integer, String, Numeric
 
 import google.api_core.exceptions
 from google.cloud.bigquery import SchemaField
 
 alembic = pytest.importorskip("alembic")
 
 
@@ -145,20 +145,27 @@
             transaction_time DATETIME NOT NULL,
             amount NUMERIC(11, 2) NOT NULL
             )
         partition by DATE(transaction_time)
         """
     )
 
-    # The only thing we can alter about a column is we can make it
-    # nullable:
-    op.alter_column("transactions", "amount", True)
+    op.alter_column("transactions", "amount", nullable=True)
     assert alembic_table("transactions", "schema") == [
         SchemaField("account", "INTEGER", "REQUIRED"),
         SchemaField("transaction_time", "DATETIME", "REQUIRED"),
         SchemaField("amount", "NUMERIC(11, 2)"),
     ]
 
     op.create_table_comment("transactions", "Transaction log")
     assert alembic_table("transactions").description == "Transaction log"
 
     op.drop_table("transactions")
+
+    # Another thing we can do is alter the datatype of a nullable column,
+    # if allowed by BigQuery's type coercion rules
+    op.create_table("identifiers", Column("id", Integer))
+
+    op.alter_column("identifiers", "id", type_=Numeric)
+    assert alembic_table("identifiers", "schema") == [SchemaField("id", "NUMERIC")]
+
+    op.drop_table("identifiers")
```

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/test_geography.py` & `sqlalchemy-bigquery-1.7.0/tests/system/test_geography.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/test_helpers.py` & `sqlalchemy-bigquery-1.7.0/tests/system/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/system/test_sqlalchemy_bigquery.py` & `sqlalchemy-bigquery-1.7.0/tests/system/test_sqlalchemy_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import datetime
 import decimal
 
 from sqlalchemy.engine import create_engine
 from sqlalchemy.schema import Table, MetaData, Column
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy import types, func, case, inspect
+from sqlalchemy import types, func, case, inspect, not_
 from sqlalchemy.sql import expression, select, literal_column
 from sqlalchemy.exc import NoSuchTableError
 from sqlalchemy.orm import sessionmaker
 import packaging.version
 from pytz import timezone
 import pytest
 import sqlalchemy
@@ -770,7 +770,85 @@
     assert " ".join(compiled.strip().split()) == (
         f"SELECT `foo_objects`"
         f" FROM"
         f" `{bigquery_dataset}.test_unnest` `{bigquery_dataset}.test_unnest_1`,"
         f" unnest(`{bigquery_dataset}.test_unnest_1`.`objects`) AS `foo_objects`"
     )
     assert sorted(r[0] for r in conn.execute(query)) == ["a", "b", "c", "x", "y"]
+
+
+@pytest.mark.skipif(
+    packaging.version.parse(sqlalchemy.__version__) < packaging.version.parse("1.4"),
+    reason="unnest (and other table-valued-function) support required version 1.4",
+)
+def test_unnest_with_cte(engine, bigquery_dataset):
+    from sqlalchemy import select, func, String
+    from sqlalchemy_bigquery import ARRAY
+
+    conn = engine.connect()
+    metadata = MetaData()
+    table_name = "test_unnest_with_cte"
+    table = Table(
+        f"{bigquery_dataset}.{table_name}",
+        metadata,
+        Column("foo", String),
+        Column("bars", ARRAY(String)),
+    )
+    metadata.create_all(engine)
+    conn.execute(
+        table.insert(),
+        [dict(foo="first", bars=["a", "b", "c"]), dict(foo="second", bars=["x", "y"])],
+    )
+    selectable = select(table.c).select_from(table).cte("cte")
+    query = select(
+        [
+            selectable.c.foo,
+            func.unnest(selectable.c.bars).column_valued("unnest_bars"),
+        ]
+    ).select_from(selectable)
+    compiled = str(query.compile(engine))
+    assert " ".join(compiled.strip().split()) == (
+        f"WITH `cte` "
+        f"AS (SELECT `{bigquery_dataset}.{table_name}`.`foo` AS `foo`,"
+        f" `{bigquery_dataset}.{table_name}`.`bars` AS `bars`"
+        f" FROM `{bigquery_dataset}.{table_name}`) "
+        f"SELECT `cte`.`foo`, `unnest_bars` "
+        f"FROM `cte`, unnest(`cte`.`bars`) AS `unnest_bars`"
+    )
+
+    assert sorted(r for r in conn.execute(query)) == [
+        ("first", "a"),
+        ("first", "b"),
+        ("first", "c"),
+        ("second", "x"),
+        ("second", "y"),
+    ]
+
+
+@pytest.mark.skipif(
+    packaging.version.parse(sqlalchemy.__version__) < packaging.version.parse("1.4"),
+    reason="regexp_match support requires version 1.4 or higher",
+)
+def test_regexp_match(session, table):
+    results = (
+        session.query(table.c.string)
+        .where(table.c.string.regexp_match(".*52 St &.*"))
+        .all()
+    )
+
+    number_of_52st_records = 12
+    assert len(results) == number_of_52st_records
+
+
+@pytest.mark.skipif(
+    packaging.version.parse(sqlalchemy.__version__) < packaging.version.parse("1.4"),
+    reason="regexp_match support requires version 1.4 or higher",
+)
+def test_not_regexp_match(session, table):
+    results = (
+        session.query(table.c.string)
+        .where(not_(table.c.string.regexp_match("^Barrow St & Hudson St$")))
+        .all()
+    )
+
+    number_of_non_barrowst_records = 993
+    assert len(results) == number_of_non_barrowst_records
```

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/conftest.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/fauxdbi.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/fauxdbi.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test__struct.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test__struct.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_catalog_functions.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_catalog_functions.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_comments.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_comments.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_compiler.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_compiler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_compliance.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_compliance.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_dialect_types.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_dialect_types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_engine.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_engine.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_geography.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_geography.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         "FROM `lake` \n"
         "WHERE ST_Contains(`lake`.`geog`, %(ST_Contains_1:geography)s)",
         {"ST_Contains_1": "POINT(4 1)"},
     )
 
     try:
         conn.execute(
-            select([lake_table.c.name, lake_table.c.geog.ST_AREA().label("area")])
+            select([lake_table.c.name, lake_table.c.geog.ST_Area().label("area")])
         )
     except Exception:
         pass  # sqlite had no special functions :)
     last_query("SELECT `lake`.`name`, ST_Area(`lake`.`geog`) AS `area` \nFROM `lake`")
 
     # Extra: Make sure we can save a retrieved value back:
 
@@ -156,24 +156,26 @@
     with pytest.raises(AssertionError, match="Extended must be True."):
         GEOGRAPHY.ElementType("data", extended=False)
 
 
 def test_GEOGRAPHY_ElementType():
     from sqlalchemy_bigquery import GEOGRAPHY, WKB
 
-    data = GEOGRAPHY.ElementType("data")
+    # The data argument here should be composed of hex characters:
+    # 1-0 and a-f
+    data = GEOGRAPHY.ElementType("123def")
     assert isinstance(data, WKB)
-    assert (data.data, data.srid, data.extended) == ("data", 4326, True)
+    assert (data.data, data.srid, data.extended) == ("123def", 4326, True)
 
 
 def test_calling_st_functions_that_dont_take_geographies(faux_conn, last_query):
     from sqlalchemy import select, func
 
     try:
-        faux_conn.execute(select([func.ST_GEOGFROMTEXT("point(0 0)")]))
+        faux_conn.execute(select([func.ST_GeogFromText("point(0 0)")]))
     except Exception:
         pass  # sqlite had no special functions :)
 
     last_query(
         "SELECT ST_AsBinary(ST_GeogFromText(%(ST_GeogFromText_2:STRING)s))"
         " AS `ST_GeogFromText_1`",
         dict(ST_GeogFromText_2="point(0 0)"),
```

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_helpers.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_like_reescape.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_like_reescape.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_parse_url.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_parse_url.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_select.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import datetime
 from decimal import Decimal
 
 import packaging.version
 import pytest
 import sqlalchemy
+from sqlalchemy import not_
 
 import sqlalchemy_bigquery
 
 from .conftest import (
     setup_table,
     sqlalchemy_version,
     sqlalchemy_1_3_or_higher,
@@ -441,7 +442,47 @@
     t = sqlalchemy.Table(
         "t",
         metadata,
         sqlalchemy.Column("a", sqlalchemy.ARRAY(sqlalchemy.String)),
     )
     got = str(sqlalchemy.select([t.c.a[0]]).compile(faux_conn.engine))
     assert got == "SELECT `t`.`a`[OFFSET(%(a_1:INT64)s)] AS `anon_1` \nFROM `t`"
+
+
+@pytest.mark.skipif(
+    packaging.version.parse(sqlalchemy.__version__) < packaging.version.parse("1.4"),
+    reason="regexp_match support requires version 1.4 or higher",
+)
+def test_visit_regexp_match_op_binary(faux_conn):
+    table = setup_table(
+        faux_conn,
+        "table",
+        sqlalchemy.Column("foo", sqlalchemy.String),
+    )
+
+    # NOTE: "sample_pattern" is not used in this test, we are not testing
+    # the regex engine, we are testing the ability to create SQL
+    sql_statement = table.c.foo.regexp_match("sample_pattern")
+    result = sql_statement.compile(faux_conn).string
+    expected = "REGEXP_CONTAINS(`table`.`foo`, %(foo_1:STRING)s)"
+
+    assert result == expected
+
+
+@pytest.mark.skipif(
+    packaging.version.parse(sqlalchemy.__version__) < packaging.version.parse("1.4"),
+    reason="regexp_match support requires version 1.4 or higher",
+)
+def test_visit_not_regexp_match_op_binary(faux_conn):
+    table = setup_table(
+        faux_conn,
+        "table",
+        sqlalchemy.Column("foo", sqlalchemy.String),
+    )
+
+    # NOTE: "sample_pattern" is not used in this test, we are not testing
+    # the regex engine, we are testing the ability to create SQL
+    sql_statement = not_(table.c.foo.regexp_match("sample_pattern"))
+    result = sql_statement.compile(faux_conn).string
+    expected = "NOT REGEXP_CONTAINS(`table`.`foo`, %(foo_1:STRING)s)"
+
+    assert result == expected
```

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_sqlalchemy_bigquery.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_sqlalchemy_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_version.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.6.1/tests/unit/test_view.py` & `sqlalchemy-bigquery-1.7.0/tests/unit/test_view.py`

 * *Files identical despite different names*

