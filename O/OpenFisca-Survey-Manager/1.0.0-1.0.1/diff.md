# Comparing `tmp/OpenFisca-Survey-Manager-1.0.0.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.0.0.tar", last modified: Sat Jun 10 06:15:36 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.0.1.tar", last modified: Tue Jul 11 09:54:03 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.0.0.tar` & `OpenFisca-Survey-Manager-1.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    16295 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/CHANGELOG.md
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    34499 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/LICENSE.AGPL.txt
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      192 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/MANIFEST.in
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    14274 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     2469 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-rw-r--   0 benjello  (1001) benjello  (1001)        1 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-rw-r--   0 benjello  (1001) benjello  (1001)       92 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-rw-r--   0 benjello  (1001) benjello  (1001)        1 2022-08-11 23:28:29.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      734 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-rw-r--   0 benjello  (1001) benjello  (1001)       25 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    14274 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/PKG-INFO
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    13360 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/README.md
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     2170 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/__init__.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    17292 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/aggregates.py
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     3551 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      451 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1571 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    12096 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     6262 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    10517 2022-09-02 13:23:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calibration.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     9929 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calmar.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     3150 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/coicop.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      741 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/config.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      836 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/google_colab.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    12877 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/input_dataframe_generator.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     4591 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/matching.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1386 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_dbf.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      653 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_sas.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      493 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_spss.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    79386 2023-06-10 04:35:43.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scenarios.py
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)        0 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/__init__.py
--rwxrwxr-x   0 benjello  (1001) benjello  (1001)    10047 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/build_collection.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    11312 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/statshelpers.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     5323 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/survey_collections.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    10119 2022-09-02 13:23:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/surveys.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     9552 2022-09-02 13:23:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tables.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     3302 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/temporary.py
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)        0 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/__init__.py
-drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/data_files/
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      381 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1100 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     2457 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_calmar.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1694 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     4147 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      989 2022-09-02 13:33:56.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     3556 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_matching.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     4373 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_quantile.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1495 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_read_sas.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)    13724 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_scenario.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      716 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1064 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_surveys.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1671 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)      386 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     8319 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/utils.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     2850 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/variables.py
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     1084 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/setup.cfg
--rw-rw-r--   0 benjello  (1001) benjello  (1001)     3155 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.933717 OpenFisca-Survey-Manager-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    17044 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.925717 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-11 09:54:03.933717 OpenFisca-Survey-Manager-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13360 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79386 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-11 09:54:03.933717 OpenFisca-Survey-Manager-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.0.0/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,217 +1,230 @@
 ﻿# Changelog
 
+### 1.0.1 [#257](https://github.com/openfisca/openfisca-survey-manager/pull/257)
+
+* Technical changes
+- In GitHub Actions workflow, fixes the `check-for-functional-changes` → **`deploy`** → `publish-to-conda` jobs sequence
+  - Fix the activation of the `deploy` job by fixing how it gets `check-for-functional-changes` output status
+  - Allow the activation of `publish-to-conda` job that needs the `deploy` job
+- Add conda configuration files to non functional files for CI
+
 # 1.0.0 [#252](https://github.com/openfisca/openfisca-survey-manager/pull/252)
 
-* Technical improvement.
-- Impacted periods: all.
-- Impacted areas: all.
-- Details:
-  - Upgrade every dependencies & use their latest versions
+* Technical improvement
+  - Impacted periods: all.
+  - Impacted areas: all.
+  - Details:
+    - Upgrade every dependencies & use their latest versions
 
-### 0.47.2 [#247](https://github.com/openfisca/openfisca-survey-manager/pull/247)
+### 0.47.2 [#249](https://github.com/openfisca/openfisca-survey-manager/pull/249)
 
 * Technical changes
-- Fix `default_config_directory` for use with `openfisca-france-data` in a CI
+  - Fix `default_config_directory` for use with `openfisca-france-data` in a CI
+
+### 0.47.1 [#246](https://github.com/openfisca/openfisca-survey-manager/pull/246)
 
