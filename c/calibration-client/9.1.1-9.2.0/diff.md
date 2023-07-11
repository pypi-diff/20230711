# Comparing `tmp/calibration_client-9.1.1.tar.gz` & `tmp/calibration_client-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibration_client-9.1.1.tar", last modified: Tue Dec 14 18:57:02 2021, max compression
+gzip compressed data, was "calibration_client-9.2.0.tar", last modified: Mon May  9 11:09:25 2022, max compression
```

## Comparing `calibration_client-9.1.1.tar` & `calibration_client-9.2.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.474073 calibration_client-9.1.1/
--rw-r--r--   0 maial      (501) staff       (20)       48 2021-12-14 14:34:43.000000 calibration_client-9.1.1/AUTHORS.rst
--rw-r--r--   0 maial      (501) staff       (20)     5995 2021-12-14 18:26:26.000000 calibration_client-9.1.1/HISTORY.rst
--rw-r--r--   0 maial      (501) staff       (20)      779 2021-12-14 14:34:43.000000 calibration_client-9.1.1/LICENSE
--rw-r--r--   0 maial      (501) staff       (20)       89 2021-12-14 14:34:43.000000 calibration_client-9.1.1/MANIFEST.in
--rw-r--r--   0 maial      (501) staff       (20)     5070 2021-12-14 18:57:02.473671 calibration_client-9.1.1/PKG-INFO
--rw-r--r--   0 maial      (501) staff       (20)     3773 2021-12-14 14:34:43.000000 calibration_client-9.1.1/README.rst
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.425652 calibration_client-9.1.1/calibration_client/
--rw-r--r--   0 maial      (501) staff       (20)      245 2021-12-14 18:33:55.000000 calibration_client-9.1.1/calibration_client/__init__.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.437686 calibration_client-9.1.1/calibration_client/apis/
--rw-r--r--   0 maial      (501) staff       (20)      521 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     2194 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/calibration_api.py
--rw-r--r--   0 maial      (501) staff       (20)     4450 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/calibration_constant_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2008 2021-12-14 18:14:28.000000 calibration_client-9.1.1/calibration_client/apis/calibration_constant_version_api.py
--rw-r--r--   0 maial      (501) staff       (20)      820 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/condition_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1217 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/detector_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1120 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/detector_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1058 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/parameter_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2264 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/physical_detector_unit_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1253 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/report_api.py
--rw-r--r--   0 maial      (501) staff       (20)      372 2021-12-14 14:34:54.000000 calibration_client-9.1.1/calibration_client/apis/user_api.py
--rw-r--r--   0 maial      (501) staff       (20)    36273 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/calibration_client.py
--rw-r--r--   0 maial      (501) staff       (20)      426 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/calibration_client_api.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.440562 calibration_client-9.1.1/calibration_client/common/
--rw-r--r--   0 maial      (501) staff       (20)       46 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/common/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     8840 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/common/base.py
--rw-r--r--   0 maial      (501) staff       (20)      764 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/common/config.py
--rw-r--r--   0 maial      (501) staff       (20)      766 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/common/util.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.447867 calibration_client-9.1.1/calibration_client/modules/
--rw-r--r--   0 maial      (501) staff       (20)      428 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     3754 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/calibration.py
--rw-r--r--   0 maial      (501) staff       (20)     5990 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/calibration_constant.py
--rw-r--r--   0 maial      (501) staff       (20)     9813 2021-12-14 18:21:36.000000 calibration_client-9.1.1/calibration_client/modules/calibration_constant_version.py
--rw-r--r--   0 maial      (501) staff       (20)     3232 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/condition.py
--rw-r--r--   0 maial      (501) staff       (20)     3921 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/detector.py
--rw-r--r--   0 maial      (501) staff       (20)     2864 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/detector_type.py
--rw-r--r--   0 maial      (501) staff       (20)     3381 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/parameter.py
--rw-r--r--   0 maial      (501) staff       (20)     4540 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/physical_detector_unit.py
--rw-r--r--   0 maial      (501) staff       (20)     3287 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/modules/report.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.451893 calibration_client-9.1.1/calibration_client/tests/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/__init__.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.461382 calibration_client-9.1.1/calibration_client/tests/apis/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     1341 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/api_base.py
--rw-r--r--   0 maial      (501) staff       (20)     4602 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/calibration_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8378 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/calibration_constant_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8263 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/calibration_constant_version_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6661 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/condition_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6237 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/detector_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     3986 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/detector_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4863 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/parameter_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6523 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/physical_detector_unit_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4920 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/report_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     1391 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/apis/user_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)    32644 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/calibration_client_by_detector_test.py
--rw-r--r--   0 maial      (501) staff       (20)    22891 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/calibration_client_test.py
--rw-r--r--   0 maial      (501) staff       (20)    12105 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/calibration_test_hash.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.465533 calibration_client-9.1.1/calibration_client/tests/common/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/common/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     3226 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/common/base_test.py
--rw-r--r--   0 maial      (501) staff       (20)      796 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/common/config_test.py
--rw-r--r--   0 maial      (501) staff       (20)     1266 2021-12-14 14:35:22.000000 calibration_client-9.1.1/calibration_client/tests/common/generators.py
--rw-r--r--   0 maial      (501) staff       (20)     2536 2021-12-14 18:56:41.000000 calibration_client-9.1.1/calibration_client/tests/common/secrets.py
--rw-r--r--   0 maial      (501) staff       (20)      319 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/common/util.py
--rw-r--r--   0 maial      (501) staff       (20)     1936 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/common/util_test.py
--rw-r--r--   0 maial      (501) staff       (20)      752 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/conftest.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.473022 calibration_client-9.1.1/calibration_client/tests/modules/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     8629 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/calibration_constant_test.py
--rw-r--r--   0 maial      (501) staff       (20)    21636 2021-12-14 18:24:02.000000 calibration_client-9.1.1/calibration_client/tests/modules/calibration_constant_version_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4865 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/calibration_test.py
--rw-r--r--   0 maial      (501) staff       (20)    10093 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/condition_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4976 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/detector_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4234 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/detector_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     3700 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/module_base.py
--rw-r--r--   0 maial      (501) staff       (20)     4801 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/parameter_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5297 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/physical_detector_unit_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4463 2021-12-14 14:35:10.000000 calibration_client-9.1.1/calibration_client/tests/modules/report_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2021-12-14 18:57:02.428859 calibration_client-9.1.1/calibration_client.egg-info/
--rw-r--r--   0 maial      (501) staff       (20)     5070 2021-12-14 18:57:02.000000 calibration_client-9.1.1/calibration_client.egg-info/PKG-INFO
--rw-r--r--   0 maial      (501) staff       (20)     3252 2021-12-14 18:57:02.000000 calibration_client-9.1.1/calibration_client.egg-info/SOURCES.txt
--rw-r--r--   0 maial      (501) staff       (20)        1 2021-12-14 18:57:02.000000 calibration_client-9.1.1/calibration_client.egg-info/dependency_links.txt
--rw-r--r--   0 maial      (501) staff       (20)      124 2021-12-14 18:57:02.000000 calibration_client-9.1.1/calibration_client.egg-info/requires.txt
--rw-r--r--   0 maial      (501) staff       (20)       19 2021-12-14 18:57:02.000000 calibration_client-9.1.1/calibration_client.egg-info/top_level.txt
--rw-r--r--   0 maial      (501) staff       (20)       38 2021-12-14 18:57:02.474177 calibration_client-9.1.1/setup.cfg
--rw-r--r--   0 maial      (501) staff       (20)     2545 2021-12-14 18:33:33.000000 calibration_client-9.1.1/setup.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.242042 calibration_client-9.2.0/
+-rw-r--r--   0 maial      (501) staff       (20)       48 2021-12-14 14:34:43.000000 calibration_client-9.2.0/AUTHORS.rst
+-rw-r--r--   0 maial      (501) staff       (20)     6250 2022-05-09 11:07:57.000000 calibration_client-9.2.0/HISTORY.rst
+-rw-r--r--   0 maial      (501) staff       (20)      779 2021-12-14 14:34:43.000000 calibration_client-9.2.0/LICENSE
+-rw-r--r--   0 maial      (501) staff       (20)       89 2021-12-14 14:34:43.000000 calibration_client-9.2.0/MANIFEST.in
+-rw-r--r--   0 maial      (501) staff       (20)     8766 2022-05-09 11:09:25.241586 calibration_client-9.2.0/PKG-INFO
+-rw-r--r--   0 maial      (501) staff       (20)     7697 2022-05-09 11:07:53.000000 calibration_client-9.2.0/README.rst
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.210337 calibration_client-9.2.0/calibration_client/
+-rw-r--r--   0 maial      (501) staff       (20)      245 2022-05-09 11:07:53.000000 calibration_client-9.2.0/calibration_client/__init__.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.218294 calibration_client-9.2.0/calibration_client/apis/
+-rw-r--r--   0 maial      (501) staff       (20)      521 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     2194 2022-05-05 23:00:37.000000 calibration_client-9.2.0/calibration_client/apis/calibration_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     4450 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/calibration_constant_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2008 2021-12-14 20:28:57.000000 calibration_client-9.2.0/calibration_client/apis/calibration_constant_version_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      820 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/condition_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1217 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/detector_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1120 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/detector_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1058 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/parameter_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2264 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/physical_detector_unit_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1253 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/report_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      372 2021-12-14 14:34:54.000000 calibration_client-9.2.0/calibration_client/apis/user_api.py
+-rw-r--r--   0 maial      (501) staff       (20)    36273 2022-05-05 22:58:41.000000 calibration_client-9.2.0/calibration_client/calibration_client.py
+-rw-r--r--   0 maial      (501) staff       (20)      426 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/calibration_client_api.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.220105 calibration_client-9.2.0/calibration_client/common/
+-rw-r--r--   0 maial      (501) staff       (20)       46 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/common/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     9272 2022-05-09 11:07:53.000000 calibration_client-9.2.0/calibration_client/common/base.py
+-rw-r--r--   0 maial      (501) staff       (20)     1215 2022-05-05 23:27:29.000000 calibration_client-9.2.0/calibration_client/common/config.py
+-rw-r--r--   0 maial      (501) staff       (20)      766 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/common/util.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.224716 calibration_client-9.2.0/calibration_client/modules/
+-rw-r--r--   0 maial      (501) staff       (20)      428 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     3754 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/calibration.py
+-rw-r--r--   0 maial      (501) staff       (20)     5990 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/calibration_constant.py
+-rw-r--r--   0 maial      (501) staff       (20)     9813 2021-12-14 20:28:57.000000 calibration_client-9.2.0/calibration_client/modules/calibration_constant_version.py
+-rw-r--r--   0 maial      (501) staff       (20)     3232 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/condition.py
+-rw-r--r--   0 maial      (501) staff       (20)     3921 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/detector.py
+-rw-r--r--   0 maial      (501) staff       (20)     2864 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/detector_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     3381 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/parameter.py
+-rw-r--r--   0 maial      (501) staff       (20)     4540 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/physical_detector_unit.py
+-rw-r--r--   0 maial      (501) staff       (20)     3287 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/modules/report.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.227091 calibration_client-9.2.0/calibration_client/tests/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/__init__.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.232410 calibration_client-9.2.0/calibration_client/tests/apis/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     1341 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/api_base.py
+-rw-r--r--   0 maial      (501) staff       (20)     4553 2022-05-05 17:16:50.000000 calibration_client-9.2.0/calibration_client/tests/apis/calibration_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8378 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/calibration_constant_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8263 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/calibration_constant_version_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6661 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/condition_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6237 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/detector_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3986 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/detector_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4810 2022-05-05 17:16:50.000000 calibration_client-9.2.0/calibration_client/tests/apis/parameter_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6533 2022-05-05 17:16:50.000000 calibration_client-9.2.0/calibration_client/tests/apis/physical_detector_unit_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4833 2022-05-05 23:27:29.000000 calibration_client-9.2.0/calibration_client/tests/apis/report_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     1391 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/apis/user_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    32644 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/calibration_client_by_detector_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    22891 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/calibration_client_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    12105 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/calibration_test_hash.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.235366 calibration_client-9.2.0/calibration_client/tests/common/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/common/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     3226 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/common/base_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     1247 2022-05-05 23:27:29.000000 calibration_client-9.2.0/calibration_client/tests/common/config_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     1266 2021-12-14 14:35:22.000000 calibration_client-9.2.0/calibration_client/tests/common/generators.py
+-rw-r--r--   0 maial      (501) staff       (20)     2762 2022-05-05 23:51:25.000000 calibration_client-9.2.0/calibration_client/tests/common/secrets.py
+-rw-r--r--   0 maial      (501) staff       (20)      319 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/common/util.py
+-rw-r--r--   0 maial      (501) staff       (20)     1936 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/common/util_test.py
+-rw-r--r--   0 maial      (501) staff       (20)      752 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/conftest.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.240895 calibration_client-9.2.0/calibration_client/tests/modules/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/modules/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     8629 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/modules/calibration_constant_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    21636 2021-12-14 20:28:57.000000 calibration_client-9.2.0/calibration_client/tests/modules/calibration_constant_version_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4809 2022-05-05 17:16:50.000000 calibration_client-9.2.0/calibration_client/tests/modules/calibration_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    10093 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/modules/condition_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4976 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/modules/detector_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4234 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/modules/detector_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3700 2021-12-14 14:35:10.000000 calibration_client-9.2.0/calibration_client/tests/modules/module_base.py
+-rw-r--r--   0 maial      (501) staff       (20)     4745 2022-05-05 17:16:50.000000 calibration_client-9.2.0/calibration_client/tests/modules/parameter_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5237 2022-05-05 17:16:50.000000 calibration_client-9.2.0/calibration_client/tests/modules/physical_detector_unit_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4377 2022-05-05 23:27:29.000000 calibration_client-9.2.0/calibration_client/tests/modules/report_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-09 11:09:25.212733 calibration_client-9.2.0/calibration_client.egg-info/
+-rw-r--r--   0 maial      (501) staff       (20)     8766 2022-05-09 11:09:24.000000 calibration_client-9.2.0/calibration_client.egg-info/PKG-INFO
+-rw-r--r--   0 maial      (501) staff       (20)     3252 2022-05-09 11:09:25.000000 calibration_client-9.2.0/calibration_client.egg-info/SOURCES.txt
+-rw-r--r--   0 maial      (501) staff       (20)        1 2022-05-09 11:09:24.000000 calibration_client-9.2.0/calibration_client.egg-info/dependency_links.txt
+-rw-r--r--   0 maial      (501) staff       (20)      124 2022-05-09 11:09:24.000000 calibration_client-9.2.0/calibration_client.egg-info/requires.txt
+-rw-r--r--   0 maial      (501) staff       (20)       19 2022-05-09 11:09:24.000000 calibration_client-9.2.0/calibration_client.egg-info/top_level.txt
+-rw-r--r--   0 maial      (501) staff       (20)       38 2022-05-09 11:09:25.242163 calibration_client-9.2.0/setup.cfg
+-rw-r--r--   0 maial      (501) staff       (20)     2328 2022-05-05 23:27:29.000000 calibration_client-9.2.0/setup.py
```

### Comparing `calibration_client-9.1.1/HISTORY.rst` & `calibration_client-9.2.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 -------
 
