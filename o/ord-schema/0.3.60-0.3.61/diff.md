# Comparing `tmp/ord-schema-0.3.60.tar.gz` & `tmp/ord-schema-0.3.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.60.tar", last modified: Mon Jul 10 14:10:55 2023, max compression
+gzip compressed data, was "ord-schema-0.3.61.tar", last modified: Tue Jul 11 17:26:09 2023, max compression
```

## Comparing `ord-schema-0.3.60.tar` & `ord-schema-0.3.61.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.092354 ord-schema-0.3.60/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-10 14:10:26.000000 ord-schema-0.3.60/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 14:10:26.000000 ord-schema-0.3.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 14:10:26.000000 ord-schema-0.3.60/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-10 14:10:55.092354 ord-schema-0.3.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 14:10:26.000000 ord-schema-0.3.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.076354 ord-schema-0.3.60/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.080354 ord-schema-0.3.60/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.084354 ord-schema-0.3.60/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.084354 ord-schema-0.3.60/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49196 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.088354 ord-schema-0.3.60/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45675 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.080354 ord-schema-0.3.60/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.092354 ord-schema-0.3.60/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-10 14:10:26.000000 ord-schema-0.3.60/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-07-10 14:10:26.000000 ord-schema-0.3.60/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-10 14:10:26.000000 ord-schema-0.3.60/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-10 14:10:26.000000 ord-schema-0.3.60/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:10:55.092354 ord-schema-0.3.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-10 14:10:32.000000 ord-schema-0.3.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.639879 ord-schema-0.3.61/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 17:25:48.000000 ord-schema-0.3.61/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 17:25:48.000000 ord-schema-0.3.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 17:25:48.000000 ord-schema-0.3.61/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-11 17:26:09.639879 ord-schema-0.3.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-11 17:25:48.000000 ord-schema-0.3.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.635879 ord-schema-0.3.61/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.635879 ord-schema-0.3.61/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.635879 ord-schema-0.3.61/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.635879 ord-schema-0.3.61/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49196 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.635879 ord-schema-0.3.61/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45675 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-11 17:25:48.000000 ord-schema-0.3.61/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.635879 ord-schema-0.3.61/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-11 17:26:09.000000 ord-schema-0.3.61/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-11 17:26:09.000000 ord-schema-0.3.61/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:26:09.000000 ord-schema-0.3.61/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-11 17:26:09.000000 ord-schema-0.3.61/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:26:09.000000 ord-schema-0.3.61/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:26:09.639879 ord-schema-0.3.61/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-11 17:25:48.000000 ord-schema-0.3.61/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-07-11 17:25:48.000000 ord-schema-0.3.61/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-11 17:25:48.000000 ord-schema-0.3.61/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:25:48.000000 ord-schema-0.3.61/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:26:09.639879 ord-schema-0.3.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-11 17:25:50.000000 ord-schema-0.3.61/setup.py
```

### Comparing `ord-schema-0.3.60/LICENSE` & `ord-schema-0.3.61/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/PKG-INFO` & `ord-schema-0.3.61/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.60
+Version: 0.3.61
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -63,12 +63,13 @@
 ##### Created: 2023.07.04
 
 ##### Last updated: 2023.07.04
 
 ##### Description: 
 1. The preferred field for compound stoichiometry is the map `Compound.features` or `ProductCompound.features`.
 2. The key should be "stoichiometric_coefficient" or "stoichiometric_ratio".
