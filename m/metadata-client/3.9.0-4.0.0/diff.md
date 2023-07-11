# Comparing `tmp/metadata_client-3.9.0.tar.gz` & `tmp/metadata_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadata_client-3.9.0.tar", last modified: Fri Jul  1 10:12:12 2022, max compression
+gzip compressed data, was "metadata_client-4.0.0.tar", last modified: Tue Jul 11 18:09:05 2023, max compression
```

## Comparing `metadata_client-3.9.0.tar` & `metadata_client-4.0.0.tar`

### file list

```diff
@@ -1,113 +1,123 @@
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.961401 metadata_client-3.9.0/
--rw-r--r--   0 maial      (501) staff       (20)       48 2021-12-14 20:32:26.000000 metadata_client-3.9.0/AUTHORS.rst
--rw-r--r--   0 maial      (501) staff       (20)     6238 2022-06-24 11:54:57.000000 metadata_client-3.9.0/HISTORY.rst
--rw-r--r--   0 maial      (501) staff       (20)      779 2021-12-14 20:32:26.000000 metadata_client-3.9.0/LICENSE
--rw-r--r--   0 maial      (501) staff       (20)       89 2021-12-14 20:32:26.000000 metadata_client-3.9.0/MANIFEST.in
--rw-r--r--   0 maial      (501) staff       (20)    15042 2022-07-01 10:12:12.961017 metadata_client-3.9.0/PKG-INFO
--rw-r--r--   0 maial      (501) staff       (20)    13987 2022-06-24 11:54:57.000000 metadata_client-3.9.0/README.rst
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.891679 metadata_client-3.9.0/metadata_client/
--rw-r--r--   0 maial      (501) staff       (20)      216 2022-06-24 11:54:57.000000 metadata_client-3.9.0/metadata_client/__init__.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.908379 metadata_client-3.9.0/metadata_client/apis/
--rw-r--r--   0 maial      (501) staff       (20)      833 2021-12-14 20:30:26.000000 metadata_client-3.9.0/metadata_client/apis/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     1791 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/dark_run_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1683 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_file_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1767 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_group_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2041 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_group_repository_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1740 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_group_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)      473 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_source_group_api.py
--rw-r--r--   0 maial      (501) staff       (20)      848 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_source_group_version_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1293 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1773 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/experiment_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1452 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/experiment_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/instrument_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1772 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/parameter_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1432 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/parameter_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/proposal_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1536 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/repostory_api.py
--rwxr-xr-x   0 maial      (501) staff       (20)     2345 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/run_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1742 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/sample_api.py
--rw-r--r--   0 maial      (501) staff       (20)      615 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/user_api.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.911533 metadata_client-3.9.0/metadata_client/common/
--rw-r--r--   0 maial      (501) staff       (20)       46 2021-12-14 20:30:57.000000 metadata_client-3.9.0/metadata_client/common/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     9438 2022-05-13 12:22:51.000000 metadata_client-3.9.0/metadata_client/common/base.py
--rw-r--r--   0 maial      (501) staff       (20)     3413 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/common/config.py
--rw-r--r--   0 maial      (501) staff       (20)     1136 2021-12-14 20:30:57.000000 metadata_client-3.9.0/metadata_client/common/util.py
--rw-r--r--   0 maial      (501) staff       (20)    31396 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/metadata_client.py
--rw-r--r--   0 maial      (501) staff       (20)      353 2021-12-14 20:32:42.000000 metadata_client-3.9.0/metadata_client/metadata_client_api.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.927359 metadata_client-3.9.0/metadata_client/modules/
--rw-r--r--   0 maial      (501) staff       (20)      708 2021-12-14 20:30:50.000000 metadata_client-3.9.0/metadata_client/modules/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     4831 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/dark_run.py
--rw-r--r--   0 maial      (501) staff       (20)     3506 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_file.py
--rw-r--r--   0 maial      (501) staff       (20)     5680 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_group.py
--rw-r--r--   0 maial      (501) staff       (20)     4927 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_group_repository.py
--rw-r--r--   0 maial      (501) staff       (20)     3292 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_group_type.py
--rw-r--r--   0 maial      (501) staff       (20)      771 2021-12-14 20:30:50.000000 metadata_client-3.9.0/metadata_client/modules/data_source_group.py
--rw-r--r--   0 maial      (501) staff       (20)     1225 2021-12-14 20:30:50.000000 metadata_client-3.9.0/metadata_client/modules/data_source_group_version.py
--rw-r--r--   0 maial      (501) staff       (20)     2849 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_type.py
--rw-r--r--   0 maial      (501) staff       (20)     4038 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/experiment.py
--rw-r--r--   0 maial      (501) staff       (20)     2933 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/experiment_type.py
--rw-r--r--   0 maial      (501) staff       (20)     3396 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/instrument.py
--rw-r--r--   0 maial      (501) staff       (20)     5303 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/parameter.py
--rw-r--r--   0 maial      (501) staff       (20)     2919 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/parameter_type.py
--rw-r--r--   0 maial      (501) staff       (20)     6792 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/proposal.py
--rw-r--r--   0 maial      (501) staff       (20)     3874 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/repository.py
--rw-r--r--   0 maial      (501) staff       (20)     6406 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/run.py
--rw-r--r--   0 maial      (501) staff       (20)     5091 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/sample.py
--rw-r--r--   0 maial      (501) staff       (20)     1082 2021-12-14 20:31:10.000000 metadata_client-3.9.0/metadata_client/modules/user.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.929621 metadata_client-3.9.0/metadata_client/tests/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:12.000000 metadata_client-3.9.0/metadata_client/tests/__init__.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.942142 metadata_client-3.9.0/metadata_client/tests/apis/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     1893 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/api_base.py
--rw-r--r--   0 maial      (501) staff       (20)     4239 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/dark_run_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5169 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_file_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8048 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_group_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6309 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_group_repository_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5488 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_group_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5329 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6791 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/experiment_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5491 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/experiment_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     3730 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/instrument_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6759 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/parameter_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5464 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/parameter_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)    14173 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/tests/apis/proposal_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6879 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/repository_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8955 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/tests/apis/run_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6919 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/tests/apis/sample_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     2002 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/user_api_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.948017 metadata_client-3.9.0/metadata_client/tests/common/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:33.000000 metadata_client-3.9.0/metadata_client/tests/common/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     4432 2022-05-13 12:22:51.000000 metadata_client-3.9.0/metadata_client/tests/common/base_test.py
--rw-r--r--   0 maial      (501) staff       (20)     3353 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/common/config_test.py
--rw-r--r--   0 maial      (501) staff       (20)     2117 2021-12-14 20:31:33.000000 metadata_client-3.9.0/metadata_client/tests/common/generators.py
--rwxr-xr-x   0 maial      (501) staff       (20)     2824 2022-05-05 17:15:10.000000 metadata_client-3.9.0/metadata_client/tests/common/secrets.py
--rw-r--r--   0 maial      (501) staff       (20)     5003 2021-12-14 20:31:50.000000 metadata_client-3.9.0/metadata_client/tests/common/util.py
--rw-r--r--   0 maial      (501) staff       (20)     1813 2021-12-14 20:31:50.000000 metadata_client-3.9.0/metadata_client/tests/common/util_datetime.py
--rw-r--r--   0 maial      (501) staff       (20)     2373 2021-12-14 20:31:50.000000 metadata_client-3.9.0/metadata_client/tests/common/util_test.py
--rw-r--r--   0 maial      (501) staff       (20)     1579 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/metadata_client_connection_test.py
--rw-r--r--   0 maial      (501) staff       (20)    56026 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/metadata_client_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.960413 metadata_client-3.9.0/metadata_client/tests/modules/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     8729 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/dark_run_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6105 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_file_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5156 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_group_repository_test.py
--rw-r--r--   0 maial      (501) staff       (20)    11675 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_group_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6370 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_group_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4973 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     7136 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/experiment_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5078 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/experiment_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4607 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/module_base.py
--rw-r--r--   0 maial      (501) staff       (20)     9271 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/parameter_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5059 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/parameter_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)    14605 2022-05-03 12:44:12.000000 metadata_client-3.9.0/metadata_client/tests/modules/proposal_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6643 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/repository_test.py
--rw-r--r--   0 maial      (501) staff       (20)    10473 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/run_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8838 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/sample_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.894713 metadata_client-3.9.0/metadata_client.egg-info/
--rw-r--r--   0 maial      (501) staff       (20)    15042 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/PKG-INFO
--rw-r--r--   0 maial      (501) staff       (20)     4120 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/SOURCES.txt
--rw-r--r--   0 maial      (501) staff       (20)        1 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/dependency_links.txt
--rw-r--r--   0 maial      (501) staff       (20)      124 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/requires.txt
--rw-r--r--   0 maial      (501) staff       (20)       16 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/top_level.txt
--rw-r--r--   0 maial      (501) staff       (20)       38 2022-07-01 10:12:12.961503 metadata_client-3.9.0/setup.cfg
--rw-r--r--   0 maial      (501) staff       (20)     2313 2022-06-24 11:54:57.000000 metadata_client-3.9.0/setup.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.240335 metadata_client-4.0.0/
+-rw-r--r--   0 maial      (501) staff       (20)       48 2021-12-14 20:32:26.000000 metadata_client-4.0.0/AUTHORS.rst
+-rw-r--r--   0 maial      (501) staff       (20)     7129 2023-07-11 17:50:23.000000 metadata_client-4.0.0/HISTORY.rst
+-rw-r--r--   0 maial      (501) staff       (20)      779 2021-12-14 20:32:26.000000 metadata_client-4.0.0/LICENSE
+-rw-r--r--   0 maial      (501) staff       (20)       89 2021-12-14 20:32:26.000000 metadata_client-4.0.0/MANIFEST.in
+-rw-r--r--   0 maial      (501) staff       (20)    15025 2023-07-11 18:09:05.239650 metadata_client-4.0.0/PKG-INFO
+-rw-r--r--   0 maial      (501) staff       (20)    13975 2023-07-11 17:50:23.000000 metadata_client-4.0.0/README.rst
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.094717 metadata_client-4.0.0/metadata_client/
+-rw-r--r--   0 maial      (501) staff       (20)      216 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/__init__.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.122637 metadata_client-4.0.0/metadata_client/apis/
+-rw-r--r--   0 maial      (501) staff       (20)      907 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/apis/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     1791 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/dark_run_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1683 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_file_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1767 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_group_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2041 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_group_repository_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1740 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_group_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      473 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_source_group_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      848 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_source_group_version_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1293 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/data_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1773 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/experiment_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1452 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/experiment_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/instrument_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1772 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/parameter_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1432 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/parameter_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/proposal_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1233 2023-01-24 08:40:34.000000 metadata_client-4.0.0/metadata_client/apis/proposal_technique_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1530 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/apis/report_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1536 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/repostory_api.py
+-rwxr-xr-x   0 maial      (501) staff       (20)     2345 2023-05-18 14:20:46.000000 metadata_client-4.0.0/metadata_client/apis/run_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1742 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/sample_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2187 2023-05-19 01:00:58.000000 metadata_client-4.0.0/metadata_client/apis/technique_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      615 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/apis/user_api.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.127955 metadata_client-4.0.0/metadata_client/common/
+-rw-r--r--   0 maial      (501) staff       (20)       46 2021-12-14 20:30:57.000000 metadata_client-4.0.0/metadata_client/common/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     9438 2022-05-13 12:22:51.000000 metadata_client-4.0.0/metadata_client/common/base.py
+-rw-r--r--   0 maial      (501) staff       (20)     3547 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/common/config.py
+-rw-r--r--   0 maial      (501) staff       (20)     1136 2023-05-18 16:21:23.000000 metadata_client-4.0.0/metadata_client/common/util.py
+-rw-r--r--   0 maial      (501) staff       (20)    31863 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/metadata_client.py
+-rw-r--r--   0 maial      (501) staff       (20)      353 2021-12-14 20:32:42.000000 metadata_client-4.0.0/metadata_client/metadata_client_api.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.145312 metadata_client-4.0.0/metadata_client/modules/
+-rw-r--r--   0 maial      (501) staff       (20)      768 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/modules/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     4831 2023-05-24 13:57:41.000000 metadata_client-4.0.0/metadata_client/modules/dark_run.py
+-rw-r--r--   0 maial      (501) staff       (20)     3506 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/data_file.py
+-rw-r--r--   0 maial      (501) staff       (20)     5680 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/data_group.py
+-rw-r--r--   0 maial      (501) staff       (20)     4927 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/data_group_repository.py
+-rw-r--r--   0 maial      (501) staff       (20)     3292 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/data_group_type.py
+-rw-r--r--   0 maial      (501) staff       (20)      771 2021-12-14 20:30:50.000000 metadata_client-4.0.0/metadata_client/modules/data_source_group.py
+-rw-r--r--   0 maial      (501) staff       (20)     1225 2021-12-14 20:30:50.000000 metadata_client-4.0.0/metadata_client/modules/data_source_group_version.py
+-rw-r--r--   0 maial      (501) staff       (20)     2849 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/data_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     4038 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/experiment.py
+-rw-r--r--   0 maial      (501) staff       (20)     2933 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/experiment_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     3396 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/instrument.py
+-rw-r--r--   0 maial      (501) staff       (20)     5303 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/parameter.py
+-rw-r--r--   0 maial      (501) staff       (20)     2919 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/parameter_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     6792 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/proposal.py
+-rw-r--r--   0 maial      (501) staff       (20)     1557 2023-01-24 08:40:34.000000 metadata_client-4.0.0/metadata_client/modules/proposal_technique.py
+-rw-r--r--   0 maial      (501) staff       (20)     2553 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/modules/report.py
+-rw-r--r--   0 maial      (501) staff       (20)     3874 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/repository.py
+-rw-r--r--   0 maial      (501) staff       (20)     6813 2023-05-19 01:00:58.000000 metadata_client-4.0.0/metadata_client/modules/run.py
+-rw-r--r--   0 maial      (501) staff       (20)     5091 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/modules/sample.py
+-rw-r--r--   0 maial      (501) staff       (20)     4667 2023-01-24 08:40:34.000000 metadata_client-4.0.0/metadata_client/modules/technique.py
+-rw-r--r--   0 maial      (501) staff       (20)     1082 2021-12-14 20:31:10.000000 metadata_client-4.0.0/metadata_client/modules/user.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.148228 metadata_client-4.0.0/metadata_client/tests/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:12.000000 metadata_client-4.0.0/metadata_client/tests/__init__.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.191679 metadata_client-4.0.0/metadata_client/tests/apis/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     2039 2023-05-19 01:00:58.000000 metadata_client-4.0.0/metadata_client/tests/apis/api_base.py
+-rw-r--r--   0 maial      (501) staff       (20)     5185 2023-05-19 01:00:58.000000 metadata_client-4.0.0/metadata_client/tests/apis/dark_run_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5169 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/data_file_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8048 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/data_group_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6309 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/data_group_repository_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5488 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/data_group_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5329 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/data_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6791 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/experiment_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5491 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/experiment_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3730 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/instrument_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6759 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/parameter_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5464 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/parameter_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    14173 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/tests/apis/proposal_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4710 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/tests/apis/report_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6879 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/repository_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    10276 2023-05-19 03:59:31.000000 metadata_client-4.0.0/metadata_client/tests/apis/run_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6919 2022-05-05 17:15:05.000000 metadata_client-4.0.0/metadata_client/tests/apis/sample_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3047 2023-01-24 08:40:34.000000 metadata_client-4.0.0/metadata_client/tests/apis/technique_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     2002 2021-12-14 20:31:39.000000 metadata_client-4.0.0/metadata_client/tests/apis/user_api_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.212936 metadata_client-4.0.0/metadata_client/tests/common/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:33.000000 metadata_client-4.0.0/metadata_client/tests/common/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     4432 2022-05-13 12:22:51.000000 metadata_client-4.0.0/metadata_client/tests/common/base_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3487 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/tests/common/config_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     2684 2023-01-24 08:40:34.000000 metadata_client-4.0.0/metadata_client/tests/common/generators.py
+-rwxr-xr-x   0 maial      (501) staff       (20)     2704 2023-07-11 18:08:11.000000 metadata_client-4.0.0/metadata_client/tests/common/secrets.py
+-rw-r--r--   0 maial      (501) staff       (20)     5118 2023-05-19 01:00:58.000000 metadata_client-4.0.0/metadata_client/tests/common/util.py
+-rw-r--r--   0 maial      (501) staff       (20)     1813 2021-12-14 20:31:50.000000 metadata_client-4.0.0/metadata_client/tests/common/util_datetime.py
+-rw-r--r--   0 maial      (501) staff       (20)     2373 2021-12-14 20:31:50.000000 metadata_client-4.0.0/metadata_client/tests/common/util_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     1579 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/metadata_client_connection_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    57578 2023-06-26 11:55:10.000000 metadata_client-4.0.0/metadata_client/tests/metadata_client_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.238640 metadata_client-4.0.0/metadata_client/tests/modules/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     8729 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/dark_run_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6105 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/data_file_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5156 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/data_group_repository_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    11675 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/data_group_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6370 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/data_group_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4973 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/data_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     7136 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/experiment_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5078 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/experiment_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4607 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/module_base.py
+-rw-r--r--   0 maial      (501) staff       (20)     9271 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/parameter_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5059 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/parameter_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    14605 2022-05-03 12:44:12.000000 metadata_client-4.0.0/metadata_client/tests/modules/proposal_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5280 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/tests/modules/report_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6643 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/repository_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    10473 2021-12-14 20:32:03.000000 metadata_client-4.0.0/metadata_client/tests/modules/run_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8838 2022-05-05 17:15:06.000000 metadata_client-4.0.0/metadata_client/tests/modules/sample_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5792 2023-07-11 17:50:23.000000 metadata_client-4.0.0/metadata_client/tests/modules/technique_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2023-07-11 18:09:05.098723 metadata_client-4.0.0/metadata_client.egg-info/
+-rw-r--r--   0 maial      (501) staff       (20)    15025 2023-07-11 18:09:04.000000 metadata_client-4.0.0/metadata_client.egg-info/PKG-INFO
+-rw-r--r--   0 maial      (501) staff       (20)     4545 2023-07-11 18:09:05.000000 metadata_client-4.0.0/metadata_client.egg-info/SOURCES.txt
+-rw-r--r--   0 maial      (501) staff       (20)        1 2023-07-11 18:09:04.000000 metadata_client-4.0.0/metadata_client.egg-info/dependency_links.txt
+-rw-r--r--   0 maial      (501) staff       (20)      129 2023-07-11 18:09:04.000000 metadata_client-4.0.0/metadata_client.egg-info/requires.txt
+-rw-r--r--   0 maial      (501) staff       (20)       16 2023-07-11 18:09:04.000000 metadata_client-4.0.0/metadata_client.egg-info/top_level.txt
+-rw-r--r--   0 maial      (501) staff       (20)       38 2023-07-11 18:09:05.240612 metadata_client-4.0.0/setup.cfg
+-rw-r--r--   0 maial      (501) staff       (20)     2312 2023-05-19 01:32:01.000000 metadata_client-4.0.0/setup.py
```

### Comparing `metadata_client-3.9.0/HISTORY.rst` & `metadata_client-4.0.0/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 History
 -------
 