+v9.2.0 (9 May 2022)
++++++++++++++++++++
+- Update internal libraries used as external_dependencies, especially oauth2_xfel_client
+- Expose `max_retries`, `timeout` and `ssl_verify` parameters from oauth2_xfel_client
+- Improve documentation in README file
+
 v9.1.0 (14 December 2021)
 +++++++++++++++++++++++++
 - Add new CalCat APIs to interact with Calibration Constant Versions
 - Update external dependency
 - Add python 3.10 to Gitlab-ci
 
 v9.0.6 (3 June 2021)
```

### Comparing `calibration_client-9.1.1/LICENSE` & `calibration_client-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/__init__.py` & `calibration_client-9.2.0/calibration_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/calibration_api.py` & `calibration_client-9.2.0/calibration_client/apis/calibration_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/calibration_constant_api.py` & `calibration_client-9.2.0/calibration_client/apis/calibration_constant_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/calibration_constant_version_api.py` & `calibration_client-9.2.0/calibration_client/apis/calibration_constant_version_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/condition_api.py` & `calibration_client-9.2.0/calibration_client/apis/condition_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/detector_api.py` & `calibration_client-9.2.0/calibration_client/apis/detector_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/detector_type_api.py` & `calibration_client-9.2.0/calibration_client/apis/detector_type_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/parameter_api.py` & `calibration_client-9.2.0/calibration_client/apis/parameter_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/physical_detector_unit_api.py` & `calibration_client-9.2.0/calibration_client/apis/physical_detector_unit_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/apis/report_api.py` & `calibration_client-9.2.0/calibration_client/apis/report_api.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/calibration_client.py` & `calibration_client-9.2.0/calibration_client/calibration_client.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/common/base.py` & `calibration_client-9.2.0/calibration_client/common/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import logging
 from functools import wraps
 from http import HTTPStatus
 
 from oauth2_xfel_client.oauth2_client_backend import Oauth2ClientBackend
 from oauthlib.oauth2 import TokenExpiredError
 
