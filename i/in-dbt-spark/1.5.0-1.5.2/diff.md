# Comparing `tmp/in-dbt-spark-1.5.0.tar.gz` & `tmp/in-dbt-spark-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.5.0.tar", last modified: Thu Jun  1 19:24:18 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.5.2.tar", last modified: Tue Jul 11 07:20:24 2023, max compression
```

## Comparing `in-dbt-spark-1.5.0.tar` & `in-dbt-spark-1.5.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.134134 in-dbt-spark-1.5.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.134134 in-dbt-spark-1.5.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    25553 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    25848 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.134134 in-dbt-spark-1.5.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.873319 in-dbt-spark-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-11 07:20:24.873319 in-dbt-spark-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.865319 in-dbt-spark-1.5.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.865319 in-dbt-spark-1.5.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.865319 in-dbt-spark-1.5.2/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.865319 in-dbt-spark-1.5.2/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29624 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.865319 in-dbt-spark-1.5.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.869319 in-dbt-spark-1.5.2/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.869319 in-dbt-spark-1.5.2/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    21436 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.869319 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.869319 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.873319 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:20:24.873319 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-11 07:20:24.000000 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-11 07:20:24.000000 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:20:24.000000 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:20:24.000000 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 07:20:24.000000 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 07:20:24.000000 in-dbt-spark-1.5.2/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 07:20:24.873319 in-dbt-spark-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-11 07:20:12.000000 in-dbt-spark-1.5.2/setup.py
```

### Comparing `in-dbt-spark-1.5.0/PKG-INFO` & `in-dbt-spark-1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.5.0
+Version: 1.5.2
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: ODBC
 Provides-Extra: PyHive
 Provides-Extra: session
 Provides-Extra: all
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.0 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.2 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: ODBC
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra: ODBC
 Provides-Extra: PyHive Provides-Extra: session Provides-Extra: all
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
```

### Comparing `in-dbt-spark-1.5.0/README.md` & `in-dbt-spark-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/client.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     deserializing the response as JSON and raising an exception when an error
     HTTP code is received.
     """
 
     def __init__(
         self,
         url: str,
-        auth: Auth = None,
+        auth: Optional[Auth] = None,
         verify: Verify = False,
-        requests_session: requests.Session = None,
-        cert: Cert = None,
-        datavault_token: str = None,
+        requests_session: Optional[requests.Session] = None,
+        cert: Optional[Cert] = None,
+        datavault_token: Optional[str] = None,
     ) -> None:
         self.url = url
         self.auth = auth
         self.verify = verify
         self.headers = {"Content-Type": "application/json"}
         if datavault_token:
             self.headers["DVToken"] = datavault_token
@@ -62,31 +62,31 @@
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         self.close()
 
     def close(self) -> None:
         if self.managed_session:
             self.session.close()
 
-    def get(self, endpoint: str = "", params: dict = None) -> dict:
+    def get(self, endpoint: str = "", params: Optional[dict] = None) -> dict:
         return self._request("GET", endpoint, params=params, headers=self.headers, cert=self.cert)
 
-    def post(self, endpoint: str, data: dict = None) -> dict:
+    def post(self, endpoint: str, data: Optional[dict] = None) -> dict:
         return self._request("POST", endpoint, data, headers=self.headers, cert=self.cert)
 
     def delete(self, endpoint: str = "") -> dict:
         return self._request("DELETE", endpoint, headers=self.headers, cert=self.cert)
 
     def _request(
         self,
         method: str,
         endpoint: str,
-        data: dict = None,
-        params: dict = None,
-        headers: dict = None,
-        cert: Tuple[str, str] = None,
+        data: Optional[dict] = None,
+        params: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        cert: Optional[Tuple[str, str]] = None,
     ) -> dict:
         url = self.url.rstrip("/") + "/" + endpoint.lstrip("/")
         response = self.session.request(
             method,
             url,
             auth=self.auth,
             verify=self.verify,
@@ -103,15 +103,15 @@
     """
     A Client wrapper for all SETU API interactions
     """
 
     def __init__(
         self,
         url: str,
-        auth: Auth = None,
+        auth: Optional[Auth] = None,
         verify: Verify = True,
     ) -> None:
         self._client = JsonClient(
             url=url,
             auth=auth,
             verify=verify,
             cert=get_grestin_certs(),
@@ -259,15 +259,15 @@
                 f"Failed while fetching list of statements of setu session with id {session_id}",
                 e,
             )
             raise
         return [Statement.from_json(session_id, response) for data in response["statements"]]
 
     def create_statement(
-        self, session_id: str, code: str, kind: StatementKind = None
+        self, session_id: str, code: str, kind: Optional[StatementKind] = None
     ) -> Statement:
         """
         create a statement in a session. This is not a blocking call.
         :param session_id: The ID of the session.
         :param code: The code to execute.
         :param kind: The kind of code to execute.
         """
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/models.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,18 @@
 }
 SESSION_STATE_FINISHED = {
     SessionState.ERROR,
     SessionState.DEAD,
     SessionState.KILLED,
     SessionState.SUCCESS,
 }
+SESSION_STATE_READY = {
+    SessionState.BUSY,
+    SessionState.IDLE,
+}
 
 
 @dataclass
 class SessionAppInfo:
     sparkUiUrl: str
     yarnQueue: str
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/session.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import time
 
 import dbt.exceptions
 from dbt.events import AdapterLogger
 from dbt.adapters.setu.client import SetuClient, Auth, Verify
-from dbt.adapters.setu.models import SessionState, SESSION_STATE_NOT_READY, SESSION_INVALID_STATE
+from dbt.adapters.setu.models import SessionState, SESSION_STATE_READY, SESSION_INVALID_STATE
 from dbt.adapters.setu.session_cursor import SetuStatementCursor
 from dbt.adapters.setu.utils import (
     get_platform,
     platform_supports_setu_session_reuse,
     polling_intervals,
 )
+from typing import Optional
 
 logger = AdapterLogger("Spark")
 
 
 class SetuSession:
     """Manages a remote SETU session and high-level interactions with it.
 