-## 0.47.1 [#246](https://github.com/openfisca/openfisca-survey-manager/pull/246)
+* Bug fix
+  - Debug france data ci (fixes 0.47.0)
+
+## 0.47.0 [#245](https://github.com/openfisca/openfisca-survey-manager/pull/245)
 
 * Technical changes
-- Fix `default_config_directory` for use with `openfisca-france-data` in a CI
+  - Fix `default_config_directory` for use with `openfisca-france-data` in a CI
 
 ### 0.46.19 [#244](https://github.com/openfisca/openfisca-survey-manager/pull/244)
 
 * Technical changes
-- Bump to publish package
+  - Bump to publish package
 
 ### 0.46.18 [#243](https://github.com/openfisca/openfisca-survey-manager/pull/243)
 
 * Technical changes
-- Bump to publish package
+  - Bump to publish package
 
 ### 0.46.17 [#242](https://github.com/openfisca/openfisca-survey-manager/pull/242)
 
 * Technical changes
-- Fix bug in `SurveyCollection.load`
+  - Bug fix in `SurveyCollection.load`
 
 ### 0.46.16
 
 * CI test
 
 ### 0.46.15 [#236](https://github.com/openfisca/openfisca-survey-manager/pull/236)
 
 * Technical changes
-- Put back test in CI
-- Fix coveralls config fot GitHub Actions
-- Add a test for create_data_frame_by_entity
-- Bump Actions and Python version to fix warnings
+  - Put back test in CI
+  - Fix coveralls config fot GitHub Actions
+  - Add a test for create_data_frame_by_entity
+  - Bump Actions and Python version to fix warnings
 
 ### 0.46.14 [#234](https://github.com/openfisca/openfisca-survey-manager/pull/234)
 
 * Technical changes
-- Convert every cells of a column to string.
+  - Convert every cells of a column to string.
 
 ### 0.46.13 [#233](https://github.com/openfisca/openfisca-survey-manager/pull/233)
 
 * Technical changes
-- Correcting the code asking for the period before it's instated
-- Checking the new period assignment
+  - Correcting the code asking for the period before it's instated
+  - Checking the new period assignment
 
 ### 0.46.12 [#232](https://github.com/openfisca/openfisca-survey-manager/pull/232)
 
 * Technical changes
-- Deal with Nan in Enum variables
+  - Deal with Nan in Enum variables
 
 ### 0.46.11 [#227](https://github.com/openfisca/openfisca-survey-manager/pull/227)
 
 * Technical changes
-- Add build of a tar.gz
-- Add a make entry for build
-- Move CI from Circle CI to GitHub Action (Except `make test` that run only on CircleCI)
+  - Add build of a tar.gz
+  - Add a make entry for build
+  - Move CI from Circle CI to GitHub Action (Except `make test` that run only on CircleCI)
 
 ### 0.46.10 [#229](https://github.com/openfisca/openfisca-survey-manager/pull/229)
 
 * Technical changes
-- Add tar.gz to PyPi
-- Add display readme to PyPi
+  - Add tar.gz to PyPi
+  - Add display readme to PyPi
 
 ### 0.46.9 [#228](https://github.com/openfisca/openfisca-survey-manager/pull/228)
 
 * Technical changes
-- Refactor tables method to mutualize code
-- Save variables in table survey data
+  - Refactor tables method to mutualize code
+  - Save variables in table survey data
 
 ### 0.46.8 [#226](https://github.com/openfisca/openfisca-survey-manager/pull/226)
 
 * Technical changes
-- Add a set seed in `mark_weighted_percentiles`, so that when a survey scenario with a baseline and a reform is run, variables which use this function take the same value for a given entity between the baseline and the reform.
+  - Add a set seed in `mark_weighted_percentiles`, so that when a survey scenario with a baseline and a reform is run, variables which use this function take the same value for a given entity between the baseline and the reform.
 
 ### 0.46.7 [#227](https://github.com/openfisca/openfisca-survey-manager/pull/225)
 
 * Technical changes
