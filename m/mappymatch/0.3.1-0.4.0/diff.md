# Comparing `tmp/mappymatch-0.3.1.tar.gz` & `tmp/mappymatch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappymatch-0.3.1.tar", last modified: Tue Apr  4 15:41:12 2023, max compression
+gzip compressed data, was "mappymatch-0.4.0.tar", last modified: Tue Jul 11 21:44:36 2023, max compression
```

## Comparing `mappymatch-0.3.1.tar` & `mappymatch-0.4.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.925080 mappymatch-0.3.1/
--rw-r--r--   0 nreinick (760205184) staff       (20)     1529 2022-05-02 21:53:13.000000 mappymatch-0.3.1/LICENSE
--rw-r--r--   0 nreinick (760205184) staff       (20)       40 2022-12-20 16:13:49.000000 mappymatch-0.3.1/MANIFEST.in
--rw-r--r--   0 nreinick (760205184) staff       (20)     3242 2023-04-04 15:41:12.924670 mappymatch-0.3.1/PKG-INFO
--rw-r--r--   0 nreinick (760205184) staff       (20)     2464 2023-04-03 21:07:46.000000 mappymatch-0.3.1/README.md
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.897916 mappymatch-0.3.1/mappymatch/
--rw-r--r--   0 nreinick (760205184) staff       (20)       88 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/__init__.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.903104 mappymatch-0.3.1/mappymatch/constructs/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/constructs/__init__.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     2525 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/constructs/coordinate.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     2948 2023-03-31 21:23:16.000000 mappymatch-0.3.1/mappymatch/constructs/geofence.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1309 2023-03-21 21:13:31.000000 mappymatch-0.3.1/mappymatch/constructs/match.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1770 2023-03-31 21:54:47.000000 mappymatch-0.3.1/mappymatch/constructs/road.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     9314 2023-03-21 21:14:35.000000 mappymatch-0.3.1/mappymatch/constructs/trace.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.904687 mappymatch-0.3.1/mappymatch/maps/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/maps/__init__.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     2138 2023-04-03 17:57:45.000000 mappymatch-0.3.1/mappymatch/maps/map_interface.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.905540 mappymatch-0.3.1/mappymatch/maps/nx/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/maps/nx/__init__.py
--rw-r--r--   0 nreinick (760205184) staff       (20)    11240 2023-04-03 19:32:55.000000 mappymatch-0.3.1/mappymatch/maps/nx/nx_map.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.906743 mappymatch-0.3.1/mappymatch/maps/nx/readers/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/maps/nx/readers/__init__.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     4474 2023-03-31 21:28:58.000000 mappymatch-0.3.1/mappymatch/maps/nx/readers/osm_readers.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.909404 mappymatch-0.3.1/mappymatch/matchers/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/matchers/__init__.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.911716 mappymatch-0.3.1/mappymatch/matchers/lcss/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/matchers/lcss/__init__.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     8236 2023-02-02 16:29:56.000000 mappymatch-0.3.1/mappymatch/matchers/lcss/constructs.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     5673 2023-04-03 17:27:57.000000 mappymatch-0.3.1/mappymatch/matchers/lcss/lcss.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     6530 2023-04-03 17:57:45.000000 mappymatch-0.3.1/mappymatch/matchers/lcss/ops.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     3519 2022-06-15 22:29:36.000000 mappymatch-0.3.1/mappymatch/matchers/lcss/utils.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1206 2022-12-20 16:13:49.000000 mappymatch-0.3.1/mappymatch/matchers/line_snap.py
--rw-r--r--   0 nreinick (760205184) staff       (20)      650 2023-03-21 21:13:31.000000 mappymatch-0.3.1/mappymatch/matchers/match_result.py
--rw-r--r--   0 nreinick (760205184) staff       (20)      875 2022-12-20 16:13:49.000000 mappymatch-0.3.1/mappymatch/matchers/matcher_interface.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     3364 2023-03-31 21:56:28.000000 mappymatch-0.3.1/mappymatch/matchers/osrm.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     4114 2023-02-03 21:34:27.000000 mappymatch-0.3.1/mappymatch/matchers/valhalla.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.912245 mappymatch-0.3.1/mappymatch/resources/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/resources/__init__.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.913271 mappymatch-0.3.1/mappymatch/resources/traces/
--rw-r--r--   0 nreinick (760205184) staff       (20)    22920 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/resources/traces/sample_trace_1.csv
--rw-r--r--   0 nreinick (760205184) staff       (20)    17321 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/resources/traces/sample_trace_2.csv
--rw-r--r--   0 nreinick (760205184) staff       (20)    31962 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/resources/traces/sample_trace_3.csv
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.916568 mappymatch-0.3.1/mappymatch/utils/
--rw-r--r--   0 nreinick (760205184) staff       (20)        0 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/utils/__init__.py
--rw-r--r--   0 nreinick (760205184) staff       (20)       66 2022-05-03 14:33:16.000000 mappymatch-0.3.1/mappymatch/utils/crs.py
--rw-r--r--   0 nreinick (760205184) staff       (20)      122 2022-05-09 16:10:22.000000 mappymatch-0.3.1/mappymatch/utils/exceptions.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1181 2022-10-10 22:36:21.000000 mappymatch-0.3.1/mappymatch/utils/geo.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     6011 2023-02-03 21:34:27.000000 mappymatch-0.3.1/mappymatch/utils/plot.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1734 2022-05-09 16:10:22.000000 mappymatch-0.3.1/mappymatch/utils/process_trace.py
--rw-r--r--   0 nreinick (760205184) staff       (20)      453 2022-05-09 16:10:22.000000 mappymatch-0.3.1/mappymatch/utils/url.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.900137 mappymatch-0.3.1/mappymatch.egg-info/
--rw-r--r--   0 nreinick (760205184) staff       (20)     3242 2023-04-04 15:41:12.000000 mappymatch-0.3.1/mappymatch.egg-info/PKG-INFO
--rw-r--r--   0 nreinick (760205184) staff       (20)     1815 2023-04-04 15:41:12.000000 mappymatch-0.3.1/mappymatch.egg-info/SOURCES.txt
--rw-r--r--   0 nreinick (760205184) staff       (20)        1 2023-04-04 15:41:12.000000 mappymatch-0.3.1/mappymatch.egg-info/dependency_links.txt
--rw-r--r--   0 nreinick (760205184) staff       (20)      312 2023-04-04 15:41:12.000000 mappymatch-0.3.1/mappymatch.egg-info/requires.txt
--rw-r--r--   0 nreinick (760205184) staff       (20)       11 2023-04-04 15:41:12.000000 mappymatch-0.3.1/mappymatch.egg-info/top_level.txt
--rw-r--r--   0 nreinick (760205184) staff       (20)     3267 2023-04-04 15:41:01.000000 mappymatch-0.3.1/pyproject.toml
--rw-r--r--   0 nreinick (760205184) staff       (20)       38 2023-04-04 15:41:12.925284 mappymatch-0.3.1/setup.cfg
--rw-r--r--   0 nreinick (760205184) staff       (20)       38 2022-09-28 21:13:14.000000 mappymatch-0.3.1/setup.py
-drwxr-xr-x   0 nreinick (760205184) staff       (20)        0 2023-04-04 15:41:12.924019 mappymatch-0.3.1/tests/
--rw-r--r--   0 nreinick (760205184) staff       (20)      767 2022-10-10 22:36:21.000000 mappymatch-0.3.1/tests/test_coordinate.py
--rw-r--r--   0 nreinick (760205184) staff       (20)      399 2022-09-30 15:34:30.000000 mappymatch-0.3.1/tests/test_geofence.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     8856 2023-03-31 22:08:46.000000 mappymatch-0.3.1/tests/test_lcss_add_match_for_stationary.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     3086 2022-05-09 15:27:45.000000 mappymatch-0.3.1/tests/test_lcss_compress.py
--rw-r--r--   0 nreinick (760205184) staff       (20)    12069 2022-05-09 15:27:45.000000 mappymatch-0.3.1/tests/test_lcss_drop_stationary_points.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     7939 2022-05-09 15:27:45.000000 mappymatch-0.3.1/tests/test_lcss_find_stationary_points.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     8246 2023-03-31 22:09:07.000000 mappymatch-0.3.1/tests/test_lcss_forward_merge.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     7792 2023-03-31 22:06:45.000000 mappymatch-0.3.1/tests/test_lcss_merge.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     8563 2023-03-31 22:09:07.000000 mappymatch-0.3.1/tests/test_lcss_reverse_merge.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     8272 2023-03-31 22:08:32.000000 mappymatch-0.3.1/tests/test_lcss_same_trajectory_scheme.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1143 2023-03-31 21:56:40.000000 mappymatch-0.3.1/tests/test_match_result.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1659 2023-03-31 18:09:22.000000 mappymatch-0.3.1/tests/test_osm.py
--rw-r--r--   0 nreinick (760205184) staff       (20)      734 2022-09-30 15:34:30.000000 mappymatch-0.3.1/tests/test_process_trace.py
--rw-r--r--   0 nreinick (760205184) staff       (20)     1632 2023-02-03 21:34:27.000000 mappymatch-0.3.1/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.526218 mappymatch-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-11 21:44:24.000000 mappymatch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 21:44:24.000000 mappymatch-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 21:44:36.526218 mappymatch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-11 21:44:24.000000 mappymatch-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.506217 mappymatch-0.4.0/mappymatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/geofence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/road.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch/maps/igraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/igraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/igraph/igraph_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/map_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.514217 mappymatch-0.4.0/mappymatch/maps/nx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/nx_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.514217 mappymatch-0.4.0/mappymatch/maps/nx/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/readers/osm_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.514217 mappymatch-0.4.0/mappymatch/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.518217 mappymatch-0.4.0/mappymatch/matchers/lcss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/constructs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/lcss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/line_snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/matcher_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/osrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/valhalla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.518217 mappymatch-0.4.0/mappymatch/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.518217 mappymatch-0.4.0/mappymatch/resources/traces/
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.522217 mappymatch-0.4.0/mappymatch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-11 21:44:24.000000 mappymatch-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:44:36.526218 mappymatch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:44:24.000000 mappymatch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.526218 mappymatch-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_geofence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_add_match_for_stationary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_drop_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_find_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_forward_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_reverse_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_same_trajectory_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_trace.py
```

### Comparing `mappymatch-0.3.1/LICENSE` & `mappymatch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/PKG-INFO` & `mappymatch-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappymatch
-Version: 0.3.1
+Version: 0.4.0
 Summary: Package for mapmatching.
 Author: National Renewable Energy Laboratory
 License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
 Project-URL: Homepage, https://github.com/NREL/mappymatch
 Keywords: GPS,map,match
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappymatch-0.3.1/README.md` & `mappymatch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/constructs/coordinate.py` & `mappymatch-0.4.0/mappymatch/constructs/coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/constructs/geofence.py` & `mappymatch-0.4.0/mappymatch/constructs/geofence.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/constructs/match.py` & `mappymatch-0.4.0/mappymatch/constructs/match.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/constructs/road.py` & `mappymatch-0.4.0/mappymatch/constructs/road.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/constructs/trace.py` & `mappymatch-0.4.0/mappymatch/constructs/trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/maps/map_interface.py` & `mappymatch-0.4.0/mappymatch/maps/map_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         """
 
     @abstractmethod
     def shortest_path(
         self,
         origin: Coordinate,
         destination: Coordinate,
-        weight: Union[str, Callable] = DEFAULT_TIME_WEIGHT,
+        weight: Optional[Union[str, Callable]] = None,
     ) -> List[Road]:
         """
         Computes the shortest path on the road network
 
         Args:
             origin: The origin coordinate
             destination: The destination coordinate
