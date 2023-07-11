# Comparing `tmp/cypherdataframe-0.3.6.tar.gz` & `tmp/cypherdataframe-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.3.6.tar", last modified: Wed Jul  5 19:40:28 2023, max compression
+gzip compressed data, was "cypherdataframe-0.3.7.tar", last modified: Tue Jul 11 21:49:43 2023, max compression
```

## Comparing `cypherdataframe-0.3.6.tar` & `cypherdataframe-0.3.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.385985 cypherdataframe-0.3.6/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-05 19:40:28.385738 cypherdataframe-0.3.6/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.373442 cypherdataframe-0.3.6/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.6/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.6/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.6/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     9475 2023-07-05 19:39:27.000000 cypherdataframe-0.3.6/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.375711 cypherdataframe-0.3.6/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.376271 cypherdataframe-0.3.6/cypherdataframe/garner_domain/logistics/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/logistics/TransferBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/logistics/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.376770 cypherdataframe-0.3.6/cypherdataframe/garner_domain/measure/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      634 2023-06-09 21:00:14.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/measure/MeasureBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/measure/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.377264 cypherdataframe-0.3.6/cypherdataframe/garner_domain/queries/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      919 2023-06-29 20:44:47.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/queries/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.377766 cypherdataframe-0.3.6/cypherdataframe/garner_domain/reference/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/reference/ReferenceBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/reference/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.379114 cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/AttainedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/ForecastedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.380955 cypherdataframe-0.3.6/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.6/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.6/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.6/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.6/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.6/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.6/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.6/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.6/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.374918 cypherdataframe-0.3.6/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-05 19:40:28.000000 cypherdataframe-0.3.6/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-05 19:40:28.000000 cypherdataframe-0.3.6/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-05 19:40:28.000000 cypherdataframe-0.3.6/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-05 19:40:28.000000 cypherdataframe-0.3.6/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-05 19:40:28.000000 cypherdataframe-0.3.6/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-05 19:40:28.386072 cypherdataframe-0.3.6/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-05 19:39:54.000000 cypherdataframe-0.3.6/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.382808 cypherdataframe-0.3.6/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.6/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.6/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.6/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.6/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.383083 cypherdataframe-0.3.6/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.6/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.384405 cypherdataframe-0.3.6/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.6/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.6/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.6/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.6/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.6/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:40:28.385439 cypherdataframe-0.3.6/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.6/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.6/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.6/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.6/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.6/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.6/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.6/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.650329 cypherdataframe-0.3.7/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 21:49:43.650000 cypherdataframe-0.3.7/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.634496 cypherdataframe-0.3.7/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.7/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.7/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.7/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.3.7/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.636939 cypherdataframe-0.3.7/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.637506 cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.638230 cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-07-11 21:47:41.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.638777 cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      919 2023-06-29 20:44:47.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.639355 cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.640830 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.643619 cypherdataframe-0.3.7/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.7/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.7/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.7/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.7/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.7/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.7/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.7/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.7/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.635954 cypherdataframe-0.3.7/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 21:49:43.650406 cypherdataframe-0.3.7/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 21:49:27.000000 cypherdataframe-0.3.7/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.645826 cypherdataframe-0.3.7/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.7/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.7/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.7/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.7/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.646183 cypherdataframe-0.3.7/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.648211 cypherdataframe-0.3.7/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.7/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.7/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.7/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.7/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.649706 cypherdataframe-0.3.7/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.7/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.7/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.7/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.7/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.7/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.3.6/cypherdataframe/branch_maker.py` & `cypherdataframe-0.3.7/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/cypher.py` & `cypherdataframe-0.3.7/cypherdataframe/cypher.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,9 +312,9 @@
                 os.makedirs(gather_to_dir)
 
             df.to_csv(
                 f"{gather_to_dir}/{table_name_root}-gathered.csv",
                 index=False
             )
             df.to_feather(
-                f"{gather_to_dir}/{table_name_root}-gathered.feathered"
+                f"{gather_to_dir}/{table_name_root}-gathered.feather"
             )
```

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/logistics/TransferBranch.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/TransferBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/measure/MeasureBranch.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedBranch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from dataclasses import dataclass, field
 
 from cypherdataframe.garner_domain.BranchMaker import BranchMaker
-from cypherdataframe.garner_domain.properties_defaults import \
-    MEASURE_RELATIONSHIP, MEASURE_RETURN_POSTFIX
+from cypherdataframe.garner_domain.properties_defaults import FORECASTED_RETURN_POSTFIX, FORECASTED_RELATIONSHIP
 from cypherdataframe.model.Property import Property
 
 
 @dataclass
-class MeasureBranch(BranchMaker):
+class ForecastedBranch(BranchMaker):
+    props: list[Property]
+    relationship: str = field(default_factory=lambda: FORECASTED_RELATIONSHIP)
+    relationship_postfix: str | None = field(default_factory=lambda: FORECASTED_RETURN_POSTFIX)
+    required: bool = False
+    archived: bool = False
     domain_label: str | None = None
-    props_tag: str | None = "Measure"
-    props: list[Property] | None = None
-    not_archived: bool | None = True
-    relationship: str = field(default_factory=lambda: MEASURE_RELATIONSHIP)
-    relationship_postfix: str = field(default_factory=lambda: MEASURE_RETURN_POSTFIX)
```

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/reference/ReferenceBranch.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/ReferenceBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/AttainedBranch.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py` & `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/model/Branch.py` & `cypherdataframe-0.3.7/cypherdataframe/model/Branch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.3.7/cypherdataframe/model/LabelNode.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/model/Query.py` & `cypherdataframe-0.3.7/cypherdataframe/model/Query.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.3.7/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/cypherdataframe.egg-info/SOURCES.txt` & `cypherdataframe-0.3.7/cypherdataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/setup.py` & `cypherdataframe-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             'cypherdataframe.garner_domain.logistics',
             'cypherdataframe.garner_domain.measure',
             'cypherdataframe.garner_domain.queries',
             'cypherdataframe.garner_domain.reference',
             'cypherdataframe.garner_domain.status'
         ]
     ),
-    version='0.3.6',
+    version='0.3.7',
     description='Cypher Query to df Toolkit',
     author='Attila Vanderploeg',
     license='MIT',
     install_requires=['py2neo>=2021.2.3', 'dacite>=1.6.0'],
     setup_requires=[],
     tests_require=[],
     test_suite='tests',
```

### Comparing `cypherdataframe-0.3.6/tests/branch_maker_test.py` & `cypherdataframe-0.3.7/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.3.7/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.6/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.3.7/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