+v4.0.0 (11 July 2023)
++++++++++++++++++++++
+- Proposal `leading_scientist_id` field renamed as `instrument_leader_id`
+- Proposal `deputy_leading_scientist_id` field renamed as `deputy_instrument_leader_id`
+- Added Report module APIs
+- Added Technique module APIs
+
+v3.11.1 (26 June 2023)
+++++++++++++++++++++++
+- Upgrade dependencies
+- Fix issue on failing Python test
+
+v3.11.0 (19 May 2023)
++++++++++++++++++++++
+- Add runs linked technique to the list of available keys on the Run class
+- Add runs linked technique to the general register_run and close_run methods
+- Add tests to test adding/removing runs_techniques_attributes
+- Upgrade dependencies
+
+v3.10.1 (14 February 2023)
+++++++++++++++++++++++++++
+- Upgrade dependencies
+- Update gitlab-ci proxy information
+
+v3.10.0 (17 January 2023)
++++++++++++++++++++++++++
+- Update package dependencies
+- Add Techniques module APIs and Module
+
 v3.9.0 (24 June 2022)
 +++++++++++++++++++++
 - Update dependencies certifi and requests
 - Drop support for python 3.6 (latest requests tag dropped support to python 3.6)
 - Add CI tests to python latest (currently version 3.11)
 
 v3.8.0 (13 May 2022)