@@ -25,15 +26,15 @@
         be a path to a CA bundle to use. Defaults to ``True``.
     """
 
     def __init__(
         self,
         url: str,
         session_id: str,
-        auth: Auth = None,
+        auth: Optional[Auth] = None,
         verify: Verify = False,
     ) -> None:
         self.client = SetuClient(url, auth, verify)
         self.session_id = session_id
         self.url = url
         self.diagnostics = "No diagnostics available."
 
@@ -48,30 +49,41 @@
         """print SETU session information"""
         session = self.client.get_session(session_id=self.session_id)
         logger.info("SETU session INFO = {} ".format(session))
 
     def wait_till_ready(self) -> None:
         """Wait for the session to be ready."""
         intervals = polling_intervals([1, 2, 3, 5], 10)
-        while self.state in SESSION_STATE_NOT_READY:
+        start_time = time.time()
+        timeout_seconds = 1860  # setu session timeout is 30 minutes
+
+        while self.state not in SESSION_STATE_READY:
             interval = next(intervals)
             logger.info(
                 f"Waiting to get spark resources for setu session - {self.session_id}, current state - {self.state.value}"
             )
             logger.info(f"Sleeping for {interval} seconds..")
             time.sleep(interval)
-        if self.state in SESSION_INVALID_STATE:
-            # Log setu submit error for dead state
-            if self.state == SessionState.DEAD:
-                logger.error(self.client.get_log(self.session_id))
-            logger.error(f"Unable to create setu session with {self.session_id} with error:")
-            logger.error(self.diagnostics)
-            raise dbt.exceptions.DbtRuntimeError(
-                f" Setu session state = {self.state} Unable to create setu session with {self.session_id}"
-            )
+            if self.state in SESSION_INVALID_STATE:
+                # Log setu submit error for dead state
+                if self.state == SessionState.DEAD:
+                    logger.error(self.client.get_log(self.session_id))
+                logger.error(f"Unable to create setu session with {self.session_id} with error:")
+                logger.error(self.diagnostics)
+                raise dbt.exceptions.DbtRuntimeError(
+                    f" Setu session state = {self.state} Unable to create setu session with {self.session_id}"
+                )
+
+            # Add fail safe to avoid infinite loop
+            if time.time() - start_time > timeout_seconds:
+                logger.error("Timed out waiting for setu session to be ready")
+                raise dbt.exceptions.DbtRuntimeError(
+                    "Timed out waiting for setu session to be ready"
+                )
+
         self.print_session_details()
 
     @property
     def state(self) -> SessionState:
         """The state of the managed SETU session."""
         session = self.client.get_session(self.session_id)
         if session is None:
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/session_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,7 +169,8 @@
             """
             if line.startswith("$$" + StatementKind.SPARK.value + "$$"):
                 return StatementKind.SPARK
             elif line.startswith("$$" + StatementKind.PYSPARK.value + "$$"):
                 return StatementKind.PYSPARK
             else:
                 return StatementKind.SQL
