# Comparing `tmp/fmu-sumo-0.3.10.tar.gz` & `tmp/fmu-sumo-0.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmu-sumo-0.3.10.tar", last modified: Mon Jun 26 07:52:24 2023, max compression
+gzip compressed data, was "fmu-sumo-0.3.11.tar", last modified: Tue Jul 11 11:33:20 2023, max compression
```

## Comparing `fmu-sumo-0.3.10.tar` & `fmu-sumo-0.3.11.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.168135 fmu-sumo-0.3.10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.132134 fmu-sumo-0.3.10/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/.github/workflows/build_docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/.github/workflows/run_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-26 07:52:24.168135 fmu-sumo-0.3.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3585 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/docs/explorer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/docs/uploader.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/examples/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/examples/tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/requirements/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/requirements/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:52:24.168135 fmu-sumo-0.3.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/src/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/src/fmu/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/src/fmu/sumo/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/src/fmu/sumo/config_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/config_jobs/SUMO_UPLOAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/src/fmu/sumo/explorer/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.140134 fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/realization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.140134 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_child_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_document_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/case_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/cube_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/polygons_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/surface_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/table_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/table_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/explorer/timefilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.140134 fmu-sumo-0.3.10/src/fmu/sumo/hook_implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/hook_implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/hook_implementations/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.144135 fmu-sumo-0.3.10/src/fmu/sumo/uploader/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/_fileondisk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/_fileonjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/_upload_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/caseondisk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/caseonjob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.144135 fmu-sumo-0.3.10/src/fmu/sumo/uploader/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/src/fmu/sumo/uploader/scripts/sumo_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu/sumo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.144135 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-26 07:52:24.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 07:52:23.000000 fmu-sumo-0.3.10/src/fmu_sumo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.144135 fmu-sumo-0.3.10/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.136134 fmu-sumo-0.3.10/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:52:24.168135 fmu-sumo-0.3.10/tests/data/test_case_080/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/.seismic.segy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/.surface.bin.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/.surface_error.bin.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/case.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/case_segy.yml
--rw-r--r--   0 runner    (1001) docker     (123) 22265760 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/seismic.segy
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/surface.bin
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/surface_error.bin
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/data/test_case_080/surface_no_metadata.bin
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/test_aggregated_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-06-26 07:52:06.000000 fmu-sumo-0.3.10/tests/test_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.276330 fmu-sumo-0.3.11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.208330 fmu-sumo-0.3.11/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.220330 fmu-sumo-0.3.11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/.github/workflows/build_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/.github/workflows/run_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-11 11:33:20.276330 fmu-sumo-0.3.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.220330 fmu-sumo-0.3.11/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3585 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/docs/explorer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/docs/uploader.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.220330 fmu-sumo-0.3.11/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/examples/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/examples/tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.224330 fmu-sumo-0.3.11/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/requirements/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/requirements/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 11:33:20.276330 fmu-sumo-0.3.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.224330 fmu-sumo-0.3.11/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.224330 fmu-sumo-0.3.11/src/fmu/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.224330 fmu-sumo-0.3.11/src/fmu/sumo/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.224330 fmu-sumo-0.3.11/src/fmu/sumo/config_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/config_jobs/SUMO_UPLOAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.228330 fmu-sumo-0.3.11/src/fmu/sumo/explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.228330 fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/realization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.236330 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_child_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_document_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/case_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/cube_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/polygons_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/surface_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/table_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/table_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/explorer/timefilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.236330 fmu-sumo-0.3.11/src/fmu/sumo/hook_implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/hook_implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/hook_implementations/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.236330 fmu-sumo-0.3.11/src/fmu/sumo/uploader/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/_fileondisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/_fileonjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/_upload_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/caseondisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/caseonjob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.240330 fmu-sumo-0.3.11/src/fmu/sumo/uploader/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/src/fmu/sumo/uploader/scripts/sumo_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-11 11:33:19.000000 fmu-sumo-0.3.11/src/fmu/sumo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.240330 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 11:33:20.000000 fmu-sumo-0.3.11/src/fmu_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.240330 fmu-sumo-0.3.11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.216330 fmu-sumo-0.3.11/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:33:20.272330 fmu-sumo-0.3.11/tests/data/test_case_080/
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/.seismic.segy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/.surface.bin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/.surface_error.bin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/case.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/case_segy.yml
+-rw-r--r--   0 runner    (1001) docker     (123) 22265760 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/seismic.segy
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/surface.bin
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/surface_error.bin
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/data/test_case_080/surface_no_metadata.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/test_aggregated_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-11 11:33:01.000000 fmu-sumo-0.3.11/tests/test_uploader.py
```

### Comparing `fmu-sumo-0.3.10/.github/workflows/build_docs.yaml` & `fmu-sumo-0.3.11/.github/workflows/build_docs.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/.github/workflows/publish_release.yaml` & `fmu-sumo-0.3.11/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/.github/workflows/run_tests.yaml` & `fmu-sumo-0.3.11/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/.gitignore` & `fmu-sumo-0.3.11/.gitignore`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/LICENSE` & `fmu-sumo-0.3.11/LICENSE`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/PKG-INFO` & `fmu-sumo-0.3.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-sumo
-Version: 0.3.10
+Version: 0.3.11
 Summary: Python package for interacting with Sumo in an FMU setting
 Home-page: https://github.com/equinor/fmu-sumo
 Author: Equinor
 License: Apache 2.0
 Keywords: fmu,sumo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `fmu-sumo-0.3.10/README.md` & `fmu-sumo-0.3.11/README.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/docs/conf.py` & `fmu-sumo-0.3.11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/docs/explorer.rst` & `fmu-sumo-0.3.11/docs/explorer.rst`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/docs/index.rst` & `fmu-sumo-0.3.11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/docs/uploader.rst` & `fmu-sumo-0.3.11/docs/uploader.rst`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/examples/explorer.ipynb` & `fmu-sumo-0.3.11/examples/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/examples/tables.ipynb` & `fmu-sumo-0.3.11/examples/tables.ipynb`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/setup.py` & `fmu-sumo-0.3.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 CMDCLASS = {}
 
 try:
     from sphinx.setup_command import BuildDoc
 
     CMDCLASS.update({"build_sphinx": BuildDoc})