-3. The value should be a Data mesaage with its float_value representing the compound's stoichiometric coefficient or ratio.SInformation about also put stoichiometry ratio/coefficient here
+3. The value should be a `Data` message with its `float_value` representing the compound's stoichiometric 
+coefficient or ratio.
 
 ##### Related links: 
 [#683](https://github.com/open-reaction-database/ord-schema/issues/683) 
 [#684](https://github.com/open-reaction-database/ord-schema/pull/684)
```

### Comparing `ord-schema-0.3.60/README.md` & `ord-schema-0.3.61/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,12 +47,13 @@
 ##### Created: 2023.07.04
 
 ##### Last updated: 2023.07.04
 
 ##### Description: 
 1. The preferred field for compound stoichiometry is the map `Compound.features` or `ProductCompound.features`.
 2. The key should be "stoichiometric_coefficient" or "stoichiometric_ratio".
-3. The value should be a Data mesaage with its float_value representing the compound's stoichiometric coefficient or ratio.SInformation about also put stoichiometry ratio/coefficient here
+3. The value should be a `Data` message with its `float_value` representing the compound's stoichiometric 
+coefficient or ratio.
 
 ##### Related links: 
 [#683](https://github.com/open-reaction-database/ord-schema/issues/683) 
 [#684](https://github.com/open-reaction-database/ord-schema/pull/684)
```

### Comparing `ord-schema-0.3.60/ord_schema/__init__.py` & `ord-schema-0.3.61/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/frozen_message.py` & `ord-schema-0.3.61/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/frozen_message_test.py` & `ord-schema-0.3.61/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/logging.py` & `ord-schema-0.3.61/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/macros/__init__.py` & `ord-schema-0.3.61/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/macros/solutions.py` & `ord-schema-0.3.61/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.61/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/macros/workups.py` & `ord-schema-0.3.61/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/message_helpers.py` & `ord-schema-0.3.61/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/message_helpers_test.py` & `ord-schema-0.3.61/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/__init__.py` & `ord-schema-0.3.61/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/conftest.py` & `ord-schema-0.3.61/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/database.py` & `ord-schema-0.3.61/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/database_test.py` & `ord-schema-0.3.61/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/mappers.py` & `ord-schema-0.3.61/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.61/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.61/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.61/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/proto/__init__.py` & `ord-schema-0.3.61/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.61/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.61/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.61/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.61/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.61/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/resolvers.py` & `ord-schema-0.3.61/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/resolvers_test.py` & `ord-schema-0.3.61/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/__init__.py` & `ord-schema-0.3.61/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.61/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.61/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.61/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.61/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.61/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.61/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.61/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.61/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.61/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.61/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.61/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/templating.py` & `ord-schema-0.3.61/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/templating_test.py` & `ord-schema-0.3.61/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/units.py` & `ord-schema-0.3.61/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/units_test.py` & `ord-schema-0.3.61/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/updates.py` & `ord-schema-0.3.61/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/updates_test.py` & `ord-schema-0.3.61/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/validations.py` & `ord-schema-0.3.61/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema/validations_test.py` & `ord-schema-0.3.61/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.61/ord_schema.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.60
+Version: 0.3.61
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -63,12 +63,13 @@
 ##### Created: 2023.07.04
 
 ##### Last updated: 2023.07.04
 
 ##### Description: 
 1. The preferred field for compound stoichiometry is the map `Compound.features` or `ProductCompound.features`.
 2. The key should be "stoichiometric_coefficient" or "stoichiometric_ratio".
-3. The value should be a Data mesaage with its float_value representing the compound's stoichiometric coefficient or ratio.SInformation about also put stoichiometry ratio/coefficient here
+3. The value should be a `Data` message with its `float_value` representing the compound's stoichiometric 
+coefficient or ratio.
 
 ##### Related links: 
 [#683](https://github.com/open-reaction-database/ord-schema/issues/683) 
 [#684](https://github.com/open-reaction-database/ord-schema/pull/684)
```

### Comparing `ord-schema-0.3.60/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.61/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.61/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/proto/dataset.proto` & `ord-schema-0.3.61/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/proto/reaction.proto` & `ord-schema-0.3.61/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/proto/test.proto` & `ord-schema-0.3.61/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.60/setup.py` & `ord-schema-0.3.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.60",
+    version="0.3.61",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