-from ..common.config import CREATE, DELETE, UPDATE, GET, SET
+from ..common.config import CREATE, DELETE, UPDATE, GET, SET, \
+    DEF_MAX_RETRIES, DEF_TIMEOUT, DEF_SSL_VERIFY
 
 
 def replace_expired_token(func):
     """Decorator to catch TokenExpiredError and make a session with a new token
 
     Doing it this way avoids a race condition where a token can expire between
     checking and using it. It also hopefully copes better if the client and
@@ -42,22 +43,28 @@
 
 
 class Base:
     def __init__(self,
                  client_id, client_secret,
                  token_url, refresh_url, auth_url, scope,
                  user_email, base_api_url,
-                 session_token=None):
+                 session_token=None,
+                 max_retries=DEF_MAX_RETRIES,
+                 timeout=DEF_TIMEOUT,
+                 ssl_verify=DEF_SSL_VERIFY):
         self.oauth_client = Oauth2ClientBackend(client_id=client_id,
                                                 client_secret=client_secret,
                                                 scope=scope,
                                                 token_url=token_url,
                                                 refresh_url=refresh_url,
                                                 auth_url=auth_url,
-                                                session_token=session_token)
+                                                session_token=session_token,
+                                                max_retries=max_retries,
+                                                timeout=timeout,
+                                                ssl_verify=ssl_verify)
 
         self.headers = default_headers(user_email)
         # Ensure the base URL has a trailing slash
         self.base_api_url = base_api_url.rstrip('/') + '/'
 
     @staticmethod
     def load_json_from_str(hash_str):
@@ -97,16 +104,17 @@
             res = Base.response_error(module_name, action, r_content)
 
         # In any other case an Error is reported
         else:
             if 'info' in r_content:
                 app_info = r_content['info']
             else:
-                app_info = '{}:{}'.format("HTTP request status code",
-                                          response.status_code)
+                app_info = '{}: expected {}, got {}'.format(
+                    "HTTP response unexpected status code",
+                    success_code, response.status_code)
             res = Base.response_error(module_name, action, app_info)
 
         return res
 
     @staticmethod
     # TODO, Make it validate and return key, value criteria
     def unique_key_format_result(res, module_name, unique_id=None):
```

### Comparing `calibration_client-9.1.1/calibration_client/common/util.py` & `calibration_client-9.2.0/calibration_client/common/util.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/calibration.py` & `calibration_client-9.2.0/calibration_client/modules/calibration.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/calibration_constant.py` & `calibration_client-9.2.0/calibration_client/modules/calibration_constant.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/calibration_constant_version.py` & `calibration_client-9.2.0/calibration_client/modules/calibration_constant_version.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/condition.py` & `calibration_client-9.2.0/calibration_client/modules/condition.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/detector.py` & `calibration_client-9.2.0/calibration_client/modules/detector.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/detector_type.py` & `calibration_client-9.2.0/calibration_client/modules/detector_type.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/parameter.py` & `calibration_client-9.2.0/calibration_client/modules/parameter.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/physical_detector_unit.py` & `calibration_client-9.2.0/calibration_client/modules/physical_detector_unit.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/modules/report.py` & `calibration_client-9.2.0/calibration_client/modules/report.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/api_base.py` & `calibration_client-9.2.0/calibration_client/tests/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/calibration_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/calibration_api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         assert receive == expect
         assert response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
 
     def __update_entry_api(self, entry_id, expect):
         unique_name = generate_unique_name('CalibrationApiUpd')
         calibration_upd = {
             'calibration': {
-                'name': unique_name,
+                'name': expect['name'],
                 # 'unit_id': '-1',
                 'max_value': 12.0,
                 'min_value': 3.0,
                 'allowed_deviation': 0.5,
                 'description': 'desc 01 updated!'
             }
         }
@@ -102,15 +102,14 @@
         # Add parameters not send to the update API
         calibration_upd['calibration']['unit_id'] = -1
         expect_upd = calibration_upd['calibration']
 
         self.fields_validation(receive, expect_upd)
         assert resp.status_code == HTTPStatus.OK
 
-        assert expect['name'] != expect_upd['name']
         assert expect['max_value'] != expect_upd['max_value']
         assert expect['min_value'] != expect_upd['min_value']
         assert expect['allowed_deviation'] != expect_upd['allowed_deviation']
         assert expect['description'] != expect_upd['description']
 
     def __get_all_entries_by_name_api(self, name, expect):
         response = self.cal_client.get_all_calibrations_by_name_api(name)
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/calibration_constant_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/calibration_constant_api_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/calibration_constant_version_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/calibration_constant_version_api_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/condition_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/condition_api_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/detector_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/detector_api_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/detector_type_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/detector_type_api_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/parameter_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/parameter_api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         assert receive == expect
         assert response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
 
     def __update_entry_api(self, entry_id, expect):
         unique_name_upd = generate_unique_name('ParameterApiUpd')
         parameter_upd = {
             PARAMETER: {
-                'name': unique_name_upd,
+                'name': expect['name'],
                 # 'unit_id': '-1',
                 'flg_available': False,
                 'flg_logarithmic': True,
                 'def_lower_deviation_value': 0.0,
                 'def_upper_deviation_value': 10.2,
                 'description': 'desc 01 updated!!!'
             }
@@ -101,15 +101,14 @@
         # Add parameters not send to the update API
         parameter_upd[PARAMETER]['unit_id'] = -1
         expect_upd = parameter_upd[PARAMETER]
 
         self.fields_validation(receive, expect_upd)
         assert res.status_code == HTTPStatus.OK
 
-        assert expect['name'] != expect_upd['name']
         assert expect['flg_available'] != expect_upd['flg_available']
         assert expect['flg_logarithmic'] != expect_upd['flg_logarithmic']
         assert expect['def_lower_deviation_value'] \
                != expect_upd['def_lower_deviation_value']
         assert expect['def_upper_deviation_value'] \
                != expect_upd['def_upper_deviation_value']
         assert expect['description'] != expect_upd['description']
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/physical_detector_unit_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/physical_detector_unit_api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         assert receive == expect
         assert resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
 
     def __update_entry_api(self, entry_id, expect):
         unique_name_upd = generate_unique_name('PhysicalDevApiUpd')
         physical_dev_upd = {
             PHYSICAL_DETECTOR_UNIT: {
-                'physical_name': unique_name_upd,
+                'physical_name': expect['physical_name'],
                 'karabo_da': unique_name_upd,
                 'virtual_device_name': unique_name_upd,
                 'uuid': expect['uuid'],
                 # 'detector_type_id': '-1',
                 # 'detector_id': '-1',
                 'flg_available': False,
                 'description': 'desc 01 updated!!!'
@@ -117,15 +117,15 @@
         physical_dev_upd[PHYSICAL_DETECTOR_UNIT]['detector_type_id'] = -1
         physical_dev_upd[PHYSICAL_DETECTOR_UNIT]['detector_id'] = -1
         expect_upd = physical_dev_upd[PHYSICAL_DETECTOR_UNIT]
 
         self.fields_validation(receive, expect_upd)
         assert resp.status_code == HTTPStatus.OK
 
-        assert expect['physical_name'] != expect_upd['physical_name']
+        # assert expect['physical_name'] != expect_upd['physical_name']
         assert expect['karabo_da'] != expect_upd['karabo_da']
         assert expect['virtual_device_name'] != expect_upd[
             'virtual_device_name']
         assert expect['flg_available'] != expect_upd['flg_available']
         assert expect['description'] != expect_upd['description']
 
     def __get_all_entries_by_name_api(self, physical_name, expect):
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/report_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/report_api_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,17 @@
         repo_name = created_entry_received['name']
         repo_file_path = created_entry_received['file_path']
 
         try:
             # Check that expected creation result was received
             self.fields_validation(created_entry_received, expect)
 
-            # Create duplicated entry (should throw an error)
-            self.__create_error_entry_uk_api(report)
+            # Create duplicated entry
+            # (should NOT throw an error and return the report from the DB)
+            self.__create_failsafe_duplicate_entry_uk_api(report, expect)
 
             # Get entry by name
             self.__get_all_entries_by_name_api(repo_name, expect)
 
             # Get entry by identifier
             self.__get_all_entries_by_name_and_path_api(repo_name,
                                                         repo_file_path,
@@ -76,22 +77,18 @@
     def __create_entry_api(self, entry_info, expect):
         response = self.cal_client.create_report_api(entry_info)
 
         receive = self.get_and_validate_create_entry(response)
         self.fields_validation(receive, expect)
         return receive
 
-    def __create_error_entry_uk_api(self, entry_info):
+    def __create_failsafe_duplicate_entry_uk_api(self, entry_info, expect):
         response = self.cal_client.create_report_api(entry_info)
-        receive = self.load_response_content(response)
-
-        expect = {'info': {'name': ['has already been taken'],
-                           'file_path': ['has already been taken']}}
-        assert receive == expect
-        assert response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
+        receive = self.get_and_validate_create_entry(response)
+        self.fields_validation(receive, expect)
 
     def __update_entry_api(self, entry_id, expect):
         unique_name_upd = 'ReportApi-Dynamic_UPD-TO_DELETED'
         report_upd = {
             'report': {
                 'name': unique_name_upd,
                 'file_path': unique_name_upd,
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/apis/user_api_test.py` & `calibration_client-9.2.0/calibration_client/tests/apis/user_api_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/calibration_client_by_detector_test.py` & `calibration_client-9.2.0/calibration_client/tests/calibration_client_by_detector_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/calibration_client_test.py` & `calibration_client-9.2.0/calibration_client/tests/calibration_client_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/calibration_test_hash.py` & `calibration_client-9.2.0/calibration_client/tests/calibration_test_hash.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/common/base_test.py` & `calibration_client-9.2.0/calibration_client/tests/common/base_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/common/generators.py` & `calibration_client-9.2.0/calibration_client/tests/common/generators.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/common/util_test.py` & `calibration_client-9.2.0/calibration_client/tests/common/util_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/conftest.py` & `calibration_client-9.2.0/calibration_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/calibration_constant_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/calibration_constant_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/calibration_constant_version_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/calibration_constant_version_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/calibration_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/calibration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             'min_value': 1.0,
             'allowed_deviation': 0.1,
             'description': 'desc 01'
         }
 
         __unique_name_upd = generate_unique_name('CalibrationUpd01')
         self.cal_01_upd = {
-            'name': __unique_name_upd,
+            'name': __unique_name1,
             'unit_id': -1,
             'max_value': 12.0,
             'min_value': 3.0,
             'allowed_deviation': 0.5,
             'description': 'desc 01 updated!'
         }
 
@@ -82,22 +82,22 @@
             cal_01.min_value = self.cal_01_upd['min_value']
             cal_01.allowed_deviation = self.cal_01_upd['allowed_deviation']
             cal_01.description = self.cal_01_upd['description']
             result6 = cal_01.update()
             self.assert_update_success(MODULE_NAME, result6, self.cal_01_upd)
 
             # Put entry information (update some fields should throw an error)
-            cal_01.name = '__THIS_NAME_IS_1_CHARACTERS_LONGER_THAN_THE_ALLOWED_MAX_NUM__'  # noqa
+            cal_01.name = '__THIS_NAME_CANNOT_BE_UPDATED'  # noqa
             cal_01.max_value = self.cal_01_upd['max_value']
             cal_01.min_value = self.cal_01_upd['min_value']
             cal_01.allowed_deviation = self.cal_01_upd['allowed_deviation']
             cal_01.description = self.cal_01_upd['description']
             result7 = cal_01.update()
             expect_app_info = {
-                'name': ['is too long (maximum is 60 characters)']}
+                'name': ['cannot be updated']}
             self.assert_update_error(MODULE_NAME, result7, expect_app_info)
 
         finally:
             # Delete entry (should succeed)
             # (test purposes only to keep the DB clean)
             result8 = cal_01.delete()
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/condition_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/condition_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/detector_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/detector_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/detector_type_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/detector_type_test.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/module_base.py` & `calibration_client-9.2.0/calibration_client/tests/modules/module_base.py`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/parameter_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/parameter_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             'def_lower_deviation_value': 1.0,
             'def_upper_deviation_value': 1.2,
             'description': 'desc 01'
         }
 
         __unique_name_upd = generate_unique_name('ParameterUpd01')
         self.par_01_upd = {
-            'name': __unique_name_upd,
+            'name': __unique_name1,
             'unit_id': -1,
             'flg_available': True,
             'flg_logarithmic': False,
             'def_lower_deviation_value': 1.0,
             'def_upper_deviation_value': 1.2,
             'description': 'desc 01'
         }
@@ -78,20 +78,20 @@
             param_01.name = self.par_01_upd['name']
             param_01.flg_available = self.par_01_upd['flg_available']
             param_01.description = self.par_01_upd['description']
             result6 = param_01.update()
             self.assert_update_success(MODULE_NAME, result6, self.par_01_upd)
 
             # Put entry information (update some fields should throw an error)
-            param_01.name = '__THIS_NAME_IS_1_CHARACTERS_LONGER_THAN_THE_ALLOWED_MAX_NUM__'  # noqa
+            param_01.name = '__THIS_NAME_CANNOT_BE_UPDATED'  # noqa
             param_01.flg_available = self.par_01_upd['flg_available']
             param_01.description = self.par_01_upd['description']
             result7 = param_01.update()
             expect_app_info = {
-                'name': ['is too long (maximum is 60 characters)']}
+                'name': ['cannot be updated']}
             self.assert_update_error(MODULE_NAME, result7, expect_app_info)
 
         finally:
             # Delete entry (should succeed)
             # (test purposes only to keep the DB clean)
             result8 = param_01.delete()
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/physical_detector_unit_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/physical_detector_unit_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             'detector_id': -1,
             'flg_available': True,
             'description': 'desc 01'
         }
 
         __unique_name_upd = generate_unique_name('PhysicalDevUpd01')
         self.pd_01_upd = {
-            'physical_name': __unique_name_upd,
+            'physical_name': __unique_name1,
             'karabo_da': __unique_name_upd,
             'virtual_device_name': __unique_name_upd,
             'detector_type_id': -1,
             'detector_id': -1,
             'flg_available': False,
             'description': 'desc 01 Updated!!!'
         }
@@ -84,20 +84,20 @@
             pd_01.virtual_device_name = self.pd_01_upd['virtual_device_name']
             pd_01.flg_available = self.pd_01_upd['flg_available']
             pd_01.description = self.pd_01_upd['description']
             result6 = pd_01.update()
             self.assert_update_success(MODULE_NAME, result6, self.pd_01_upd)
 
             # Put entry information (update some fields should throw an error)
-            pd_01.physical_name = '__THIS_NAME_IS_1_CHARACTERS_LONGER_THAN_THE_ALLOWED_MAX_NUM__1234'  # noqa
+            pd_01.physical_name = '__THIS_NAME_CANNOT_BE_UPDATED'  # noqa
             pd_01.flg_available = self.pd_01_upd['flg_available']
             pd_01.description = self.pd_01_upd['description']
             result7 = pd_01.update()
             expect_app_info = {
-                'physical_name': ['is too long (maximum is 64 characters)']}
+                'physical_name': ['cannot be updated']}
             self.assert_update_error(MODULE_NAME, result7, expect_app_info)
 
         finally:
             # Delete entry (should succeed)
             # (test purposes only to keep the DB clean)
             result8 = pd_01.delete()
```

### Comparing `calibration_client-9.1.1/calibration_client/tests/modules/report_test.py` & `calibration_client-9.2.0/calibration_client/tests/modules/report_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,20 +46,19 @@
         try:
             self.assert_create_success(MODULE_NAME, result1, self.report_01)
 
             report_id = result1['data']['id']
             report_name = result1['data']['name']
             report_file_path = result1['data']['file_path']
 
-            # Create duplicated entry (should throw an error)
+            # Create duplicated entry
+            # (should NOT throw an error and return the report from the DB)
             report_01_dup = report_01
             result2 = report_01_dup.create()
-            expect_app_info = {'name': ['has already been taken'],
-                               'file_path': ['has already been taken']}
-            self.assert_create_error(MODULE_NAME, result2, expect_app_info)
+            self.assert_create_success(MODULE_NAME, result2, self.report_01)
 
             # Get entry by name & file_path
             result3 = Report.get_by_name_and_file_path(self.cal_client,
                                                        report_name,
                                                        report_file_path)
             self.assert_find_success(MODULE_NAME, result3, self.report_01)
```

### Comparing `calibration_client-9.1.1/calibration_client.egg-info/SOURCES.txt` & `calibration_client-9.2.0/calibration_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calibration_client-9.1.1/setup.py` & `calibration_client-9.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,36 +39,32 @@
     url='https://git.xfel.eu/gitlab/ITDM/calibration_client',
     platforms='any',
     license='MIT',
     packages=find_packages(),
     install_requires=['oauthlib',
                       'requests',
                       'requests-oauthlib',
-                      'oauth2_xfel_client >=6.0',
+                      'oauth2_xfel_client >=6.1',
                       'pytz'],
     extras_require={'test': [
         'pytest',
         'pytest-cov',
         'python-dateutil',
         'pytz',
         'pycodestyle'
     ]},
+    python_requires='>=3.6',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ]
 )
```