-except ImportError as e:
+except ImportError:
     # sphinx not installed - do not provide build_sphinx cmd
     pass
 
 is_docs = os.getenv("READTHEDOCS") == "True"
 
 REQUIREMENTS = (
     [] if is_docs else parse_requirements("requirements/requirements.txt")
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/config_jobs/SUMO_UPLOAD` & `fmu-sumo-0.3.11/src/fmu/sumo/config_jobs/SUMO_UPLOAD`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/_utils.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,14 +36,44 @@
             query["sort"] = sort
 
         res = self._sumo.post("/search", json=query)
         buckets = res.json()["aggregations"][field]["buckets"]
 
         return buckets
 
+    async def get_buckets_async(
+        self,
+        field: str,
+        query: Dict,
+        sort: List = None,
+    ) -> List[Dict]:
+        """Get a List of buckets
+
+        Arguments:
+            - field (str): a field in the metadata
+            - query (List[Dict] or None): filter options
+            - sort (List or None): sorting options
+
+        Returns:
+            A List of unique values for a given field
+        """
+        query = {
+            "size": 0,
+            "aggs": {f"{field}": {"terms": {"field": field, "size": 2000}}},
+            "query": query,
+        }
+
+        if sort is not None:
+            query["sort"] = sort
+
+        res = await self._sumo.post_async("/search", json=query)
+        buckets = res.json()["aggregations"][field]["buckets"]
+
+        return buckets
+
     def get_objects(
         self,
         size: int,
         query: Dict,
         select: List[str] = None,
     ) -> List[Dict]:
         """Get objects
@@ -61,14 +91,39 @@
         if select is not None:
             query["_source"] = select
 
         res = self._sumo.post("/search", json=query)
 
         return res.json()["hits"]["hits"]
 
+    async def get_objects_async(
+        self,
+        size: int,
+        query: Dict,
+        select: List[str] = None,
+    ) -> List[Dict]:
+        """Get objects
+
+        Args:
+            size (int): number of objects to return
+            query (List[Dict] or None): filter options
+            select (List[str] or None): list of metadata fields to return
+
+        Returns:
+            List[Dict]: A List of metadata
+        """
+        query = {"size": size, "query": query}
+
+        if select is not None:
+            query["_source"] = select
+
+        res = await self._sumo.post_async("/search", json=query)
+
+        return res.json()["hits"]["hits"]
+
     def get_object(self, uuid: str, select: List[str] = None) -> Dict:
         """Get metadata object by uuid
 
         Args:
             uuid (str): uuid of metadata object
             select (List[str]): list of metadata fields to return
 
@@ -88,14 +143,41 @@
         hits = res.json()["hits"]["hits"]
 
         if len(hits) == 0:
             raise Exception(f"Document not found: {uuid}")
 
         return hits[0]
 
+    async def get_object_async(self, uuid: str, select: List[str] = None) -> Dict:
+        """Get metadata object by uuid
+
+        Args:
+            uuid (str): uuid of metadata object
+            select (List[str]): list of metadata fields to return
+
+        Returns:
+            Dict: a metadata object
+        """
+
+        query = {
+            "query": {"term": {"_id": uuid}},
+            "size": 1,
+        }
+
+        if select is not None:
+            query["_source"] = select
+
+        res = await self._sumo.post_async("/search", json=query)
+        hits = res.json()["hits"]["hits"]
+
+        if len(hits) == 0:
+            raise Exception(f"Document not found: {uuid}")
+
+        return hits[0]
+
     def extend_query_object(self, old: Dict, new: Dict) -> Dict:
         """Extend query object
 
         Args:
             old (Dict): old query object
             new (Dict): new query object
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/aggregation.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/aggregation.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/observation.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/observation.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/contexts/realization.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/contexts/realization.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/__init__.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_child.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_child.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,7 +77,16 @@
     def blob(self) -> BytesIO:
         """Object blob"""
         if self._blob is None:
             res = self._sumo.get(f"/objects('{self.uuid}')/blob")
             self._blob = BytesIO(res)
 
         return self._blob
+
+    @property
+    async def blob_async(self) -> BytesIO:
+        """Object blob"""
+        if self._blob is None:
+            res = await self._sumo.get_async(f"/objects('{self.uuid}')/blob")
+            self._blob = BytesIO(res)
+
+        return self._blob
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_child_collection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_child_collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,48 +48,88 @@
 
     @property
     def names(self) -> List[str]:
         """List of unique object names"""
         return self._get_field_values("data.name.keyword")
 
     @property
+    async def names_async(self) -> List[str]:
+        """List of unique object names"""
+        return await self._get_field_values_async("data.name.keyword")
+
+    @property
     def tagnames(self) -> List[str]:
         """List of unqiue object tagnames"""
         return self._get_field_values("data.tagname.keyword")
 
     @property
+    async def tagnames_async(self) -> List[str]:
+        """List of unqiue object tagnames"""
+        return await self._get_field_values_async("data.tagname.keyword")
+
+    @property
     def iterations(self) -> List[int]:
         """List of unique object iteration names"""
         return self._get_field_values("fmu.iteration.name.keyword")
 
     @property
+    async def iterations_async(self) -> List[int]:
+        """List of unique object iteration names"""
+        return await self._get_field_values_async("fmu.iteration.name.keyword")
+
+    @property
     def realizations(self) -> List[int]:
         """List of unique object realization ids"""
         return self._get_field_values("fmu.realization.id")
 
     @property
+    async def realizations_async(self) -> List[int]:
+        """List of unique object realization ids"""
+        return await self._get_field_values_async("fmu.realization.id")
+
+    @property
     def aggregations(self) -> List[str]:
         """List of unique object aggregation operations"""
         return self._get_field_values("fmu.aggregation.operation.keyword")
 
     @property
+    async def aggregations_async(self) -> List[str]:
+        """List of unique object aggregation operations"""
+        return await self._get_field_values_async("fmu.aggregation.operation.keyword")
+
+    @property
     def stages(self) -> List[str]:
         """List of unique stages"""
         return self._get_field_values("fmu.context.stage.keyword")
 
     @property
+    async def stages_async(self) -> List[str]:
+        """List of unique stages"""
+        return await self._get_field_values_async("fmu.context.stage.keyword")
+
+    @property
     def stratigraphic(self) -> List[str]:
         """List of unqiue object stratigraphic"""
         return self._get_field_values("data.stratigraphic")
 
     @property
+    async def stratigraphic_async(self) -> List[str]:
+        """List of unqiue object stratigraphic"""
+        return await self._get_field_values_async("data.stratigraphic")
+
+    @property
     def vertical_domain(self) -> List[str]:
         """List of unqiue object vertical domain"""
         return self._get_field_values("data.vertical_domain")
 
+    @property
+    async def vertical_domain_async(self) -> List[str]:
+        """List of unqiue object vertical domain"""
+        return await self._get_field_values_async("data.vertical_domain")
+
     def _init_query(self, doc_type: str, query: Dict = None) -> Dict:
         new_query = super()._init_query(doc_type, query)
         case_filter = {
             "bool": {
                 "must": [
                     {"term": {"_sumo.parent_object.keyword": self._case_uuid}}
                 ]
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/_document.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/_document.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/case_collection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/case_collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,35 +29,62 @@
 
     @property
     def names(self) -> List[str]:
         """List of unique case names"""
         return self._get_field_values("fmu.case.name.keyword")
 
     @property
+    async def names_async(self) -> List[str]:
+        """List of unique case names"""
+        return await self._get_field_values_async("fmu.case.name.keyword")
+
+    @property
     def statuses(self) -> List[str]:
         """List of unique statuses"""
         return self._get_field_values("_sumo.status.keyword")
 
     @property
+    async def statuses_async(self) -> List[str]:
+        """List of unique statuses"""
+        return await self._get_field_values_async("_sumo.status.keyword")
+
+    @property
     def users(self) -> List[str]:
         """List of unique user names"""
         return self._get_field_values("fmu.case.user.id.keyword")
 
     @property
+    async def users_async(self) -> List[str]:
+        """List of unique user names"""
+        return await self._get_field_values_async("fmu.case.user.id.keyword")
+
+    @property
     def assets(self) -> List[str]:
         """List of unique asset names"""
         return self._get_field_values("access.asset.name.keyword")
 
     @property
+    async def assets_async(self) -> List[str]:
+        """List of unique asset names"""
+        return await self._get_field_values_async("access.asset.name.keyword")
+
+    @property
     def fields(self) -> List[str]:
         """List of unique field names"""
         return self._get_field_values(
             "masterdata.smda.field.identifier.keyword"
         )
 
+    @property
+    async def fields_async(self) -> List[str]:
+        """List of unique field names"""
+        return await self._get_field_values_async(
+            "masterdata.smda.field.identifier.keyword"
+        )
+
     def __getitem__(self, index: int) -> Case:
         doc = super().__getitem__(index)
         return Case(self._sumo, doc, self._pit)
 
     def filter(
         self,
         uuid: Union[str, List[str]] = None,
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/cube.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/cube.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,43 +21,82 @@
 
     def _populate_url(self):
         res = self._sumo.get(f"/objects('{self.uuid}')/blob/authuri")
         try:
             res = json.loads(res.decode("UTF-8"))
             self._url = res.get("baseuri") + self.uuid
             self._sas = res.get("auth")
-        except:
+        except Exception:
+            self._url = res.decode("UTF-8")
+
+    async def _populate_url_async(self):
+        res = await self._sumo.get_async(f"/objects('{self.uuid}')/blob/authuri")
+        try:
+            res = json.loads(res.decode("UTF-8"))
+            self._url = res.get("baseuri") + self.uuid
+            self._sas = res.get("auth")
+        except Exception:
             self._url = res.decode("UTF-8")
 
     @property
     def url(self) -> str:
         if self._url is None:
             self._populate_url()
         if self._sas is None:
-            return self._url    
-        else: 
+            return self._url
+        else:
+            return self._url.split("?")[0] + "/"
+
+    @property
+    async def url_async(self) -> str:
+        if self._url is None:
+            await self._populate_url_async()
+        if self._sas is None:
+            return self._url
+        else:
             return self._url.split("?")[0] + "/"
 
     @property
     def sas(self) -> str:
         if self._url is None:
             self._populate_url()
         if self._sas is None:
             return self._url.split("?")[1]
         else:
             return self._sas
 
     @property
+    async def sas_async(self) -> str:
+        if self._url is None:
+            await self._populate_url_async()
+        if self._sas is None:
+            return self._url.split("?")[1]
+        else:
+            return self._sas
+
+    @property
     def openvds_handle(self) -> openvds.core.VDS:
         if self._url is None:
             self._populate_url()
-        
+
+        if self._sas is None:
+            return openvds.open(self._url)
+        else:
+            url = "azureSAS" + self._url[5:] + "/"
+            sas = "Suffix=?" + self._sas
+            return openvds.open(url, sas)
+
+    @property
+    async def openvds_handle_async(self) -> openvds.core.VDS:
+        if self._url is None:
+            await self._populate_url_async()
+
         if self._sas is None:
             return openvds.open(self._url)
-        else: 
+        else:
             url = "azureSAS" + self._url[5:] + "/"
             sas = "Suffix=?" + self._sas
             return openvds.open(url, sas)
 
     @property
     def timestamp(self) -> str:
         """Surface timestmap data"""
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/cube_collection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/cube_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,24 +41,65 @@
     def timestamps(self) -> List[str]:
         """List of unique timestamps in CubeCollection"""
         return self._get_field_values(
             "data.time.t0.value", TIMESTAMP_QUERY, True
         )
 
     @property
+    async def timestamps_async(self) -> List[str]:
+        """List of unique timestamps in CubeCollection"""
+        return await self._get_field_values_async(
+            "data.time.t0.value", TIMESTAMP_QUERY, True
+        )
+
+    @property
     def intervals(self) -> List[Tuple]:
         """List of unique intervals in CubeCollection"""
         res = self._sumo.post(
             "/search",
             json={
                 "query": self._query,
                 "aggs": {
                     "t0": {
                         "terms": {"field": "data.time.t0.value", "size": 50},
                         "aggs": {
+                            "t1": {
+                                "terms": {
+                                    "field": "data.time.t1.value",
+                                    "size": 50,
+                                }
+                            }
+                        },
+                    }
+                },
+            },
+        )
+
+        buckets = res.json()["aggregations"]["t0"]["buckets"]
+        intervals = []
+
+        for bucket in buckets:
+            t0 = bucket["key_as_string"]
+
+            for t1 in bucket["t1"]["buckets"]:
+                intervals.append((t0, t1["key_as_string"]))
+
+        return intervals
+
+    @property
+    async def intervals_async(self) -> List[Tuple]:
+        """List of unique intervals in CubeCollection"""
+        res = await self._sumo.post_async(
+            "/search",
+            json={
+                "query": self._query,
+                "aggs": {
+                    "t0": {
+                        "terms": {"field": "data.time.t0.value", "size": 50},
+                        "aggs": {
                             "t1": {
                                 "terms": {
                                     "field": "data.time.t1.value",
                                     "size": 50,
                                 }
                             }
                         },
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/polygons.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/polygons.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,20 +25,32 @@
         """
         warn(
             ".to_dataframe() is deprecated, renamed to .to_pandas() ",
             DeprecationWarning,
             stacklevel=2,
         )
 
-        return self.to_pandas
+        return self.to_pandas()
 
     def to_pandas(self) -> pd.DataFrame:
         """Get polygons object as a DataFrame
 
         Returns:
             DataFrame: A DataFrame object
         """
 
         try:
             return pd.read_csv(self.blob)
         except TypeError as type_err:
             raise TypeError(f"Unknown format: {self.format}") from type_err
+
+    async def to_pandas_async(self) -> pd.DataFrame:
+        """Get polygons object as a DataFrame
+
+        Returns:
+            DataFrame: A DataFrame object
+        """
+
+        try:
+            return pd.read_csv(await self.blob_async)
+        except TypeError as type_err:
+            raise TypeError(f"Unknown format: {self.format}") from type_err
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/polygons_collection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/polygons_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/surface.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/surface.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,18 @@
         Returns:
             RegularSurface: A RegularSurface object
         """
         try:
             return surface_from_file(self.blob)
         except TypeError as type_err:
             raise TypeError(f"Unknown format: {self.format}") from type_err
+
+    async def to_regular_surface_async(self) -> RegularSurface:
+        """Get surface object as a RegularSurface
+
+        Returns:
+            RegularSurface: A RegularSurface object
+        """
+        try:
+            return surface_from_file(await self.blob_async)
+        except TypeError as type_err:
+            raise TypeError(f"Unknown format: {self.format}") from type_err
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/surface_collection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/surface_collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,14 +45,21 @@
     def timestamps(self) -> List[str]:
         """List of unique timestamps in SurfaceCollection"""
         return self._get_field_values(
             "data.time.t0.value", TIMESTAMP_QUERY, True
         )
 
     @property
+    async def timestamps_async(self) -> List[str]:
+        """List of unique timestamps in CubeCollection"""
+        return await self._get_field_values_async(
+            "data.time.t0.value", TIMESTAMP_QUERY, True
+        )
+
+    @property
     def intervals(self) -> List[Tuple]:
         """List of unique intervals in SurfaceCollection"""
         res = self._sumo.post(
             "/search",
             json={
                 "query": self._query,
                 "aggs": {
@@ -78,14 +85,48 @@
             t0 = bucket["key_as_string"]
 
             for t1 in bucket["t1"]["buckets"]:
                 intervals.append((t0, t1["key_as_string"]))
 
         return intervals
 
+    @property
+    async def intervals_async(self) -> List[Tuple]:
+        """List of unique intervals in SurfaceCollection"""
+        res = await self._sumo.post_async(
+            "/search",
+            json={
+                "query": self._query,
+                "aggs": {
+                    "t0": {
+                        "terms": {"field": "data.time.t0.value", "size": 50},
+                        "aggs": {
+                            "t1": {
+                                "terms": {
+                                    "field": "data.time.t1.value",
+                                    "size": 50,
+                                }
+                            }
+                        },
+                    }
+                },
+            },
+        )
+
+        buckets = res.json()["aggregations"]["t0"]["buckets"]
+        intervals = []
+
+        for bucket in buckets:
+            t0 = bucket["key_as_string"]
+
+            for t1 in bucket["t1"]["buckets"]:
+                intervals.append((t0, t1["key_as_string"]))
+
+        return intervals
+
     def _aggregate(self, operation: str) -> xtgeo.RegularSurface:
         if operation not in self._aggregation_cache:
             objects = self._utils.get_objects(500, self._query, ["_id"])
             object_ids = list(map(lambda obj: obj["_id"], objects))
 
             res = self._sumo.post(
                 "/aggregate",
@@ -94,14 +135,30 @@
 
             self._aggregation_cache[operation] = xtgeo.surface_from_file(
                 BytesIO(res.content)
             )
 
         return self._aggregation_cache[operation]
 
+    async def _aggregate_async(self, operation: str) -> xtgeo.RegularSurface:
+        if operation not in self._aggregation_cache:
+            objects = await self._utils.get_objects_async(500, self._query, ["_id"])
+            object_ids = list(map(lambda obj: obj["_id"], objects))
+
+            res = await self._sumo.post_async(
+                "/aggregate",
+                json={"operation": [operation], "object_ids": object_ids},
+            )
+
+            self._aggregation_cache[operation] = xtgeo.surface_from_file(
+                BytesIO(res.content)
+            )
+
+        return self._aggregation_cache[operation]
+
     def filter(
         self,
         name: Union[str, List[str], bool] = None,
         tagname: Union[str, List[str], bool] = None,
         stratigraphic: Union[str, List[str], bool] = None,
         vertical_domain: Union[str, List[str], bool] = None,
         iteration: Union[str, List[str], bool] = None,
@@ -180,30 +237,58 @@
 
         return SurfaceCollection(self._sumo, self._case_uuid, query, self._pit)
 
     def mean(self) -> xtgeo.RegularSurface:
         """Perform a mean aggregation"""
         return self._aggregate("mean")
 
+    async def mean_async(self) -> xtgeo.RegularSurface:
+        """Perform a mean aggregation"""
+        return await self._aggregate_async("mean")
+
     def min(self) -> xtgeo.RegularSurface:
         """Perform a minimum aggregation"""
         return self._aggregate("min")
 
+    async def min_async(self) -> xtgeo.RegularSurface:
+        """Perform a minimum aggregation"""
+        return await self._aggregate_async("min")
+
     def max(self) -> xtgeo.RegularSurface:
         """Perform a maximum aggregation"""
         return self._aggregate("max")
 
+    async def max_async(self) -> xtgeo.RegularSurface:
+        """Perform a maximum aggregation"""
+        return await self._aggregate_async("max")
+
     def std(self) -> xtgeo.RegularSurface:
         """Perform a standard deviation aggregation"""
         return self._aggregate("std")
 
+    async def std_async(self) -> xtgeo.RegularSurface:
+        """Perform a standard deviation aggregation"""
+        return await self._aggregate_async("std")
+
     def p10(self) -> xtgeo.RegularSurface:
         """Perform a percentile aggregation"""
         return self._aggregate("p10")
 
+    async def p10_async(self) -> xtgeo.RegularSurface:
+        """Perform a percentile aggregation"""
+        return await self._aggregate_async("p10")
+
     def p50(self) -> xtgeo.RegularSurface:
         """Perform a percentile aggregation"""
         return self._aggregate("p50")
 
+    async def p50_async(self) -> xtgeo.RegularSurface:
+        """Perform a percentile aggregation"""
+        return await self._aggregate_async("p50")
+
     def p90(self) -> xtgeo.RegularSurface:
         """Perform a percentile aggregation"""
         return self._aggregate("p90")
+
+    async def p90_async(self) -> xtgeo.RegularSurface:
+        """Perform a percentile aggregation"""
+        return await self._aggregate_async("p90")
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/table.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,14 +68,48 @@
                         raise TypeError(
                             "Come on, no way this is converting to pandas!!"
                         ) from ud_error
 
         self._logger.debug("Read blob as %s to return pandas", worked)
         return self._dataframe
 
+    async def to_pandas_async(self) -> pd.DataFrame:
+        """Return object as a pandas DataFrame
+
+        Returns:
+            DataFrame: A DataFrame object
+        """
+
+        if self._dataframe is None:
+            if self["data"]["format"] == "csv":
+                worked = "csv"
+                self._logger.debug("Treating blob as csv")
+                try:
+                    self._dataframe = pd.read_csv(await self.blob_async)
+                    worked = "csv"
+
+                except UnicodeDecodeError as ud_e:
+                    raise UnicodeDecodeError("Maybe not csv?") from ud_e
+            else:
+                try:
+                    worked = "feather"
+                    self._dataframe = pf.read_feather(await self.blob_async)
+                except pa.lib.ArrowInvalid:
+                    try:
+                        worked = "parquet"
+                        self._dataframe = pd.read_parquet(await self.blob_async)
+
+                    except UnicodeDecodeError as ud_error:
+                        raise TypeError(
+                            "Come on, no way this is converting to pandas!!"
+                        ) from ud_error
+
+        self._logger.debug("Read blob as %s to return pandas", worked)
+        return self._dataframe
+
     @to_pandas.setter
     def to_pandas(self, frame: pd.DataFrame):
         self._dataframe = frame
 
     @property
     def arrowtable(self) -> pa.Table:
         """Return object as an arrow Table
@@ -85,17 +119,16 @@
         """
         warn(
             ".arrowtable is deprecated, renamed to .to_arrow",
             DeprecationWarning,
             stacklevel=2,
         )
 
-        return self.to_arrow
+        return self.to_arrow()
 
-    @property
     def to_arrow(self) -> pa.Table:
         """Return object as an arrow Table
 
         Returns:
             pa.Table: _description_
         """
         if self._arrowtable is None:
@@ -117,8 +150,39 @@
                     )
 
                 except TypeError as type_err:
                     raise OSError("Cannot read this into arrow") from type_err
 
             self._logger.debug("Read blob as %s to return arrow", worked)
 
+        return self._arrowtable
+
+    async def to_arrow_async(self) -> pa.Table:
+        """Return object as an arrow Table
+
+        Returns:
+            pa.Table: _description_
+        """
+        if self._arrowtable is None:
+            if self["data"]["format"] == "arrow":
+                try:
+                    worked = "feather"
+                    self._arrowtable = pf.read_table(await self.blob_async)
+                except pa.lib.ArrowInvalid:
+                    worked = "parquet"
+                    self._arrowtable = pq.read_table(await self.blob_async)
+            else:
+                warn(
+                    "Reading csv format into arrow, you will not get the full benefit of native arrow"
+                )
+                worked = "csv"
+                try:
+                    self._arrowtable = pa.Table.from_pandas(
+                        pd.read_csv(await self.blob_async)
+                    )
+
+                except TypeError as type_err:
+                    raise OSError("Cannot read this into arrow") from type_err
+
+            self._logger.debug("Read blob as %s to return arrow", worked)
+
         return self._arrowtable
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/table_aggregated.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/table_aggregated.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,14 +75,45 @@
 
             res = self._sumo.post("/search", json=query)
             doc = res.json()["hits"]["hits"][0]
             self._parameters = doc["_source"]["fmu"]["iteration"]["parameters"]
 
         return self._parameters
 
+    @property
+    async def parameters_async(self):
+        """Return parameter set for iteration
+
+        Returns:
+            dict: parameters connected to iteration
+        """
+        if not self._parameters:
+            must = self._utils.build_terms(
+                {
+                    "class.keyword": "table",
+                    "_sumo.parent_object.keyword": self._case.uuid,
+                    "data.name.keyword": self._name,
+                    "data.tagname.keyword": self._tag,
+                    "fmu.iteration.name.keyword": self._iteration,
+                    "fmu.aggregation.operation.keyword": "collection",
+                }
+            )
+
+            query = {
+                "size": 1,
+                "_source": ["fmu.iteration.parameters"],
+                "query": {"bool": {"must": must}},
+            }
+
+            res = await self._sumo.post_async("/search", json=query)
+            doc = res.json()["hits"]["hits"][0]
+            self._parameters = doc["_source"]["fmu"]["iteration"]["parameters"]
+
+        return self._parameters
+
     def __len__(self):
         return len(self._collection)
 
     def __getitem__(self, column) -> Table:
         try:
             return self._collection.filter(column=column)[0]
         except IndexError as i_ex:
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/objects/table_collection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/objects/table_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,19 @@
         return Table(self._sumo, doc)
 
     @property
     def columns(self) -> List[str]:
         """List of unique column names"""
         return self._get_field_values("data.spec.columns.keyword")
 
+    @property
+    async def columns_async(self) -> List[str]:
+        """List of unique column names"""
+        return await self._get_field_values_async("data.spec.columns.keyword")
+
     def filter(
         self,
         name: Union[str, List[str], bool] = None,
         tagname: Union[str, List[str], bool] = None,
         iteration: Union[str, List[str], bool] = None,
         realization: Union[int, List[int], bool] = None,
         aggregation: Union[str, List[str], bool] = None,
```

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/pit.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/pit.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/explorer/timefilter.py` & `fmu-sumo-0.3.11/src/fmu/sumo/explorer/timefilter.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/hook_implementations/jobs.py` & `fmu-sumo-0.3.11/src/fmu/sumo/hook_implementations/jobs.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/_connection.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/_connection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/_fileondisk.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/_fileondisk.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/_fileonjob.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/_fileonjob.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/_upload_files.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/_upload_files.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/caseondisk.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/caseondisk.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/caseonjob.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/caseonjob.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu/sumo/uploader/scripts/sumo_upload.py` & `fmu-sumo-0.3.11/src/fmu/sumo/uploader/scripts/sumo_upload.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/src/fmu_sumo.egg-info/PKG-INFO` & `fmu-sumo-0.3.11/src/fmu_sumo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-sumo
-Version: 0.3.10
+Version: 0.3.11
 Summary: Python package for interacting with Sumo in an FMU setting
 Home-page: https://github.com/equinor/fmu-sumo
 Author: Equinor
 License: Apache 2.0
 Keywords: fmu,sumo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `fmu-sumo-0.3.10/src/fmu_sumo.egg-info/SOURCES.txt` & `fmu-sumo-0.3.11/src/fmu_sumo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/context.py` & `fmu-sumo-0.3.11/tests/context.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/data/test_case_080/.seismic.segy.yml` & `fmu-sumo-0.3.11/tests/data/test_case_080/.seismic.segy.yml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/data/test_case_080/.surface.bin.yml` & `fmu-sumo-0.3.11/tests/data/test_case_080/.surface.bin.yml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/data/test_case_080/.surface_error.bin.yml` & `fmu-sumo-0.3.11/tests/data/test_case_080/.surface_error.bin.yml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/data/test_case_080/case.yml` & `fmu-sumo-0.3.11/tests/data/test_case_080/case.yml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/data/test_case_080/case_segy.yml` & `fmu-sumo-0.3.11/tests/data/test_case_080/case_segy.yml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/data/test_case_080/seismic.segy` & `fmu-sumo-0.3.11/tests/data/test_case_080/seismic.segy`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/test_aggregated_table.py` & `fmu-sumo-0.3.11/tests/test_aggregated_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     case = explorer.cases.filter(name="drogon_ahm-2023-02-22")[0]
 
     table = AggregatedTable(case, "summary", "eclipse", "iter-0")
 
     assert len(table.columns) == 972 + 2
     column = table["FOPT"]
 
-    assert isinstance(column.to_arrow, pa.Table)
+    assert isinstance(column.to_arrow(), pa.Table)
     with pytest.raises(IndexError) as e_info:
         table = table["banana"]
         assert (
             e_info.value.args[0] == "Column: 'banana' does not exist try again"
         )
 
 
@@ -47,15 +47,15 @@
     table = AggregatedTable(case, "summary", "eclipse", "iter-0")
 
     assert len(table.columns) == 972 + 2
     column = table["FOPT"]
 
     with pytest.warns(
         DeprecationWarning,
-        match=".arrowtable is deprecated, renamed to .to_arrow",
+        match=".arrowtable is deprecated, renamed to .to_arrow()",
     ):
         assert isinstance(column.arrowtable, pa.Table)
     with pytest.raises(IndexError) as e_info:
         table = table["banana"]
         assert (
             e_info.value.args[0] == "Column: 'banana' does not exist try again"
         )
@@ -70,15 +70,15 @@
 
 def test_aggregated_summary_pandas_with_deprecated_function_name(
     explorer: Explorer,
 ):
     """Test usage of Aggregated class with item_type=pandas with deprecated function name"""
     case = explorer.cases.filter(name="drogon_ahm-2023-02-22")[0]
     table = AggregatedTable(case, "summary", "eclipse", "iter-0")
-    with pytest.warns(match=".dataframe is deprecated, renamed to .to_pandas"):
+    with pytest.warns(match=".dataframe is deprecated, renamed to .to_pandas()"):
         mydata = table["FOPT"].dataframe
     assert isinstance(mydata, pd.DataFrame)
 
 
 def test_get_fmu_iteration_parameters(explorer: Explorer):
     """Test getting the metadata of of an object"""
     case = explorer.cases.filter(name="drogon_ahm-2023-02-22")[0]
```

### Comparing `fmu-sumo-0.3.10/tests/test_explorer.py` & `fmu-sumo-0.3.11/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-0.3.10/tests/test_uploader.py` & `fmu-sumo-0.3.11/tests/test_uploader.py`

 * *Files identical despite different names*