```

### Comparing `mappymatch-0.3.1/mappymatch/maps/nx/nx_map.py` & `mappymatch-0.4.0/mappymatch/maps/nx/nx_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,60 +70,62 @@
         self._time_weight = time_weight
         self._geom_key = geom_key
         self._metadata_key = metadata_key
         self._crs_key = crs_key
 
         self._build_rtree()
 
+    def _has_road_id(self, road_id: RoadId) -> bool:
+        return self.g.has_edge(*road_id)
+
     def _build_road(
         self,
-        origin_id: Union[str, int],
-        destination_id: Union[str, int],
-        key: Union[str, int],
-        edge_data: Dict[str, Any],
+        road_id: RoadId,
     ) -> Road:
         """
-        Build a road from an origin, destination and networkx edge data
+        Build a road from a road id, pulling the edge data from the graph
+
+        Be sure to check if the road id (_has_road_id) is in the graph before calling this method
         """
+        edge_data = self.g.get_edge_data(*road_id)
+
         metadata = edge_data.get(self._metadata_key)
 
         if metadata is None:
             metadata = {}
         else:
             metadata = metadata.copy()
 
         metadata[self._dist_weight] = edge_data.get(self._dist_weight)
         metadata[self._time_weight] = edge_data.get(self._time_weight)
 
