# Comparing `tmp/rondsspark-0.0.4.6.tar.gz` & `tmp/rondsspark-0.0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rondsspark-0.0.4.6.tar", last modified: Thu Jul  6 12:00:26 2023, max compression
+gzip compressed data, was "dist/rondsspark-0.0.4.7.tar", last modified: Tue Jul 11 05:56:12 2023, max compression
```

## Comparing `rondsspark-0.0.4.6.tar` & `rondsspark-0.0.4.7.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/
--rw-rw-rw-   0        0        0      220 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/rondsspark.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/rondsspark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/rondsspark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/rondsspark.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1502 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/rondsspark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/rondsspark.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/dataframe/
--rw-rw-rw-   0        0        0     4377 2023-06-26 08:10:36.000000 rondsspark-0.0.4.6/ronds_sdk/dataframe/pvalue.py
--rw-rw-rw-   0        0        0        0 2023-06-08 01:43:15.000000 rondsspark-0.0.4.6/ronds_sdk/dataframe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/datasources/
--rw-rw-rw-   0        0        0     3296 2023-07-06 11:55:04.000000 rondsspark-0.0.4.6/ronds_sdk/datasources/cassandra_manager.py
--rw-rw-rw-   0        0        0        0 2023-06-27 13:38:08.000000 rondsspark-0.0.4.6/ronds_sdk/datasources/__init__.py
--rw-rw-rw-   0        0        0      792 2023-06-08 13:00:10.000000 rondsspark-0.0.4.6/ronds_sdk/error.py
--rw-rw-rw-   0        0        0      267 2023-07-05 12:51:09.000000 rondsspark-0.0.4.6/ronds_sdk/logger_config.py
--rw-rw-rw-   0        0        0      531 2023-06-07 03:32:55.000000 rondsspark-0.0.4.6/ronds_sdk/logging_config.yml
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/ml/
--rw-rw-rw-   0        0        0        0 2023-06-07 06:10:31.000000 rondsspark-0.0.4.6/ronds_sdk/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/options/
--rw-rw-rw-   0        0        0     7492 2023-07-06 08:25:07.000000 rondsspark-0.0.4.6/ronds_sdk/options/pipeline_options.py
--rw-rw-rw-   0        0        0     6424 2023-06-09 11:16:10.000000 rondsspark-0.0.4.6/ronds_sdk/options/value_provider.py
--rw-rw-rw-   0        0        0        0 2023-06-08 03:30:12.000000 rondsspark-0.0.4.6/ronds_sdk/options/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-07-03 10:06:11.000000 rondsspark-0.0.4.6/ronds_sdk/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/runners/
--rw-rw-rw-   0        0        0        0 2023-06-08 09:17:22.000000 rondsspark-0.0.4.6/ronds_sdk/runners/pipeline_context.py
--rw-rw-rw-   0        0        0      538 2023-07-04 02:31:48.000000 rondsspark-0.0.4.6/ronds_sdk/runners/python_runner.py
--rw-rw-rw-   0        0        0     2953 2023-06-29 09:56:08.000000 rondsspark-0.0.4.6/ronds_sdk/runners/runner.py
--rw-rw-rw-   0        0        0     2772 2023-07-06 08:28:02.000000 rondsspark-0.0.4.6/ronds_sdk/runners/spark_runner.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/runners/visitors/
--rw-rw-rw-   0        0        0     3858 2023-07-06 08:30:51.000000 rondsspark-0.0.4.6/ronds_sdk/runners/visitors/spark_runner_visitor.py
--rw-rw-rw-   0        0        0        0 2023-06-29 09:25:38.000000 rondsspark-0.0.4.6/ronds_sdk/runners/visitors/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:10:46.000000 rondsspark-0.0.4.6/ronds_sdk/runners/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/tools/
--rw-rw-rw-   0        0        0     1416 2023-07-06 02:14:39.000000 rondsspark-0.0.4.6/ronds_sdk/tools/utils.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:11:02.000000 rondsspark-0.0.4.6/ronds_sdk/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/
--rw-rw-rw-   0        0        0       73 2023-06-08 13:20:13.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/core.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/
--rw-rw-rw-   0        0        0     6484 2023-07-06 11:58:58.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/cassandra_rule.py
--rw-rw-rw-   0        0        0     4868 2023-06-30 11:12:05.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/rule_merge_data.py
--rw-rw-rw-   0        0        0     6126 2023-07-06 07:24:05.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/transforms.py
--rw-rw-rw-   0        0        0        0 2023-06-30 02:11:50.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/__init__.py
--rw-rw-rw-   0        0        0     7460 2023-07-03 06:11:22.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/ptransform.py
--rw-rw-rw-   0        0        0      530 2023-06-29 12:12:57.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/remote_debug.py
--rw-rw-rw-   0        0        0     5253 2023-07-06 07:02:37.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/ronds.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/spark/
--rw-rw-rw-   0        0        0     4755 2023-07-06 07:03:56.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/spark/transforms.py
--rw-rw-rw-   0        0        0        0 2023-06-30 02:11:59.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/spark/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-08 01:41:33.000000 rondsspark-0.0.4.6/ronds_sdk/transforms/__init__.py
--rw-rw-rw-   0        0        0      855 2023-07-04 10:53:54.000000 rondsspark-0.0.4.6/ronds_sdk/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-07-06 11:59:48.000000 rondsspark-0.0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/test/
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/test/sdk/
--rw-rw-rw-   0        0        0     3598 2023-07-04 07:02:09.000000 rondsspark-0.0.4.6/test/sdk/sdk_test.py
--rw-rw-rw-   0        0        0     3130 2023-07-04 06:44:02.000000 rondsspark-0.0.4.6/test/sdk/sdk_unitest.py
--rw-rw-rw-   0        0        0        0 2023-06-13 06:59:02.000000 rondsspark-0.0.4.6/test/sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/test/simple/
--rw-rw-rw-   0        0        0      949 2023-06-09 13:10:50.000000 rondsspark-0.0.4.6/test/simple/overloading_test.py
--rw-rw-rw-   0        0        0        0 2023-06-09 13:04:55.000000 rondsspark-0.0.4.6/test/simple/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:26.000000 rondsspark-0.0.4.6/test/spark/
--rw-rw-rw-   0        0        0      522 2023-06-07 07:41:05.000000 rondsspark-0.0.4.6/test/spark/SimpleTest.py
--rw-rw-rw-   0        0        0     2830 2023-06-19 11:56:18.000000 rondsspark-0.0.4.6/test/spark/SparkTest.py
--rw-rw-rw-   0        0        0        0 2023-06-07 03:03:37.000000 rondsspark-0.0.4.6/test/spark/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-07 03:06:08.000000 rondsspark-0.0.4.6/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/tools/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/spark/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/spark/transforms.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/core.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/remote_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/
+-rw-r--r--   0 root         (0) root         (0)     6620 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/cassandra_rule.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/transforms.py
+-rw-r--r--   0 root         (0) root         (0)     4742 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/rule_merge_data.py
+-rw-r--r--   0 root         (0) root         (0)     6452 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/ronds.py
+-rw-r--r--   0 root         (0) root         (0)     8334 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/ptransform.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/logger_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/runners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/runners/visitors/
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/runners/visitors/spark_runner_visitor.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/visitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/runner.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/python_runner.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/pipeline_context.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/runners/spark_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/templates/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/templates/phm_rules_editor.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/dataframe/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/dataframe/pvalue.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/logging_config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/options/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/options/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/options/value_provider.py
+-rw-r--r--   0 root         (0) root         (0)     7532 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/options/pipeline_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/ml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/ml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/cassandra_manager.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/kafka_manager.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-11 05:36:08.000000 rondsspark-0.0.4.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/sdk/
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/sdk/sdk_test.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/test/sdk/sdk_unitest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/simple/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/simple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/simple/overloading_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/spark/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/spark/SparkTest.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/spark/SimpleTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/__init__.py
```

### Comparing `rondsspark-0.0.4.6/rondsspark.egg-info/SOURCES.txt` & `rondsspark-0.0.4.7/rondsspark.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 ronds_sdk/logger_config.py
 ronds_sdk/logging_config.yml
 ronds_sdk/pipeline.py
 ronds_sdk/dataframe/__init__.py
 ronds_sdk/dataframe/pvalue.py
 ronds_sdk/datasources/__init__.py
 ronds_sdk/datasources/cassandra_manager.py
+ronds_sdk/datasources/kafka_manager.py
 ronds_sdk/ml/__init__.py
 ronds_sdk/options/__init__.py
 ronds_sdk/options/pipeline_options.py
 ronds_sdk/options/value_provider.py
 ronds_sdk/runners/__init__.py
 ronds_sdk/runners/pipeline_context.py
 ronds_sdk/runners/python_runner.py
 ronds_sdk/runners/runner.py
 ronds_sdk/runners/spark_runner.py
 ronds_sdk/runners/visitors/__init__.py
 ronds_sdk/runners/visitors/spark_runner_visitor.py
+ronds_sdk/templates/__init__.py
+ronds_sdk/templates/phm_rules_editor.py
 ronds_sdk/tools/__init__.py