-- Handle explicitly SAS related dependecy.
+  - Handle explicitly SAS related dependecy.
 
 ### 0.46.6 [#224](https://github.com/openfisca/openfisca-survey-manager/pull/224)
 
 * Bug fix
-- Using pyreadstat instead of SAS7BDAT which is no more the canonical way to read sas files into pandas dataframes.
+  - Using pyreadstat instead of SAS7BDAT which is no more the canonical way to read sas files into pandas dataframes.
 
 ### 0.46.5 [#223](https://github.com/openfisca/openfisca-survey-manager/pull/223)
 
 * Bug fix
-- Deal with HDF5 file opening strict policy in build-collection
+  - Deal with HDF5 file opening strict policy in build-collection
 
 ### 0.46.4 [#219](https://github.com/openfisca/openfisca-survey-manager/pull/219)
 
 * Technical changes
-- Better handling of CategoricalDtype in input data
+  - Better handling of CategoricalDtype in input data
 
 ### 0.46.3 [#217](https://github.com/openfisca/openfisca-survey-manager/pull/217)
 
 * Bug fix
-- Deal with HDF5 file opening strict policy
+  - Deal with HDF5 file opening strict policy
 
 ### 0.46.2 [#214](https://github.com/openfisca/openfisca-survey-manager/pull/214)
 
 * New features
-- Introduce AbsstractSurveyScenario.calculate_series
+  - Introduce AbsstractSurveyScenario.calculate_series
 
 ### 0.46.1 [#211](https://github.com/openfisca/openfisca-survey-manager/pull/211)
 
 * Technical changes
-- Improve dialect detection for csv files
+  - Improve dialect detection for csv files
 
 ## 0.46 [#210](https://github.com/openfisca/openfisca-survey-manager/pull/210)
 
 * Technical changes
-- Hack to deal with encodings and delimiter not detected by pandas.read_csv
+  - Hack to deal with encodings and delimiter not detected by pandas.read_csv
 
 ## 0.45 [#143](https://github.com/openfisca/openfisca-survey-manager/pull/143)
 
 * Technical changes
-- In compute_marginal_tax_rate allow for automatic aggregation on group entity when target and varying variables entity are not the same and the varying variable entity is a person one.
+  - In compute_marginal_tax_rate allow for automatic aggregation on group entity when target and varying variables entity are not the same and the varying variable entity is a person one.
 
 ### 0.44.2 [#208](https://github.com/openfisca/openfisca-survey-manager/pull/208)
 
-* Fix bug:
-- Fix typo.
+* Bug fix
+  - Fix typo.
 
 ### 0.44.1 [#207](https://github.com/openfisca/openfisca-survey-manager/pull/207)
 
-* Fix bug:
-- Fix aggregates export to html.
+* Bug fix
+  - Fix aggregates export to html.
 
 ## 0.44 [#206](https://github.com/openfisca/openfisca-survey-manager/pull/206)
 
-* New feature:
-- Ability to export aggregates to html.
+* New feature
+  - Ability to export aggregates to html.
 
 ## 0.43 [#135](https://github.com/openfisca/openfisca-survey-manager/pull/135)
 
-* New feature:
-- Introduce aggregates.
+* New feature
+  - Introduce aggregates.
 
 ### 0.42.3 [#189](https://github.com/openfisca/openfisca-survey-manager/pull/189)
 
 * Technical changes
-- Accept categorical columns in input data frames to initialize Enum variables.
+  - Accept categorical columns in input data frames to initialize Enum variables.
 
 ### 0.42.2 [#204](https://github.com/openfisca/openfisca-survey-manager/pull/204)
 
 * Technical changes
-- Add on sub-periods when creating a quantile on a larger period
+  - Add on sub-periods when creating a quantile on a larger period
 
 ### 0.42.1 [#200](https://github.com/openfisca/openfisca-survey-manager/pull/200)
 
-* Fix bug:
-- Let numpy dependence come from openfisca-core
+* Bug fix
+  - Let numpy dependence come from openfisca-core
 
 ### 0.42.0 [#198](https://github.com/openfisca/openfisca-survey-manager/pull/198)
 