-        road_id = RoadId(origin_id, destination_id, key)
-
         road = Road(
             road_id,
             edge_data[self._geom_key],
             metadata=metadata,
         )
 
         return road
 
     def _build_rtree(self):
-        road_lookup = {}
 
         idx = rt.index.Index()
         for i, gtuple in enumerate(self.g.edges(data=True, keys=True)):
             u, v, k, d = gtuple
-            road = self._build_road(u, v, k, d)
+            road_id = RoadId(u, v, k)
+            # road = self._build_road(u, v, k, d)
             geom = d[self._geom_key]
             box = geom.bounds
 
-            idx.insert(i, box, obj=road.road_id)
+            idx.insert(i, box, obj=road_id)
 
-            road_lookup[road.road_id] = road
+            # road_lookup[road.road_id] = road
 
         self.rtree = idx
-        self._road_lookup: Dict[RoadId, Road] = road_lookup
+        # self._road_lookup: Dict[RoadId, Road] = road_lookup
 
     def __str__(self):
         output_lines = [
             "Mappymatch NxMap object",
             f"roads: {len(self._road_lookup)} Road objects",
             f"graph: {self.g}",
         ]
@@ -146,15 +148,18 @@
 
         Args:
             road_id: The id of the road to get
 
         Returns:
             The road with the given id, or None if it does not exist
         """
-        return self._road_lookup.get(road_id)
+        if self._has_road_id(road_id):
+            return self._build_road(road_id)
+        else:
+            return None
 
     def set_road_attributes(self, attributes: Dict[RoadId, Dict[str, Any]]):
         """
         Set the attributes of the roads in the map
 
         Args:
             attributes: A dictionary mapping road ids to dictionaries of attributes