+ronds_sdk/tools/schedule.py
 ronds_sdk/tools/utils.py
 ronds_sdk/transforms/__init__.py
 ronds_sdk/transforms/core.py
 ronds_sdk/transforms/ptransform.py
 ronds_sdk/transforms/remote_debug.py
 ronds_sdk/transforms/ronds.py
 ronds_sdk/transforms/pandas/__init__.py
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/dataframe/pvalue.py` & `rondsspark-0.0.4.7/ronds_sdk/transforms/spark/transforms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,179 +1,134 @@
-from typing import TypeVar, Generic, Optional, Union
-
-from ronds_sdk.transforms.core import Windowing
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from ronds_sdk.pipeline import Pipeline, PipelineVisitor
-    from ronds_sdk.pipeline import AppliedPTransform
-
-T = TypeVar('T')
-
-
-class PValue(object):
-    """
-    Base class for PCollection.
-    主要特征:
-        (1) 属于一个 Pipeline, 初始化时加入
-        (2) 拥有一个 Transform 用来计算 value
-        (3) 拥有一个 value, 如果 Transform执行后,该值拥有意义
-    """
-
-    def __init__(self,
-                 pipeline,  # type: Pipeline
-                 tag=None,  # type: Optional[str]
-                 element_value=None,  # type: T
-                 element_type=None,  # type: Optional[Union[type]],
-                 windowing=None,  # type: Optional[Windowing]
-                 is_bounded=True,
-                 ):
-        self.pipeline = pipeline
-        self.tag = tag
-        self.element_value = element_value
-        self.element_type = element_type
-        # The AppliedPTransform instance for the application of the PTransform
-        # generating this PValue. The field gets initialized when a transform
-        # gets applied.
-        self.producer = None  # type: Optional[AppliedPTransform]
-        self.consumers = list()  # type: list[AppliedPTransform]
-        self.is_bounded = is_bounded
-        if windowing:
-            self._windowing = windowing
-        self.requires_deterministic_key_coder = None
-
-    def __str__(self):
-        return self._str_internal()
-
-    def __repr__(self):
-        return '<%s at %s>' % (self._str_internal(), hex(id(self)))
-
-    def _str_internal(self) -> str:
-        return "%s[%s.%s]" % (
-            self.__class__.__name__,
-            self.producer.full_label if self.producer else None,
-            self.tag
-        )
-
-    def apply(self, *args, **kwargs):
-        """Applies a transform or callable to a PValue"""
-        arg_list = list(args)
-        arg_list.insert(1, self)
-        return self.pipeline.apply(*arg_list, **kwargs)
-
-    def visit(self,
-              visitor,  # type: PipelineVisitor
-              ):
-        # type: (...) -> bool
-        if visitor.visit_value(self) and self.consumers:
-            for consumer in self.consumers:
-                consumer.visit(visitor)
-            return True
-        return False
-
-    def add_consumer(self,
-                     consumer  # type: AppliedPTransform
-                     ):
-        self.consumers.append(consumer)
-
-
-class PCollection(PValue, Generic[T]):
-
-    def __init__(self,
-                 pipeline,  # type: Pipeline
-                 tag=None,  # type: Optional[str]
-                 element_value=None,  # type: T
-                 element_type=None,  # type: Optional[Union[type]],
-                 windowing=None,  # type: Optional[Windowing]
-                 is_bounded=True,
-                 ):
-        super(PCollection, self).__init__(pipeline, tag, element_value,
-                                          element_type, windowing, is_bounded)
-
-    def __eq__(self, other):
-        if isinstance(other, PCollection):
-            return self.tag == other.tag and self.producer == other.producer
-
-    def __hash__(self):
-        return hash((self.tag, self.producer))
-
-
-class AsSideInput(object):
-    def __init__(self, p_coll):
-        # type: (PCollection) -> None
-        self.pvalue = p_coll
-
-
-class PBegin(PValue):
-    """pipelines input 的 begin marker, 用于 create/read transforms"""
-    pass
-
-
-class PDone(PValue):
-    """
-    PDone 代表 transform 的 output,具有简单的结果, 例如 Write
-    """
-
-    def __init__(self,
-                 pipeline,  # type: Pipeline
-                 tag=None,  # type: Optional[str]
-                 element_type=None,  # type: Optional[Union[type]],
-                 windowing=None,  # type: Optional[Windowing]
-                 is_bounded=True,
-                 stream_writer=None,
-                 ):
-        super().__init__(pipeline, tag, element_type=element_type, windowing=windowing, is_bounded=is_bounded)
-        self.stream_writer = stream_writer
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+import logging
+import time
+
+from ronds_sdk import error
+from ronds_sdk.transforms.ptransform import PTransform, ForeachBatchTransform
+from ronds_sdk.dataframe import pvalue
+from ronds_sdk.runners.spark_runner import SparkRunner
+from pyspark.sql import DataFrame
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ronds_sdk.transforms import ronds
+
+
+class Sleep(PTransform):
+
+    def __init__(self,
+                 _sleep  # type: ronds.Sleep
+                 ):
+        super(Sleep, self).__init__()
+        self._sleep = _sleep
+
+    def expand(self, input_inputs, action_func=None):
+        logging.info("start sleep~")
+        time.sleep(self._sleep.seconds)
+        logging.info("end sleep~")
+        return input_inputs
+
+
+class Create(PTransform):
+    def __init__(self,
+                 create,  # type: ronds.Create
+                 ):
+        super(Create, self).__init__()
+        self.values = create.values
+
+    def expand(self, p_begin, action_func=None):
+        assert isinstance(p_begin, pvalue.PBegin)
+        df = get_spark(p_begin).createDataFrame(self.values)
+        return pvalue.PCollection(p_begin.pipeline,
+                                  element_value=df,
+                                  element_type=DataFrame,
+                                  is_bounded=True)
+
+
+class Socket(ForeachBatchTransform):
+    def __init__(self,
+                 socket,  # type: ronds.Socket
+                 ):
+        super(Socket, self).__init__()
+        self.host = socket.host
+        self.port = socket.port
+
+    def expand(self, p_begin, action_func=None):
+        assert isinstance(p_begin, pvalue.PBegin)
+        df = get_spark(p_begin).readStream \
+            .format("socket") \
+            .option("host", self.host) \
+            .option("port", self.port) \
+            .load()
+        if action_func:
+            writer = df.writeStream.foreachBatch(action_func.call)
+            return pvalue.PDone(p_begin.pipeline,
+                                element_type=DataFrame,
+                                is_bounded=False,
+                                stream_writer=writer)
+        return pvalue.PCollection(p_begin.pipeline,
+                                  element_type=DataFrame,
+                                  element_value=df,
+                                  is_bounded=False)
+
+
+class Filter(PTransform):
+    def __init__(self,
+                 filter_,  # type: ronds.Filter
+                 ):
+        super(Filter, self).__init__()
+        self.where = filter_.where
+        self.select_cols = filter_.select_cols
+
+    def expand(self, input_inputs, action_func=None):
+        assert isinstance(input_inputs, pvalue.PCollection)
+        if input_inputs.element_value:
+            df = input_inputs.element_value
+            assert isinstance(df, DataFrame)
+            new_df = df.select(self.select_cols).where(self.where)
+            return pvalue.PCollection(input_inputs.pipeline,
+                                      element_value=new_df,
+                                      element_type=DataFrame,
+                                      is_bounded=input_inputs.is_bounded)
+        raise error.PValueError(
+            "unexpected input_inputs.element_value: %s" % input_inputs.tag)
+
+
+class Console(PTransform):
+
+    def __init__(self,
+                 console,  # type: ronds.Console
+                 ):
+        super(Console, self).__init__('Console')
+        self.mode = console.mode
+
+    def expand(self, input_inputs, action_func=None):
+        assert isinstance(input_inputs, pvalue.PCollection)
+        df = input_inputs.element_value
+        assert isinstance(df, DataFrame)
+        if not df.isStreaming:
+            df.show()
+            return pvalue.PDone(input_inputs.pipeline,
+                                element_type=DataFrame,
+                                is_bounded=True)
+        else:
+            query = df.writeStream \
+                .outputMode(self.mode) \
+                .format("console")
+            return pvalue.PDone(input_inputs.pipeline,
+                                element_type=DataFrame,
+                                is_bounded=False,
+                                stream_writer=query)
+
+
+def get_spark(p_coll: pvalue.PValue):
+    """
+    从 runner 中 获取 SparkSession
+    :param p_coll: 数据集
+    :return: SparkSession
+    """
+    if p_coll:
+        runner = p_coll.pipeline.runner
+        if isinstance(runner, SparkRunner):
+            return runner.spark
+        raise TypeError("expect SparkRunner, but found %s " % runner)
+    else:
+        raise error.PValueError("get_spark, PValue is null!")
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/datasources/cassandra_manager.py` & `rondsspark-0.0.4.7/ronds_sdk/datasources/cassandra_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,86 @@
-import datetime
-import logging
-import uuid
-from typing import Sequence, List
-
-from cassandra.cluster import Cluster, Session, ResultSet
-from ronds_sdk.options.pipeline_options import CassandraOptions
-
-
-class Singleton(object):
-    def __init__(self, cls):
-        self._cls = cls
-        self._instance = {}
-
-    def __call__(self, *args, **kwargs):
-        if self._cls not in self._instance:
-            self._instance[self._cls] = self._cls(*args, **kwargs)
-        return self._instance[self._cls]
-
-
-@Singleton
-class CassandraManager(object):
-    """
-    Cassandra 数据库的操作类, 单例
-    连接到固定的一个 Cassandra 集群, 可以操作多个 keyspace
-    """
-
-    def __init__(self,
-                 options,  # type: CassandraOptions
-                 ):
-        self.cluster = Cluster(options.cassandra_host)
-        self.session_cache = dict()  # type: dict[str, Session]
-
-    def get_session(self, keyspace):
-        # type: (str) -> Session
-        if not self.session_cache.__contains__(keyspace):
-            self.session_cache[keyspace] = self.cluster.connect(keyspace)
-        return self.session_cache.get(keyspace)
-
-    def query(self, keyspace: str, sql: str, params: List[str]) -> ResultSet:
-        result = self.get_session(keyspace).execute(sql, params)
-        return result
-
-    def execute(self, keyspace: str, sql: str, params: List[str]) -> None:
-        self.get_session(keyspace).execute(sql, params)
-
-    def __del__(self):
-        try:
-            self.cluster.shutdown()
-            logging.info("cassandra cluster shutdown~")
-        except Exception as ex:
-            logging.error("CassandraManager cluster shutdown failed: %s" % ex)
-            raise ex
-
-
-class ProcessDataManager(object):
-    """
-    内置的操作工艺数据表的操作类
-    """
-
-    def __init__(self,
-                 options,  # type: CassandraOptions
-                 keyspace=None,  # type: str
-                 ):
-        self._options = options
-        self._table_name = options.cassandra_table_process  # type: str
-        self.cassandra_manager = CassandraManager(options)  # type: CassandraManager
-        if keyspace:
-            self.keyspace = keyspace
-        elif options.cassandra_keyspace:
-            self.keyspace = options.cassandra_keyspace
-
-    @property
-    def _get_session(self):
-        return self.cassandra_manager.get_session(self.keyspace)
-
-    @property
-    def _get_window_select_prepare(self):
-        return self._get_session.prepare("""SELECT id, time, value
-                                            FROM %s 
-                                            where id in ?
-                                            AND time >= ? 
-                                            AND time < ?""" % self._table_name)
-
-    def window_select(self,
-                      uid_list,  # type: Sequence[str],
-                      start_time,  # type: datetime.datetime
-                      end_time,  # type: datetime.datetime
-                      ):
-        # type:  (...) -> ResultSet
-        uuid_list = [uuid.UUID(uid) for uid in uid_list]
-        return self._get_session.execute(self._get_window_select_prepare, [uuid_list, start_time, end_time])
+import datetime
+import logging
+import uuid
+from typing import Sequence, List
+
+from cassandra.cluster import Cluster, Session, ResultSet
+from ronds_sdk.options.pipeline_options import CassandraOptions
+from ronds_sdk.tools.utils import Singleton
+
+
+class CassandraManager(metaclass=Singleton):
+    """
+    Cassandra 数据库的操作类, 单例
+    连接到固定的一个 Cassandra 集群, 可以操作多个 keyspace
+    """
+
+    def __init__(self,
+                 options,  # type: CassandraOptions
+                 ):
+        self.cluster = Cluster(options.cassandra_host)
+        self.session_cache = dict()  # type: dict[str, Session]
+
+    def get_session(self, keyspace):
+        # type: (str) -> Session
+        if not self.session_cache.__contains__(keyspace):
+            self.session_cache[keyspace] = self.cluster.connect(keyspace)
+        return self.session_cache.get(keyspace)
+
+    def query(self, keyspace: str, sql: str, params: List[str]) -> ResultSet:
+        result = self.get_session(keyspace).execute(sql, params)
+        return result
+
+    def execute(self, keyspace: str, sql: str, params: List[str]) -> None:
+        self.get_session(keyspace).execute(sql, params)
+
+    def __del__(self):
+        try:
+            self.cluster.shutdown()
+            logging.info("cassandra cluster shutdown~")
+        except Exception as ex:
+            logging.error("CassandraManager cluster shutdown failed: %s" % ex)
+            raise ex
+
+
+class ProcessDataManager(object):
+    """
+    内置的操作工艺数据表的操作类
+    """
+
+    def __init__(self,
+                 options,  # type: CassandraOptions
+                 keyspace=None,  # type: str
+                 ):
+        self._options = options
+        self._table_name = options.cassandra_table_process  # type: str
+        self.cassandra_manager = CassandraManager(options)  # type: CassandraManager
+        if keyspace:
+            self.keyspace = keyspace
+        elif options.cassandra_keyspace:
+            self.keyspace = options.cassandra_keyspace
+
+    @property
+    def _get_session(self):
+        return self.cassandra_manager.get_session(self.keyspace)
+
+    @property
+    def _get_window_select_prepare(self):
+        return self._get_session.prepare("""SELECT id, time, value
+                                            FROM %s 
+                                            where id in ?
+                                            AND time >= ? 
+                                            AND time < ?""" % self._table_name)
+
+    def window_select(self,
+                      uid_list,  # type: Sequence[str],
+                      start_time,  # type: datetime.datetime
+                      end_time,  # type: datetime.datetime
+                      ):
+        # type:  (...) -> ResultSet
+        try:
+            uuid_list = [uuid.UUID(uid) for uid in uid_list]
+            return self._get_session.execute(self._get_window_select_prepare, [uuid_list, start_time, end_time])
+        except Exception as ex:
+            logging.error('window_select failed, uid_list: %s, start_time: %s, end_time: %s, ex:\n %s' % (
+                str(uid_list), start_time, end_time, str(ex)))
+            raise ex
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/error.py` & `rondsspark-0.0.4.7/ronds_sdk/error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-
-"""Python Dataflow error class"""
-
-
-class RondsError(Exception):
-    """Base class for all Ronds errors"""
-
-
-class PipelineError(RondsError):
-    """An error in the pipeline object (e.g. a PValue not linked to it)."""
-
-
-class PValueError(RondsError):
-    """An error related to a PValue object (e.g. value is not computed)."""
-
-
-class RunnerError(RondsError):
-    """An error related to a Runner object (e.g. cannot find a runner to run)."""
-
-
-class RuntimeValueProviderError(RuntimeError):
-    """An error related to a ValueProvider object raised during runtime."""
-
-
-class SideInputError(RondsError):
-    """An error related to a side input to a parallel Do operation."""
-
-
-class TransformError(RondsError):
-    """An error related to a PTransform object."""
+
+"""Python Dataflow error class"""
+
+
+class RondsError(Exception):
+    """Base class for all Ronds errors"""
+
+
+class PipelineError(RondsError):
+    """An error in the pipeline object (e.g. a PValue not linked to it)."""
+
+
+class PValueError(RondsError):
+    """An error related to a PValue object (e.g. value is not computed)."""
+
+
+class RunnerError(RondsError):
+    """An error related to a Runner object (e.g. cannot find a runner to run)."""
+
+
+class RuntimeValueProviderError(RuntimeError):
+    """An error related to a ValueProvider object raised during runtime."""
+
+
+class SideInputError(RondsError):
+    """An error related to a side input to a parallel Do operation."""
+
+
+class TransformError(RondsError):
+    """An error related to a PTransform object."""
+
+
+class KafkaError(RondsError):
+    """An error related to a Kafka"""
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/options/pipeline_options.py` & `rondsspark-0.0.4.7/ronds_sdk/options/pipeline_options.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,229 +1,236 @@
-import argparse
-from typing import Optional, Any, List, Iterable, Type, TypeVar, NoReturn
-
-__all__ = [
-    'PipelineOptions',
-    'SparkRunnerOptions',
-    'CassandraOptions',
-    'AlgorithmOptions',
-    'KafkaOptions',
-]
-
-from ronds_sdk.options.value_provider import StaticValueProvider, RuntimeValueProvider
-
-PipelineOptionsT = TypeVar('PipelineOptionsT', bound='PipelineOptions')
-
-
-class PipelineOptions(object):
-
-    def __init__(self, flags=None, **kwargs):
-        # type: (Optional[List[str]], **Any) -> None
-        self._flags = flags
-
-        parser = _RondsArgumentParser()
-        for cls in type(self).mro():
-            if cls == PipelineOptions:
-                self.add_argparse_args(parser)
-                break
-            elif '_add_argparse_args' in cls.__dict__:
-                cls._add_argparse_args(parser)  # type: ignore
-
-        self._visible_options, _ = parser.parse_known_args(flags)
-
-        self._all_options = kwargs
-
-        for option_name in self._visible_option_list():
-            # Note that options specified in kwargs will not be overwritten
-            if option_name not in self._all_options:
-                self._all_options[option_name] = getattr(self._visible_options, option_name)
-
-    @classmethod
-    def add_argparse_args(cls, parser):
-        # type: (_RondsArgumentParser) -> None
-        # Override this in subclasses to provide options.
-        parser.add_argument(
-            '--transform_package',
-            default='ronds_sdk.transforms.spark.transforms',
-            help='运行任务时, 物理执行算子的 package 路径, runner 有默认值, 一般无需修改'
-        )
-        parser.add_argument(
-            '--enable_executor_debug',
-            default=False,
-            help='是否启用 Spark Executor 端的 DEBUG 功能, 仅用于测试'
-        )
-
-    def view_as(self, cls):
-        # type: (Type[PipelineOptionsT]) -> PipelineOptionsT
-        view: PipelineOptions = cls(self._flags)
-
-        for option_name in view._visible_option_list():  # type: ignore
-            if option_name not in self._all_options:
-                self._all_options[option_name] = getattr(
-                    view._visible_options, option_name)
-        view._all_options = self._all_options
-        return view
-
-    def _visible_option_list(self):
-        # type: () -> List[str]
-        return sorted(
-            option for option in dir(self._visible_options) if option[0] != '_'
-        )
-
-    def __dir__(self) -> Iterable[str]:
-        return sorted(
-            dir(type(self)) + list(self.__dict__) + self._visible_option_list()
-        )
-
-    def __getattr__(self, name):
-        if name[:2] == name[-2:] == '__':
-            return object.__getattribute__(self, name)
-        elif name in self._visible_option_list():
-            return self._all_options[name]
-        else:
-            raise AttributeError(
-                "'%s' object has no attribute '%s'" % (type(self).__name__, name)
-            )
-
-    def __setattr__(self, name, value):
-        if name in ('_flags', '_all_options', '_visible_options'):
-            super().__setattr__(name, value)
-        elif name in self._visible_option_list():
-            self._all_options[name] = value
-        else:
-            raise AttributeError(
-                "'%s' object has no attribute '%s'" % (type(self).__name__, name))
-
-    def __str__(self):
-        return '%s(%s)' % (
-            type(self).__name__,
-            ', '.join(
-                '%s=%s' % (option, getattr(self, option))
-                for option in self._visible_option_list()
-            )
-        )
-
-
-class _RondsArgumentParser(argparse.ArgumentParser):
-    """An ArgumentParser that supports ValueProvider options.
-
-      Example Usage::
-
-        class TemplateUserOptions(PipelineOptions):
-          @classmethod
-          def _add_argparse_args(cls, parser):
-            parser.add_value_provider_argument('--vp_arg1', default='start')
-            parser.add_value_provider_argument('--vp_arg2')
-            parser.add_argument('--non_vp_arg')
-
-      """
-
-    def add_value_provider_argument(self, *args, **kwargs):
-        assert args != () and len(args[0]) >= 1
-        if args[0][0] != '-':
-            option_name = args[0]
-            if kwargs.get('nargs') is None:
-                kwargs['nargs'] = '?'
-        else:
-            option_name = [i.repalce('--', '') for i in args if i[:2] == '--'][0]
-        value_type = kwargs.get('type') or str
-        kwargs['type'] = _static_value_provider_of(value_type)
-        default_value = kwargs.get('default')
-        kwargs['default'] = RuntimeValueProvider(
-            option_name=option_name,
-            value_type=value_type,
-            default_value=default_value
-        )
-        self.add_argument(*args, **kwargs)
-
-    def error(self, message: str) -> NoReturn:
-        if message.startswith('ambiguous option: '):
-            return
-        super().error(message)
-
-
-class SparkRunnerOptions(PipelineOptions):
-    @classmethod
-    def _add_argparse_args(cls, parser):  # type: (_RondsArgumentParser) -> None
-        parser.add_argument(
-            '--spark_master_url',
-            default=None,
-        )
-        parser.add_argument(
-            '--spark_job_server_jar',
-        )
-        parser.add_argument(
-            '--spark_version',
-            default='3'
-        )
-        parser.add_argument(
-            '--spark_repartition_num',
-            default=2,
-            help='Spark DataFrame repartition num if necessary'
-        )
-        parser.add_argument(
-            '--spark_window_duration',
-            default=5,
-            help='window duration minutes'
-        )
-
-
-class CassandraOptions(PipelineOptions):
-
-    # noinspection SpellCheckingInspection
-    @classmethod
-    def _add_argparse_args(cls, parser):
-        parser.add_argument(
-            '--cassandra_window_duration',
-            default=10,
-            help='cassandra scan window duration seconds'
-        )
-        parser.add_argument(
-            '--cassandra_host',
-            default=['192.168.1.186']
-        )
-        parser.add_argument(
-            '--cassandra_keyspace',
-            default='rzbigdata'
-        )
-        parser.add_argument(
-            '--cassandra_table_process',
-            default='processdata',
-            help='table name for precess table'
-        )
-        parser.add_argument(
-            '--cassandra_start_datetime',
-            default=None
-        )
-
-
-class KafkaOptions(PipelineOptions):
-
-    # noinspection SpellCheckingInspection
-    @classmethod
-    def _add_argparse_args(cls, parser):
-        pass
-
-
-class AlgorithmOptions(PipelineOptions):
-
-    # noinspection SpellCheckingInspection
-    @classmethod
-    def _add_argparse_args(cls, parser):
-        parser.add_argument(
-            '--algorithm_path',
-            default='../ruleeditor',
-            help='Relative or absolute algorithm file path'
-        )
-        parser.add_argument(
-            '--algorithm_funcname',
-            default='__init__platform.run',
-            help='algorithm function reference'
-        )
-
-
-def _static_value_provider_of(value_type):
-    def _f(value):
-        _f.__name__ = value_type.__name__
-        return StaticValueProvider(value_type, value)
-
-    return _f
+import argparse
+from typing import Optional, Any, List, Iterable, Type, TypeVar, NoReturn
+
+__all__ = [
+    'PipelineOptions',
+    'SparkRunnerOptions',
+    'CassandraOptions',
+    'AlgorithmOptions',
+    'KafkaOptions',
+]
+
+from ronds_sdk.options.value_provider import StaticValueProvider, RuntimeValueProvider
+
+PipelineOptionsT = TypeVar('PipelineOptionsT', bound='PipelineOptions')
+
+
+class PipelineOptions(object):
+
+    def __init__(self, flags=None, **kwargs):
+        # type: (Optional[List[str]], **Any) -> None
+        self._flags = flags
+
+        parser = _RondsArgumentParser()
+        for cls in type(self).mro():
+            if cls == PipelineOptions:
+                self.add_argparse_args(parser)
+                break
+            elif '_add_argparse_args' in cls.__dict__:
+                cls._add_argparse_args(parser)  # type: ignore
+
+        self._visible_options, _ = parser.parse_known_args(flags)
+
+        self._all_options = kwargs
+
+        for option_name in self._visible_option_list():
+            # Note that options specified in kwargs will not be overwritten
+            if option_name not in self._all_options:
+                self._all_options[option_name] = getattr(self._visible_options, option_name)
+
+    @classmethod
+    def add_argparse_args(cls, parser):
+        # type: (_RondsArgumentParser) -> None
+        # Override this in subclasses to provide options.
+        parser.add_argument(
+            '--transform_package',
+            default='ronds_sdk.transforms.spark.transforms',
+            help='运行任务时, 物理执行算子的 package 路径, runner 有默认值, 一般无需修改'
+        )
+        parser.add_argument(
+            '--enable_executor_debug',
+            default=False,
+            help='是否启用 Spark Executor 端的 DEBUG 功能, 仅用于测试'
+        )
+
+    def view_as(self, cls):
+        # type: (Type[PipelineOptionsT]) -> PipelineOptionsT
+        view: PipelineOptions = cls(self._flags)
+
+        for option_name in view._visible_option_list():  # type: ignore
+            if option_name not in self._all_options:
+                self._all_options[option_name] = getattr(
+                    view._visible_options, option_name)
+        view._all_options = self._all_options
+        return view
+
+    def _visible_option_list(self):
+        # type: () -> List[str]
+        return sorted(
+            option for option in dir(self._visible_options) if option[0] != '_'
+        )
+
+    def __dir__(self) -> Iterable[str]:
+        return sorted(
+            dir(type(self)) + list(self.__dict__) + self._visible_option_list()
+        )
+
+    def __getattr__(self, name):
+        if name[:2] == name[-2:] == '__':
+            return object.__getattribute__(self, name)
+        elif name in self._visible_option_list():
+            return self._all_options[name]
+        else:
+            raise AttributeError(
+                "'%s' object has no attribute '%s'" % (type(self).__name__, name)
+            )
+
+    def __setattr__(self, name, value):
+        if name in ('_flags', '_all_options', '_visible_options'):
+            super().__setattr__(name, value)
+        elif name in self._visible_option_list():
+            self._all_options[name] = value
+        else:
+            raise AttributeError(
+                "'%s' object has no attribute '%s'" % (type(self).__name__, name))
+
+    def __str__(self):
+        return '%s(%s)' % (
+            type(self).__name__,
+            ', '.join(
+                '%s=%s' % (option, getattr(self, option))
+                for option in self._visible_option_list()
+            )
+        )
+
+
+class _RondsArgumentParser(argparse.ArgumentParser):
+    """An ArgumentParser that supports ValueProvider options.
+
+      Example Usage::
+
+        class TemplateUserOptions(PipelineOptions):
+          @classmethod
+          def _add_argparse_args(cls, parser):
+            parser.add_value_provider_argument('--vp_arg1', default='start')
+            parser.add_value_provider_argument('--vp_arg2')
+            parser.add_argument('--non_vp_arg')
+
+      """
+
+    def add_value_provider_argument(self, *args, **kwargs):
+        assert args != () and len(args[0]) >= 1
+        if args[0][0] != '-':
+            option_name = args[0]
+            if kwargs.get('nargs') is None:
+                kwargs['nargs'] = '?'
+        else:
+            option_name = [i.repalce('--', '') for i in args if i[:2] == '--'][0]
+        value_type = kwargs.get('type') or str
+        kwargs['type'] = _static_value_provider_of(value_type)
+        default_value = kwargs.get('default')
+        kwargs['default'] = RuntimeValueProvider(
+            option_name=option_name,
+            value_type=value_type,
+            default_value=default_value
+        )
+        self.add_argument(*args, **kwargs)
+
+    def error(self, message: str) -> NoReturn:
+        if message.startswith('ambiguous option: '):
+            return
+        super().error(message)
+
+
+class SparkRunnerOptions(PipelineOptions):
+    @classmethod
+    def _add_argparse_args(cls, parser):  # type: (_RondsArgumentParser) -> None
+        parser.add_argument(
+            '--spark_master_url',
+            default=None,
+        )
+        parser.add_argument(
+            '--spark_job_server_jar',
+        )
+        parser.add_argument(
+            '--spark_version',
+            default='3'
+        )
+        parser.add_argument(
+            '--spark_repartition_num',
+            default=2,
+            help='Spark DataFrame repartition num if necessary'
+        )
+        parser.add_argument(
+            '--spark_window_duration',
+            default=5,
+            help='window duration minutes'
+        )
+
+
+class CassandraOptions(PipelineOptions):
+
+    # noinspection SpellCheckingInspection
+    @classmethod
+    def _add_argparse_args(cls, parser):
+        parser.add_argument(
+            '--cassandra_window_duration',
+            default=10,
+            help='cassandra scan window duration seconds'
+        )
+        parser.add_argument(
+            '--cassandra_host',
+            default=['192.168.1.186']
+        )
+        parser.add_argument(
+            '--cassandra_keyspace',
+            default='eimp'
+        )
+        parser.add_argument(
+            '--cassandra_table_process',
+            default='processdata',
+            help='table name for precess table'
+        )
+        parser.add_argument(
+            '--cassandra_start_datetime',
+            default=None
+        )
+
+
+class KafkaOptions(PipelineOptions):
+
+    # noinspection SpellCheckingInspection
+    @classmethod
+    def _add_argparse_args(cls, parser):
+        parser.add_argument(
+            '--kafka_bootstrap_servers',
+            default=None,
+            help='kafka bootstrap servers, eg. "host1:9092,host2:9092" .'
+        )
+        parser.add_argument(
+            '--kafka_send_mock',
+            default=False,
+            help='if true, print messages instead of sending to Kafka cluster, for test'
+        )
+
+
+class AlgorithmOptions(PipelineOptions):
+
+    # noinspection SpellCheckingInspection
+    @classmethod
+    def _add_argparse_args(cls, parser):
+        parser.add_argument(
+            '--algorithm_path',
+            help='Relative or absolute algorithm file path'
+        )
+        parser.add_argument(
+            '--algorithm_funcname',
+            help='algorithm function reference'
+        )
+
+
+def _static_value_provider_of(value_type):
+    def _f(value):
+        _f.__name__ = value_type.__name__
+        return StaticValueProvider(value_type, value)
+
+    return _f
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/options/value_provider.py` & `rondsspark-0.0.4.7/ronds_sdk/options/value_provider.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one or more
-# contributor license agreements.  See the NOTICE file distributed with
-# this work for additional information regarding copyright ownership.
-# The ASF licenses this file to You under the Apache License, Version 2.0
-# (the "License"); you may not use this file except in compliance with
-# the License.  You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-
-"""A ValueProvider abstracts the notion of fetching a value that may or
-may not be currently available.
-
-This can be used to parameterize transforms that only read values in at
-runtime, for example.
-"""
-
-# pytype: skip-file
-
-from functools import wraps
-from typing import Set
-
-from ronds_sdk import error
-
-__all__ = [
-    'ValueProvider',
-    'StaticValueProvider',
-    'RuntimeValueProvider',
-    'NestedValueProvider',
-    'check_accessible',
-]
-
-
-class ValueProvider(object):
-    """Base class that all other ValueProviders must implement.
-  """
-
-    def is_accessible(self):
-        """Whether the contents of this ValueProvider is available to routines
-    that run at graph construction time.
-    """
-        raise NotImplementedError(
-            'ValueProvider.is_accessible implemented in derived classes')
-
-    def get(self):
-        """Return the value wrapped by this ValueProvider.
-    """
-        raise NotImplementedError(
-            'ValueProvider.get implemented in derived classes')
-
-
-class StaticValueProvider(ValueProvider):
-    """StaticValueProvider is an implementation of ValueProvider that allows
-  for a static value to be provided.
-  """
-
-    def __init__(self, value_type, value):
-        """
-    Args:
-        value_type: Type of the static value
-        value: Static value
-    """
-        self.value_type = value_type
-        self.value = value_type(value)
-
-    def is_accessible(self):
-        return True
-
-    def get(self):
-        return self.value
-
-    def __str__(self):
-        return str(self.value)
-
-    def __eq__(self, other):
-        if self.value == other:
-            return True
-        if isinstance(other, StaticValueProvider):
-            if self.value_type == other.value_type and self.value == other.value:
-                return True
-        return False
-
-    def __hash__(self):
-        return hash((type(self), self.value_type, self.value))
-
-
-class RuntimeValueProvider(ValueProvider):
-    """RuntimeValueProvider is an implementation of ValueProvider that
-  allows for a value to be provided at execution time rather than
-  at graph construction time.
-  """
-    runtime_options = None
-    experiments = set()  # type: Set[str]
-
-    def __init__(self, option_name, value_type, default_value):
-        self.option_name = option_name
-        self.default_value = default_value
-        self.value_type = value_type
-
-    def is_accessible(self):
-        return RuntimeValueProvider.runtime_options is not None
-
-    @classmethod
-    def get_value(cls, option_name, value_type, default_value):
-        if not RuntimeValueProvider.runtime_options:
-            return default_value
-
-        candidate = RuntimeValueProvider.runtime_options.get(option_name)
-        if candidate:
-            return value_type(candidate)
-        else:
-            return default_value
-
-    def get(self):
-        if RuntimeValueProvider.runtime_options is None:
-            raise error.RuntimeValueProviderError(
-                '%s.get() not called from a runtime context' % self)
-
-        return RuntimeValueProvider.get_value(
-            self.option_name, self.value_type, self.default_value)
-
-    @classmethod
-    def set_runtime_options(cls, pipeline_options):
-        RuntimeValueProvider.runtime_options = pipeline_options
-        RuntimeValueProvider.experiments = RuntimeValueProvider.get_value(
-            'experiments', set, set())
-
-    def __str__(self):
-        return '%s(option: %s, type: %s, default_value: %s)' % (
-            self.__class__.__name__,
-            self.option_name,
-            self.value_type.__name__,
-            repr(self.default_value))
-
-
-class NestedValueProvider(ValueProvider):
-    """NestedValueProvider is an implementation of ValueProvider that allows
-  for wrapping another ValueProvider object.
-  """
-
-    def __init__(self, value, translator):
-        """Creates a NestedValueProvider that wraps the provided ValueProvider.
-
-    Args:
-      value: ValueProvider object to wrap
-      translator: function that is applied to the ValueProvider
-    Raises:
-      ``RuntimeValueProviderError``: if any of the provided objects are not
-        accessible.
-    """
-        self.value = value
-        self.translator = translator
-        self.cached_value = None
-
-    def is_accessible(self):
-        return self.value.is_accessible()
-
-    def get(self):
-        try:
-            return self.cached_value
-        except AttributeError:
-            self.cached_value = self.translator(self.value.get())
-            return self.cached_value
-
-    def __str__(self):
-        return "%s(value: %s, translator: %s)" % (
-            self.__class__.__name__,
-            self.value,
-            self.translator.__name__,
-        )
-
-
-def check_accessible(value_provider_list):
-    """A decorator that checks accessibility of a list of ValueProvider objects.
-
-  Args:
-    value_provider_list: list of ValueProvider objects
-  Raises:
-    ``RuntimeValueProviderError``: if any of the provided objects are not
-      accessible.
-  """
-    assert isinstance(value_provider_list, list)
-
-    def _check_accessible(fnc):
-        @wraps(fnc)
-        def _f(self, *args, **kwargs):
-            for obj in [getattr(self, vp) for vp in value_provider_list]:
-                if not obj.is_accessible():
-                    raise error.RuntimeValueProviderError('%s not accessible' % obj)
-            return fnc(self, *args, **kwargs)
-
-        return _f
-
-    return _check_accessible
-
-
-
-
-
+#
+# Licensed to the Apache Software Foundation (ASF) under one or more
+# contributor license agreements.  See the NOTICE file distributed with
+# this work for additional information regarding copyright ownership.
+# The ASF licenses this file to You under the Apache License, Version 2.0
+# (the "License"); you may not use this file except in compliance with
+# the License.  You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
+"""A ValueProvider abstracts the notion of fetching a value that may or
+may not be currently available.
+
+This can be used to parameterize transforms that only read values in at
+runtime, for example.
+"""
+
+# pytype: skip-file
+
+from functools import wraps
+from typing import Set
+
+from ronds_sdk import error
+
+__all__ = [
+    'ValueProvider',
+    'StaticValueProvider',
+    'RuntimeValueProvider',
+    'NestedValueProvider',
+    'check_accessible',
+]
+
+
+class ValueProvider(object):
+    """Base class that all other ValueProviders must implement.
+  """
+
+    def is_accessible(self):
+        """Whether the contents of this ValueProvider is available to routines
+    that run at graph construction time.
+    """
+        raise NotImplementedError(
+            'ValueProvider.is_accessible implemented in derived classes')
+
+    def get(self):
+        """Return the value wrapped by this ValueProvider.
+    """
+        raise NotImplementedError(
+            'ValueProvider.get implemented in derived classes')
+
+
+class StaticValueProvider(ValueProvider):
+    """StaticValueProvider is an implementation of ValueProvider that allows
+  for a static value to be provided.
+  """
+
+    def __init__(self, value_type, value):
+        """
+    Args:
+        value_type: Type of the static value
+        value: Static value
+    """
+        self.value_type = value_type
+        self.value = value_type(value)
+
+    def is_accessible(self):
+        return True
+
+    def get(self):
+        return self.value
+
+    def __str__(self):
+        return str(self.value)
+
+    def __eq__(self, other):
+        if self.value == other:
+            return True
+        if isinstance(other, StaticValueProvider):
+            if self.value_type == other.value_type and self.value == other.value:
+                return True
+        return False
+
+    def __hash__(self):
+        return hash((type(self), self.value_type, self.value))
+
+
+class RuntimeValueProvider(ValueProvider):
+    """RuntimeValueProvider is an implementation of ValueProvider that
+  allows for a value to be provided at execution time rather than
+  at graph construction time.
+  """
+    runtime_options = None
+    experiments = set()  # type: Set[str]
+
+    def __init__(self, option_name, value_type, default_value):
+        self.option_name = option_name
+        self.default_value = default_value
+        self.value_type = value_type
+
+    def is_accessible(self):
+        return RuntimeValueProvider.runtime_options is not None
+
+    @classmethod
+    def get_value(cls, option_name, value_type, default_value):
+        if not RuntimeValueProvider.runtime_options:
+            return default_value
+
+        candidate = RuntimeValueProvider.runtime_options.get(option_name)
+        if candidate:
+            return value_type(candidate)
+        else:
+            return default_value
+
+    def get(self):
+        if RuntimeValueProvider.runtime_options is None:
+            raise error.RuntimeValueProviderError(
+                '%s.get() not called from a runtime context' % self)
+
+        return RuntimeValueProvider.get_value(
+            self.option_name, self.value_type, self.default_value)
+
+    @classmethod
+    def set_runtime_options(cls, pipeline_options):
+        RuntimeValueProvider.runtime_options = pipeline_options
+        RuntimeValueProvider.experiments = RuntimeValueProvider.get_value(
+            'experiments', set, set())
+
+    def __str__(self):
+        return '%s(option: %s, type: %s, default_value: %s)' % (
+            self.__class__.__name__,
+            self.option_name,
+            self.value_type.__name__,
+            repr(self.default_value))
+
+
+class NestedValueProvider(ValueProvider):
+    """NestedValueProvider is an implementation of ValueProvider that allows
+  for wrapping another ValueProvider object.
+  """
+
+    def __init__(self, value, translator):
+        """Creates a NestedValueProvider that wraps the provided ValueProvider.
+
+    Args:
+      value: ValueProvider object to wrap
+      translator: function that is applied to the ValueProvider
+    Raises:
+      ``RuntimeValueProviderError``: if any of the provided objects are not
+        accessible.
+    """
+        self.value = value
+        self.translator = translator
+        self.cached_value = None
+
+    def is_accessible(self):
+        return self.value.is_accessible()
+
+    def get(self):
+        try:
+            return self.cached_value
+        except AttributeError:
+            self.cached_value = self.translator(self.value.get())
+            return self.cached_value
+
+    def __str__(self):
+        return "%s(value: %s, translator: %s)" % (
+            self.__class__.__name__,
+            self.value,
+            self.translator.__name__,
+        )
+
+
+def check_accessible(value_provider_list):
+    """A decorator that checks accessibility of a list of ValueProvider objects.
+
+  Args:
+    value_provider_list: list of ValueProvider objects
+  Raises:
+    ``RuntimeValueProviderError``: if any of the provided objects are not
+      accessible.
+  """
+    assert isinstance(value_provider_list, list)
+
+    def _check_accessible(fnc):
+        @wraps(fnc)
+        def _f(self, *args, **kwargs):
+            for obj in [getattr(self, vp) for vp in value_provider_list]:
+                if not obj.is_accessible():
+                    raise error.RuntimeValueProviderError('%s not accessible' % obj)
+            return fnc(self, *args, **kwargs)
+
+        return _f
+
+    return _check_accessible
+
+
+
+
+
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/pipeline.py` & `rondsspark-0.0.4.7/ronds_sdk/pipeline.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,357 +1,357 @@
-import importlib
-import logging
-import re
-import tempfile
-import time
-from collections import defaultdict
-from types import TracebackType
-from typing import Optional, List, Union, Mapping, Dict, Set, Any, Type
-
-import unicodedata
-
-from ronds_sdk import error
-from ronds_sdk.options.pipeline_options import PipelineOptions
-from ronds_sdk.transforms import ptransform
-from ronds_sdk.dataframe import pvalue
-
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from ronds_sdk.runners.runner import PipelineRunner, PipelineResult
-    from ronds_sdk.transforms.ptransform import PTransform
-
-__all__ = ['Pipeline', 'AppliedPTransform', 'PipelineVisitor']
-
-
-class Pipeline(object):
-    """
-    Pipeline 对象代表 DAG, 由
-    :class:`ronds_sdk.dataframe.pvalue.PValue` and
-    :class:`ronds_sdk.transforms.ptransform.PTransform` 组成.
-
-    PValue 是 DAG 的 nodes, 算子 PTransform 是 DAG 的 edges.
-
-    所有应用到 Pipeline 的 PTransform 算子必须有唯一的 full label.
-    """
-
-    def __init__(self, options=None, argv=None):
-        # type: (Optional[PipelineOptions], Optional[List[str]]) -> None
-        """
-        初始化 Pipeline
-        :param options: 运行 Pipeline 需要的参数
-        :param argv: 当 options=None 时, 用于构建 options
-        """
-        logging.basicConfig()
-
-        # parse PipelineOptions
-        if options is not None:
-            if isinstance(options, PipelineOptions):
-                self._options = options
-            else:
-                raise ValueError(
-                    'Parameter options, if specified, must be of type PipelineOptions. '
-                    'Received : %r' % options)
-        elif argv is not None:
-            if isinstance(argv, list):
-                self._options = PipelineOptions(argv)
-            else:
-                raise ValueError(
-                    'Parameter argv, if specified, must be a list. Received : %r' %
-                    argv)
-        else:
-            self._options = PipelineOptions([])
-
-        self.local_tempdir = tempfile.mkdtemp(prefix='ronds-pipeline-temp')
-
-        self.root_transform = AppliedPTransform(None, None, '', None, is_root=True)
-        # Set of transform labels (full labels) applied to the pipeline.
-        # If a transform is applied and the full label is already in the set
-        # then the transform will have to be cloned with a new label.
-        self.applied_labels = set()  # type: Set[str]
-        # Create a ComponentIdMap for assigning IDs to components.
-        self.component_id_map = ComponentIdMap()
-        # Records whether this pipeline contains any external transforms.
-        self.contain_external_transforms = False
-        self.job_context = None
-
-    @property
-    def options(self):
-        return self._options
-
-    def _root_transform(self):
-        # type: () -> AppliedPTransform
-        """
-        返回 root transform
-        :return: root transform
-        """
-        return self.root_transform
-
-    def run(self):
-        # type: () -> PipelineResult
-        from ronds_sdk.runners.spark_runner import SparkRunner
-        runner = SparkRunner(self.options)
-        return runner.run_pipeline(self, self._options)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self,
-                 exc_type,  # type: Optional[Type[BaseException]]
-                 exc_val,  # type: Optional[BaseException]
-                 exc_tb  # type: Optional[TracebackType]
-                 ):
-        start = time.time()
-        try:
-            if not exc_type:
-                self.result = self.run()
-                self.result.wait_until_finish()
-        finally:
-            end = time.time()
-            logging.info('pipeline exited, cost: %s ~' % str(end - start))
-
-    def visit(self, visitor):
-        # type: (PipelineVisitor) -> None
-        self._root_transform().visit(visitor, )
-
-    def apply(self,
-              transform,  # type: ptransform.PTransform
-              p_valueish=None,  # type: Optional[pvalue.PValue]
-              label=None  # type: Optional[str]
-              ):
-        # type: (...) -> pvalue.PValue
-        # noinspection PyProtectedMember
-        if isinstance(transform, ptransform._NamedPTransform):
-            self.apply(transform.transform, p_valueish, label or transform.label)
-        if not isinstance(transform, ptransform.PTransform):
-            raise TypeError("Expected a PTransform object, got %s" % transform)
-        full_label = label or transform.label
-        if full_label in self.applied_labels:
-            raise RuntimeError(
-                'A transform with label "%s" already exists in the pipeline. '
-                'To apply a transform with a specified label write '
-                'pvalue | "label" >> transform' % full_label)
-        self.applied_labels.add(full_label)
-
-        # noinspection PyProtectedMember
-        p_valueish, inputs = transform._extract_input_p_values(p_valueish)
-        try:
-            if not isinstance(inputs, dict):
-                inputs = {str(ix): inp for (ix, inp) in enumerate(inputs)}
-        except TypeError:
-            raise NotImplementedError(
-                'Unable to extract PValue inputs from %s; either %s does not accept '
-                'inputs of this format, or it does not properly override '
-                '_extract_input_p_values' % (p_valueish, transform))
-        for t, leaf_input in inputs.items():
-            if not isinstance(leaf_input, pvalue.PValue) or not isinstance(t, str):
-                raise NotImplementedError(
-                    '%s does not properly override _extract_input_p_values, '
-                    'returned %s from %s' % (transform, inputs, p_valueish))
-        current = AppliedPTransform(
-            p_valueish.producer, transform, full_label, inputs
-        )
-        p_valueish.add_consumer(current)
-        try:
-            p_valueish_result = self.expand(transform, p_valueish, self._options)
-
-            for tag, result in ptransform.get_named_nested_p_values(p_valueish_result):
-                assert isinstance(result, pvalue.PValue)
-
-                if result.producer is None:
-                    result.producer = current
-
-                assert isinstance(result.producer.inputs, tuple)
-                base = tag
-                counter = 0
-                while tag in current.outputs:
-                    counter += 1
-                    tag = '%s_%d' % (base, counter)
-
-                current.add_output(result, tag)
-        except Exception as r:
-            logging.error('unexpected error: %s' % repr(r))
-            raise r
-        return p_valueish_result
-
-    @staticmethod
-    def expand(transform,  # type: PTransform
-               input,
-               options,  # type: PipelineOptions
-               ):
-        # sp_transform = self.load_spark_transform(transform)
-        return transform.expand(input)
-
-
-class AppliedPTransform(object):
-    """
-    A transform node representing an instance of applying a PTransform
-    """
-
-    def __init__(self,
-                 parent,  # type: Optional[AppliedPTransform]
-                 transform,  # type: Optional[ptransform],
-                 full_label,  # type: str
-                 main_inputs,  # type: Optional[Mapping[str, Union[pvalue.PBegin, pvalue.PCollection]]]
-                 environment_id=None,  # type: Optional[str]
-                 annotations=None,  # type: Optional[Dict[str, bytes]]
-                 is_root=False  # type: bool
-                 ):
-        # type: (...) -> None
-        self.parent = parent
-        self.transform = transform
-        self.full_label = full_label
-        self.main_input = dict(main_inputs or {})
-
-        self.side_input = tuple() if transform is None else transform.side_inputs
-        self.outputs = {}  # type: Dict[Union[str, int, None], pvalue.PValue]
-        self.parts = []  # type: List[AppliedPTransform]
-        self.environment_id = environment_id if environment_id else None  # type: Optional[str]
-        self._is_root = is_root
-
-    @property
-    def inputs(self):
-        # type: () -> tuple[Union[pvalue.PBegin, pvalue.PCollection]]
-        return tuple(self.main_input.values())
-
-    def is_root(self):
-        # type: () -> bool
-        return self._is_root
-
-    def __repr__(self):
-        # type: () -> str
-        return "%s(%s, %s)" % (
-            self.__class__.__name__, self.full_label, type(self.transform).__name__)
-
-    def add_output(self,
-                   output,  # type: Union[pvalue.PValue]
-                   tag  # type: Union[str, int, None]
-                   ):
-        # (...) -> None
-        if isinstance(output, pvalue.PValue):
-            if tag not in self.outputs:
-                self.outputs[tag] = output
-            else:
-                raise error.TransformError('tag[%s] has existed in outputs')
-        else:
-            raise TypeError("Unexpected out type: %s" % output)
-
-    def add_part(self, part):
-        # type: (AppliedPTransform) -> None
-        assert isinstance(part, AppliedPTransform)
-        self.parts.append(part)
-
-    def is_composite(self):
-        # type: () -> bool
-        return bool(self.parts) or all(
-            p_val.producer is not self for p_val in self.outputs.values()
-        )
-
-    def visit(self,
-              visitor,  # type: PipelineVisitor
-              ):
-        # type: (...) -> None
-        """Visits all nodes reachable from the current node."""
-        if self._is_root and self.outputs and self.outputs['__root']:
-            root = self.outputs['__root']
-            assert isinstance(root, pvalue.PValue)
-            for consumer in root.consumers:
-                consumer.visit(visitor)
-        elif visitor.visit_transform(self) and self.outputs:
-            for p_value in self.outputs.values():
-                assert isinstance(p_value, pvalue.PValue)
-                p_value.visit(visitor)
-        visitor.leave_transform(self)
-
-
-class ComponentIdMap(object):
-    """
-    A utility for assigning unique component ids to Beam components.
-
-    Component ID assignments are only guaranteed to be unique and consistent
-    within the scope of a ComponentIdMap instance.
-    """
-
-    def __init__(self, namespace="ref"):
-        self.namespace = namespace
-        self._counters = defaultdict(lambda: 0)  # type:Dict[type, int]
-        self._obj_to_id = {}  # type: Dict[Any, str]
-
-    def get_or_assign(self, obj=None, obj_type=None, label=None):
-        if obj not in self._obj_to_id:
-            self._obj_to_id[obj] = self._unique_ref(obj, obj_type, label)
-        return self._obj_to_id[obj]
-
-    def _unique_ref(self, obj=None, obj_type=None, label=None):
-        # Normalize, trim, and unify.
-        prefix = self._normalize(
-            "%s_%s_%s" % (self.namespace, obj_type.__name__, label or type(obj).__name__)
-        )[0:100]
-        self._counters[obj_type] += 1
-        return '%s_%d' % (prefix, self._counters[obj_type])
-
-    @staticmethod
-    def _normalize(str_value):
-        str_value = unicodedata.normalize('NFC', str_value)
-        return re.sub(r'[^a-zA-Z0-9-_]+', '-', str_value)
-
-
-class PipelineVisitor(object):
-    """
-    Visitor pattern class used to traverse a DAG of transforms
-    """
-
-    def __init__(self):
-        self.stream_writers = list()
-        self.module = None
-        self.__trans_cache = dict()  # type: dict[PTransform, PTransform]
-
-    def load_spark_transform(self,  # type: PipelineVisitor
-                             transform,  # type: PTransform,
-                             options=None,  # type: PipelineOptions
-                             **kwargs,
-                             ):
-        # type: (...) -> PTransform
-        # cache first
-        if self.__trans_cache.__contains__(transform):
-            return self.__trans_cache[transform]
-
-        # create new PTransform
-        if not self.module:
-            self.module = importlib.import_module(self.transform_package(options))
-        d = getattr(self.module, transform.__class__.__name__)
-        if d:
-            all_kwargs = dict()
-            if 'options' in d.__dict__['__init__'].__code__.co_varnames:
-                all_kwargs['options'] = options
-            for key in kwargs.keys():
-                if key in d.__dict__['__init__'].__code__.co_varnames:
-                    all_kwargs[key] = kwargs[key]
-            sp_trans = d(transform, **all_kwargs)
-            self.__trans_cache[transform] = sp_trans
-            return sp_trans
-        else:
-            raise NotImplementedError(
-                "transform [%s] not implemented by Spark!" % transform.__class__.__name__)
-
-    @staticmethod
-    def transform_package(options):
-        if options is None:
-            raise error.PipelineError("load_spark_transform pipeline options is null!")
-        return options.transform_package
-
-    def visit_value(self, value):
-        # type: (pvalue.PValue) -> bool
-        """
-        Callback for visiting a PValue in the pipeline DAG.
-        :param value: PValue visited (typically a PCollection instance).
-        :return:
-        """
-        return True
-
-    def visit_transform(self, transform_node):
-        # type: (AppliedPTransform) -> bool
-        return True
-
-    def leave_transform(self, transform_node):
-        # type: (AppliedPTransform) -> None
-        pass
+import importlib
+import logging
+import re
+import tempfile
+import time
+from collections import defaultdict
+from types import TracebackType
+from typing import Optional, List, Union, Mapping, Dict, Set, Any, Type
+
+import unicodedata
+
+from ronds_sdk import error
+from ronds_sdk.options.pipeline_options import PipelineOptions
+from ronds_sdk.transforms import ptransform
+from ronds_sdk.dataframe import pvalue
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ronds_sdk.runners.runner import PipelineRunner, PipelineResult
+    from ronds_sdk.transforms.ptransform import PTransform
+
+__all__ = ['Pipeline', 'AppliedPTransform', 'PipelineVisitor']
+
+
+class Pipeline(object):
+    """
+    Pipeline 对象代表 DAG, 由
+    :class:`ronds_sdk.dataframe.pvalue.PValue` and
+    :class:`ronds_sdk.transforms.ptransform.PTransform` 组成.
+
+    PValue 是 DAG 的 nodes, 算子 PTransform 是 DAG 的 edges.
+
+    所有应用到 Pipeline 的 PTransform 算子必须有唯一的 full label.
+    """
+
+    def __init__(self, options=None, argv=None):
+        # type: (Optional[PipelineOptions], Optional[List[str]]) -> None
+        """
+        初始化 Pipeline
+        :param options: 运行 Pipeline 需要的参数
+        :param argv: 当 options=None 时, 用于构建 options
+        """
+        logging.basicConfig()
+
+        # parse PipelineOptions
+        if options is not None:
+            if isinstance(options, PipelineOptions):
+                self._options = options
+            else:
+                raise ValueError(
+                    'Parameter options, if specified, must be of type PipelineOptions. '
+                    'Received : %r' % options)
+        elif argv is not None:
+            if isinstance(argv, list):
+                self._options = PipelineOptions(argv)
+            else:
+                raise ValueError(
+                    'Parameter argv, if specified, must be a list. Received : %r' %
+                    argv)
+        else:
+            self._options = PipelineOptions([])
+
+        self.local_tempdir = tempfile.mkdtemp(prefix='ronds-pipeline-temp')
+
+        self.root_transform = AppliedPTransform(None, None, '', None, is_root=True)
+        # Set of transform labels (full labels) applied to the pipeline.
+        # If a transform is applied and the full label is already in the set
+        # then the transform will have to be cloned with a new label.
+        self.applied_labels = set()  # type: Set[str]
+        # Create a ComponentIdMap for assigning IDs to components.
+        self.component_id_map = ComponentIdMap()
+        # Records whether this pipeline contains any external transforms.
+        self.contain_external_transforms = False
+        self.job_context = None
+
+    @property
+    def options(self):
+        return self._options
+
+    def _root_transform(self):
+        # type: () -> AppliedPTransform
+        """
+        返回 root transform
+        :return: root transform
+        """
+        return self.root_transform
+
+    def run(self):
+        # type: () -> PipelineResult
+        from ronds_sdk.runners.spark_runner import SparkRunner
+        runner = SparkRunner(self.options)
+        return runner.run_pipeline(self, self._options)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self,
+                 exc_type,  # type: Optional[Type[BaseException]]
+                 exc_val,  # type: Optional[BaseException]
+                 exc_tb  # type: Optional[TracebackType]
+                 ):
+        start = time.time()
+        try:
+            if not exc_type:
+                self.result = self.run()
+                self.result.wait_until_finish()
+        finally:
+            end = time.time()
+            logging.info('pipeline exited, cost: %s ~' % str(end - start))
+
+    def visit(self, visitor):
+        # type: (PipelineVisitor) -> None
+        self._root_transform().visit(visitor, )
+
+    def apply(self,
+              transform,  # type: ptransform.PTransform
+              p_valueish=None,  # type: Optional[pvalue.PValue]
+              label=None  # type: Optional[str]
+              ):
+        # type: (...) -> pvalue.PValue
+        # noinspection PyProtectedMember
+        if isinstance(transform, ptransform._NamedPTransform):
+            self.apply(transform.transform, p_valueish, label or transform.label)
+        if not isinstance(transform, ptransform.PTransform):
+            raise TypeError("Expected a PTransform object, got %s" % transform)
+        full_label = label or transform.label
+        if full_label in self.applied_labels:
+            raise RuntimeError(
+                'A transform with label "%s" already exists in the pipeline. '
+                'To apply a transform with a specified label write '
+                'pvalue | "label" >> transform' % full_label)
+        self.applied_labels.add(full_label)
+
+        # noinspection PyProtectedMember
+        p_valueish, inputs = transform._extract_input_p_values(p_valueish)
+        try:
+            if not isinstance(inputs, dict):
+                inputs = {str(ix): inp for (ix, inp) in enumerate(inputs)}
+        except TypeError:
+            raise NotImplementedError(
+                'Unable to extract PValue inputs from %s; either %s does not accept '
+                'inputs of this format, or it does not properly override '
+                '_extract_input_p_values' % (p_valueish, transform))
+        for t, leaf_input in inputs.items():
+            if not isinstance(leaf_input, pvalue.PValue) or not isinstance(t, str):
+                raise NotImplementedError(
+                    '%s does not properly override _extract_input_p_values, '
+                    'returned %s from %s' % (transform, inputs, p_valueish))
+        current = AppliedPTransform(
+            p_valueish.producer, transform, full_label, inputs
+        )
+        p_valueish.add_consumer(current)
+        try:
+            p_valueish_result = self.expand(transform, p_valueish, self._options)
+
+            for tag, result in ptransform.get_named_nested_p_values(p_valueish_result):
+                assert isinstance(result, pvalue.PValue)
+
+                if result.producer is None:
+                    result.producer = current
+
+                assert isinstance(result.producer.inputs, tuple)
+                base = tag
+                counter = 0
+                while tag in current.outputs:
+                    counter += 1
+                    tag = '%s_%d' % (base, counter)
+
+                current.add_output(result, tag)
+        except Exception as r:
+            logging.error('unexpected error: %s' % repr(r))
+            raise r
+        return p_valueish_result
+
+    @staticmethod
+    def expand(transform,  # type: PTransform
+               input,
+               options,  # type: PipelineOptions
+               ):
+        # sp_transform = self.load_spark_transform(transform)
+        return transform.expand(input)
+
+
+class AppliedPTransform(object):
+    """
+    A transform node representing an instance of applying a PTransform
+    """
+
+    def __init__(self,
+                 parent,  # type: Optional[AppliedPTransform]
+                 transform,  # type: Optional[ptransform],
+                 full_label,  # type: str
+                 main_inputs,  # type: Optional[Mapping[str, Union[pvalue.PBegin, pvalue.PCollection]]]
+                 environment_id=None,  # type: Optional[str]
+                 annotations=None,  # type: Optional[Dict[str, bytes]]
+                 is_root=False  # type: bool
+                 ):
+        # type: (...) -> None
+        self.parent = parent
+        self.transform = transform
+        self.full_label = full_label
+        self.main_input = dict(main_inputs or {})
+
+        self.side_input = tuple() if transform is None else transform.side_inputs
+        self.outputs = {}  # type: Dict[Union[str, int, None], pvalue.PValue]
+        self.parts = []  # type: List[AppliedPTransform]
+        self.environment_id = environment_id if environment_id else None  # type: Optional[str]
+        self._is_root = is_root
+
+    @property
+    def inputs(self):
+        # type: () -> tuple[Union[pvalue.PBegin, pvalue.PCollection]]
+        return tuple(self.main_input.values())
+
+    def is_root(self):
+        # type: () -> bool
+        return self._is_root
+
+    def __repr__(self):
+        # type: () -> str
+        return "%s(%s, %s)" % (
+            self.__class__.__name__, self.full_label, type(self.transform).__name__)
+
+    def add_output(self,
+                   output,  # type: Union[pvalue.PValue]
+                   tag  # type: Union[str, int, None]
+                   ):
+        # (...) -> None
+        if isinstance(output, pvalue.PValue):
+            if tag not in self.outputs:
+                self.outputs[tag] = output
+            else:
+                raise error.TransformError('tag[%s] has existed in outputs')
+        else:
+            raise TypeError("Unexpected out type: %s" % output)
+
+    def add_part(self, part):
+        # type: (AppliedPTransform) -> None
+        assert isinstance(part, AppliedPTransform)
+        self.parts.append(part)
+
+    def is_composite(self):
+        # type: () -> bool
+        return bool(self.parts) or all(
+            p_val.producer is not self for p_val in self.outputs.values()
+        )
+
+    def visit(self,
+              visitor,  # type: PipelineVisitor
+              ):
+        # type: (...) -> None
+        """Visits all nodes reachable from the current node."""
+        if self._is_root and self.outputs and self.outputs['__root']:
+            root = self.outputs['__root']
+            assert isinstance(root, pvalue.PValue)
+            for consumer in root.consumers:
+                consumer.visit(visitor)
+        elif visitor.visit_transform(self) and self.outputs:
+            for p_value in self.outputs.values():
+                assert isinstance(p_value, pvalue.PValue)
+                p_value.visit(visitor)
+        visitor.leave_transform(self)
+
+
+class ComponentIdMap(object):
+    """
+    A utility for assigning unique component ids to Beam components.
+
+    Component ID assignments are only guaranteed to be unique and consistent
+    within the scope of a ComponentIdMap instance.
+    """
+
+    def __init__(self, namespace="ref"):
+        self.namespace = namespace
+        self._counters = defaultdict(lambda: 0)  # type:Dict[type, int]
+        self._obj_to_id = {}  # type: Dict[Any, str]
+
+    def get_or_assign(self, obj=None, obj_type=None, label=None):
+        if obj not in self._obj_to_id:
+            self._obj_to_id[obj] = self._unique_ref(obj, obj_type, label)
+        return self._obj_to_id[obj]
+
+    def _unique_ref(self, obj=None, obj_type=None, label=None):
+        # Normalize, trim, and unify.
+        prefix = self._normalize(
+            "%s_%s_%s" % (self.namespace, obj_type.__name__, label or type(obj).__name__)
+        )[0:100]
+        self._counters[obj_type] += 1
+        return '%s_%d' % (prefix, self._counters[obj_type])
+
+    @staticmethod
+    def _normalize(str_value):
+        str_value = unicodedata.normalize('NFC', str_value)
+        return re.sub(r'[^a-zA-Z0-9-_]+', '-', str_value)
+
+
+class PipelineVisitor(object):
+    """
+    Visitor pattern class used to traverse a DAG of transforms
+    """
+
+    def __init__(self):
+        self.stream_writers = list()
+        self.module = None
+        self.__trans_cache = dict()  # type: dict[PTransform, PTransform]
+
+    def load_spark_transform(self,  # type: PipelineVisitor
+                             transform,  # type: PTransform,
+                             options=None,  # type: PipelineOptions
+                             **kwargs,
+                             ):
+        # type: (...) -> PTransform
+        # cache first
+        if self.__trans_cache.__contains__(transform):
+            return self.__trans_cache[transform]
+
+        # create new PTransform
+        if not self.module:
+            self.module = importlib.import_module(self.transform_package(options))
+        d = getattr(self.module, transform.__class__.__name__)
+        if d:
+            all_kwargs = dict()
+            if 'options' in d.__dict__['__init__'].__code__.co_varnames:
+                all_kwargs['options'] = options
+            for key in kwargs.keys():
+                if key in d.__dict__['__init__'].__code__.co_varnames:
+                    all_kwargs[key] = kwargs[key]
+            sp_trans = d(transform, **all_kwargs)
+            self.__trans_cache[transform] = sp_trans
+            return sp_trans
+        else:
+            raise NotImplementedError(
+                "transform [%s] not implemented by Spark!" % transform.__class__.__name__)
+
+    @staticmethod
+    def transform_package(options):
+        if options is None:
+            raise error.PipelineError("load_spark_transform pipeline options is null!")
+        return options.transform_package
+
+    def visit_value(self, value):
+        # type: (pvalue.PValue) -> bool
+        """
+        Callback for visiting a PValue in the pipeline DAG.
+        :param value: PValue visited (typically a PCollection instance).
+        :return:
+        """
+        return True
+
+    def visit_transform(self, transform_node):
+        # type: (AppliedPTransform) -> bool
+        return True
+
+    def leave_transform(self, transform_node):
+        # type: (AppliedPTransform) -> None
+        pass
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/runners/spark_runner.py` & `rondsspark-0.0.4.7/ronds_sdk/runners/spark_runner.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import logging
-
-from pyspark.sql import SparkSession
-
-from ronds_sdk.pipeline import PipelineVisitor
-from ronds_sdk.dataframe import pvalue
-from ronds_sdk.runners.runner import PipelineRunner, PipelineResult
-from ronds_sdk.runners.visitors.spark_runner_visitor import SparkRunnerVisitor
-from ronds_sdk.options.pipeline_options import PipelineOptions, SparkRunnerOptions
-
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from ronds_sdk.transforms.ptransform import PTransform
-
-
-class SparkRunner(PipelineRunner):
-
-    def __init__(self,
-                 options  # type: PipelineOptions
-                 ):
-        super(SparkRunner, self).__init__(options)
-        import findspark
-        findspark.init()
-        self.spark_options = self.options.view_as(SparkRunnerOptions)
-        self.spark = self.new_spark(self.spark_options)
-
-    @staticmethod
-    def new_spark(options):
-        builder = SparkSession.builder
-        logging.info("spark master url: %s" % options.spark_master_url)
-        if options.spark_master_url is not None:
-            builder.master(options.spark_master_url)
-        return builder.getOrCreate()
-
-    def transform_package(self):
-        return self.spark_options.spark_transform_package
-
-    def run_pipeline(self, pipeline, options):
-        visitor = SparkRunnerVisitor(self.options, self.spark)
-        pipeline.visit(visitor)
-        stream_writers = visitor.stream_writers
-        return SparkPipelineResult(stream_writers, 'STARTED')
-
-    def apply(self,
-              transform,  # type: PTransform
-              input,
-              options,  # type: PipelineOptions
-              ):
-        # sp_transform = self.load_spark_transform(transform)
-        return transform.expand(input)
-
-
-class SparkPipelineVisitor(PipelineVisitor):
-
-    def visit_value(self, value):
-        # type: (pvalue.PValue) -> bool
-        if isinstance(value, pvalue.PDone):
-            if value.stream_writer:
-                self.stream_writers.append(value.stream_writer)
-        return super().visit_value(value)
-
-
-class SparkPipelineResult(PipelineResult):
-
-    def __init__(self,
-                 stream_writers,
-                 state,
-                 ):
-        super(SparkPipelineResult, self).__init__(state)
-        self._stream_writers = stream_writers
-
-    def wait_until_finish(self, duration=None):
-        await_list = list()
-        if self._stream_writers:
-            for w in self._stream_writers:
-                query = w.start()
-                await_list.append(query)
-                logging.warning("query started, attention please ~")
-        if await_list:
-            for query in await_list:
-                query.awaitTermination()
+import logging
+
+from pyspark.sql import SparkSession
+
+from ronds_sdk.pipeline import PipelineVisitor
+from ronds_sdk.dataframe import pvalue
+from ronds_sdk.runners.runner import PipelineRunner, PipelineResult
+from ronds_sdk.runners.visitors.spark_runner_visitor import SparkRunnerVisitor
+from ronds_sdk.options.pipeline_options import PipelineOptions, SparkRunnerOptions
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ronds_sdk.transforms.ptransform import PTransform
+
+
+class SparkRunner(PipelineRunner):
+
+    def __init__(self,
+                 options  # type: PipelineOptions
+                 ):
+        super(SparkRunner, self).__init__(options)
+        import findspark
+        findspark.init()
+        self.spark_options = self.options.view_as(SparkRunnerOptions)
+        self.spark = self.new_spark(self.spark_options)
+
+    @staticmethod
+    def new_spark(options):
+        builder = SparkSession.builder
+        logging.info("spark master url: %s" % options.spark_master_url)
+        if options.spark_master_url is not None:
+            builder.master(options.spark_master_url)
+        return builder.getOrCreate()
+
+    def transform_package(self):
+        return self.spark_options.spark_transform_package
+
+    def run_pipeline(self, pipeline, options):
+        visitor = SparkRunnerVisitor(self.options, self.spark)
+        pipeline.visit(visitor)
+        stream_writers = visitor.stream_writers
+        return SparkPipelineResult(stream_writers, 'STARTED')
+
+    def apply(self,
+              transform,  # type: PTransform
+              input,
+              options,  # type: PipelineOptions
+              ):
+        # sp_transform = self.load_spark_transform(transform)
+        return transform.expand(input)
+
+
+class SparkPipelineVisitor(PipelineVisitor):
+
+    def visit_value(self, value):
+        # type: (pvalue.PValue) -> bool
+        if isinstance(value, pvalue.PDone):
+            if value.stream_writer:
+                self.stream_writers.append(value.stream_writer)
+        return super().visit_value(value)
+
+
+class SparkPipelineResult(PipelineResult):
+
+    def __init__(self,
+                 stream_writers,
+                 state,
+                 ):
+        super(SparkPipelineResult, self).__init__(state)
+        self._stream_writers = stream_writers
+
+    def wait_until_finish(self, duration=None):
+        await_list = list()
+        if self._stream_writers:
+            for w in self._stream_writers:
+                query = w.start()
+                await_list.append(query)
+                logging.warning("query started, attention please ~")
+        if await_list:
+            for query in await_list:
+                query.awaitTermination()
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/runners/visitors/spark_runner_visitor.py` & `rondsspark-0.0.4.7/ronds_sdk/runners/visitors/spark_runner_visitor.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import logging
-
-from typing import TYPE_CHECKING, List
-from ronds_sdk import error
-from ronds_sdk.dataframe import pvalue
-from ronds_sdk.options.pipeline_options import PipelineOptions
-from ronds_sdk.tools.utils import ForeachBatchFunc
-from ronds_sdk.pipeline import PipelineVisitor
-from ronds_sdk.transforms.ptransform import PTransform, ForeachBatchTransform
-
-if TYPE_CHECKING:
-    from ronds_sdk.pipeline import AppliedPTransform
-    from pyspark.sql import SparkSession
-
-
-def foreach_batch(df,
-                  epoch_id,  # type: str
-                  transform_root,  # type: AppliedPTransform
-                  options,  # type: PipelineOptions
-                  ):
-    logging.info("batch_id: %s, consumer size: %d"
-                 % (epoch_id, len(transform_root.outputs)))
-    for p_coll in transform_root.outputs.values():
-        p_coll.element_value = df
-        p_coll.tag = epoch_id
-        # todo 如果包含不可序列化对象, 此处会报序列化异常
-        p_coll.visit(SparkRunnerVisitor(options))
-
-
-class SparkRunnerVisitor(PipelineVisitor):
-    def __init__(self,
-                 options,  # type: PipelineOptions
-                 spark=None,  # type: SparkSession
-                 ):
-        super(SparkRunnerVisitor, self).__init__()
-        self._options = options
-        self._spark = spark
-
-    def visit_transform(self, transform_node):
-        # type: (AppliedPTransform) -> bool
-        transform = transform_node.transform  # type: PTransform
-        sp_transform = self.load_spark_transform(transform, self._options, spark=self._spark)
-        input_or_inputs = transform.extract_input_if_one_p_values(transform_node.inputs)
-        # process SourceTransform
-        p_coll = transform_node.outputs.get(None)
-        if isinstance(sp_transform, ForeachBatchTransform):
-            p_coll.is_bounded = True
-            return self.visit_foreach_batch(sp_transform, transform_node, input_or_inputs)
-
-        # process PTransform
-        sp_coll = sp_transform.expand(input_or_inputs)
-        if sp_coll is None:
-            raise error.TransformError('Transform [%s] expand return None error!'
-                                       % sp_transform.__class__.__name__)
-        assert isinstance(sp_coll, pvalue.PValue)
-        p_coll.element_value = sp_coll.element_value
-        first_input = transform.extract_first_input_p_values(input_or_inputs)
-        p_coll.is_bounded = first_input.is_bounded
-        return super().visit_transform(transform_node)
-
-    def visit_foreach_batch(self,
-                            sp_transform,  # type: PTransform
-                            transform_node,  # type: AppliedPTransform
-                            first_input,  # type: pvalue.PValue
-                            ):
-        #  type: (...) -> bool
-        p_coll = sp_transform.expand(first_input,
-                                     ForeachBatchFunc(foreach_batch,
-                                                      transform_root=transform_node,
-                                                      options=self._options))
-        if isinstance(p_coll, pvalue.PDone):
-            self.stream_writers.append(p_coll.stream_writer)
-        else:
-            raise error.TransformError(
-                "PDone output of SourceTransform expected, but [%s]" % p_coll)
-        return False
-
-    @staticmethod
-    def get_first_output(transform_node  # type: AppliedPTransform
-                         ):
-        # type: (...) -> pvalue.PValue
-        if transform_node.outputs:
-            return next(iter(transform_node.outputs.values()))
-
-    @staticmethod
-    def is_stream_begin(p_values: List[pvalue.PValue]):
-        if p_values and len(p_values) == 1:
-            return not p_values[0].is_bounded
-        return False
+import logging
+
+from typing import TYPE_CHECKING, List
+from ronds_sdk import error
+from ronds_sdk.dataframe import pvalue
+from ronds_sdk.options.pipeline_options import PipelineOptions
+from ronds_sdk.tools.utils import ForeachBatchFunc
+from ronds_sdk.pipeline import PipelineVisitor
+from ronds_sdk.transforms.ptransform import PTransform, ForeachBatchTransform
+
+if TYPE_CHECKING:
+    from ronds_sdk.pipeline import AppliedPTransform
+    from pyspark.sql import SparkSession
+
+
+def foreach_batch(df,
+                  epoch_id,  # type: str
+                  transform_root,  # type: AppliedPTransform
+                  options,  # type: PipelineOptions
+                  ):
+    logging.info("batch_id: %s, consumer size: %d"
+                 % (epoch_id, len(transform_root.outputs)))
+    for p_coll in transform_root.outputs.values():
+        p_coll.element_value = df
+        p_coll.tag = epoch_id
+        # todo 如果包含不可序列化对象, 此处会报序列化异常
+        p_coll.visit(SparkRunnerVisitor(options))
+
+
+class SparkRunnerVisitor(PipelineVisitor):
+    def __init__(self,
+                 options,  # type: PipelineOptions
+                 spark=None,  # type: SparkSession
+                 ):
+        super(SparkRunnerVisitor, self).__init__()
+        self._options = options
+        self._spark = spark
+
+    def visit_transform(self, transform_node):
+        # type: (AppliedPTransform) -> bool
+        transform = transform_node.transform  # type: PTransform
+        sp_transform = self.load_spark_transform(transform, self._options, spark=self._spark)
+        input_or_inputs = transform.extract_input_if_one_p_values(transform_node.inputs)
+        # process SourceTransform
+        p_coll = transform_node.outputs.get(None)
+        if isinstance(sp_transform, ForeachBatchTransform):
+            p_coll.is_bounded = True
+            return self.visit_foreach_batch(sp_transform, transform_node, input_or_inputs)
+
+        # process PTransform
+        sp_coll = sp_transform.expand(input_or_inputs)
+        if sp_coll is None:
+            raise error.TransformError('Transform [%s] expand return None error!'
+                                       % sp_transform.__class__.__name__)
+        assert isinstance(sp_coll, pvalue.PValue)
+        p_coll.element_value = sp_coll.element_value
+        first_input = transform.extract_first_input_p_values(input_or_inputs)
+        p_coll.is_bounded = first_input.is_bounded
+        return super().visit_transform(transform_node)
+
+    def visit_foreach_batch(self,
+                            sp_transform,  # type: PTransform
+                            transform_node,  # type: AppliedPTransform
+                            first_input,  # type: pvalue.PValue
+                            ):
+        #  type: (...) -> bool
+        p_coll = sp_transform.expand(first_input,
+                                     ForeachBatchFunc(foreach_batch,
+                                                      transform_root=transform_node,
+                                                      options=self._options))
+        if isinstance(p_coll, pvalue.PDone):
+            self.stream_writers.append(p_coll.stream_writer)
+        else:
+            raise error.TransformError(
+                "PDone output of SourceTransform expected, but [%s]" % p_coll)
+        return False
+
+    @staticmethod
+    def get_first_output(transform_node  # type: AppliedPTransform
+                         ):
+        # type: (...) -> pvalue.PValue
+        if transform_node.outputs:
+            return next(iter(transform_node.outputs.values()))
+
+    @staticmethod
+    def is_stream_begin(p_values: List[pvalue.PValue]):
+        if p_values and len(p_values) == 1:
+            return not p_values[0].is_bounded
+        return False
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/cassandra_rule.py` & `rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/cassandra_rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,165 +1,176 @@
-import datetime
-import logging
-import time
-import traceback
-from functools import lru_cache
-
-import pandas as pd
-from cassandra.cluster import ResultSet
-
-from ronds_sdk.datasources.cassandra_manager import ProcessDataManager
-from ronds_sdk.options.pipeline_options import CassandraOptions
-from ronds_sdk.tools.utils import RuleParser, ForeachBatchFunc, WrapperFunc
-from ronds_sdk.transforms.pandas.rule_merge_data import RuleData
-
-
-class DatetimeHolder(object):
-    def __init__(self,
-                 d_time,  # type: datetime.datetime
-                 ):
-        self._d_time = d_time
-
-    def datetime(self):
-        return self._d_time
-
-    def update(self, new_d_time):
-        """
-        update time by new_d_time that is less or equal now(), otherwise set now()
-        :param new_d_time:
-        :return:
-        """
-        c_d_time = datetime.datetime.today()
-        if new_d_time > c_d_time:
-            self._d_time = c_d_time
-        else:
-            self._d_time = new_d_time
-
-
-class ForeachRule(object):
-    def __init__(self,
-                 c_options,  # type: CassandraOptions
-                 action_func,  # type: WrapperFunc
-                 ):
-        self.c_options = c_options
-        self.action_func = action_func
-
-    def foreach_rules(self,
-                      rules,
-                      ):
-        if self.c_options.enable_executor_debug:
-            # enable spark executor debug, only for test
-            import pydevd_pycharm
-            pydevd_pycharm.settrace('localhost', port=12345, stdoutToServer=True, stderrToServer=True)
-        import schedule
-        interval_seconds = self.c_options.cassandra_window_duration
-        current_timestamp = datetime.datetime.today() \
-            if self.c_options.cassandra_start_datetime is None \
-            else datetime.datetime.strptime(
-            self.c_options.cassandra_start_datetime, RuleParser.datetime_format()
-        )
-        end_datetime_holder = DatetimeHolder(current_timestamp)
-        process_manager = ProcessDataManager(self.c_options)
-
-        # iter to tuple
-        rules = self.iter_to_list(rules)
-
-        # schedule task
-        schedule.every(interval_seconds).seconds.do(self.rule_task,
-                                                    rules=rules,
-                                                    process_manager=process_manager,
-                                                    end_datetime_holder=end_datetime_holder,
-                                                    interval_seconds=interval_seconds,
-                                                    action_func=self.action_func)
-        while True:
-            logging.info("running pending ~")
-            schedule.run_pending()
-            time.sleep(5)
-
-    def rule_task(self,
-                  rules,
-                  process_manager,  # type: ProcessDataManager
-                  end_datetime_holder,  # type: DatetimeHolder
-                  interval_seconds,  # type: int
-                  action_func,  # type: ForeachBatchFunc
-                  ):
-        # noinspection PyBroadException
-        try:
-            end_datetime = end_datetime_holder.datetime()
-            delta = datetime.timedelta(seconds=interval_seconds)
-            start_datetime = end_datetime - delta
-            end_datetime_str = end_datetime.strftime(RuleParser.datetime_format())
-            logging.info("start_time: %s, end_time: %s" % (
-                start_datetime.strftime(RuleParser.datetime_format()),
-                end_datetime_str))
-
-            # process rules
-            result_list = list()
-            for rule in rules:
-                uid_list = self.get_point_id_list(rule)
-                device_id = rule.assetId
-                logging.info("uid_list size: %s" % len(uid_list))
-                if len(uid_list) == 0:
-                    continue
-                result_set = process_manager.window_select(uid_list, start_datetime, end_datetime)
-                rule_data = self.transform_to_rule_data_pd(result_set, device_id)
-                if rule_data is not None:
-                    result_list.append(rule_data)
-                del result_set
-            p_dataframe = pd.DataFrame(result_list)
-            action_func.call(df=p_dataframe, epoch_id=end_datetime_str)
-
-            # update end_datetime
-            end_datetime_holder.update(end_datetime + delta)
-        except Exception as ex:
-            logging.error("rule_task error: \n%s" % traceback.format_exc())
-
-    @staticmethod
-    def transform_to_rule_data_pd(process_result_set: ResultSet, device_id: str) -> dict:
-        rule_data = None
-        for r in process_result_set:
-            if r.time is None or r.value is None:
-                continue
-            if rule_data is None:
-                rule_data = RuleData(device_id)
-            rule_data.add_process_data(str(r.id),
-                                       r.time.strftime(RuleParser.datetime_format()),
-                                       r.value)
-        return rule_data.get_data() if rule_data is not None else None
-
-    @lru_cache(maxsize=100)
-    def scan_cassandra(self,
-                       process_manager,  # type: ProcessDataManager
-                       uid_list,  # type: tuple[str]
-                       start_time,  # type: datetime.datetime
-                       end_time,  # type: datetime.datetime
-                       ):
-        #  type: (...) -> ResultSet
-        """
-        maybe useful but memory dangerous, for future
-        :param process_manager: 工艺查询管理
-        :param uid_list: 测点 id 列表
-        :param start_time: 开始时间
-        :param end_time: 结束时间
-        :return: ResultSet
-        """
-        return process_manager.window_select(uid_list, start_time, end_time)
-
-    @staticmethod
-    def iter_to_list(rules):
-        res_list = list()
-        for r in rules:
-            res_list.append(r)
-        return res_list
-
-    @staticmethod
-    def get_point_id_list(rule,
-                          ):
-        if 'points' not in rule.__fields__:
-            return None
-        p_list = list()
-        for point in rule.points:
-            assert isinstance(point, dict)
-            if not point.__contains__('pointId'):
-                continue
-            p_list.append(point['pointId'])
-        return p_list
+import datetime
+import logging
+import time
+import traceback
+from functools import lru_cache
+
+import pandas as pd
+from cassandra.cluster import ResultSet
+
+from ronds_sdk import error
+from ronds_sdk.datasources.cassandra_manager import ProcessDataManager
+from ronds_sdk.options.pipeline_options import CassandraOptions
+from ronds_sdk.tools.schedule import Scheduler
+from ronds_sdk.tools.utils import RuleParser, ForeachBatchFunc, WrapperFunc
+from ronds_sdk.transforms.pandas.rule_merge_data import RuleData
+
+
+class DatetimeHolder(object):
+    def __init__(self,
+                 d_time,  # type: datetime.datetime
+                 ):
+        self._d_time = d_time
+
+    def datetime(self):
+        return self._d_time
+
+    def update(self, new_d_time):
+        """
+        update time by new_d_time that is less or equal now(), otherwise set now()
+        :param new_d_time:
+        :return:
+        """
+        c_d_time = datetime.datetime.today()
+        if new_d_time > c_d_time:
+            self._d_time = c_d_time
+        else:
+            self._d_time = new_d_time
+
+
+class ForeachRule(object):
+    def __init__(self,
+                 c_options,  # type: CassandraOptions
+                 action_func,  # type: WrapperFunc
+                 ):
+        self.c_options = c_options
+        self.action_func = action_func
+        self.scheduler = Scheduler()
+
+    def foreach_rules(self,
+                      rules,
+                      ):
+        from ronds_sdk import logger_config
+        logger_config.config()
+
+        if self.c_options.enable_executor_debug:
+            # enable spark executor debug, only for test
+            import pydevd_pycharm
+            pydevd_pycharm.settrace('localhost', port=12345, stdoutToServer=True, stderrToServer=True)
+
+        interval_seconds = self.c_options.cassandra_window_duration
+        current_timestamp = datetime.datetime.today() \
+            if self.c_options.cassandra_start_datetime is None \
+            else datetime.datetime.strptime(
+            self.c_options.cassandra_start_datetime, RuleParser.datetime_format()
+        )
+        end_datetime_holder = DatetimeHolder(current_timestamp)
+        process_manager = ProcessDataManager(self.c_options)
+
+        # iter to tuple
+        rules = self.iter_to_list(rules)
+
+        # schedule task
+        self.scheduler.every(interval_seconds).seconds.do(self.rule_task,
+                                                          rules=rules,
+                                                          process_manager=process_manager,
+                                                          end_datetime_holder=end_datetime_holder,
+                                                          interval_seconds=interval_seconds,
+                                                          action_func=self.action_func)
+        last_ex = None
+        while True:
+            # noinspection PyBroadException
+            try:
+                logging.info("running pending ~")
+                self.scheduler.run_pending()
+            except error.KafkaError:
+                logging.error("rule_task kafka error: \n%s" % traceback.format_exc())
+
+            except Exception:
+                logging.error("rule_task error: \n%s" % traceback.format_exc())
+            finally:
+                time.sleep(5)
+
+    def rule_task(self,
+                  rules,
+                  process_manager,  # type: ProcessDataManager
+                  end_datetime_holder,  # type: DatetimeHolder
+                  interval_seconds,  # type: int
+                  action_func,  # type: ForeachBatchFunc
+                  ):
+        end_datetime = end_datetime_holder.datetime()
+        delta = datetime.timedelta(seconds=interval_seconds)
+        start_datetime = end_datetime - delta
+        end_datetime_str = end_datetime.strftime(RuleParser.datetime_format())
+        logging.info("start_time: %s, end_time: %s" % (
+            start_datetime.strftime(RuleParser.datetime_format()),
+            end_datetime_str))
+
+        # process rules
+        result_list = list()
+        for rule in rules:
+            uid_list = self.get_point_id_list(rule)
+            device_id = rule.assetId
+            logging.info("uid_list size: %s" % len(uid_list))
+            if len(uid_list) == 0:
+                continue
+            result_set = process_manager.window_select(uid_list, start_datetime, end_datetime)
+            rule_data = self.transform_to_rule_data_pd(result_set, device_id)
+            if rule_data is not None:
+                result_list.append(rule_data)
+            del result_set
+        p_dataframe = pd.DataFrame(result_list)
+        action_func.call(df=p_dataframe, epoch_id=end_datetime_str)
+
+        # update end_datetime
+        end_datetime_holder.update(end_datetime + delta)
+
+    @staticmethod
+    def transform_to_rule_data_pd(process_result_set: ResultSet, device_id: str) -> dict:
+        rule_data = None
+        for r in process_result_set:
+            if r.time is None or r.value is None:
+                continue
+            if rule_data is None:
+                rule_data = RuleData(device_id)
+            rule_data.add_process_data(str(r.id),
+                                       r.time.strftime(RuleParser.datetime_format()),
+                                       r.value)
+        return rule_data.get_data() if rule_data is not None else None
+
+    @lru_cache(maxsize=100)
+    def scan_cassandra(self,
+                       process_manager,  # type: ProcessDataManager
+                       uid_list,  # type: tuple[str]
+                       start_time,  # type: datetime.datetime
+                       end_time,  # type: datetime.datetime
+                       ):
+        #  type: (...) -> ResultSet
+        """
+        maybe useful but memory dangerous, for future
+        :param process_manager: 工艺查询管理
+        :param uid_list: 测点 id 列表
+        :param start_time: 开始时间
+        :param end_time: 结束时间
+        :return: ResultSet
+        """
+        return process_manager.window_select(uid_list, start_time, end_time)
+
+    @staticmethod
+    def iter_to_list(rules):
+        res_list = list()
+        for r in rules:
+            res_list.append(r)
+        return res_list
+
+    @staticmethod
+    def get_point_id_list(rule,
+                          ):
+        if 'points' not in rule.__fields__:
+            return None
+        p_list = list()
+        for point in rule.points:
+            assert isinstance(point, dict)
+            if not point.__contains__('pointId'):
+                continue
+            p_list.append(point['pointId'])
+        return p_list
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/transforms/pandas/rule_merge_data.py` & `rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/rule_merge_data.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from typing import Union
-
-
-# noinspection SpellCheckingInspection
-class RuleData(object):
-
-    def __init__(self,
-                 device_id,  # type: str
-                 nodes=None,  # type: list
-                 edges=None,  # type: list
-                 datasources=None,  # type: list
-                 indices=None,  # type: list
-                 events=None,  # type: list
-                 running_time=None,  # type: float
-                 datasource_times=None,  # type: str
-                 ):
-        """
-        根据规则读取 Cassandra 数据, 组合成算法能够识别的 JSON 格式数据
-        :param nodes: 设备 DAG nodes
-        :param edges: 设备 DAG edges
-        :param datasources: 数据源的具体数据
-        :param indices: 需要存储到 Cassandra 的数据
-        :param events: 需要发送到 Kafka 告警主题的数据
-        :param running_time: 运行时间
-        :param datasource_times: 数据源数据批次生成 时间
-        """
-        self._data_dict = {
-            'device_id': device_id,
-            'nodes': nodes if nodes else [],
-            'edges': edges if edges else [],
-            'datasource': datasources if datasources else [[]],
-            'version': '1.0.0',
-            'indices': indices if indices else [],
-            'events': events if events else [],
-            'runningtime': running_time if running_time else [],
-            'datasourcetimes': [datasource_times] if datasource_times else []
-        }
-        self._data_index = dict()
-
-    def get_data(self) -> dict:
-        return self._data_dict
-
-    def get_datasource(self) -> list:
-        return self._data_dict['datasource'][0]
-
-    def set_nodes(self, nodes: list) -> None:
-        if nodes:
-            self._data_dict['nodes'] = nodes
-
-    def set_edges(self, edges: list) -> None:
-        if edges:
-            self._data_dict['edges'] = edges
-
-    def add_process_data(self,  # type: RuleData
-                         asset_id,  # type: str
-                         c_time,  # type: str
-                         value,  # type: Union[float, int]
-                         data_type=106,  # type: int
-                         ):
-        # type: (...) -> None
-        """
-        添加工艺数据
-        :param asset_id: 测点 id
-        :param c_time: 数据产生时间
-        :param value: 数据内容
-        :param data_type: 数据类型, 默认工艺 data_type = 106
-        :return: None
-        """
-        if not self._data_index.__contains__(asset_id):
-            datasource = {
-                'assetid': asset_id,
-                'value': {
-                    'channeldata': {
-                        'code': '',
-                        'nodetype': '',
-                        'data': [],
-                        'assetid': asset_id,
-                        'caption': '',
-                        'property': {
-                            'sernortype': 0,
-                            'direct': '',
-                            'direction': 1
-                        }
-                    }
-                }
-            }
-            self._data_index[asset_id] = datasource
-            self.get_datasource().append(datasource)
-        datasource = self._data_index[asset_id]
-        self.fill_channel_data(data_type, asset_id, c_time, value, datasource)
-
-    @staticmethod
-    def get_data_key(*args) -> str:
-        return '_'.join([str(s) for s in args])
-
-    def fill_channel_data(self,  # type: RuleData
-                          data_type,  # type: int
-                          asset_id,  # type: str
-                          c_time,  # type: str
-                          value,  # type: float
-                          datasource,  # type: dict
-                          ):
-        # type: (...) -> None
-        """
-        按照格式填充 datasource.value.chaneldata.data 的数据
-        :param value: 工艺数据值
-        :param c_time: 数据产生时间
-        :param asset_id: 测点 id
-        :param data_type: 设备类型
-        :param datasource: 需要填充的 datasource
-        """
-        channel_data_key = self.get_data_key(asset_id, data_type)
-        if not self._data_index.__contains__(channel_data_key):
-            channel_data = {
-                'times': [],
-                'values': [],
-                'datatype': data_type,
-                'indexcode': -1,
-                'conditions': [],
-                'properties': []
-            }
-            self._data_index[channel_data_key] = channel_data
-            datasource['value']['channeldata']['data'].append(channel_data)
-        channel_data = self._data_index[channel_data_key]
-        channel_data['times'].append(c_time)
-        channel_data['values'].append(value)
+from typing import Union
+
+
+# noinspection SpellCheckingInspection
+class RuleData(object):
+
+    def __init__(self,
+                 device_id,  # type: str
+                 nodes=None,  # type: list
+                 edges=None,  # type: list
+                 datasources=None,  # type: list
+                 indices=None,  # type: list
+                 events=None,  # type: list
+                 running_time=None,  # type: float
+                 datasource_times=None,  # type: str
+                 ):
+        """
+        根据规则读取 Cassandra 数据, 组合成算法能够识别的 JSON 格式数据
+        :param nodes: 设备 DAG nodes
+        :param edges: 设备 DAG edges
+        :param datasources: 数据源的具体数据
+        :param indices: 需要存储到 Cassandra 的数据
+        :param events: 需要发送到 Kafka 告警主题的数据
+        :param running_time: 运行时间
+        :param datasource_times: 数据源数据批次生成 时间
+        """
+        self._data_dict = {
+            'device_id': device_id,
+            'nodes': nodes if nodes else [],
+            'edges': edges if edges else [],
+            'datasource': datasources if datasources else [[]],
+            'version': '1.0.0',
+            'indices': indices if indices else [],
+            'events': events if events else [],
+            'runningtime': running_time if running_time else [],
+            'datasourcetimes': [datasource_times] if datasource_times else []
+        }
+        self._data_index = dict()
+
+    def get_data(self) -> dict:
+        return self._data_dict
+
+    def get_datasource(self) -> list:
+        return self._data_dict['datasource'][0]
+
+    def set_nodes(self, nodes: list) -> None:
+        if nodes:
+            self._data_dict['nodes'] = nodes
+
+    def set_edges(self, edges: list) -> None:
+        if edges:
+            self._data_dict['edges'] = edges
+
+    def add_process_data(self,  # type: RuleData
+                         asset_id,  # type: str
+                         c_time,  # type: str
+                         value,  # type: Union[float, int]
+                         data_type=106,  # type: int
+                         ):
+        # type: (...) -> None
+        """
+        添加工艺数据
+        :param asset_id: 测点 id
+        :param c_time: 数据产生时间
+        :param value: 数据内容
+        :param data_type: 数据类型, 默认工艺 data_type = 106
+        :return: None
+        """
+        if not self._data_index.__contains__(asset_id):
+            datasource = {
+                'assetid': asset_id,
+                'value': {
+                    'channeldata': {
+                        'code': '',
+                        'nodetype': '',
+                        'data': [],
+                        'assetid': asset_id,
+                        'caption': '',
+                        'property': {
+                            'sernortype': 0,
+                            'direct': '',
+                            'direction': 1
+                        }
+                    }
+                }
+            }
+            self._data_index[asset_id] = datasource
+            self.get_datasource().append(datasource)
+        datasource = self._data_index[asset_id]
+        self.fill_channel_data(data_type, asset_id, c_time, value, datasource)
+
+    @staticmethod
+    def get_data_key(*args) -> str:
+        return '_'.join([str(s) for s in args])
+
+    def fill_channel_data(self,  # type: RuleData
+                          data_type,  # type: int
+                          asset_id,  # type: str
+                          c_time,  # type: str
+                          value,  # type: float
+                          datasource,  # type: dict
+                          ):
+        # type: (...) -> None
+        """
+        按照格式填充 datasource.value.chaneldata.data 的数据
+        :param value: 工艺数据值
+        :param c_time: 数据产生时间
+        :param asset_id: 测点 id
+        :param data_type: 设备类型
+        :param datasource: 需要填充的 datasource
+        """
+        channel_data_key = self.get_data_key(asset_id, data_type)
+        if not self._data_index.__contains__(channel_data_key):
+            channel_data = {
+                'times': [],
+                'values': [],
+                'datatype': data_type,
+                'indexcode': -1,
+                'conditions': [],
+                'properties': []
+            }
+            self._data_index[channel_data_key] = channel_data
+            datasource['value']['channeldata']['data'].append(channel_data)
+        channel_data = self._data_index[channel_data_key]
+        channel_data['times'].append(c_time)
+        channel_data['values'].append(value)
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/transforms/ptransform.py` & `rondsspark-0.0.4.7/ronds_sdk/transforms/ptransform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,210 +1,233 @@
-from typing import TypeVar, Generic, Sequence, Optional, Callable, Union
-
-from ronds_sdk import error
-from ronds_sdk.dataframe import pvalue
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from ronds_sdk.pipeline import Pipeline, AppliedPTransform
-    from ronds_sdk.tools.utils import WrapperFunc
-
-
-InputT = TypeVar('InputT')
-OutputT = TypeVar('OutputT')
-PTransformT = TypeVar('PTransformT', bound='PTransform')
-
-
-class PTransform(object):
-    # 默认, transform 不包含 side inputs
-    side_inputs = ()  # type: Sequence[pvalue.AsSideInput]
-
-    # used for nullity transforms
-    pipeline = None  # type: Optional[Pipeline]
-
-    # Default is unset
-    _user_label = None  # type:  Optional[str]
-
-    def __init__(self, label=None):
-        # type:  (Optional[str]) -> None
-        super().__init__()
-        self.label = label
-
-    @property
-    def label(self):
-        # type:  () -> str
-        return self._user_label or self.default_label()
-
-    @label.setter
-    def label(self, value):
-        # type: (Optional[str]) -> None
-        self._user_label = value
-
-    def default_label(self):
-        # type: () -> str
-        return self.__class__.__name__
-
-    def expand(self,
-               input_inputs,  # type: InputT
-               action_func=None  # type: WrapperFunc
-               ):
-        # type: (...) -> OutputT
-        raise NotImplementedError
-
-    def __str__(self):
-        return '<%s>' % self._str_internal()
-
-    def __repr__(self):
-        return '<%s at %s>' % (self._str_internal(), hex(id(self)))
-
-    def _str_internal(self) -> str:
-        return '%s(PTransform)%s%s%s' % (
-            self.__class__.__name__,
-            ' label=[%s]' % self.label if (hasattr(self, 'label') and self.label) else '',
-            ' inputs=%s ' % str(self.inputs) if (hasattr(self, 'inputs') and self.inputs) else '',
-            ' side_inputs=%s' % str(self.side_inputs) if self.side_inputs else ''
-        )
-
-    def __rrshift__(self, label):
-        return _NamedPTransform(self, label)
-
-    def __or__(self, right):
-        """Used to compose PTransforms, e.g., ptransform1 | ptransform2."""
-        if isinstance(right, PTransform):
-            return _ChainedPTransform(self, right)
-        return NotImplemented
-
-    def __ror__(self, left, label):
-        p_valueish, p_values = self._extract_input_p_values(left)
-        if isinstance(p_values, dict):
-            p_values = tuple(p_values.values())
-        pipelines = [v.pipeline for v in p_values if isinstance(v, pvalue.PValue)]
-        if not pipelines:
-            if self.pipeline is not None:
-                p = self.pipeline
-            else:
-                raise ValueError('"%s" requires a pipeline to be specified '
-                                 'as there are no deferred inputs.' % self.label)
-        else:
-            p = self.pipeline or pipelines[0]
-            for pp in pipelines:
-                if p != pp:
-                    raise ValueError(
-                        'Mixing values in different pipelines is not allowed.'
-                        '\n{%r} != {%r}' % (p, pp))
-        # deferred = not getattr(p.runner, 'is_eager', False)
-        self.pipeline = p
-        result = p.apply(self, p_valueish, label)
-        return result
-
-    @staticmethod
-    def extract_input_if_one_p_values(input_inputs) -> pvalue.PValue:
-        """
-        In most scenarios, if Collection contain one element, return the element directly
-        :param input_inputs: inputs
-        :return:
-        """
-
-        if isinstance(input_inputs, tuple) or isinstance(input_inputs, list):
-            return input_inputs[0] if len(input_inputs) == 1 else input_inputs
-        elif isinstance(input_inputs, dict):
-            return next(iter(input_inputs.values())) if len(input_inputs) == 1 else input_inputs
-        return input_inputs
-
-    @staticmethod
-    def extract_first_input_p_values(input_inputs) -> pvalue.PValue:
-        """
-        extract first input for use
-        :param input_inputs: inputs
-        :return: first input
-        """
-        if isinstance(input_inputs, tuple) or isinstance(input_inputs, list):
-            return input_inputs[0]
-        elif isinstance(input_inputs, dict):
-            return next(iter(input_inputs.values()))
-        assert isinstance(input_inputs, pvalue.PValue)
-        return input_inputs
-
-    @staticmethod
-    def _extract_input_p_values(p_valueish):
-        from ronds_sdk import pipeline
-        if isinstance(p_valueish, pipeline.Pipeline):
-            if not p_valueish.root_transform.outputs:
-                p_begin = pvalue.PBegin(p_valueish)
-                p_valueish.root_transform.add_output(p_begin, '__root')
-            p_valueish = p_valueish.root_transform.outputs.get('__root')
-        return p_valueish, {
-            str(tag): value
-            for (tag, value) in get_named_nested_p_values(p_valueish, as_inputs=True)
-        }
-
-    @staticmethod
-    def _check_pcollection(p_coll):
-        # type: (pvalue.PCollection) -> None
-        if not isinstance(p_coll, pvalue.PCollection):
-            raise error.TransformError('Expecting a PCollection argument.')
-        if not p_coll.pipeline:
-            raise error.TransformError('PCollection not part of a pipeline')
-
-
-class ForeachBatchTransform(PTransform):
-
-    def expand(self, input_inputs, action_func=None):
-        raise NotImplementedError
-
-
-def get_named_nested_p_values(p_valueish, as_inputs=False):
-    if isinstance(p_valueish, tuple):
-        fields = getattr(p_valueish, '_fields', None)
-        if fields and len(fields) == len(p_valueish):
-            tagged_values = zip(fields, p_valueish)
-        else:
-            tagged_values = enumerate(p_valueish)
-    elif isinstance(p_valueish, list):
-        if as_inputs:
-            yield None, p_valueish
-            return
-        tagged_values = enumerate(p_valueish)
-    elif isinstance(p_valueish, dict):
-        tagged_values = p_valueish.items()
-    else:
-        if as_inputs or isinstance(p_valueish, pvalue.PValue):
-            yield None, p_valueish
-        return
-    for tag, sub_value in tagged_values:
-        for sub_tag, sub_sub_value in get_named_nested_p_values(
-                sub_value, as_inputs=as_inputs):
-            if sub_tag is None:
-                yield tag, sub_sub_value
-            else:
-                yield '%s.%s' % (tag, sub_tag), sub_sub_value
-
-
-class _NamedPTransform(PTransform):
-    def __init__(self, transform, label):
-        super().__init__(label)
-        self.transform = transform
-
-    def __ror__(self, p_valueish, _unused=None):
-        return self.transform.__ror__(p_valueish, self.label)
-
-    def expand(self, p_value):
-        raise RuntimeError("Should never be expanded directly.")
-
-
-class _ChainedPTransform(PTransform):
-    def __init__(self, *parts):
-        # type: (*PTransform) -> None
-        super().__init__(label=self._chain_label(parts))
-        self._parts = parts
-
-    @staticmethod
-    def _chain_label(parts):
-        return '|'.join(p.label for p in parts)
-
-    def __or__(self, right):
-        if isinstance(right, PTransform):
-            return _ChainedPTransform(*(self._parts + (right,)))
-        return NotImplemented
-
-    def expand(self, p_val):
-        raise NotImplementedError
+from typing import TypeVar, Generic, Sequence, Optional, Callable, Union
+
+from ronds_sdk import error
+from ronds_sdk.dataframe import pvalue
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ronds_sdk.pipeline import Pipeline, AppliedPTransform
+    from ronds_sdk.tools.utils import WrapperFunc
+
+
+InputT = TypeVar('InputT')
+OutputT = TypeVar('OutputT')
+PTransformT = TypeVar('PTransformT', bound='PTransform')
+
+
+class PTransform(object):
+    # 默认, transform 不包含 side inputs
+    side_inputs = ()  # type: Sequence[pvalue.AsSideInput]
+
+    # used for nullity transforms
+    pipeline = None  # type: Optional[Pipeline]
+
+    # Default is unset
+    _user_label = None  # type:  Optional[str]
+
+    def __init__(self, label=None):
+        # type:  (Optional[str]) -> None
+        super().__init__()
+        self.label = label
+
+    @property
+    def label(self):
+        # type:  () -> str
+        return self._user_label or self.default_label()
+
+    @label.setter
+    def label(self, value):
+        # type: (Optional[str]) -> None
+        self._user_label = value
+
+    def default_label(self):
+        # type: () -> str
+        return self.__class__.__name__
+
+    def expand(self,  # type: PTransform
+               input_inputs,  # type: InputT
+               action_func=None  # type: WrapperFunc
+               ):
+        # type: (...) -> OutputT
+        if not self.validate_input_inputs(input_inputs):
+            raise NotImplementedError(
+                "transform not implemented: %s" % self.__class__.__name__)
+        return pvalue.PCollection(input_inputs.pipeline,
+                                  element_type=pvalue.PCollection,
+                                  is_bounded=input_inputs.is_bounded,
+                                  )
+
+    @staticmethod
+    def validate_input_inputs(input_inputs,
+                              ):
+        if isinstance(input_inputs, pvalue.PValue):
+            return input_inputs.element_value is None
+        if isinstance(input_inputs, list):
+            for input in input_inputs:
+                if not isinstance(input, pvalue.PValue) \
+                        or input.element_value is not None:
+                    return False
+        if isinstance(input_inputs, dict):
+            for input in input_inputs.values():
+                if not isinstance(input, pvalue.PValue) \
+                        or input.element_value is not None:
+                    return False
+        return True
+
+    def __str__(self):
+        return '<%s>' % self._str_internal()
+
+    def __repr__(self):
+        return '<%s at %s>' % (self._str_internal(), hex(id(self)))
+
+    def _str_internal(self) -> str:
+        return '%s(PTransform)%s%s%s' % (
+            self.__class__.__name__,
+            ' label=[%s]' % self.label if (hasattr(self, 'label') and self.label) else '',
+            ' inputs=%s ' % str(self.inputs) if (hasattr(self, 'inputs') and self.inputs) else '',
+            ' side_inputs=%s' % str(self.side_inputs) if self.side_inputs else ''
+        )
+
+    def __rrshift__(self, label):
+        return _NamedPTransform(self, label)
+
+    def __or__(self, right):
+        """Used to compose PTransforms, e.g., ptransform1 | ptransform2."""
+        if isinstance(right, PTransform):
+            return _ChainedPTransform(self, right)
+        return NotImplemented
+
+    def __ror__(self, left, label):
+        p_valueish, p_values = self._extract_input_p_values(left)
+        if isinstance(p_values, dict):
+            p_values = tuple(p_values.values())
+        pipelines = [v.pipeline for v in p_values if isinstance(v, pvalue.PValue)]
+        if not pipelines:
+            if self.pipeline is not None:
+                p = self.pipeline
+            else:
+                raise ValueError('"%s" requires a pipeline to be specified '
+                                 'as there are no deferred inputs.' % self.label)
+        else:
+            p = self.pipeline or pipelines[0]
+            for pp in pipelines:
+                if p != pp:
+                    raise ValueError(
+                        'Mixing values in different pipelines is not allowed.'
+                        '\n{%r} != {%r}' % (p, pp))
+        # deferred = not getattr(p.runner, 'is_eager', False)
+        self.pipeline = p
+        result = p.apply(self, p_valueish, label)
+        return result
+
+    @staticmethod
+    def extract_input_if_one_p_values(input_inputs) -> pvalue.PValue:
+        """
+        In most scenarios, if Collection contain one element, return the element directly
+        :param input_inputs: inputs
+        :return:
+        """
+
+        if isinstance(input_inputs, tuple) or isinstance(input_inputs, list):
+            return input_inputs[0] if len(input_inputs) == 1 else input_inputs
+        elif isinstance(input_inputs, dict):
+            return next(iter(input_inputs.values())) if len(input_inputs) == 1 else input_inputs
+        return input_inputs
+
+    @staticmethod
+    def extract_first_input_p_values(input_inputs) -> pvalue.PValue:
+        """
+        extract first input for use
+        :param input_inputs: inputs
+        :return: first input
+        """
+        if isinstance(input_inputs, tuple) or isinstance(input_inputs, list):
+            return input_inputs[0]
+        elif isinstance(input_inputs, dict):
+            return next(iter(input_inputs.values()))
+        assert isinstance(input_inputs, pvalue.PValue)
+        return input_inputs
+
+    @staticmethod
+    def _extract_input_p_values(p_valueish):
+        from ronds_sdk import pipeline
+        if isinstance(p_valueish, pipeline.Pipeline):
+            if not p_valueish.root_transform.outputs:
+                p_begin = pvalue.PBegin(p_valueish)
+                p_valueish.root_transform.add_output(p_begin, '__root')
+            p_valueish = p_valueish.root_transform.outputs.get('__root')
+        return p_valueish, {
+            str(tag): value
+            for (tag, value) in get_named_nested_p_values(p_valueish, as_inputs=True)
+        }
+
+    @staticmethod
+    def _check_pcollection(p_coll):
+        # type: (pvalue.PCollection) -> None
+        if not isinstance(p_coll, pvalue.PCollection):
+            raise error.TransformError('Expecting a PCollection argument.')
+        if not p_coll.pipeline:
+            raise error.TransformError('PCollection not part of a pipeline')
+
+
+class ForeachBatchTransform(PTransform):
+
+    def expand(self, input_inputs, action_func=None):
+        raise NotImplementedError
+
+
+def get_named_nested_p_values(p_valueish, as_inputs=False):
+    if isinstance(p_valueish, tuple):
+        fields = getattr(p_valueish, '_fields', None)
+        if fields and len(fields) == len(p_valueish):
+            tagged_values = zip(fields, p_valueish)
+        else:
+            tagged_values = enumerate(p_valueish)
+    elif isinstance(p_valueish, list):
+        if as_inputs:
+            yield None, p_valueish
+            return
+        tagged_values = enumerate(p_valueish)
+    elif isinstance(p_valueish, dict):
+        tagged_values = p_valueish.items()
+    else:
+        if as_inputs or isinstance(p_valueish, pvalue.PValue):
+            yield None, p_valueish
+        return
+    for tag, sub_value in tagged_values:
+        for sub_tag, sub_sub_value in get_named_nested_p_values(
+                sub_value, as_inputs=as_inputs):
+            if sub_tag is None:
+                yield tag, sub_sub_value
+            else:
+                yield '%s.%s' % (tag, sub_tag), sub_sub_value
+
+
+class _NamedPTransform(PTransform):
+    def __init__(self, transform, label):
+        super().__init__(label)
+        self.transform = transform
+
+    def __ror__(self, p_valueish, _unused=None):
+        return self.transform.__ror__(p_valueish, self.label)
+
+    def expand(self, p_value):
+        raise RuntimeError("Should never be expanded directly.")
+
+
+class _ChainedPTransform(PTransform):
+    def __init__(self, *parts):
+        # type: (*PTransform) -> None
+        super().__init__(label=self._chain_label(parts))
+        self._parts = parts
+
+    @staticmethod
+    def _chain_label(parts):
+        return '|'.join(p.label for p in parts)
+
+    def __or__(self, right):
+        if isinstance(right, PTransform):
+            return _ChainedPTransform(*(self._parts + (right,)))
+        return NotImplemented
+
+    def expand(self, p_val):
+        raise NotImplementedError
```

### Comparing `rondsspark-0.0.4.6/ronds_sdk/__init__.py` & `rondsspark-0.0.4.7/ronds_sdk/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-"""
-RondsSpark SDK for Python3
-"""
-import sys
-import warnings
-
-if sys.version_info.major == 3:
-    if sys.version_info.minor <= 6:
-        warnings.warn(
-            'This version of SDK has not been sufficiently tested on '
-            'Python %s.%s. You may encounter bugs or missing features.' %
-            (sys.version_info.major, sys.version_info.minor))
-        pass
-else:
-    raise RuntimeError(
-        'The SDK for Python is only supported on Python3. '
-        'It is not supported on Python [%s].' % (str(sys.version_info))
-    )
-from ronds_sdk.dataframe.pvalue import PCollection
-from ronds_sdk import logger_config
-from ronds_sdk.options.pipeline_options import PipelineOptions
-from ronds_sdk.transforms.ronds import *
-from ronds_sdk.pipeline import Pipeline
-
-Options = PipelineOptions
-
-logger_config.config()
-
-
+"""
+RondsSpark SDK for Python3
+"""
+import sys
+import warnings
+
+if sys.version_info.major == 3:
+    if sys.version_info.minor <= 6:
+        warnings.warn(
+            'This version of SDK has not been sufficiently tested on '
+            'Python %s.%s. You may encounter bugs or missing features.' %
+            (sys.version_info.major, sys.version_info.minor))
+        pass
+else:
+    raise RuntimeError(
+        'The SDK for Python is only supported on Python3. '
+        'It is not supported on Python [%s].' % (str(sys.version_info))
+    )
+from ronds_sdk.dataframe.pvalue import PCollection
+from ronds_sdk import logger_config
+from ronds_sdk.options.pipeline_options import PipelineOptions
+from ronds_sdk.transforms.ronds import *
+from ronds_sdk.pipeline import Pipeline
+from ronds_sdk.templates import *
+
+Options = PipelineOptions
+
+logger_config.config()
+
+
```

### Comparing `rondsspark-0.0.4.6/test/simple/overloading_test.py` & `rondsspark-0.0.4.7/test/simple/overloading_test.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-class pipely(object):
-    def __init__(self, *args, **kw):
-        self._args = args
-        self.__dict__.update(kw)
-
-    def __ror__(self, other):
-        if isinstance(other, bad):
-            return other.val()
-        return (self.map(x) for x in other if self.filter(x))
-
-    def map(self, x):
-        return x
-
-    def filter(self, x):
-        return True
-
-
-class sieve(pipely):
-    def filter(self, x):
-        n = self._args[0]
-        return x == n or x % n
-
-
-class strify(pipely):
-    def map(self, x):
-        return str(x)
-
-
-class startswith(pipely):
-    def filter(self, x):
-        n = str(self._args[0])
-        if x.startswith(n):
-            return x
-
-
-class bad(object):
-    def val(self):
-        return 1, 2, 3
-
-
-def main():
-    for i in range(2, 100) | sieve(2) | sieve(3) | sieve(5) | sieve(7) | strify() | startswith(5):
-        print(i)
-
-
-if __name__ == '__main__':
-    main()
+class pipely(object):
+    def __init__(self, *args, **kw):
+        self._args = args
+        self.__dict__.update(kw)
+
+    def __ror__(self, other):
+        if isinstance(other, bad):
+            return other.val()
+        return (self.map(x) for x in other if self.filter(x))
+
+    def map(self, x):
+        return x
+
+    def filter(self, x):
+        return True
+
+
+class sieve(pipely):
+    def filter(self, x):
+        n = self._args[0]
+        return x == n or x % n
+
+
+class strify(pipely):
+    def map(self, x):
+        return str(x)
+
+
+class startswith(pipely):
+    def filter(self, x):
+        n = str(self._args[0])
+        if x.startswith(n):
+            return x
+
+
+class bad(object):
+    def val(self):
+        return 1, 2, 3
+
+
+def main():
+    for i in range(2, 100) | sieve(2) | sieve(3) | sieve(5) | sieve(7) | strify() | startswith(5):
+        print(i)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `rondsspark-0.0.4.6/test/spark/SparkTest.py` & `rondsspark-0.0.4.7/test/spark/SparkTest.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from datetime import datetime, date
-
-from pyspark import SparkContext
-from pyspark.sql import SparkSession
-from pyspark.sql import Row
-import logging
-
-from pyspark.sql.functions import explode, split
-from pyspark.streaming import StreamingContext
-from pyspark.sql import functions as F
-
-from ronds_sdk import logger_config
-
-logger = logging.getLogger(__name__)
-
-
-def spark_df1(spark: SparkSession):
-    # spark run
-    df = spark.createDataFrame([
-        Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
-        Row(a=2, b=2., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
-        Row(a=3, b=2., c='string2', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0)),
-    ])
-    print(df.schema)
-
-
-def spark_df2(spark: SparkSession):
-    # spark df 指定元数据
-    df = spark.createDataFrame([
-        (1, 2., "string1", date(2000, 1, 1), datetime(2000, 1, 1, 12, 0)),
-        (2, 2., "string1", date(2000, 2, 1), datetime(2000, 1, 2, 12, 0)),
-        (3, 2., "string1", date(2000, 3, 1), datetime(2000, 1, 3, 12, 0)),
-    ], schema="a long, b double, c string, d date, e timestamp")
-    logger.info(df.schema)
-
-
-def structured_streaming1(spark: SparkSession):
-    """
-    :param spark: spark 入口
-    :return:  None
-    """
-    lines = spark.readStream \
-        .format("socket") \
-        .option("host", "localhost") \
-        .option("port", 9999) \
-        .load()
-    words = lines.select(explode(split(lines.value, " ")).alias("word"))
-    word_counts = words.groupBy(words.word).agg(F.count(words.word))
-    query = word_counts \
-        .writeStream \
-        .outputMode("update") \
-        .format("console") \
-        .start()
-    query.awaitTermination()
-
-
-def structured_streaming2(spark: SparkSession):
-    lines = spark.readStream \
-        .format("socket") \
-        .option("host", "localhost") \
-        .option("port", 9999) \
-        .load()
-    lines.createOrReplaceTempView("my_table")
-    words_2 = spark.sql('select explode(split(value, " ")) as word2 from my_table')
-
-    query2 = words_2 \
-        .writeStream \
-        .outputMode("append") \
-        .format("console") \
-        .start()
-    query2.awaitTermination()
-
-
-def spark_streaming1():
-    sc = SparkContext("local[2]", "NetworkWordCount")
-    ssc = StreamingContext(sc, 1)
-    lines = ssc.socketTextStream("127.0.0.1", 9999)
-    words = lines.flatMap(lambda line: line.split(" "))
-    words.count()
-    words.pprint(10)
-    ssc.start()  # Start the computation
-    ssc.awaitTermination()
-
-
-def main():
-    logger_config.config()
-    spark = SparkSession.builder.getOrCreate()
-    # spark_df1(spark)
-    # spark_df2(spark)
-    structured_streaming2(spark)
-
-
-if __name__ == '__main__':
-    main()
+from datetime import datetime, date
+
+from pyspark import SparkContext
+from pyspark.sql import SparkSession
+from pyspark.sql import Row
+import logging
+
+from pyspark.sql.functions import explode, split
+from pyspark.streaming import StreamingContext
+from pyspark.sql import functions as F
+
+from ronds_sdk import logger_config
+
+logger = logging.getLogger(__name__)
+
+
+def spark_df1(spark: SparkSession):
+    # spark run
+    df = spark.createDataFrame([
+        Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
+        Row(a=2, b=2., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
+        Row(a=3, b=2., c='string2', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0)),
+    ])
+    print(df.schema)
+
+
+def spark_df2(spark: SparkSession):
+    # spark df 指定元数据
+    df = spark.createDataFrame([
+        (1, 2., "string1", date(2000, 1, 1), datetime(2000, 1, 1, 12, 0)),
+        (2, 2., "string1", date(2000, 2, 1), datetime(2000, 1, 2, 12, 0)),
+        (3, 2., "string1", date(2000, 3, 1), datetime(2000, 1, 3, 12, 0)),
+    ], schema="a long, b double, c string, d date, e timestamp")
+    logger.info(df.schema)
+
+
+def structured_streaming1(spark: SparkSession):
+    """
+    :param spark: spark 入口
+    :return:  None
+    """
+    lines = spark.readStream \
+        .format("socket") \
+        .option("host", "localhost") \
+        .option("port", 9999) \
+        .load()
+    words = lines.select(explode(split(lines.value, " ")).alias("word"))
+    word_counts = words.groupBy(words.word).agg(F.count(words.word))
+    query = word_counts \
+        .writeStream \
+        .outputMode("update") \
+        .format("console") \
+        .start()
+    query.awaitTermination()
+
+
+def structured_streaming2(spark: SparkSession):
+    lines = spark.readStream \
+        .format("socket") \
+        .option("host", "localhost") \
+        .option("port", 9999) \
+        .load()
+    lines.createOrReplaceTempView("my_table")
+    words_2 = spark.sql('select explode(split(value, " ")) as word2 from my_table')
+
+    query2 = words_2 \
+        .writeStream \
+        .outputMode("append") \
+        .format("console") \
+        .start()
+    query2.awaitTermination()
+
+
+def spark_streaming1():
+    sc = SparkContext("local[2]", "NetworkWordCount")
+    ssc = StreamingContext(sc, 1)
+    lines = ssc.socketTextStream("127.0.0.1", 9999)
+    words = lines.flatMap(lambda line: line.split(" "))
+    words.count()
+    words.pprint(10)
+    ssc.start()  # Start the computation
+    ssc.awaitTermination()
+
+
+def main():
+    logger_config.config()
+    spark = SparkSession.builder.getOrCreate()
+    # spark_df1(spark)
+    # spark_df2(spark)
+    structured_streaming2(spark)
+
+
+if __name__ == '__main__':
+    main()
```