-* New feature:
-- Allow to build collections/surveys from csv files
+* New feature
+  - Allow to build collections/surveys from csv files
 
 ### 0.41.3 [#196](https://github.com/openfisca/openfisca-survey-manager/pull/196)
 
 * Bug fix
-- Enforce HDF store closing when done
+  - Enforce HDF store closing when done
 
 ### 0.41.2 [#194](https://github.com/openfisca/openfisca-survey-manager/pull/194)
 
 * Bug fix
-- Enforce us of np.array for weights and filters when computing aggregates
+  - Enforce us of np.array for weights and filters when computing aggregates
 
 ### 0.41.1 [#187](https://github.com/openfisca/openfisca-survey-manager/pull/187)
 
 * Update dependencies
 ### 0.41.0 [#185](https://github.com/openfisca/openfisca-survey-manager/pull/186)
 
 * New features
+  - Add a method to compute quantile
+  - Extend the computation of marginal tax rate
 
-- Add a method to compute quantile
-- Extend the computation of marginal tax rate
 ### 0.40.1 [#185](https://github.com/openfisca/openfisca-survey-manager/pull/185)
 
 * Technical improvement
-- Introduce weighted option in `compute_aggregate` and `compute_pivot_table`
-- Change `weights` to `alternative_weights` in `compute_aggregate` and `compute_pivot_table`
+  - Introduce weighted option in `compute_aggregate` and `compute_pivot_table`
+  - Change `weights` to `alternative_weights` in `compute_aggregate` and `compute_pivot_table`
 
 ### 0.40.0 [#184](https://github.com/openfisca/openfisca-survey-manager/pull/184)
 
 * Technical improvement
-- Add weights keyword argument to `compute_aggregate` and `compute_pivot_table`
+  - Add weights keyword argument to `compute_aggregate` and `compute_pivot_table`
 
 * Improve documentation
-- Use googl style in docstring
-- Add some docstring
+  - Use googl style in docstring
+  - Add some docstring
 
 ### 0.39.1 [#178](https://github.com/openfisca/openfisca-survey-manager/pull/178)
 
 * Bug fix
-- Fix inflate that inflated twice when baseline_simulation == simulation
+  - Fix inflate that inflated twice when baseline_simulation == simulation
 
 ### 0.39.0 [#170](https://github.com/openfisca/openfisca-survey-manager/pull/170)
 
 - Add statistical helpers to compute top and bottom shares
 
 ### 0.38.3 [#XXX](https://github.com/openfisca/openfisca-survey-manager/pull/XXX)
 
@@ -223,60 +236,60 @@
 
 ### 0.38.1 [#158](https://github.com/openfisca/openfisca-survey-manager/pull/158)
 
 - Clarify documentation on configuration directory and build-collection command
 
 ## 0.38.0 [#156](https://github.com/openfisca/openfisca-survey-manager/pull/156)
 
-##### New features
-- Introduce `survey_scenario.generate_performance_data(output_dir)`
-  - This generates a performance graph and CSV tables containing details about execution times of OpenFisca formulas
+* New features
+  - Introduce `survey_scenario.generate_performance_data(output_dir)`
+    - This generates a performance graph and CSV tables containing details about execution times of OpenFisca formulas
 
 ### 0.37.3 [#157](https://github.com/openfisca/openfisca-survey-manager/pull/157)
 
 * Technical changes
-- Add `tables` library to default requirements
+  - Add `tables` library to default requirements
 * Add documentation for users installing, configuring and running the module for the first time
 
 ### 0.37.2 [#155](https://github.com/openfisca/openfisca-survey-manager/pull/155)
 
 * Technical changes
-- Improve error mesage in build_collection (fix previous version)
+  - Improve error mesage in build_collection (fix previous version)
 
 ### 0.37.1 [#154](https://github.com/openfisca/openfisca-survey-manager/pull/154)
 
 * Technical changes
-- Improve error mesage in build_collection
+  - Improve error mesage in build_collection
 
 ## 0.37.0
 
 * Technical changes