@@ -163,15 +168,19 @@
             None
         """
         nx.set_edge_attributes(self.g, attributes)
         self._build_rtree()
 
     @property
     def roads(self) -> List[Road]:
-        return list(self._road_lookup.values())
+        roads = [
+            self._build_road(RoadId(u, v, k))
+            for u, v, k in self.g.edges(keys=True)
+        ]
+        return roads
 
     @classmethod
     def from_file(cls, file: Union[str, Path]) -> NxMap:
         """
         Build a NxMap instance from a file
 
         Args:
@@ -301,28 +310,28 @@
 
         if len(nearest_candidates) == 0:
             raise ValueError(f"No roads found for {coord}")
         elif len(nearest_candidates) == 1:
             nearest_id = nearest_candidates[0]
         else:
             distances = [
-                self._road_lookup[i].geom.distance(coord.geom)
+                self._build_road(i).geom.distance(coord.geom)
                 for i in nearest_candidates
             ]
             nearest_id = nearest_candidates[np.argmin(distances)]
 
-        road = self._road_lookup[nearest_id]
+        road = self._build_road(nearest_id)
 
         return road
 
     def shortest_path(
         self,
         origin: Coordinate,
         destination: Coordinate,
-        weight: Union[str, Callable] = DEFAULT_TIME_WEIGHT,
+        weight: Optional[Union[str, Callable]] = None,
     ) -> List[Road]:
         """
         Computes the shortest path between an origin and a destination
 
         Args:
             origin: The origin coordinate
             destination: The destination coordinate
@@ -336,14 +345,17 @@
                 f"crs of origin {origin.crs} must match crs of map {self.crs}"
             )
         elif destination.crs != self.crs:
             raise ValueError(
                 f"crs of destination {destination.crs} must match crs of map {self.crs}"
             )
 
+        if weight is None:
+            weight = self._time_weight
+
         origin_road = self.nearest_road(origin)
         dest_road = self.nearest_road(destination)
 
         ostart = Point(origin_road.geom.coords[0])
         oend = Point(origin_road.geom.coords[-1])
 
         dstart = Point(dest_road.geom.coords[0])
@@ -378,12 +390,12 @@
             road_end_node = nx_route[i]
 
             edge_data = self.g.get_edge_data(road_start_node, road_end_node)
             road_key = list(edge_data.keys())[0]
 
             road_id = RoadId(road_start_node, road_end_node, road_key)
 
-            road = self._road_lookup[road_id]
+            road = self._build_road(road_id)
 
             path.append(road)
 
         return path
```

### Comparing `mappymatch-0.3.1/mappymatch/maps/nx/readers/osm_readers.py` & `mappymatch-0.4.0/mappymatch/maps/nx/readers/osm_readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,14 +154,17 @@
         "name",
         "maxspeed",
         "highway",
         "length",
         "speed_kph",
         "osmid",
         "street_count",
+        "junction",
+        "bridge",
+        "tunnel",
         "y",
         "x",
     ]
 
     for _, _, d in g.edges(data=True):
         for k in keys_to_delete:
             try:
```

### Comparing `mappymatch-0.3.1/mappymatch/matchers/lcss/constructs.py` & `mappymatch-0.4.0/mappymatch/matchers/lcss/constructs.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/lcss/lcss.py` & `mappymatch-0.4.0/mappymatch/matchers/lcss/lcss.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/lcss/ops.py` & `mappymatch-0.4.0/mappymatch/matchers/lcss/ops.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/lcss/utils.py` & `mappymatch-0.4.0/mappymatch/matchers/lcss/utils.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/line_snap.py` & `mappymatch-0.4.0/mappymatch/matchers/line_snap.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/match_result.py` & `mappymatch-0.4.0/mappymatch/matchers/match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/matcher_interface.py` & `mappymatch-0.4.0/mappymatch/matchers/matcher_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/osrm.py` & `mappymatch-0.4.0/mappymatch/matchers/osrm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/matchers/valhalla.py` & `mappymatch-0.4.0/mappymatch/matchers/valhalla.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/resources/traces/sample_trace_1.csv` & `mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_1.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/resources/traces/sample_trace_2.csv` & `mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_2.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/resources/traces/sample_trace_3.csv` & `mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_3.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/utils/geo.py` & `mappymatch-0.4.0/mappymatch/utils/geo.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/utils/plot.py` & `mappymatch-0.4.0/mappymatch/utils/plot.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch/utils/process_trace.py` & `mappymatch-0.4.0/mappymatch/utils/process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/mappymatch.egg-info/PKG-INFO` & `mappymatch-0.4.0/mappymatch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappymatch
-Version: 0.3.1
+Version: 0.4.0
 Summary: Package for mapmatching.
 Author: National Renewable Energy Laboratory
 License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
 Project-URL: Homepage, https://github.com/NREL/mappymatch
 Keywords: GPS,map,match
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappymatch-0.3.1/mappymatch.egg-info/SOURCES.txt` & `mappymatch-0.4.0/mappymatch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 mappymatch/constructs/coordinate.py
 mappymatch/constructs/geofence.py
 mappymatch/constructs/match.py
 mappymatch/constructs/road.py
 mappymatch/constructs/trace.py
 mappymatch/maps/__init__.py
 mappymatch/maps/map_interface.py
+mappymatch/maps/igraph/__init__.py
+mappymatch/maps/igraph/igraph_map.py
 mappymatch/maps/nx/__init__.py
 mappymatch/maps/nx/nx_map.py
 mappymatch/maps/nx/readers/__init__.py
 mappymatch/maps/nx/readers/osm_readers.py
 mappymatch/matchers/__init__.py
 mappymatch/matchers/line_snap.py
 mappymatch/matchers/match_result.py
```

### Comparing `mappymatch-0.3.1/pyproject.toml` & `mappymatch-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mappymatch"
-version = "0.3.1"
+version = "0.4.0"
 description = "Package for mapmatching."
 readme = "README.md"
 authors = [{ name = "National Renewable Energy Laboratory" }]
 license = { text = "BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
@@ -25,14 +25,15 @@
   "rtree",
   "pyproj",
   "pandas",
   "numpy",
   "matplotlib",
   "osmnx",
   "networkx<3",
+  "igraph",
   "folium",
   "requests",
   "polyline",
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
@@ -104,15 +105,15 @@
 
 [tool.tbump]
 # Uncomment  this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
 # Make sure this matches current_version before using tbump
-current = "0.3.1"
+current = "0.4.0"
 # Example of a semver regexp.
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `mappymatch-0.3.1/tests/test_coordinate.py` & `mappymatch-0.4.0/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_add_match_for_stationary.py` & `mappymatch-0.4.0/tests/test_lcss_add_match_for_stationary.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_compress.py` & `mappymatch-0.4.0/tests/test_lcss_compress.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_drop_stationary_points.py` & `mappymatch-0.4.0/tests/test_lcss_drop_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_find_stationary_points.py` & `mappymatch-0.4.0/tests/test_lcss_find_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_forward_merge.py` & `mappymatch-0.4.0/tests/test_lcss_forward_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_merge.py` & `mappymatch-0.4.0/tests/test_lcss_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_reverse_merge.py` & `mappymatch-0.4.0/tests/test_lcss_reverse_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_lcss_same_trajectory_scheme.py` & `mappymatch-0.4.0/tests/test_lcss_same_trajectory_scheme.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_match_result.py` & `mappymatch-0.4.0/tests/test_match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_osm.py` & `mappymatch-0.4.0/tests/test_osm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_process_trace.py` & `mappymatch-0.4.0/tests/test_process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.3.1/tests/test_trace.py` & `mappymatch-0.4.0/tests/test_trace.py`

 * *Files identical despite different names*