+        return StatementKind.SQL
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/session_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,22 +41,22 @@
     Manages creation and closing of SETU sessions
     """
 
     @classmethod
     def create_session(
         cls,
         url: str,
-        auth: Auth = None,
+        auth: Optional[Auth] = None,
         verify: Verify = False,
-        proxy_user: str = None,
-        jars: List[str] = None,
-        py_files: List[str] = None,
-        archives: List[str] = None,
-        files: List[str] = None,
-        manifest_file_location: str = None,
+        proxy_user: Optional[str] = None,
+        jars: Optional[List[str]] = None,
+        py_files: Optional[List[str]] = None,
+        archives: Optional[List[str]] = None,
+        files: Optional[List[str]] = None,
+        manifest_file_location: Optional[str] = None,
         queue: str = DEFAULT_YARN_QUEUE,
         setu_session_name: str = DEFAULT_SPARK_APPLICATION_NAME,
         spark_version: str = DEFAULT_SPARK_VERSION,
         execution_tags: Dict[str, Any] = dict(),
         spark_conf: Dict[str, Any] = dict(),
         metadata: Dict[str, Any] = dict(),
         heartbeat_timeout_in_seconds: int = DEFAULT_HEARTBEAT_TIMEOUT,
@@ -94,36 +94,36 @@
         :param enable_ssl: enable ssl configurations on driver and executors
         :param execution_tags: Dict of tags to be inferred by Infra
         :param spark_version: version of the spark session
         :param manifest_file_location: location of manifest file with all the dependencies
         """
         with cls.session_lock:
             session_initialization_config = SessionInitializationConfig(
-                proxy_user=proxy_user,
-                jars=jars,
-                py_files=py_files,
-                files=files,
-                archives=archives,
-                manifest_file_location=manifest_file_location,
+                proxy_user=proxy_user,  # type: ignore
+                jars=jars,  # type: ignore
+                py_files=py_files,  # type: ignore
+                files=files,  # type: ignore
+                archives=archives,  # type: ignore
+                manifest_file_location=manifest_file_location,  # type: ignore
                 driver_memory=spark_conf.get(
-                    SPARK_RESOURCE_KEYS.get("driver_memory"), DEFAULT_DRIVER_MEMORY
+                    SPARK_RESOURCE_KEYS.get("driver_memory"), DEFAULT_DRIVER_MEMORY  # type: ignore
                 ),
                 driver_cores=spark_conf.get(
-                    SPARK_RESOURCE_KEYS.get("driver_cores"), DEFAULT_DRIVER_CORES
+                    SPARK_RESOURCE_KEYS.get("driver_cores"), DEFAULT_DRIVER_CORES  # type: ignore
                 ),
                 executor_memory=spark_conf.get(
-                    SPARK_RESOURCE_KEYS.get("executor_memory"),
+                    SPARK_RESOURCE_KEYS.get("executor_memory"),  # type: ignore
                     DEFAULT_EXECUTOR_MEMORY,
                 ),
                 executor_cores=spark_conf.get(
-                    SPARK_RESOURCE_KEYS.get("executor_cores"),
+                    SPARK_RESOURCE_KEYS.get("executor_cores"),  # type: ignore
                     DEFAULT_EXECUTOR_CORES,
                 ),
                 num_executors=spark_conf.get(
-                    SPARK_RESOURCE_KEYS.get("num_executors"), DEFAULT_NUM_EXECUTORS
+                    SPARK_RESOURCE_KEYS.get("num_executors"), DEFAULT_NUM_EXECUTORS  # type: ignore
                 ),
                 queue=queue,
                 session_name=generate_unique_session_name(setu_session_name),
                 spark_version=spark_version,
                 execution_tags=set_execution_tags_with_defaults(execution_tags),
                 spark_conf=set_spark_conf_with_defaults(spark_conf),
                 metadata=set_session_runtime_metadata(metadata),
@@ -173,15 +173,15 @@
                     verify,
                 )
 
     @classmethod
     def close_session(
         cls,
         url: str,
-        auth: Auth = None,
+        auth: Optional[Auth] = None,
         verify: Verify = False,
     ):
         """Close the managed SETU session."""
         logger.info(f"Trying to close session for : {cls.session_id}")
         if cls.session_id is None:
             logger.info("No setu session active")
             return
@@ -208,15 +208,15 @@
                 client.close()
 
     @classmethod
     def get_session_if_active(
         cls,
         url: str,
         session_id: str,
-        auth: Auth = None,
+        auth: Optional[Auth] = None,
         verify: Verify = False,
     ):
         """get SETU session if still active."""
         with SetuClient(url, auth, verify) as client:
             session = client.get_session(session_id)
         if session is not None:
             return SetuSession(url, session.session_id, auth, verify)