-- Add ignorecase argument to Survey.get_values
+  - Add ignorecase argument to Survey.get_values
 
 ### 0.36.3 [#152](https://github.com/openfisca/openfisca-survey-manager/pull/152)
 
 * Technical changes
-- Fix asof for `TaxScale`
-- Use `simulation.get_known_periods` instead of `Holder`'s method in `summariaze_variable`
+  - Fix asof for `TaxScale`
+  - Use `simulation.get_known_periods` instead of `Holder`'s method in `summariaze_variable`
 
 ## 0.36.0 [#152](https://github.com/openfisca/openfisca-survey-manager/pull/152)
 
 * Technical changes
-- Create collections directory when it is missing
+  - Create collections directory when it is missing
 
 ### 0.35.2 [#150](https://github.com/openfisca/openfisca-survey-manager/pull/150)
 
 * Technical changes
-- Fix assets inclusion
+  - Fix assets inclusion
 
 ### 0.35.1 [#149](https://github.com/openfisca/openfisca-survey-manager/pull/149)
 
 * Technical changes
-- Fix deprecation in pandas.
-- Fix stripping of coicop categories
+  - Fix deprecation in pandas.
+  - Fix stripping of coicop categories
 
 ## 0.35 [#148](https://github.com/openfisca/openfisca-survey-manager/pull/148)
 
 * Introduce some functions to deal with coicop nomenclature
 
 ## 0.34 [#147](https://github.com/openfisca/openfisca-survey-manager/pull/147)
 
@@ -306,43 +319,43 @@
 
 * Adding description
 * Adding function documentation.
 
 ## 0.29.0 [#134](https://github.com/openfisca/openfisca-survey-manager/pull/134)
 
 * New features
-- Introduce compute_marginal_tax_rate.
+  - Introduce compute_marginal_tax_rate.
 
 ## 0.28.0 [#133](https://github.com/openfisca/openfisca-survey-manager/pull/133)
 
 - Fix _set_used_as_input_variables_by_entity
 - Add missing custom_input_data_frame before initializing the data
 - Fix entity ids setting
 
 ## 0.27.0 [#132](https://github.com/openfisca/openfisca-survey-manager/pull/132)
 
 * Technical changes
-- Fix create_data_frame_by_entity
-- Fix some deprecations
+  - Fix create_data_frame_by_entity
+  - Fix some deprecations
 
 ## 0.26.0
 
 * New features
-- Neutralized variables are now correctly handled by summarize_variable
-- Extend testing to doctest
+  - Neutralized variables are now correctly handled by summarize_variable
+  - Extend testing to doctest
 
 ## 0.25.0 [#126](https://github.com/openfisca/openfisca-survey-manager/pull/126)
 
 * New features
-- create_data_frame_by_entity is able to handle expressions for filtering (filter_by can be an expression)
-- This allow compute_aggregate and compute_pivot_table to handle expressions as well for filter_by.
+  - create_data_frame_by_entity is able to handle expressions for filtering (filter_by can be an expression)
+  - This allow compute_aggregate and compute_pivot_table to handle expressions as well for filter_by.
 
 * Deprecations
-- Deprecate helper get_entity
-- Deprecate helper get_weights
+  - Deprecate helper get_entity
+  - Deprecate helper get_weights
 
 ## 0.24.0 [#127](https://github.com/openfisca/openfisca-survey-manager/pull/127)
 
 * Fix a bug in create_data_frame_by_entity
 
 ## 0.23.0 [#124](https://github.com/openfisca/openfisca-survey-manager/pull/124)
```

### Comparing `OpenFisca-Survey-Manager-1.0.0/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.0.1/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/PKG-INFO` & `OpenFisca-Survey-Manager-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.0.0/README.md` & `OpenFisca-Survey-Manager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scenarios.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/setup.cfg` & `OpenFisca-Survey-Manager-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.0/setup.py` & `OpenFisca-Survey-Manager-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.0.0',
+    version = '1.0.1',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

