# Comparing `tmp/discovery-capability-0.3.10.tar.gz` & `tmp/discovery-capability-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.3.10.tar", last modified: Mon Jul 10 23:33:56 2023, max compression
+gzip compressed data, was "discovery-capability-0.3.9.tar", last modified: Mon Jul 10 15:37:16 2023, max compression
```

## Comparing `discovery-capability-0.3.10.tar` & `discovery-capability-0.3.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:56.004874 discovery-capability-0.3.10/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.3.10/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.3.10/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11228 2023-07-10 23:33:56.005118 discovery-capability-0.3.10/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.3.10/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.838632 discovery-capability-0.3.10/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11228 2023-07-10 23:33:55.000000 discovery-capability-0.3.10/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2277 2023-07-10 23:33:55.000000 discovery-capability-0.3.10/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-10 23:33:55.000000 discovery-capability-0.3.10/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-10 23:33:55.000000 discovery-capability-0.3.10/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-10 23:33:55.000000 discovery-capability-0.3.10/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.839071 discovery-capability-0.3.10/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      176 2023-07-10 23:33:27.000000 discovery-capability-0.3.10/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.843103 discovery-capability-0.3.10/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.3.10/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13813 2023-07-01 22:58:06.000000 discovery-capability-0.3.10/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1336 2023-06-29 23:02:32.000000 discovery-capability-0.3.10/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6359 2023-07-01 22:36:22.000000 discovery-capability-0.3.10/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.3.10/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.843992 discovery-capability-0.3.10/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.3.10/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.849569 discovery-capability-0.3.10/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.3.10/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11272 2023-07-09 15:15:11.000000 discovery-capability-0.3.10/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.3.10/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.3.10/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    64528 2023-07-09 21:53:32.000000 discovery-capability-0.3.10/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13425 2023-07-08 16:42:07.000000 discovery-capability-0.3.10/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.852342 discovery-capability-0.3.10/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.3.10/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.3.10/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.3.10/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.3.10/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.997020 discovery-capability-0.3.10/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.3.10/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.3.10/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-10 23:33:56.005950 discovery-capability-0.3.10/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.3.10/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:55.998200 discovery-capability-0.3.10/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.3.10/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:56.000667 discovery-capability-0.3.10/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.3.10/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2072 2023-07-01 22:50:31.000000 discovery-capability-0.3.10/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.3.10/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:56.001563 discovery-capability-0.3.10/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.3.10/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 23:33:56.004124 discovery-capability-0.3.10/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.3.10/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2715 2023-07-09 23:06:27.000000 discovery-capability-0.3.10/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.3.10/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2946 2023-07-09 20:40:49.000000 discovery-capability-0.3.10/test/intent/fb_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.669992 discovery-capability-0.3.9/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.3.9/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.3.9/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-10 15:37:16.670201 discovery-capability-0.3.9/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.3.9/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.507549 discovery-capability-0.3.9/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2277 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.507878 discovery-capability-0.3.9/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-09 20:27:05.000000 discovery-capability-0.3.9/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.512700 discovery-capability-0.3.9/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.3.9/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13813 2023-07-01 22:58:06.000000 discovery-capability-0.3.9/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1336 2023-06-29 23:02:32.000000 discovery-capability-0.3.9/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6359 2023-07-01 22:36:22.000000 discovery-capability-0.3.9/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.3.9/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.514252 discovery-capability-0.3.9/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.3.9/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.519410 discovery-capability-0.3.9/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.3.9/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11272 2023-07-09 15:15:11.000000 discovery-capability-0.3.9/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.3.9/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.3.9/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    64528 2023-07-09 21:53:32.000000 discovery-capability-0.3.9/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13425 2023-07-08 16:42:07.000000 discovery-capability-0.3.9/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.524035 discovery-capability-0.3.9/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.3.9/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.3.9/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.3.9/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.3.9/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.664138 discovery-capability-0.3.9/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.3.9/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-10 15:37:16.671000 discovery-capability-0.3.9/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.3.9/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.665083 discovery-capability-0.3.9/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.3.9/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.666698 discovery-capability-0.3.9/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.3.9/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2072 2023-07-01 22:50:31.000000 discovery-capability-0.3.9/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.3.9/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.667409 discovery-capability-0.3.9/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.3.9/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.669327 discovery-capability-0.3.9/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.3.9/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2715 2023-07-09 23:06:27.000000 discovery-capability-0.3.9/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.3.9/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2946 2023-07-09 20:40:49.000000 discovery-capability-0.3.9/test/intent/fb_intent_test.py
```

### Comparing `discovery-capability-0.3.10/LICENSE.txt` & `discovery-capability-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/PKG-INFO` & `discovery-capability-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.3.10
+Version: 0.3.9
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.3.10/README.rst` & `discovery-capability-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.3.9/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.3.10
+Version: 0.3.9
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.3.10/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.3.9/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.3.9/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/components/commons.py` & `discovery-capability-0.3.9/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/components/discovery.py` & `discovery-capability-0.3.9/ds_capability/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/components/feature_build.py` & `discovery-capability-0.3.9/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.3.9/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/intent/common_intent.py` & `discovery-capability-0.3.9/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.3.9/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.3.9/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.3.9/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.3.9/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.3.9/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.3.9/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.3.9/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.3.9/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.3.9/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.3.9/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.3.9/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/ds_capability/sample/sample_data.py` & `discovery-capability-0.3.9/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/setup.py` & `discovery-capability-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/test/component/discovery_test.py` & `discovery-capability-0.3.9/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/test/component/synthetic_test.py` & `discovery-capability-0.3.9/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.3.9/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.3.9/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.10/test/intent/fb_intent_test.py` & `discovery-capability-0.3.9/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