@@ -263,27 +263,27 @@
                 client.cancel_session(persisted_session_details.session_id)
             return None
 
         return persisted_session_details
 
     @classmethod
     def persist_session(
-        cls, session_initialization_config: SessionInitializationConfig, url: str = None
+        cls, session_initialization_config: SessionInitializationConfig, url: Optional[str] = None
     ):
         """return persisted setu session if present."""
 
         # if platform is not supported, return
         if not platform_supports_setu_session_reuse():
             return
 
         # persist session details for next run
         session_details_file_path = get_session_details_file_path()
         SessionDetails(
-            session_id=cls.session_id,
-            url=url,
+            session_id=cls.session_id,  # type: ignore
+            url=url,  # type: ignore
             session_initialization_config=session_initialization_config,
         ).persist(session_details_file_path)
 
 
 class SetuCluster:
     """get setu cluster information from in-dbt"""
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.5.2/dbt/adapters/setu/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,16 @@
     for key in list(spark_conf):
         if key.startswith("conf."):
             new_key = key.replace("conf.", "", 1)
             spark_conf[new_key] = spark_conf.pop(key)
 
     for key in DEFAULT_SPARK_CONF.keys():
         if key in SPARK_CONF_APPEND_KEYS and key in spark_conf:
-            user_config = spark_conf[key].split(",")
-            default_config = DEFAULT_SPARK_CONF[key].split(",")
+            user_config = str(spark_conf[key]).split(",")
+            default_config = str(DEFAULT_SPARK_CONF[key]).split(",")
             user_config.extend(default_config)
             spark_conf[key] = ",".join(user_config)
         else:
             spark_conf.setdefault(key, DEFAULT_SPARK_CONF[key])
     return spark_conf
 
 
@@ -180,15 +180,15 @@
         return False
     if platform not in Platform.get_platforms_supporting_session_reuse():
         return False
     return True
 
 
 def polling_intervals(
-    start: Iterable[float], rest: float, max_duration: float = None
+    start: Iterable[float], rest: float, max_duration: Optional[float] = None
 ) -> Iterator[float]:
     def _intervals():
         yield from start
         while True:
             yield rest
 
     cumulative = 0.0
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/__init__.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/column.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,29 @@
     SETU = "setu"  # OSS Apache Livy offering @ LinkedIn
 
 
 @dataclass
 class SparkCredentials(Credentials):
     method: SparkConnectionMethod = SparkConnectionMethod.SETU
     host: Optional[str] = None
-    database: Optional[str] = None
+    database: Optional[str] = None  # type: ignore
     driver: Optional[str] = None
     cluster: Optional[str] = None
     endpoint: Optional[str] = None
     token: Optional[str] = None
     user: Optional[str] = None
     password: Optional[str] = None
     port: int = 443
     auth: Optional[str] = None
     kerberos_service_name: Optional[str] = None
 
     #  **********   setu specific configs   **********
     url: Optional[str] = None
     session_name: Optional[str] = None
-    schema: Optional[str] = None
+    schema: Optional[str] = None  # type: ignore
     queue: Optional[str] = None
     proxy_user: Optional[str] = None
     jars: Optional[List[str]] = None
     py_files: Optional[List[str]] = None
     archives: Optional[List[str]] = None
     files: Optional[List[str]] = None
     manifest_file_location: Optional[str] = None
@@ -174,15 +174,19 @@
     @property
     def type(self):
         return "spark"
 
     @property
     def unique_field(self):
         if self.method == SparkConnectionMethod.SETU:
-            return self.url
+            if not self.cluster:
+                raise dbt.exceptions.DbtRuntimeError(
+                    "`cluster` must be set when using the Setu method to connect to Spark"
+                )
+            return self.cluster
         else:
             return self.host
 
     def _connection_keys(self):
         if self.method == SparkConnectionMethod.SETU:
             return ("url", "schema", "session_name")
         else:
@@ -566,15 +570,15 @@
                         f"set to true.\n\tRetrying in "
                         f"{creds.connect_timeout} seconds "
                         f"({i} of {creds.connect_retries})"
                     )
                     logger.warning(msg)
                     time.sleep(creds.connect_timeout)
                 else:
-                    raise dbt.exceptions.FailedToConnectException(
+                    raise dbt.exceptions.FailedToConnectError(
                         "Failed to connect with error: {}".format(str(e))
                     ) from e
         else:
             raise exc
 
         connection.handle = handle
         connection.state = ConnectionState.OPEN
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 import re
 from concurrent.futures import Future
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Union, Type, Tuple, Callable
+from typing import (
+    Any,
+    Dict,
+    DefaultDict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Union,
+    Type,
+    Tuple,
+    Callable,
+    Set,
+)
 from typing_extensions import TypeAlias
 from dbt.contracts.graph.manifest import Manifest
 
 import agate
 from agate import Table
 
 from dbt.contracts.relation import RelationType
 
 import dbt
 import dbt.exceptions
 
 from dbt.adapters.base import AdapterConfig, PythonJobHelper
 from dbt.adapters.base.impl import catch_as_completed
+from dbt.events.functions import fire_event
+from dbt.events.types import ListRelations
+from dbt.adapters.cache import _make_ref_key_dict
 from dbt.contracts.connection import AdapterResponse
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.spark import SparkConnectionManager
 from dbt.adapters.spark import SparkRelation
 from dbt.adapters.spark import SparkColumn
+from dbt.adapters.spark.spark_utils import is_openhouse
 from dbt.adapters.spark.python_submissions import (
     JobClusterPythonJobHelper,
     AllPurposeClusterPythonJobHelper,
 )
 from dbt.adapters.base import BaseRelation, available
 from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt.events import AdapterLogger
 from dbt.flags import get_flags
-from dbt.utils import executor, AttrDict
+from dbt.utils import executor, AttrDict, cast_to_str
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
 
 logger = AdapterLogger("Spark")
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
 LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
@@ -67,15 +84,15 @@
     def parse(cls, partition_by) -> Optional["PartitionConfig"]:
         if partition_by is None:
             return None
         try:
             cls.validate(partition_by)
             return cls.from_dict(partition_by)
         except ValidationError as exc:
-            raise dbt.exceptions.ValidationException("Could not parse partition config") from exc
+            raise dbt.exceptions.DbtConfigError("Could not parse partition config") from exc
         except TypeError:
             raise dbt.exceptions.CompilationError(
                 f"Invalid partition_by config:\n"
                 f"  Got: {partition_by}\n"
                 f'  Expected a dictionary with "field" and "data_type" keys'
             )
 
@@ -177,32 +194,30 @@
         try:
             _schema, name, _, information = row
         except ValueError:
             raise dbt.exceptions.DbtRuntimeError(
                 f'Invalid value from "show tables extended ...", got {len(row)} values, expected 4'
             )
 
-        return schema_relation.database, _schema, name, information
+        return schema_relation.database, _schema, name, information  # type: ignore
 
     def _get_relation_information_using_describe(
         self, schema_relation: BaseRelation, row: agate.Row
     ) -> RelationInfo:
         """Relation info fetched using SHOW TABLES and an auxiliary DESCRIBE statement"""
         try:
             _schema, name = row
         except ValueError:
             raise dbt.exceptions.DbtRuntimeError(
                 f'Invalid value from "show tables ...", got {len(row)} values, expected 2'
             )
 
-        is_openhouse = schema_relation.database == "openhouse" or "." in schema_relation.schema
-
         # database is needed where relations can exist in different catalogs
         table_name = f"{_schema}.{name}"
-        if is_openhouse:
+        if is_openhouse(schema_relation.database, schema_relation.schema):
             if not table_name.startswith("openhouse."):
                 table_name = "openhouse." + table_name
             _schema = "openhouse." + _schema
 
         try:
             table_results = self.execute_macro(
                 DESCRIBE_TABLE_EXTENDED_MACRO_NAME, kwargs={"table_name": table_name}
@@ -213,15 +228,42 @@
 
         information = ""
         for info_row in table_results:
             info_type, info_value, _ = info_row
             if not info_type.startswith("#"):
                 information += f"{info_type}: {info_value}\n"
 
-        return schema_relation.database, _schema, name, information
+        return schema_relation.database, _schema, name, information  # type: ignore
+
+    def _get_relation_map(
+        self, manifest: Manifest
+    ) -> DefaultDict[Optional[str], List[SparkRelation]]:
+        """Relations compiled together based on schema"""
+        relations = [
+            self.Relation.create_from(self.config, node)  # keep the identifier
+            for node in manifest.nodes.values()
+            if (node.is_relational and not node.is_ephemeral_model)
+        ]
+        sources = [
+            self.Relation.create_from(self.config, node)  # keep the identifier
+            for node in manifest.sources.values()
+        ]
+
+        import collections
+
+        relation_map = collections.defaultdict(list)
+        for r in relations:
+            relation_map[r.schema].append(r)
+        for s in sources:
+            if s.database == "openhouse" and "." not in str(s.schema):
+                relation_map[f"{s.database}.{s.schema}"].append(s)
+            else:
+                relation_map[s.schema].append(s)
+
+        return relation_map
 
     def _build_spark_relation_list(
         self,
         schema_relation: BaseRelation,
         row_list: agate.Table,
         relation_info_func: Callable[[BaseRelation, agate.Row], RelationInfo],
     ) -> List[BaseRelation]:
@@ -235,15 +277,15 @@
             )
             is_delta: bool = "Provider: delta" in information
             is_hudi: bool = "Provider: hudi" in information
             is_iceberg: bool = "Provider: iceberg" in information
             is_openhouse: bool = "Provider: openhouse" in information
 
             relation: BaseRelation = self.Relation.create(  # type: ignore
-                database=database if database else None,
+                database=database if database and not _schema.startswith("openhouse.") else None,
                 schema=_schema,
                 identifier=name,
                 type=rel_type,
                 information=information,
                 is_delta=is_delta,
                 is_iceberg=is_iceberg,
                 is_hudi=is_hudi,
@@ -255,18 +297,16 @@
 
     def list_relations_without_caching(self, schema_relation: BaseRelation) -> List[BaseRelation]:
         """Distinct Spark compute engines may not support the same SQL featureset. Thus, we must
         try different methods to fetch relation information."""
 
         kwargs = {"schema_relation": schema_relation}
 
-        is_openhouse = schema_relation.database == "openhouse" or "." in schema_relation.schema
-
         try:
-            if is_openhouse:
+            if is_openhouse(schema_relation.database, schema_relation.schema):
                 # Iceberg behavior: 3-row result of relations obtained
                 show_table_rows = self.execute_macro(
                     LIST_RELATIONS_SHOW_TABLES_MACRO_NAME, kwargs=kwargs
                 )
                 return self._build_spark_relation_list(
                     schema_relation=schema_relation,
                     row_list=show_table_rows,
@@ -311,15 +351,15 @@
                 )
                 return []
 
     def get_relation(self, database: str, schema: str, identifier: str) -> Optional[BaseRelation]:
         if not self.Relation.get_default_include_policy().database:
             database = None  # type: ignore
         else:
-            database = database if database else None
+            database = database if database else None  # type: ignore
 
         return super().get_relation(database, schema, identifier)
 
     def parse_describe_extended(
         self, relation: BaseRelation, raw_rows: AttrDict
     ) -> List[SparkColumn]:
         # Convert the Row to a dict
@@ -404,14 +444,34 @@
                 column=column_name,
                 dtype=column_type,
                 table_stats=table_stats,
             )
             columns.append(column)
         return columns
 
+    # overriding this method to optimize the performance of list_relations_without_caching
+    def _get_cache_schemas(self, manifest: Manifest) -> Set[BaseRelation]:
+        """Get the set of schema relations that the cache logic needs to
+        populate. This means only executable nodes are included.
+        """
+        relation_map = self._get_relation_map(manifest)
+
+        schemas = [
+            self.Relation.create(
+                schema=schema,
+                identifier=(
+                    "|".join(r.identifier for r in relations if r.identifier)
+                    if len(relations) < 100
+                    else "*"
+                ),
+            )
+            for schema, relations in relation_map.items()
+        ]
+        return set(schemas)
+
     def _get_columns_for_catalog(self, relation: BaseRelation) -> Iterable[Dict[str, Any]]:
         columns = self.parse_columns_from_information(relation)
 
         if not columns:
             # Columns are empty for openhouse, since it's trying to parse using spark logic
             logger.info(
                 "parse_columns_from_information doesn't return any columns, format may be openhouse"
@@ -465,16 +525,18 @@
             raise dbt.exceptions.CompilationError(
                 f"Expected only one schema in spark _get_one_catalog, found " f"{schemas}"
             )
 
         database = information_schema.database
         schema = list(schemas)[0]
 
+        relation_map = self._get_relation_map(manifest)
+
         columns: List[Dict[str, Any]] = []
-        for relation in self.list_relations(database, schema):
+        for relation in self.list_relations(database, schema, relation_map=relation_map):
             logger.debug("Getting table schema for relation {}", str(relation))
             columns.extend(self._get_columns_for_catalog(relation))
         return agate.Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
 
     def list_schemas(self, database: str) -> List[str]:
         connection = self.connections.get_if_exists()
         if connection is not None:
@@ -490,14 +552,58 @@
 
         # The catalog for `show table extended` needs to match the current catalog.
         with self._catalog(database):
             results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": schema})
         schema_list = [row[0] for row in results]
         return schema_list
 
+    def list_relations(self, database: Optional[str], schema: str, **kwargs) -> List[BaseRelation]:
+        if self._schema_is_cached(database, schema):
+            return self.cache.get_relations(database, schema)
+
+        relation_map = kwargs.get("relation_map", None)
+
+        if relation_map:
+            if database == "openhouse" and "." not in schema:
+                schema = f"{database}.{schema}"
+
+        schema_relation = self.Relation.create(
+            database=database,
+            schema=schema,
+            identifier="|".join(r.identifier for r in relation_map[schema])
+            if relation_map
+            else "",
+            quote_policy=self.config.quoting,
+        )
+
+        # we can't build the relations cache because we don't have a
+        # manifest so we can't run any operations.
+        relations = self.list_relations_without_caching(schema_relation)
+
+        # if the cache is already populated, add this schema in
+        # otherwise, skip updating the cache and just ignore
+        if self.cache:
+            for relation in relations:
+                self.cache.add(relation)
+            if not relations:
+                # it's possible that there were no relations in some schemas. We want
+                # to insert the schemas we query into the cache's `.schemas` attribute
+                # so we can check it later
+                self.cache.update_schemas([(database, schema)])
+
+        fire_event(
+            ListRelations(
+                database=cast_to_str(database),
+                schema=schema,
+                relations=[_make_ref_key_dict(x) for x in relations],
+            )
+        )
+
+        return relations
+
     def check_schema_exists(self, database, schema):
         # in case the user is using "openhouse" as a catalog, the format of schema will be 'openhouse.db'.
         # so derive the catalog/database value from schema until we support `openhouse` catalog natively.
         if schema is not None and "." in schema:
             tokens = schema.split(".")
             database = tokens[0]
             schema = tokens[1]
```

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/python_submissions.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/adapters/spark/session.py` & `in-dbt-spark-1.5.2/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/adapters.sql`

 * *Files 19% similar despite different names*

```diff
@@ -75,14 +75,39 @@
     {% endif %}
   {%- elif raw_persist_docs -%}
     {{ exceptions.raise_compiler_error("Invalid value provided for 'persist_docs'. Expected dict but got value: " ~ raw_persist_docs) }}
   {% endif %}
 {%- endmacro -%}
 
 
+{% macro set_dbt_tblproperties(relation, model) %}
+  {{ return(adapter.dispatch('set_dbt_tblproperties', 'dbt')(relation, model)) }}
+{%- endmacro -%}
+
+{% macro spark__set_dbt_tblproperties(relation, model) %}
+  {%- set mp_name = var('MULTIPRODUCT_NAME', None) -%}
+  {%- set project_name = model.package_name -%}
+  {%- set model_name = model.name -%}
+
+  {% if target.name == 'prod' and config.get('file_format', 'openhouse') == 'openhouse' %}
+    {% set set_tblproperties_query %}
+        {% if mp_name is not none %}
+            alter table {{ relation }} set tblproperties ('dbt.mp_name'='{{ mp_name }}',
+                                                            'dbt.project_name'='{{ project_name }}',
+                                                            'dbt.model_name'='{{ model_name }}');
+        {% else %}
+            alter table {{ relation }} set tblproperties ('dbt.project_name'='{{ project_name }}',
+                                                            'dbt.model_name'='{{ model_name }}');
+        {% endif %}
+    {% endset %}
+    {% do run_query(set_tblproperties_query) %}
+  {% endif %}
+{% endmacro %}
+
+
 {% macro partition_cols(label, required=false) %}
   {{ return(adapter.dispatch('partition_cols', 'dbt')(label, required)) }}
 {%- endmacro -%}
 
 {% macro spark__partition_cols(label, required=false) %}
   {%- set raw_partition_by = config.get('partition_by', validator=validation.any[list, dict]) -%}
   {%- set file_format = config.get('file_format', validator=validation.any[basestring]) -%}
@@ -297,15 +322,15 @@
 {% endmacro %}
 
 {% macro list_relations_show_tables_without_caching(schema_relation) %}
   {#-- Spark with iceberg tables don't work with show table extended for #}
   {#-- V2 iceberg tables #}
   {#-- https://issues.apache.org/jira/browse/SPARK-33393 #}
   {% call statement('list_relations_without_caching_show_tables', fetch_result=True) -%}
-    show tables in {{ schema_relation }} like '*'
+    show tables in {{ schema_relation.schema }} like '{{ schema_relation.identifier or "*" }}'
   {% endcall %}
 
   {% do return(load_result('list_relations_without_caching_show_tables').table) %}
 {% endmacro %}
 
 {% macro describe_table_extended_without_caching(table_name) %}
   {#-- Spark with iceberg tables don't work with show table extended for #}
@@ -449,7 +474,88 @@
             {% endfor %}
 
   {%- endset -%}
 
   {% do run_query(sql) %}
 
 {% endmacro %}
+
+{% macro spark__get_binding_char() %}
+  {{ return('?' if target.method == 'odbc' else '%s') }}
+{% endmacro %}
+
+
+{% macro spark__reset_csv_table(model, full_refresh, old_relation, agate_table) %}
+    {% if old_relation %}
+        {{ adapter.drop_relation(old_relation) }}
+    {% endif %}
+    {% set sql = create_csv_table(model, agate_table) %}
+    {{ return(sql) }}
+{% endmacro %}
+
+
+{% macro spark__load_csv_rows(model, agate_table) %}
+
+  {% set batch_size = get_batch_size() %}
+  {% set column_override = model['config'].get('column_types', {}) %}
+
+  {% set statements = [] %}
+
+  {% for chunk in agate_table.rows | batch(batch_size) %}
+      {% set bindings = [] %}
+
+      {% for row in chunk %}
+          {% do bindings.extend(row) %}
+      {% endfor %}
+
+      {% set sql %}
+          insert into {{ this.render() }} values
+          {% for row in chunk -%}
+              ({%- for col_name in agate_table.column_names -%}
+                  {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
+                  {%- set type = column_override.get(col_name, inferred_type) -%}
+                    {# todo- https://jira01.corp.linkedin.com:8443/browse/DATAFND-660 #}
+                    cast('{{ row.get(col_name) if row.get(col_name) is not none else null }}' as {{type}})
+                  {%- if not loop.last%},{%- endif %}
+              {%- endfor -%})
+              {%- if not loop.last%},{%- endif %}
+          {%- endfor %}
+      {% endset %}
+
+      {% do adapter.add_query(sql, bindings=bindings, abridge_sql_log=True) %}
+
+      {% if loop.index0 == 0 %}
+          {% do statements.append(sql) %}
+      {% endif %}
+  {% endfor %}
+
+  {# Return SQL so we can render it out into the compiled files #}
+  {{ return(statements[0]) }}
+{% endmacro %}
+
+
+{% macro spark__create_csv_table(model, agate_table) %}
+  {%- set column_override = model['config'].get('column_types', {}) -%}
+  {%- set quote_seed_column = model['config'].get('quote_columns', None) -%}
+
+  {% set sql %}
+    create table {{ this.render() }} (
+        {%- for col_name in agate_table.column_names -%}
+            {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
+            {%- set type = column_override.get(col_name, inferred_type) -%}
+            {%- set column_name = (col_name | string) -%}
+            {{ adapter.quote_seed_column(column_name, quote_seed_column) }} {{ type }} {%- if not loop.last -%}, {%- endif -%}
+        {%- endfor -%}
+    )
+    {{ file_format_clause() }}
+    {{ partition_cols(label="partitioned by") }}
+    {{ clustered_cols(label="clustered by") }}
+    {{ location_clause() }}
+    {{ comment_clause() }}
+  {% endset %}
+
+  {% call statement('_') -%}
+    {{ sql }}
+  {%- endcall %}
+
+  {{ return(sql) }}
+{% endmacro %}
```

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files 4% similar despite different names*

```diff
@@ -86,13 +86,14 @@
     {%- endif -%}
   {%- endif -%}
 
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
   {% do apply_retention(target_relation, retention) %}
   {% do persist_docs(target_relation, model) %}
+  {% do set_dbt_tblproperties(target_relation, model) %}
 
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files 0% similar despite different names*

```diff
@@ -252,14 +252,15 @@
       {{ final_sql }}
   {% endcall %}
 
   {% set should_revoke = should_revoke(target_relation_exists, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
+  {% do set_dbt_tblproperties(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {{ adapter.commit() }}
 
   {% if staging_table is defined %}
       {% do post_snapshot(staging_table) %}
```

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/table.sql`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     {{ create_table_as(False, target_relation, compiled_code, language) }}
   {%- endcall -%}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
   {% do apply_retention(target_relation, retention) %}
   {% do persist_docs(target_relation, model) %}
+  {% do set_dbt_tblproperties(target_relation, model) %}
 
   {% do persist_constraints(target_relation, model) %}
 
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]})}}
```

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/materializations/validate.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.5.2/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.5.2/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.5.2/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.5.0
+Version: 1.5.2
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: ODBC
 Provides-Extra: PyHive
 Provides-Extra: session
 Provides-Extra: all
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.0 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.2 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: ODBC
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra: ODBC
 Provides-Extra: PyHive Provides-Extra: session Provides-Extra: all
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
```

### Comparing `in-dbt-spark-1.5.0/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.5.2/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.0/setup.py` & `in-dbt-spark-1.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 import os
 import sys
 import re
 
 # require python 3.7 or newer
-if sys.version_info < (3, 7):
+if sys.version_info < (3, 10):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.10 or higher.")
     sys.exit(1)
 
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.5.0"
+package_version = "1.5.2"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
@@ -87,14 +87,11 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.10",
 )
```