```

### Comparing `metadata_client-3.9.0/LICENSE` & `metadata_client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/PKG-INFO` & `metadata_client-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: metadata_client
-Version: 3.9.0
+Version: 4.0.0
 Summary: Python Client for European XFEL Metadata Catalogue Web App available at https://in.xfel.eu/metadata
-Home-page: https://git.xfel.eu/gitlab/ITDM/metadata_client
+Home-page: https://git.xfel.eu/ITDM/metadata_client
 Author: Luís Maia
 Author-email: luis.maia@xfel.eu
 Maintainer: Luís Maia
 Maintainer-email: luis.maia@xfel.eu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,22 +33,22 @@
 
 This library (metadata_client) is a client for the RESTful APIs exposed
 by the European XFEL Metadata Catalogue Web Application - myMdC
 (https://in.xfel.eu/metadata).
 
 *Repository:*
 
-- https://git.xfel.eu/gitlab/ITDM/metadata_client
+- https://git.xfel.eu/ITDM/metadata_client
 
 *Dependencies:*
 
 - oauthlib (https://pypi.python.org/pypi/oauthlib)
 - requests (https://github.com/psf/requests)
 - requests-oauthlib (https://github.com/requests/requests-oauthlib)
-- oauth2_xfel_client (https://git.xfel.eu/gitlab/ITDM/oauth2_xfel_client)
+- oauth2_xfel_client (https://git.xfel.eu/ITDM/oauth2_xfel_client)
 - pytz (https://pypi.org/project/pytz/)
 
 Installation
 ------------
 
 Python project
 """"""""""""""
@@ -83,21 +83,21 @@
     # Install dependencies from local wheels files
     pip install . --no-index --find-links ./external_dependencies/
 
     # Install dependencies from the pypi
     pip install .
 
     # Force re-installation of packages
-    pip install --ignore-installed
+    pip install . --ignore-installed
 
  Installing it will place two folders under the current Python installation
  site-packages folder:
 
  - `metadata_client` with the sources;
- - `metadata_client-3.9.0.dist-info/` with Wheels configuration files.
+ - `metadata_client-4.0.0.dist-info/` with Wheels configuration files.
 
  To identify your Python site-packages folder run::
 
     python -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
 
 
 Usage
@@ -203,15 +203,15 @@
     all_xfel_instruments = client_conn.get_all_xfel_instruments(page=1, page_size=1)
     all_xfel_instruments
 
     # >>> {'success': True,
     #      'info': 'Got instrument successfully',
     #      'app_info': {},
     #      'pagination': {'Date': 'Wed, 11 May 2022 09:57:45 GMT', 'X-Total-Pages': '21', 'X-Count-Per-Page': '1', 'X-Current-Page': '1', 'X-Total-Count': '21'},
-    #      'data': [{'id': 1, 'name': 'SPB/SFX SASE1', 'identifier': 'SPB', 'url': 'https://www.xfel.eu/facility/instruments/spb_sfx', 'leading_scientist_id': 230, 'deputy_leading_scientist_id': 1018, 'facility_id': 1, 'instrument_type_id': 2, 'repository_id': 103, 'topic_id': 1, 'dsg_host': None, 'system_user': None, 'flg_online_resource': True, 'online_script': 'make_online', 'flg_available': True, 'description': 'The Single Particles, Clusters, and Biomolecules & Serial Femtosecond Crystallography (SPB/SFX) instrument of the European XFEL is primarily concerned with three-dimensional diffractive imaging, and three-dimensional structure determination, of micrometre-scale and smaller objects, at atomic or near-atomic¿resolution.', 'doi': None, 'techniques': [{'id': 250, 'identifier': 'PaNET01168', 'name': 'serial femtosecond crystallography', 'url': 'http://purl.org/pan-science/PaNET/PaNET01168', 'flg_available': True, 'description': None}, {'id': 259, 'identifier': 'PaNET01188', 'name': 'small angle x-ray scattering', 'url': 'http://purl.org/pan-science/PaNET/PaNET01188', 'flg_available': True, 'description': None}, {'id': 364, 'identifier': 'PaNET01101', 'name': 'x-ray powder diffraction', 'url': 'http://purl.org/pan-science/PaNET/PaNET01101', 'flg_available': True, 'description': None}, {'id': 28, 'identifier': 'PaNET01174', 'name': 'coherent diffraction imaging', 'url': 'http://purl.org/pan-science/PaNET/PaNET01174', 'flg_available': True, 'description': None}]}]}
+    #      'data': [{'id': 1, 'name': 'SPB/SFX SASE1', 'identifier': 'SPB', 'url': 'https://www.xfel.eu/facility/instruments/spb_sfx', 'instrument_leader_id': 230, 'deputy_instrument_leader_id': 1018, 'facility_id': 1, 'instrument_type_id': 2, 'repository_id': 103, 'topic_id': 1, 'dsg_host': None, 'system_user': None, 'flg_online_resource': True, 'online_script': 'make_online', 'flg_available': True, 'description': 'The Single Particles, Clusters, and Biomolecules & Serial Femtosecond Crystallography (SPB/SFX) instrument of the European XFEL is primarily concerned with three-dimensional diffractive imaging, and three-dimensional structure determination, of micrometre-scale and smaller objects, at atomic or near-atomic¿resolution.', 'doi': None, 'techniques': [{'id': 250, 'identifier': 'PaNET01168', 'name': 'serial femtosecond crystallography', 'url': 'http://purl.org/pan-science/PaNET/PaNET01168', 'flg_available': True, 'description': None}, {'id': 259, 'identifier': 'PaNET01188', 'name': 'small angle x-ray scattering', 'url': 'http://purl.org/pan-science/PaNET/PaNET01188', 'flg_available': True, 'description': None}, {'id': 364, 'identifier': 'PaNET01101', 'name': 'x-ray powder diffraction', 'url': 'http://purl.org/pan-science/PaNET/PaNET01101', 'flg_available': True, 'description': None}, {'id': 28, 'identifier': 'PaNET01174', 'name': 'coherent diffraction imaging', 'url': 'http://purl.org/pan-science/PaNET/PaNET01174', 'flg_available': True, 'description': None}]}]}
 
  2.3 Get instrument active proposal::
 
     active_proposal = client_conn.get_active_proposal_by_instrument(1)
 
  2.4 Register Run replica::
 
@@ -371,7 +371,9 @@
     python setup.py bdist_wheel
 
     # Upload new version .egg and .whl files
     twine upload dist/*
 
     # In case a test is necessary, it is possible to test it against test.pypi.org
     twine upload --repository-url https://test.pypi.org/legacy/ dist/* --verbose
+
+
```

### Comparing `metadata_client-3.9.0/README.rst` & `metadata_client-4.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 This library (metadata_client) is a client for the RESTful APIs exposed
 by the European XFEL Metadata Catalogue Web Application - myMdC
 (https://in.xfel.eu/metadata).
 
 *Repository:*
 
-- https://git.xfel.eu/gitlab/ITDM/metadata_client
+- https://git.xfel.eu/ITDM/metadata_client
 
 *Dependencies:*
 
 - oauthlib (https://pypi.python.org/pypi/oauthlib)
 - requests (https://github.com/psf/requests)
 - requests-oauthlib (https://github.com/requests/requests-oauthlib)
-- oauth2_xfel_client (https://git.xfel.eu/gitlab/ITDM/oauth2_xfel_client)
+- oauth2_xfel_client (https://git.xfel.eu/ITDM/oauth2_xfel_client)
 - pytz (https://pypi.org/project/pytz/)
 
 Installation
 ------------
 
 Python project
 """"""""""""""
@@ -55,21 +55,21 @@
     # Install dependencies from local wheels files
     pip install . --no-index --find-links ./external_dependencies/
 
     # Install dependencies from the pypi
     pip install .
 
     # Force re-installation of packages
-    pip install --ignore-installed
+    pip install . --ignore-installed
 
  Installing it will place two folders under the current Python installation
  site-packages folder:
 
  - `metadata_client` with the sources;
- - `metadata_client-3.9.0.dist-info/` with Wheels configuration files.
+ - `metadata_client-4.0.0.dist-info/` with Wheels configuration files.
 
  To identify your Python site-packages folder run::
 
     python -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
 
 
 Usage
@@ -175,15 +175,15 @@
     all_xfel_instruments = client_conn.get_all_xfel_instruments(page=1, page_size=1)
     all_xfel_instruments
 
     # >>> {'success': True,
     #      'info': 'Got instrument successfully',
     #      'app_info': {},
     #      'pagination': {'Date': 'Wed, 11 May 2022 09:57:45 GMT', 'X-Total-Pages': '21', 'X-Count-Per-Page': '1', 'X-Current-Page': '1', 'X-Total-Count': '21'},
-    #      'data': [{'id': 1, 'name': 'SPB/SFX SASE1', 'identifier': 'SPB', 'url': 'https://www.xfel.eu/facility/instruments/spb_sfx', 'leading_scientist_id': 230, 'deputy_leading_scientist_id': 1018, 'facility_id': 1, 'instrument_type_id': 2, 'repository_id': 103, 'topic_id': 1, 'dsg_host': None, 'system_user': None, 'flg_online_resource': True, 'online_script': 'make_online', 'flg_available': True, 'description': 'The Single Particles, Clusters, and Biomolecules & Serial Femtosecond Crystallography (SPB/SFX) instrument of the European XFEL is primarily concerned with three-dimensional diffractive imaging, and three-dimensional structure determination, of micrometre-scale and smaller objects, at atomic or near-atomic¿resolution.', 'doi': None, 'techniques': [{'id': 250, 'identifier': 'PaNET01168', 'name': 'serial femtosecond crystallography', 'url': 'http://purl.org/pan-science/PaNET/PaNET01168', 'flg_available': True, 'description': None}, {'id': 259, 'identifier': 'PaNET01188', 'name': 'small angle x-ray scattering', 'url': 'http://purl.org/pan-science/PaNET/PaNET01188', 'flg_available': True, 'description': None}, {'id': 364, 'identifier': 'PaNET01101', 'name': 'x-ray powder diffraction', 'url': 'http://purl.org/pan-science/PaNET/PaNET01101', 'flg_available': True, 'description': None}, {'id': 28, 'identifier': 'PaNET01174', 'name': 'coherent diffraction imaging', 'url': 'http://purl.org/pan-science/PaNET/PaNET01174', 'flg_available': True, 'description': None}]}]}
+    #      'data': [{'id': 1, 'name': 'SPB/SFX SASE1', 'identifier': 'SPB', 'url': 'https://www.xfel.eu/facility/instruments/spb_sfx', 'instrument_leader_id': 230, 'deputy_instrument_leader_id': 1018, 'facility_id': 1, 'instrument_type_id': 2, 'repository_id': 103, 'topic_id': 1, 'dsg_host': None, 'system_user': None, 'flg_online_resource': True, 'online_script': 'make_online', 'flg_available': True, 'description': 'The Single Particles, Clusters, and Biomolecules & Serial Femtosecond Crystallography (SPB/SFX) instrument of the European XFEL is primarily concerned with three-dimensional diffractive imaging, and three-dimensional structure determination, of micrometre-scale and smaller objects, at atomic or near-atomic¿resolution.', 'doi': None, 'techniques': [{'id': 250, 'identifier': 'PaNET01168', 'name': 'serial femtosecond crystallography', 'url': 'http://purl.org/pan-science/PaNET/PaNET01168', 'flg_available': True, 'description': None}, {'id': 259, 'identifier': 'PaNET01188', 'name': 'small angle x-ray scattering', 'url': 'http://purl.org/pan-science/PaNET/PaNET01188', 'flg_available': True, 'description': None}, {'id': 364, 'identifier': 'PaNET01101', 'name': 'x-ray powder diffraction', 'url': 'http://purl.org/pan-science/PaNET/PaNET01101', 'flg_available': True, 'description': None}, {'id': 28, 'identifier': 'PaNET01174', 'name': 'coherent diffraction imaging', 'url': 'http://purl.org/pan-science/PaNET/PaNET01174', 'flg_available': True, 'description': None}]}]}
 
  2.3 Get instrument active proposal::
 
     active_proposal = client_conn.get_active_proposal_by_instrument(1)
 
  2.4 Register Run replica::
```

### Comparing `metadata_client-3.9.0/metadata_client/apis/__init__.py` & `metadata_client-4.0.0/metadata_client/apis/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 from .data_type_api import DataTypeApi
 from .experiment_api import ExperimentApi
 from .experiment_type_api import ExperimentTypeApi
 from .instrument_api import InstrumentApi
 from .parameter_api import ParameterApi
 from .parameter_type_api import ParameterTypeApi
 from .proposal_api import ProposalApi
+from .report_api import ReportApi
 from .repostory_api import RepositoryApi
 from .run_api import RunApi
 from .sample_api import SampleApi
+from .technique_api import TechniqueApi
 from .user_api import UserApi
```

### Comparing `metadata_client-3.9.0/metadata_client/apis/dark_run_api.py` & `metadata_client-4.0.0/metadata_client/apis/dark_run_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/data_file_api.py` & `metadata_client-4.0.0/metadata_client/apis/data_file_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/data_group_api.py` & `metadata_client-4.0.0/metadata_client/apis/data_group_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/data_group_repository_api.py` & `metadata_client-4.0.0/metadata_client/apis/data_group_repository_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/data_group_type_api.py` & `metadata_client-4.0.0/metadata_client/apis/data_group_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/data_source_group_version_api.py` & `metadata_client-4.0.0/metadata_client/apis/data_source_group_version_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/data_type_api.py` & `metadata_client-4.0.0/metadata_client/apis/data_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/experiment_api.py` & `metadata_client-4.0.0/metadata_client/apis/experiment_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/experiment_type_api.py` & `metadata_client-4.0.0/metadata_client/apis/experiment_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/instrument_api.py` & `metadata_client-4.0.0/metadata_client/apis/instrument_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/parameter_api.py` & `metadata_client-4.0.0/metadata_client/apis/parameter_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/parameter_type_api.py` & `metadata_client-4.0.0/metadata_client/apis/parameter_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/proposal_api.py` & `metadata_client-4.0.0/metadata_client/apis/proposal_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/repostory_api.py` & `metadata_client-4.0.0/metadata_client/apis/repostory_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/run_api.py` & `metadata_client-4.0.0/metadata_client/apis/run_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/sample_api.py` & `metadata_client-4.0.0/metadata_client/apis/sample_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/apis/user_api.py` & `metadata_client-4.0.0/metadata_client/apis/user_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/common/base.py` & `metadata_client-4.0.0/metadata_client/common/base.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/common/config.py` & `metadata_client-4.0.0/metadata_client/common/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,22 @@
 PARAMETER = 'parameter'
 PARAMETER_TYPE = 'parameter_type'
 PROPOSAL = 'proposal'
 USER = 'user'
 PROPOSALS_USER = 'proposals_user'
 REPOSITORY = 'repository'
 RUN = 'run'
+REPORT = 'report'
 RUN_DATA_GROUP = 'run_data_group'
 SAMPLE = 'sample'
 SAMPLE_TYPE = 'sample_type'
 DARK_RUN = 'dark_run'
+TECHNIQUE = 'technique'
+INSTRUMENTS_TECHNIQUE = 'instruments_technique'
+PROPOSALS_TECHNIQUE = 'proposals_technique'
 
 ##########################################################################
 #
 # API PAGINATION
 #
 ##########################################################################
 DEF_PAGE = 1
```

### Comparing `metadata_client-3.9.0/metadata_client/common/util.py` & `metadata_client-4.0.0/metadata_client/common/util.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/metadata_client.py` & `metadata_client-4.0.0/metadata_client/metadata_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import logging
 
 from .apis import (
     DataFileApi, DataGroupApi, DataGroupRepositoryApi, DataGroupTypeApi,
     DataSourceGroupApi, DataSourceGroupVersionApi, DataTypeApi, ExperimentApi,
     ExperimentTypeApi, InstrumentApi, ParameterApi, ParameterTypeApi,
     DarkRunApi,
-    ProposalApi, RepositoryApi, RunApi, SampleApi, UserApi)
+    ProposalApi, RepositoryApi, RunApi, SampleApi, UserApi,
+    TechniqueApi, ReportApi)
+from .common.config import DEF_PAGE, DEF_PAGE_SIZE
 # Import common classes
 from .common.util import Util
 from .modules import (
     DataFile, DataGroup, DataGroupRepository, DataGroupType,
     DataSourceGroup, DataSourceGroupVersion, Experiment,
     Instrument, Parameter, Proposal, Repository, Run, Sample)
-from .common.config import DEF_PAGE, DEF_PAGE_SIZE
 
 
 class MetadataClient(
     DataFileApi, DataGroupApi, DataGroupRepositoryApi, DataGroupTypeApi,
     DataSourceGroupApi, DataSourceGroupVersionApi, DataTypeApi, ExperimentApi,
     ExperimentTypeApi, InstrumentApi, ParameterApi, ParameterTypeApi,
-    DarkRunApi, ProposalApi, RepositoryApi, RunApi, SampleApi, UserApi
+    DarkRunApi, ProposalApi, RepositoryApi, RunApi, SampleApi, UserApi,
+    TechniqueApi, ReportApi
 ):
     def get_all_xfel_instruments(self, page=DEF_PAGE, page_size=DEF_PAGE_SIZE):
         resp = Instrument.get_all_from_xfel(self, page, page_size)
 
         if not resp['success']:
             error_msg = '{0} >> {1}'.format(resp['info'], resp['app_info'])
             logging.error(error_msg)
@@ -173,14 +175,15 @@
 
         if not resp['success']:
             error_msg = '{0} >> {1}'.format(resp['info'], resp['app_info'])
             logging.error(error_msg)
             return resp
 
         run_id = resp['data']['id']
+        runs_techniques = resp['data']['techniques']
         logging.debug('run_id: {0}'.format(run_id))
 
         resp = self.__create_data_group_from_dict(
             experiment_id, run_id, data_grp_dict
         )
 
         if not resp['success']:
@@ -197,14 +200,15 @@
         data_group_id = resp['data']['id']
         logging.debug('data_group_id: {0}'.format(data_group_id))
 
         # Build hash information to send back in case of success!
         result_info = {'experiment_id': str(experiment_id),
                        'sample_id': str(sample_id),
                        'run_id': str(run_id),
+                       'techniques': str(runs_techniques),
                        'data_group_id': str(data_group_id)}
 
         return {'info': 'Run registered successfully',
                 'success': True,
                 'data': result_info,
                 'app_info': {}}
 
@@ -385,14 +389,16 @@
             resp = Run.update_from_dict(self, run_id, run_dict)
 
             if not resp['success']:
                 error_msg = '{0} >> {1}'.format(resp['info'], resp['app_info'])
                 logging.error(error_msg)
                 return resp
 
+            runs_techniques = resp['data']['techniques']
+
         # CREATE Parameters from hash
         resp = self.__create_parameters_from_dict(dg_params_dict)
 
         if not resp['success']:
             error_msg = '{0} >> {1}'.format(resp['info'], resp['app_info'])
             logging.error(error_msg)
             return resp
@@ -400,15 +406,16 @@
         # data_file_id = resp['data']['id']
         # logging.debug('data_file_id: {0}'.format(data_file_id))
         logging.debug('response data: {0}'.format(resp['data']))
 
         # Build hash information to send back in case of success!
         result_info = {'experiment_id': str(experiment_id),
                        'sample_id': str(sample_id),
-                       'run_id': str(run_id)}
+                       'run_id': str(run_id),
+                       'techniques': str(runs_techniques)}
 
         return {'info': 'Run closed successfully',
                 'success': True,
                 'data': result_info,
                 'app_info': {}}
 
     def register_run_data_and_results(self,
@@ -601,14 +608,16 @@
 
         run_experiment_id = str(experiment_id)
 
         # Handles the situation when sample_id isn't specified
         run_sample_id = Util.get_opt_val(sample_id)
 
         run_run_number = run_dict['run_number']  # Mandatory
+        techniques = Util.get_opt_dict_val(run_dict,
+                                           'runs_techniques_attributes')
         run_run_alias = Util.get_opt_dict_val(run_dict, 'run_alias')
         run_begin_at = run_dict['begin_at']  # Mandatory
         run_end_at = Util.get_opt_dict_val(run_dict, 'end_at')
         run_first_train = Util.get_opt_dict_val(run_dict, 'first_train')
         run_last_train = Util.get_opt_dict_val(run_dict, 'last_train')
         run_flg_avail = Util.get_opt_dict_val(run_dict,
                                               'flg_available', 'true')
@@ -626,15 +635,16 @@
             'end_at': run_end_at,
             'first_train': run_first_train,
             'last_train': run_last_train,
             'flg_available': run_flg_avail,
             'flg_status': run_flg_status,
             'original_format': run_orig_format,
             'system_msg': run_sys_msg,
-            'description': run_desc
+            'description': run_desc,
+            'runs_techniques_attributes': techniques
         }
         logging.debug('Built Run: {0}'.format(mdc_run))
 
         #
         # Create Run from dictionary
         #
         return Run.create_from_dict(self, mdc_run)
```

### Comparing `metadata_client-3.9.0/metadata_client/modules/__init__.py` & `metadata_client-4.0.0/metadata_client/modules/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 from .data_type import DataType
 from .experiment import Experiment
 from .experiment_type import ExperimentType
 from .instrument import Instrument
 from .parameter import Parameter
 from .parameter_type import ParameterType
 from .proposal import Proposal
+from .report import Report
 from .repository import Repository
 from .run import Run
 from .sample import Sample
+from .technique import Technique
 from .user import User
```

### Comparing `metadata_client-3.9.0/metadata_client/modules/dark_run.py` & `metadata_client-4.0.0/metadata_client/modules/dark_run.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_file.py` & `metadata_client-4.0.0/metadata_client/modules/data_file.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_group.py` & `metadata_client-4.0.0/metadata_client/modules/data_group.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_group_repository.py` & `metadata_client-4.0.0/metadata_client/modules/data_group_repository.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_group_type.py` & `metadata_client-4.0.0/metadata_client/modules/data_group_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_source_group.py` & `metadata_client-4.0.0/metadata_client/modules/data_source_group.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_source_group_version.py` & `metadata_client-4.0.0/metadata_client/modules/data_source_group_version.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/data_type.py` & `metadata_client-4.0.0/metadata_client/modules/data_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/experiment.py` & `metadata_client-4.0.0/metadata_client/modules/experiment.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/experiment_type.py` & `metadata_client-4.0.0/metadata_client/modules/experiment_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/instrument.py` & `metadata_client-4.0.0/metadata_client/modules/instrument.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/parameter.py` & `metadata_client-4.0.0/metadata_client/modules/parameter.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/parameter_type.py` & `metadata_client-4.0.0/metadata_client/modules/parameter_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/proposal.py` & `metadata_client-4.0.0/metadata_client/modules/proposal.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/repository.py` & `metadata_client-4.0.0/metadata_client/modules/repository.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/run.py` & `metadata_client-4.0.0/metadata_client/modules/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 class Run:
     def __init__(self, metadata_client,
                  run_number, run_alias, experiment_id, sample_id,
                  begin_at, end_at, first_train, last_train,
                  flg_available, flg_status,
                  original_format, system_msg,
-                 description=''):
+                 description='',
+                 runs_techniques_attributes=[]):
         self.metadata_client = metadata_client
         self.id = None
         self.run_number = run_number
         self.run_alias = run_alias
         self.experiment_id = experiment_id
         self.sample_id = sample_id
         self.begin_at = begin_at
@@ -26,14 +27,15 @@
         self.first_train = first_train
         self.last_train = last_train
         self.flg_available = flg_available
         self.flg_status = flg_status
         self.original_format = original_format
         self.system_msg = system_msg
         self.description = description
+        self.runs_techniques_attributes = runs_techniques_attributes
 
     def create(self):
         mdc_client = self.metadata_client
         response = mdc_client.create_run_api(self.__get_resource())
 
         Base.cal_debug(MODULE_NAME, CREATE, response)
         res = Base.format_response(response, CREATE, CREATED, MODULE_NAME)
@@ -56,29 +58,36 @@
                                              self.__get_resource())
 
         Base.cal_debug(MODULE_NAME, UPDATE, response)
         return Base.format_response(response, UPDATE, OK, MODULE_NAME)
 
     @staticmethod
     def create_from_dict(mdc_client, run):
+
+        if 'runs_techniques_attributes' in run:
+            rt_attributes = run['runs_techniques_attributes']
+        else:
+            rt_attributes = []
+
         new_run = Run(
             metadata_client=mdc_client,
             run_number=run['run_number'],
             run_alias=run['run_alias'],
             experiment_id=run['experiment_id'],
             sample_id=run['sample_id'],
             begin_at=run['begin_at'],
             end_at=run['end_at'],
             first_train=run['first_train'],
             last_train=run['last_train'],
             flg_available=run['flg_available'],
             flg_status=run['flg_status'],
             original_format=run['original_format'],
             system_msg=run['system_msg'],
-            description=run['description'])
+            description=run['description'],
+            runs_techniques_attributes=rt_attributes)
 
         resp = new_run.create()
         return resp
 
     @staticmethod
     def update_from_dict(mdc_client, run_id, run):
         response = mdc_client.update_run_api(run_id, run)
@@ -167,12 +176,13 @@
                 'end_at': self.end_at,
                 'first_train': self.first_train,
                 'last_train': self.last_train,
                 'flg_available': self.flg_available,
                 'flg_status': self.flg_status,
                 'original_format': self.original_format,
                 'system_msg': self.system_msg,
-                'description': self.description
+                'description': self.description,
+                'runs_techniques_attributes': self.runs_techniques_attributes
             }
         }
 
         return run
```

### Comparing `metadata_client-3.9.0/metadata_client/modules/sample.py` & `metadata_client-4.0.0/metadata_client/modules/sample.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/modules/user.py` & `metadata_client-4.0.0/metadata_client/modules/user.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/api_base.py` & `metadata_client-4.0.0/metadata_client/tests/apis/api_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,23 @@
         resp_content = self.load_response_content(response)
         print('CREATE RESPONSE: {0}'.format(resp_content))
 
         self.assert_eq_status_code(response.status_code, CREATED)
 
         return resp_content
 
-    def get_and_validate_all_entries_by_name(self, response):
+    def get_and_validate_all_entries_by_name(self, response, pos_obj_ret=-1):
         resp_content = self.load_response_content(response)
         print('GET BY NAME RESPONSE: {0}'.format(resp_content))
 
         self.assert_eq_status_code(response.status_code, OK)
 
-        return resp_content[-1]
+        # By default, this method will always return the last entry
+        # of the array, unless explicitly requested.
+        return resp_content[pos_obj_ret]
 
     def get_and_validate_entry_by_id(self, response):
         resp_content = self.load_response_content(response)
         print('GET BY ID RESPONSE: {0}'.format(resp_content))
 
         self.assert_eq_status_code(response.status_code, OK)
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/dark_run_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/dark_run_api_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         scope=CLIENT_OAUTH2_INFO['SCOPE'],
         user_email=CLIENT_OAUTH2_INFO['EMAIL'],
         base_api_url=BASE_API_URL)
 
     def test_create_dark_run_api(self):
         __unique_name = Generators.generate_unique_name('DarkRunApi')
         __unique_identifier = Generators.generate_unique_identifier()
-        dark_run = {
+        dark_run_11 = {
             'dark_run': {
                 'proposal_id': -1,
                 'detector_id': -2,
                 'detector_identifier': 'TEST_DET_CI-11 - DO NOT DELETE!',
                 'detector_type_id': -1,
                 'pdu_physical_names':
                     '["PDU-3_DO_NOT_DELETE", "PDU-2_DO_NOT_DELETE"]',
@@ -42,29 +42,49 @@
                 'input_path': '',
                 'output_path': '',
                 'calcat_feedback': '',
                 'description': 'desc default1'
             }
         }
 
-        expect = dark_run['dark_run']
-
-        dark_run_id = -11
-        dark_run_proposal_id = -1
+        dark_run_12 = {
+            'dark_run': {
+                'proposal_id': -1,
+                'detector_id': -2,
+                'detector_identifier': 'TEST_DET_CI-12 - DO NOT DELETE!',
+                'detector_type_id': -1,
+                'pdu_physical_names':
+                    '["TEST_DAQ_DA_02 (Q1M2)", "TEST_DAQ_DA_03 (Q1M3)"]',
+                'runs_info': str([2]),
+                'operation_mode_id': -1,
+                'operation_mode_identifier': 'Operation_identifier-12',
+                'operation_mode_name': 'Operation Mode 2 - DO NOT DELETE!',
+                'flg_status': 'R',
+                # 'pdu_karabo_das': ['t1', 't2'],
+                'size': '',
+                'report_url': '',
+                'input_path': '',
+                'output_path': '',
+                'calcat_feedback': '',
+                'description': 'desc default2'
+            }
+        }
 
         #
         # Get entry by proposal_id
         #
+        dark_run_proposal_id = -1
         self.__get_all_entries_by_proposal_id_api(dark_run_proposal_id,
-                                                  dark_run['dark_run'])
+                                                  dark_run_12['dark_run'])
 
         #
         # Get entry by ID
         #
-        self.__get_entry_by_id_api(dark_run_id, dark_run['dark_run'])
+        dark_run_id = -11
+        self.__get_entry_by_id_api(dark_run_id, dark_run_11['dark_run'])
 
     #
     # fields_validation
     #
     def fields_validation(self, receive, expect):
         self.assert_eq_hfield(receive, expect, 'proposal_id', STRING)
         self.assert_eq_hfield(receive, expect, 'detector_id', STRING)
@@ -88,15 +108,17 @@
 
     #
     # Internal private APIs methods
     #
     def __get_all_entries_by_proposal_id_api(self, proposal_id, expect):
         response = self.client_api.get_all_dark_runs_by_proposal_id_api(
             proposal_id)
-        receive = self.get_and_validate_all_entries_by_name(response)
+
+        receive = self.get_and_validate_all_entries_by_name(response,
+                                                            pos_obj_ret=0)
         self.fields_validation(receive, expect)
 
     def __get_entry_by_id_api(self, entry_id, expect):
         response = self.client_api.get_dark_run_by_id_api(entry_id)
         receive = self.get_and_validate_entry_by_id(response)
         self.fields_validation(receive, expect)
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/data_file_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/data_file_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/data_group_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/data_group_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/data_group_repository_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/data_group_repository_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/data_group_type_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/data_group_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/data_type_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/data_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/experiment_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/experiment_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/experiment_type_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/experiment_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/instrument_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/instrument_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/parameter_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/parameter_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/parameter_type_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/parameter_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/proposal_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/proposal_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/repository_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/repository_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/run_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/run_api_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,28 +32,31 @@
                 'end_at': '2015-05-25T08:30:00.000+02:00',
                 'first_train': '1',
                 'last_train': '999',
                 'flg_available': 'true',
                 'flg_status': '1',
                 'original_format': '',
                 'system_msg': '',
-                'description': 'desc 01'
+                'description': 'desc 01',
+                'runs_techniques_attributes': [{'technique_id': -1}]
             }
         }
 
         expect = run[RUN]
 
         #
         # Create new entry (should succeed)
         #
         received = self.__create_entry_api(run, expect)
 
         run_id = received['id']
         run_number = received['run_number']
         experiment_id = received['experiment_id']
+        runs_techniques_id_pos0 = received['techniques'][0][
+            'runs_techniques_id']
 
         #
         # Create duplicated entry (should throw an error)
         #
         self.__create_error_entry_uk_api(run)
 
         #
@@ -77,15 +80,16 @@
         self.__get_entry_by_run_number_and_experiment_id_api(run_number,
                                                              experiment_id,
                                                              expect)
 
         #
         # Put entry information (update some fields should succeed)
         #
-        self.__update_entry_api(run_id, run_number, expect)
+        self.__update_entry_api(run_id, run_number,
+                                runs_techniques_id_pos0, expect)
 
         #
         # Delete entry (should succeed)
         # (test purposes only to keep the DB clean)
         #
         self.__delete_entry_by_id_api(run_id)
 
@@ -117,14 +121,24 @@
     # Internal private APIs methods
     #
     def __create_entry_api(self, entry_info, expect):
         response = self.client_api.create_run_api(entry_info)
         receive = self.get_and_validate_create_entry(response)
         self.fields_validation(receive, expect)
 
+        # Testing Technique association to the run
+        expected_linked_technique_id = \
+            expect['runs_techniques_attributes'][0]['technique_id']
+
+        self.assertEqual(len(receive['techniques']), 1,
+                         "Run should only have 1 technique linked")
+        self.assertEqual(
+            str(receive['techniques'][0]['id']),
+            str(expected_linked_technique_id), "Correctly linked technique id")
+
         return receive
 
     def __create_error_entry_uk_api(self, entry_info):
         response = self.client_api.create_run_api(entry_info)
         resp_content = self.load_response_content(response)
 
         receive = resp_content
@@ -136,30 +150,34 @@
         self.assert_eq_status_code(response.status_code, UNPROCESSABLE_ENTITY)
 
         # 'has already been taken'
         receive_msg = receive['info']['run_number'][0]
         expect_msg = expect['info']['run_number'][0]
         self.assert_eq_str(receive_msg, expect_msg)
 
-    def __update_entry_api(self, entry_id, run_number, expect):
+    def __update_entry_api(self, entry_id, run_number,
+                           runs_techniques_id_pos0, expect):
         run_upd = {
             RUN: {
                 'run_number': run_number,  # This field cannot be updated
                 'run_alias': 'Run_Alias_Updated...',
                 'experiment_id': '-1',
                 'sample_id': '-1',
-                'begin_at': '2014-06-25T08:30:00.000+02:00',
-                'end_at': '2015-06-25T08:30:00.000+02:00',
+                'begin_at': '2015-06-25T08:30:00.000+02:00',
+                'end_at': '2016-06-25T08:30:00.000+02:00',
                 'first_train': 9223372036854775802,
                 'last_train': 9223372036854775807,
                 'flg_available': 'false',
                 'flg_status': '-1',
                 'original_format': 'format updated',
                 'system_msg': 'system msg update',
-                'description': 'desc 01 updated!!!'
+                'description': 'desc 01 updated!!!',
+                'runs_techniques_attributes':
+                    [{'id': runs_techniques_id_pos0, '_destroy': 1},
+                     {'technique_id': -2}]
             }
         }
 
         res = self.client_api.update_run_api(entry_id, run_upd)
         resp_content = self.load_response_content(res)
 
         receive = resp_content
@@ -192,14 +210,24 @@
         field = 'original_format'
         self.assert_not_eq_str(expect[field], expect_upd[field], field)
         field = 'system_msg'
         self.assert_not_eq_str(expect[field], expect_upd[field], field)
         field = 'description'
         self.assert_not_eq_str(expect[field], expect_upd[field], field)
 
+        # Testing Technique association to the run
+        expected_linked_technique_id = \
+            run_upd[RUN]['runs_techniques_attributes'][1]['technique_id']
+
+        self.assertEqual(len(receive['techniques']), 1,
+                         "Run should only have 1 technique linked")
+        self.assertEqual(
+            str(receive['techniques'][0]['id']),
+            str(expected_linked_technique_id), "Correctly linked technique id")
+
     def __get_all_entries_by_run_number_api(self, run_number, expect):
         response = self.client_api.get_all_runs_by_run_number_api(
             run_number, page=DEF_PAGE, page_size=10)
         receive = self.get_and_validate_all_entries_by_name(response)
         self.fields_validation(receive, expect)
 
     def __get_all_entries_by_proposal_number_api(self, prop_number, expect):
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/sample_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/sample_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/apis/user_api_test.py` & `metadata_client-4.0.0/metadata_client/tests/apis/user_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/base_test.py` & `metadata_client-4.0.0/metadata_client/tests/common/base_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/config_test.py` & `metadata_client-4.0.0/metadata_client/tests/common/config_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,22 @@
 GROUP = 'group'
 PARAMETER = 'parameter'
 PARAMETER_TYPE = 'parameter_type'
 PROPOSAL = 'proposal'
 PROPOSALS_USER = 'proposals_user'
 REPOSITORY = 'repository'
 RUN = 'run'
+REPORT = 'report'
 RUN_DATA_GROUP = 'run_data_group'
 SAMPLE = 'sample'
 SAMPLE_TYPE = 'sample_type'
 DARK_RUN = 'dark_run'
+TECHNIQUE = 'technique'
+INSTRUMENTS_TECHNIQUE = 'instruments_technique'
+PROPOSALS_TECHNIQUE = 'proposals_technique'
 
 ##########################################################################
 #
 # API PAGINATION
 #
 ##########################################################################
 DEF_PAGE = 1
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/generators.py` & `metadata_client-4.0.0/metadata_client/tests/common/generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,30 @@
     def generate_unique_id(min_value=1, max_value=9999):
         unique_id = randrange(min_value, max_value)
 
         logging.debug('generate::unique_id == {0}'.format(unique_id))
         return unique_id
 
     @staticmethod
+    def generate_unique_name_short(prefix):
+        dt_str1 = Util.get_formatted_date('%Y-%m-%d')
+        dt_str2 = Util.get_formatted_date('%H:%M:%S')
+        host = socket.gethostname()
+        rand = randrange(999)
+
+        unique_str = '{0} {1} {2} {3} {4}'.format(prefix, dt_str2,
+                                                  host, dt_str1, rand)
+        if len(unique_str) > 32:
+            unique_str = '{0}..'.format(unique_str[:30])
+
+        logging.debug('generate::unique_name == {0}'.format(unique_str))
+
+        return unique_str
+
+    @staticmethod
     def generate_unique_name(prefix):
         dt_str = Util.get_formatted_date('%Y-%m-%d %H:%M:%S')
         host = socket.gethostname()
         rand = randrange(999)
 
         unique_str = '{0} {1} {2} {3}'.format(prefix, host, dt_str, rand)
         if len(unique_str) > 60:
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/secrets.py` & `metadata_client-4.0.0/metadata_client/tests/common/secrets.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 #
 # Listening on http://127.0.0.1:3000
 # Listening on ssl://0.0.0.0:8443?cert=/Users/maial/development/gitlab/ITDM/metadata_catalog/config/certs/localhost.crt&key=/Users/maial/development/gitlab/ITDM/metadata_catalog/config/certs/localhost.key&verify_mode=none  # noqa
 ###############################################################################
 
 # __USER_EMAIL = 'luis.maia@xfel.eu'
 # __CLIENT_ID = '201ed15ff071a63e76cb0b91a1ab17b36d5f92d24b6df4497aa646e39c46a324'  # noqa
-# __CLIENT_SECRET = 'a8ae80f5e96531f19bf2d2b6102f5a537196aca44a673ad36533310e07529757'  # noqa
+# __CLIENT_SECRET = 'PUT_HERE_YOUR_SECRET_KEY'  # noqa
 
 ###############################################################################
 # Remote setup:
 #
 # Listening on https://in.xfel.eu/test_metadata
 ###############################################################################
 
 __USER_EMAIL = 'luis.maia@xfel.eu'
-__CLIENT_ID = '1cc9d1cd5e2752c26df9aa84d64927505ce43305ecc7c388d9b54e1f4deb3aab'  # noqa
-__CLIENT_SECRET = '84b7295a40d8711b19eac7995a7d3e6b5c416a71dd11b9e033e46302aefe3925'  # noqa
+__CLIENT_ID = 'PUT_HERE_YOUR_CLIENT_KEY'  # noqa
+__CLIENT_SECRET = 'PUT_HERE_YOUR_SECRET_KEY'  # noqa
 
 ###############################################################################
 
 __OAUTH_TOKEN_URL = '{0}/oauth/token'.format(__APP_URL)
 __OAUTH_AUTHORIZE_URL = '{0}/oauth/authorize'.format(__APP_URL)
 
 ###############################################################################
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/util.py` & `metadata_client-4.0.0/metadata_client/tests/common/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """UtilTest Class with generic and util helper methods"""
 
+import ast
 import json
 import unittest
 
 from dateutil import parser
 
 from .config_test import *
 
 
 class Util(unittest.TestCase):
     @staticmethod
+    def str_to_array_of_dicts(array_str):
+        return ast.literal_eval(array_str)
+
+    @staticmethod
     def escape_and_load_json_from_str(hash_str):
         if hash_str == '':
             return {}
         else:
             protected_dict_str = hash_str.replace("'", "\"")
             return json.loads(protected_dict_str)
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/util_datetime.py` & `metadata_client-4.0.0/metadata_client/tests/common/util_datetime.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/common/util_test.py` & `metadata_client-4.0.0/metadata_client/tests/common/util_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/metadata_client_connection_test.py` & `metadata_client-4.0.0/metadata_client/tests/metadata_client_connection_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/metadata_client_test.py` & `metadata_client-4.0.0/metadata_client/tests/metadata_client_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import unittest
 
 from metadata_client.metadata_client import MetadataClient
 from .common.config_test import *
 from .common.secrets import *
+from .common.util import Util
 from .modules.module_base import ModuleBase
 
 
 class MetadataClientTest(ModuleBase, unittest.TestCase):
     def setUp(self):
         self.mdc_client = MetadataClient(
             client_id=CLIENT_OAUTH2_INFO['CLIENT_ID'],
@@ -210,15 +211,16 @@
         self.assert_eq_val(second_run['run_number'], 2)
         self.assert_eq_val(second_run['flg_status'], 1)
         self.assert_eq_val(second_run['flg_run_quality'], -1)
         self.assert_eq_val(second_run['num_files'], 0)
 
     def test_get_proposal_runs_first_page(self):
         proposal_number = 0
-        resp = self.mdc_client.get_proposal_runs(proposal_number, page=2,
+        resp = self.mdc_client.get_proposal_runs(proposal_number,
+                                                 page=DEF_PAGE,
                                                  page_size=1)
 
         # Logging information
         logging.error('resp: {0}'.format(resp))
 
         self.assert_eq_val(resp['app_info'], {})
         self.assert_eq_val(resp['success'], True)
@@ -238,15 +240,15 @@
                            'XFEL Tests Repository')
         self.assert_eq_val(first_repo['mount_point'], '/webstorage/XFEL')
         self.assert_eq_val(first_repo['data_groups'], 1)
 
     def test_get_proposal_runs_second_page(self):
         proposal_number = 0
         resp = self.mdc_client.get_proposal_runs(proposal_number,
-                                                 page=DEF_PAGE,
+                                                 page=2,
                                                  page_size=1)
 
         # Logging information
         logging.error('resp: {0}'.format(resp))
 
         self.assert_eq_val(resp['app_info'], {})
         self.assert_eq_val(resp['success'], True)
@@ -988,15 +990,16 @@
                     'end_at': '2015-06-25T08:30:00.000+02:00',
                     'last_train': -1,
                     'flg_available': 1,
                     'flg_status': 1}
         #
         dg_parameters_ar = {
             'parameters': [
-                {'data_source': 'MID/XTD6/ATT/MOTOR/BLADE_TOP',
+                {'id': -100,
+                 'data_source': 'MID/XTD6/ATT/MOTOR/BLADE_TOP',
                  'name': 'Velocity Right',
                  'value': 15.6,
                  'minimum': 15.6,
                  'maximum': 15.6,
                  'mean': 15.6,
                  'standard_deviation': 15.6,
                  'data_type_id': 2,
@@ -1052,15 +1055,16 @@
         data_group_id = run_info['data_group_id']
         data_file_id = run_info['data_file_id']
         #
         run_dict = {}
         #
         dg_parameters_ar = {
             'parameters': [
-                {'data_source': 'MID/XTD6/ATT/MOTOR/BLADE_TOP',
+                {'id': -101,
+                 'data_source': 'MID/XTD6/ATT/MOTOR/BLADE_TOP',
                  # 'name': 'Velocity Right',
                  'name': '',
                  'value': 15.6,
                  'minimum': 15.6,
                  'maximum': 15.6,
                  'mean': 15.6,
                  'standard_deviation': 15.6,
@@ -1202,19 +1206,23 @@
         self.__test_delete_parameters_by_data_group_id(data_group_id)
         # DELETE created DataGroup...
         self.__test_delete_data_group_by_id(data_group_id)
 
     def __test_successful_register_run(self):
         experiment_id = -1
         sample_id = -1
+        expected_linked_technique_id = -1
 
         run_number_val = 126
         run_dict = {'run_number': run_number_val,
                     'begin_at': '2014-06-25T08:30:00.000+02:00',
-                    'first_train': 126}
+                    'first_train': 126,
+                    'runs_techniques_attributes':
+                        [{'technique_id': expected_linked_technique_id}]
+                    }
 
         __prefix_path = '/webstorage/XFEL/raw/SPB/2016_01/p0008/e0001/'
         data_grp_dict = {'data_group_type_id': '1',
                          # 'experiment_id': '-1',
                          'creator_id': '-1',  # user_id
                          'prefix_path': __prefix_path}
 
@@ -1230,14 +1238,15 @@
         #
         # resp = {'info': 'Run registered successfully',
         #         'success': True,
         #         'app_info': {},
         #         'data': {'experiment_id': '-1',
         #                  'sample_id': '-1',
         #                  'run_id': '343',
+        #                  'runs_techniques': '[]'
         #                  'data_group_id': '574'}
         #         }
 
         # The new IDs received are:
         run_id = resp['data']['run_id']
         data_group_id = resp['data']['data_group_id']
 
@@ -1246,14 +1255,23 @@
         self.assert_eq_val(resp['success'], True)
         self.assert_eq_val(resp['app_info'], {})
         self.assert_eq_val(resp['data']['experiment_id'], experiment_id)
         self.assert_eq_val(resp['data']['sample_id'], sample_id)
         self.assert_not_eq_str(run_id, '', 'run_id')
         self.assert_not_eq_str(data_group_id, '', 'data_group_id')
 
+        # Testing Technique association to the run
+        run_techniques = Util.str_to_array_of_dicts(resp['data']['techniques'])
+
+        self.assertEqual(len(run_techniques), 1,
+                         "Run should only have 1 technique linked")
+        self.assertEqual(
+            str(run_techniques[0]['id']),
+            str(expected_linked_technique_id), "Correctly linked technique id")
+
         return {'experiment_id': experiment_id,
                 'sample_id': sample_id,
                 'run_id': run_id,
                 'run_number': run_number_val,
                 'data_group_id': data_group_id}
 
     def __test_successful_register_data_run(self):
@@ -1317,23 +1335,29 @@
         run_info = self.__test_successful_register_data_run()
         experiment_id = run_info['experiment_id']
         sample_id = run_info['sample_id']
         run_id = run_info['run_id']
         run_number = run_info['run_number']
         data_group_id = run_info['data_group_id']
         data_file_id = run_info['data_file_id']
+
+        expected_new_linked_technique_id = -2
         #
         run_dict = {'end_at': '2015-06-25T08:30:00.000+02:00',
                     'last_train': 127,
                     'flg_available': 1,
-                    'flg_status': 1}
+                    'flg_status': 1,
+                    'runs_techniques_attributes':
+                        [{'technique_id': expected_new_linked_technique_id}]
+                    }
         #
         dg_parameters_ar = {
             'parameters': [
-                {'data_source': 'MID/XTD6/ATT/MOTOR/BLADE_TOP',
+                {'id': -102,
+                 'data_source': 'MID/XTD6/ATT/MOTOR/BLADE_TOP',
                  'name': 'VelocityLeft',
                  'value': 15.6,
                  'minimum': 15.6,
                  'maximum': 15.6,
                  'mean': 15.6,
                  'standard_deviation': 15.6,
                  'data_type_id': 2,
@@ -1367,14 +1391,25 @@
         self.assert_eq_val(resp['success'], True)
         self.assert_eq_val(resp['app_info'], {})
         #
         self.assert_eq_val(resp['data']['sample_id'], sample_id)
         self.assert_eq_val(resp['data']['run_id'], run_id)
         self.assert_eq_val(resp['data']['experiment_id'], experiment_id)
 
+        # Testing Technique association to the run
+        run_techniques = Util.str_to_array_of_dicts(resp['data']['techniques'])
+
+        self.assertEqual(len(run_techniques), 2,
+                         "Run should only have 2 technique linked")
+        self.assertEqual(str(run_techniques[0]['id']), '-1',
+                         "Correctly linked old technique id")
+        self.assertEqual(str(run_techniques[1]['id']),
+                         str(expected_new_linked_technique_id),
+                         "Correctly linked new technique id")
+
         return {'experiment_id': experiment_id,
                 'sample_id': sample_id,
                 'run_id': run_id,
                 'run_number': run_number,
                 'data_group_id': data_group_id,
                 'data_file_id': data_file_id}
```

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/dark_run_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/dark_run_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/data_file_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/data_file_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/data_group_repository_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/data_group_repository_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/data_group_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/data_group_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/data_group_type_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/data_group_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/data_type_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/data_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/experiment_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/experiment_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/experiment_type_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/experiment_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/module_base.py` & `metadata_client-4.0.0/metadata_client/tests/modules/module_base.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/parameter_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/parameter_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/parameter_type_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/parameter_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/proposal_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/proposal_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/repository_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/repository_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/run_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/run_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client/tests/modules/sample_test.py` & `metadata_client-4.0.0/metadata_client/tests/modules/sample_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.9.0/metadata_client.egg-info/PKG-INFO` & `metadata_client-4.0.0/metadata_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: metadata-client
-Version: 3.9.0
+Version: 4.0.0
 Summary: Python Client for European XFEL Metadata Catalogue Web App available at https://in.xfel.eu/metadata
-Home-page: https://git.xfel.eu/gitlab/ITDM/metadata_client
+Home-page: https://git.xfel.eu/ITDM/metadata_client
 Author: Luís Maia
 Author-email: luis.maia@xfel.eu
 Maintainer: Luís Maia
 Maintainer-email: luis.maia@xfel.eu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,22 +33,22 @@
 
 This library (metadata_client) is a client for the RESTful APIs exposed
 by the European XFEL Metadata Catalogue Web Application - myMdC
 (https://in.xfel.eu/metadata).
 
 *Repository:*
 
-- https://git.xfel.eu/gitlab/ITDM/metadata_client
+- https://git.xfel.eu/ITDM/metadata_client
 
 *Dependencies:*
 
 - oauthlib (https://pypi.python.org/pypi/oauthlib)
 - requests (https://github.com/psf/requests)
 - requests-oauthlib (https://github.com/requests/requests-oauthlib)
-- oauth2_xfel_client (https://git.xfel.eu/gitlab/ITDM/oauth2_xfel_client)
+- oauth2_xfel_client (https://git.xfel.eu/ITDM/oauth2_xfel_client)
 - pytz (https://pypi.org/project/pytz/)
 
 Installation
 ------------
 
 Python project
 """"""""""""""
@@ -83,21 +83,21 @@
     # Install dependencies from local wheels files
     pip install . --no-index --find-links ./external_dependencies/
 
     # Install dependencies from the pypi
     pip install .
 
     # Force re-installation of packages
-    pip install --ignore-installed
+    pip install . --ignore-installed
 
  Installing it will place two folders under the current Python installation
  site-packages folder:
 
  - `metadata_client` with the sources;
- - `metadata_client-3.9.0.dist-info/` with Wheels configuration files.
+ - `metadata_client-4.0.0.dist-info/` with Wheels configuration files.
 
  To identify your Python site-packages folder run::
 
     python -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
 
 
 Usage
@@ -203,15 +203,15 @@
     all_xfel_instruments = client_conn.get_all_xfel_instruments(page=1, page_size=1)
     all_xfel_instruments
 
     # >>> {'success': True,
     #      'info': 'Got instrument successfully',
     #      'app_info': {},
     #      'pagination': {'Date': 'Wed, 11 May 2022 09:57:45 GMT', 'X-Total-Pages': '21', 'X-Count-Per-Page': '1', 'X-Current-Page': '1', 'X-Total-Count': '21'},
-    #      'data': [{'id': 1, 'name': 'SPB/SFX SASE1', 'identifier': 'SPB', 'url': 'https://www.xfel.eu/facility/instruments/spb_sfx', 'leading_scientist_id': 230, 'deputy_leading_scientist_id': 1018, 'facility_id': 1, 'instrument_type_id': 2, 'repository_id': 103, 'topic_id': 1, 'dsg_host': None, 'system_user': None, 'flg_online_resource': True, 'online_script': 'make_online', 'flg_available': True, 'description': 'The Single Particles, Clusters, and Biomolecules & Serial Femtosecond Crystallography (SPB/SFX) instrument of the European XFEL is primarily concerned with three-dimensional diffractive imaging, and three-dimensional structure determination, of micrometre-scale and smaller objects, at atomic or near-atomic¿resolution.', 'doi': None, 'techniques': [{'id': 250, 'identifier': 'PaNET01168', 'name': 'serial femtosecond crystallography', 'url': 'http://purl.org/pan-science/PaNET/PaNET01168', 'flg_available': True, 'description': None}, {'id': 259, 'identifier': 'PaNET01188', 'name': 'small angle x-ray scattering', 'url': 'http://purl.org/pan-science/PaNET/PaNET01188', 'flg_available': True, 'description': None}, {'id': 364, 'identifier': 'PaNET01101', 'name': 'x-ray powder diffraction', 'url': 'http://purl.org/pan-science/PaNET/PaNET01101', 'flg_available': True, 'description': None}, {'id': 28, 'identifier': 'PaNET01174', 'name': 'coherent diffraction imaging', 'url': 'http://purl.org/pan-science/PaNET/PaNET01174', 'flg_available': True, 'description': None}]}]}
+    #      'data': [{'id': 1, 'name': 'SPB/SFX SASE1', 'identifier': 'SPB', 'url': 'https://www.xfel.eu/facility/instruments/spb_sfx', 'instrument_leader_id': 230, 'deputy_instrument_leader_id': 1018, 'facility_id': 1, 'instrument_type_id': 2, 'repository_id': 103, 'topic_id': 1, 'dsg_host': None, 'system_user': None, 'flg_online_resource': True, 'online_script': 'make_online', 'flg_available': True, 'description': 'The Single Particles, Clusters, and Biomolecules & Serial Femtosecond Crystallography (SPB/SFX) instrument of the European XFEL is primarily concerned with three-dimensional diffractive imaging, and three-dimensional structure determination, of micrometre-scale and smaller objects, at atomic or near-atomic¿resolution.', 'doi': None, 'techniques': [{'id': 250, 'identifier': 'PaNET01168', 'name': 'serial femtosecond crystallography', 'url': 'http://purl.org/pan-science/PaNET/PaNET01168', 'flg_available': True, 'description': None}, {'id': 259, 'identifier': 'PaNET01188', 'name': 'small angle x-ray scattering', 'url': 'http://purl.org/pan-science/PaNET/PaNET01188', 'flg_available': True, 'description': None}, {'id': 364, 'identifier': 'PaNET01101', 'name': 'x-ray powder diffraction', 'url': 'http://purl.org/pan-science/PaNET/PaNET01101', 'flg_available': True, 'description': None}, {'id': 28, 'identifier': 'PaNET01174', 'name': 'coherent diffraction imaging', 'url': 'http://purl.org/pan-science/PaNET/PaNET01174', 'flg_available': True, 'description': None}]}]}
 
  2.3 Get instrument active proposal::
 
     active_proposal = client_conn.get_active_proposal_by_instrument(1)
 
  2.4 Register Run replica::
 
@@ -371,7 +371,9 @@
     python setup.py bdist_wheel
 
     # Upload new version .egg and .whl files
     twine upload dist/*
 
     # In case a test is necessary, it is possible to test it against test.pypi.org
     twine upload --repository-url https://test.pypi.org/legacy/ dist/* --verbose
+
+
```

### Comparing `metadata_client-3.9.0/metadata_client.egg-info/SOURCES.txt` & `metadata_client-4.0.0/metadata_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,20 @@
 metadata_client/apis/data_type_api.py
 metadata_client/apis/experiment_api.py
 metadata_client/apis/experiment_type_api.py
 metadata_client/apis/instrument_api.py
 metadata_client/apis/parameter_api.py
 metadata_client/apis/parameter_type_api.py
 metadata_client/apis/proposal_api.py
+metadata_client/apis/proposal_technique_api.py
+metadata_client/apis/report_api.py
 metadata_client/apis/repostory_api.py
 metadata_client/apis/run_api.py
 metadata_client/apis/sample_api.py
+metadata_client/apis/technique_api.py
 metadata_client/apis/user_api.py
 metadata_client/common/__init__.py
 metadata_client/common/base.py
 metadata_client/common/config.py
 metadata_client/common/util.py
 metadata_client/modules/__init__.py
 metadata_client/modules/dark_run.py
@@ -46,17 +49,20 @@
 metadata_client/modules/data_type.py
 metadata_client/modules/experiment.py
 metadata_client/modules/experiment_type.py
 metadata_client/modules/instrument.py
 metadata_client/modules/parameter.py
 metadata_client/modules/parameter_type.py
 metadata_client/modules/proposal.py
+metadata_client/modules/proposal_technique.py
+metadata_client/modules/report.py
 metadata_client/modules/repository.py
 metadata_client/modules/run.py
 metadata_client/modules/sample.py
+metadata_client/modules/technique.py
 metadata_client/modules/user.py
 metadata_client/tests/__init__.py
 metadata_client/tests/metadata_client_connection_test.py
 metadata_client/tests/metadata_client_test.py
 metadata_client/tests/apis/__init__.py
 metadata_client/tests/apis/api_base.py
 metadata_client/tests/apis/dark_run_api_test.py
@@ -67,17 +73,19 @@
 metadata_client/tests/apis/data_type_api_test.py
 metadata_client/tests/apis/experiment_api_test.py
 metadata_client/tests/apis/experiment_type_api_test.py
 metadata_client/tests/apis/instrument_api_test.py
 metadata_client/tests/apis/parameter_api_test.py
 metadata_client/tests/apis/parameter_type_api_test.py
 metadata_client/tests/apis/proposal_api_test.py
+metadata_client/tests/apis/report_api_test.py
 metadata_client/tests/apis/repository_api_test.py
 metadata_client/tests/apis/run_api_test.py
 metadata_client/tests/apis/sample_api_test.py
+metadata_client/tests/apis/technique_api_test.py
 metadata_client/tests/apis/user_api_test.py
 metadata_client/tests/common/__init__.py
 metadata_client/tests/common/base_test.py
 metadata_client/tests/common/config_test.py
 metadata_client/tests/common/generators.py
 metadata_client/tests/common/secrets.py
 metadata_client/tests/common/util.py
@@ -92,10 +100,12 @@
 metadata_client/tests/modules/data_type_test.py
 metadata_client/tests/modules/experiment_test.py
 metadata_client/tests/modules/experiment_type_test.py
 metadata_client/tests/modules/module_base.py
 metadata_client/tests/modules/parameter_test.py
 metadata_client/tests/modules/parameter_type_test.py
 metadata_client/tests/modules/proposal_test.py
+metadata_client/tests/modules/report_test.py
 metadata_client/tests/modules/repository_test.py
 metadata_client/tests/modules/run_test.py
-metadata_client/tests/modules/sample_test.py
+metadata_client/tests/modules/sample_test.py
+metadata_client/tests/modules/technique_test.py
```

### Comparing `metadata_client-3.9.0/setup.py` & `metadata_client-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     description='Python Client for European XFEL Metadata Catalogue Web App '
                 'available at https://in.xfel.eu/metadata',
     long_description=long_description,
     author='Luís Maia',
     author_email='luis.maia@xfel.eu',
     maintainer='Luís Maia',
     maintainer_email='luis.maia@xfel.eu',
-    url='https://git.xfel.eu/gitlab/ITDM/metadata_client',
+    url='https://git.xfel.eu/ITDM/metadata_client',
     platforms='any',
     license='MIT',
     packages=find_packages(),
     install_requires=['oauthlib',
-                      'requests',
+                      'requests <2.30',
                       'requests-oauthlib',
                       'oauth2_xfel_client >=6.1',
                       'pytz'],
     extras_require={'test': [
         'pytest',
         'pytest-cov',
         'python-dateutil',
```

