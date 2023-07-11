# Comparing `tmp/deepsport_utilities-4.8.2.tar.gz` & `tmp/deepsport_utilities-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepsport_utilities-4.8.2.tar", last modified: Fri Apr  7 13:58:47 2023, max compression
+gzip compressed data, was "dist/deepsport_utilities-4.9.0.tar", last modified: Tue Jul 11 11:10:40 2023, max compression
```

## Comparing `deepsport_utilities-4.8.2.tar` & `deepsport_utilities-4.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.443850 deepsport_utilities-4.8.2/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      207 2022-10-28 11:10:00.000000 deepsport_utilities-4.8.2/.gitignore
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      462 2022-11-25 12:56:28.000000 deepsport_utilities-4.8.2/.gitlab-ci.yml
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      312 2023-04-07 13:58:47.442850 deepsport_utilities-4.8.2/PKG-INFO
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     2802 2022-12-06 13:30:17.000000 deepsport_utilities-4.8.2/README.md
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.333851 deepsport_utilities-4.8.2/assets/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)   494314 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/assets/keemotion_3D_world_convention.png
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      896 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/calibration.md
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.346851 deepsport_utilities-4.8.2/deepsport_utilities/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      306 2023-02-14 09:30:53.000000 deepsport_utilities-4.8.2/deepsport_utilities/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4177 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/deepsport_utilities/calib.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    19474 2022-11-25 12:56:28.000000 deepsport_utilities-4.8.2/deepsport_utilities/court.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    11178 2023-04-07 11:55:45.000000 deepsport_utilities-4.8.2/deepsport_utilities/dataset.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.357851 deepsport_utilities-4.8.2/deepsport_utilities/ds/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        0 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     3618 2023-03-09 15:36:32.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/generic_dataset.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.368851 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1628 2023-03-09 14:36:01.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    11187 2023-03-28 12:42:37.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/dataset_splitters.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    12933 2023-03-14 09:01:44.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/instants_dataset.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4125 2023-02-16 13:53:21.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/instants_transforms.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6206 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/mod_source.c
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    19424 2023-04-07 13:55:13.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/views_dataset.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    16017 2023-04-04 09:17:54.000000 deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/views_transforms.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     9068 2023-04-04 07:02:31.000000 deepsport_utilities-4.8.2/deepsport_utilities/transforms.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    12310 2023-03-01 15:29:46.000000 deepsport_utilities-4.8.2/deepsport_utilities/utils.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.354851 deepsport_utilities-4.8.2/deepsport_utilities.egg-info/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      312 2023-04-07 13:58:47.000000 deepsport_utilities-4.8.2/deepsport_utilities.egg-info/PKG-INFO
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1964 2023-04-07 13:58:47.000000 deepsport_utilities-4.8.2/deepsport_utilities.egg-info/SOURCES.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        1 2023-04-07 13:58:47.000000 deepsport_utilities-4.8.2/deepsport_utilities.egg-info/dependency_links.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      138 2023-04-07 13:58:47.000000 deepsport_utilities-4.8.2/deepsport_utilities.egg-info/requires.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       26 2023-04-07 13:58:47.000000 deepsport_utilities-4.8.2/deepsport_utilities.egg-info/top_level.txt
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.319851 deepsport_utilities-4.8.2/docs/
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.390850 deepsport_utilities-4.8.2/docs/deepsport_utilities/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    20972 2023-04-07 13:58:45.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/calib.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    65194 2023-04-07 13:58:45.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/court.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    51011 2023-04-07 13:58:45.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/dataset.html
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.394850 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    22914 2023-04-07 13:58:45.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/generic_dataset.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     7181 2023-04-07 13:58:45.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/index.html
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.413850 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    48799 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/dataset_splitters.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)   135657 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/index.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    61527 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/instants_dataset.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    22727 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/instants_transforms.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    81674 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/views_dataset.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    70845 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/views_transforms.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     8395 2023-04-07 13:58:45.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/index.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    46607 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/transforms.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    55589 2023-04-07 13:58:46.000000 deepsport_utilities-4.8.2/docs/deepsport_utilities/utils.html
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.418850 deepsport_utilities-4.8.2/examples/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1009 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/examples/create_camera_views_dataset.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      882 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/examples/import_instants_dataset.py
--rwxr-x---   0 gvanzand (3002593) gvanzand (3002593)      541 2022-11-25 13:12:57.000000 deepsport_utilities-4.8.2/release.sh
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      226 2023-02-14 09:26:08.000000 deepsport_utilities-4.8.2/requirements.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2023-04-07 13:58:47.444850 deepsport_utilities-4.8.2/setup.cfg
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1049 2023-04-07 13:56:04.000000 deepsport_utilities-4.8.2/setup.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.423850 deepsport_utilities-4.8.2/tests/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        0 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/tests/__init__.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.426850 deepsport_utilities-4.8.2/tests/groundtruths/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    22651 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/tests/groundtruths/ball_view.png
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      287 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/tests/groundtruths/test_fill_polygon.png
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-07 13:58:47.428850 deepsport_utilities-4.8.2/tests/input_imgs/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)  2220963 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/tests/input_imgs/game_94132_frame_idx_0.png
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5912 2023-02-15 10:39:58.000000 deepsport_utilities-4.8.2/tests/test_calib.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1116 2022-10-28 08:52:47.000000 deepsport_utilities-4.8.2/tests/test_court.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:40.014399 deepsport_utilities-4.9.0/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      207 2022-10-28 11:10:00.000000 deepsport_utilities-4.9.0/.gitignore
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      462 2022-11-25 12:56:28.000000 deepsport_utilities-4.9.0/.gitlab-ci.yml
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      312 2023-07-11 11:10:40.013399 deepsport_utilities-4.9.0/PKG-INFO
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     2802 2022-12-06 13:30:17.000000 deepsport_utilities-4.9.0/README.md
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.232406 deepsport_utilities-4.9.0/assets/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)   494314 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/assets/keemotion_3D_world_convention.png
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      896 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/calibration.md
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.340405 deepsport_utilities-4.9.0/deepsport_utilities/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      306 2023-02-14 09:30:53.000000 deepsport_utilities-4.9.0/deepsport_utilities/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4177 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/deepsport_utilities/calib.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    20376 2023-07-04 12:40:53.000000 deepsport_utilities-4.9.0/deepsport_utilities/court.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    11123 2023-05-18 11:42:45.000000 deepsport_utilities-4.9.0/deepsport_utilities/dataset.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.804401 deepsport_utilities-4.9.0/deepsport_utilities/ds/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        0 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     3618 2023-03-09 15:36:32.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/generic_dataset.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.820400 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1628 2023-03-09 14:36:01.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    12606 2023-07-11 11:07:24.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/dataset_splitters.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    13084 2023-07-11 08:34:41.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/instants_dataset.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4125 2023-02-16 13:53:21.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/instants_transforms.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6206 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/mod_source.c
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    19913 2023-07-11 10:16:54.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/views_dataset.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    18244 2023-07-11 09:42:43.000000 deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/views_transforms.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     9436 2023-07-11 07:40:03.000000 deepsport_utilities-4.9.0/deepsport_utilities/transforms.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    12372 2023-05-15 09:04:58.000000 deepsport_utilities-4.9.0/deepsport_utilities/utils.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.799401 deepsport_utilities-4.9.0/deepsport_utilities.egg-info/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      312 2023-07-11 11:10:37.000000 deepsport_utilities-4.9.0/deepsport_utilities.egg-info/PKG-INFO
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1964 2023-07-11 11:10:38.000000 deepsport_utilities-4.9.0/deepsport_utilities.egg-info/SOURCES.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        1 2023-07-11 11:10:37.000000 deepsport_utilities-4.9.0/deepsport_utilities.egg-info/dependency_links.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      138 2023-07-11 11:10:37.000000 deepsport_utilities-4.9.0/deepsport_utilities.egg-info/requires.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       26 2023-07-11 11:10:37.000000 deepsport_utilities-4.9.0/deepsport_utilities.egg-info/top_level.txt
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.055407 deepsport_utilities-4.9.0/docs/
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.835400 deepsport_utilities-4.9.0/docs/deepsport_utilities/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    20972 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/calib.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    67575 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/court.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    51030 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/dataset.html
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.841400 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    22914 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/generic_dataset.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     7181 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/index.html
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.858400 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    52585 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/dataset_splitters.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)   138401 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/index.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    62304 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/instants_dataset.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    22727 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/instants_transforms.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    83650 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/views_dataset.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    77323 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/views_transforms.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     8395 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/index.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    48255 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/transforms.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    55763 2023-07-11 11:10:33.000000 deepsport_utilities-4.9.0/docs/deepsport_utilities/utils.html
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.863400 deepsport_utilities-4.9.0/examples/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1009 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/examples/create_camera_views_dataset.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      882 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/examples/import_instants_dataset.py
+-rwxr-x---   0 gvanzand (3002593) gvanzand (3002593)      541 2022-11-25 13:12:57.000000 deepsport_utilities-4.9.0/release.sh
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      226 2023-02-14 09:26:08.000000 deepsport_utilities-4.9.0/requirements.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2023-07-11 11:10:40.014399 deepsport_utilities-4.9.0/setup.cfg
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1049 2023-07-11 11:10:07.000000 deepsport_utilities-4.9.0/setup.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.869400 deepsport_utilities-4.9.0/tests/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        0 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/tests/__init__.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.873400 deepsport_utilities-4.9.0/tests/groundtruths/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    22651 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/tests/groundtruths/ball_view.png
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      287 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/tests/groundtruths/test_fill_polygon.png
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-07-11 11:10:39.875400 deepsport_utilities-4.9.0/tests/input_imgs/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)  2220963 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/tests/input_imgs/game_94132_frame_idx_0.png
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5912 2023-02-15 10:39:58.000000 deepsport_utilities-4.9.0/tests/test_calib.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1116 2022-10-28 08:52:47.000000 deepsport_utilities-4.9.0/tests/test_court.py
```

### Comparing `deepsport_utilities-4.8.2/README.md` & `deepsport_utilities-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/assets/keemotion_3D_world_convention.png` & `deepsport_utilities-4.9.0/assets/keemotion_3D_world_convention.png`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/calibration.md` & `deepsport_utilities-4.9.0/calibration.md`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/calib.py` & `deepsport_utilities-4.9.0/deepsport_utilities/calib.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/court.py` & `deepsport_utilities-4.9.0/deepsport_utilities/court.py`

 * *Files 8% similar despite different names*

```diff
@@ -295,7 +295,22 @@
 
 def sort_points_clockwise(data):
     assert data.size != 0, "Empty input data"
     mean = np.mean(data, axis=0) # center of mass of the points
     angles = np.arctan2((data-mean)[:, 1], (data-mean)[:, 0])
     angles[angles < 0] = angles[angles < 0] + 2 * np.pi # Transform angles from [-pi,pi] -> [0, 2*pi]
     return data[np.argsort(angles)]
+
+
+def draw_ball(image, calib: Calib, center: Point3D, color=(0,0,255), cross=True, label=None, thickness=1, fontsize=10):
+    pd = ProjectiveDrawer(calib, color, thickness=thickness)
+    ground3D = Point3D(center.x, center.y, 0)
+    pd.draw_line(image, center, ground3D, lineType=cv2.LINE_AA, color=color)
+    if cross:
+        pd.draw_line(image, ground3D+Point3D(100,0,0), ground3D-Point3D(100,0,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+        pd.draw_line(image, ground3D+Point3D(0,100,0), ground3D-Point3D(0,100,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+    radius = pd.calib.compute_length2D(center, BALL_DIAMETER/2)[0]
+    x, y = pd.calib.project_3D_to_2D(center).to_int_tuple()
+
+    cv2.circle(image, (x, y), int(radius), color, 1)
+    if label is not None:
+        cv2.putText(image, label, (x, y - 10), cv2.FONT_HERSHEY_SIMPLEX, fontsize, color, 2, lineType=cv2.LINE_AA)
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/dataset.py` & `deepsport_utilities-4.9.0/deepsport_utilities/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 from enum import IntFlag
 import errno
+import logging
 import os
 import random
 import shutil
 import threading
 
 import numpy as np
 
@@ -245,72 +246,81 @@
 
 #     def query_item(self, key):
 #         if self.filename:
 #             super().__init__(self.filename)
 #             self.query_item = super().query_item
 #         return super().query_item(key)
 
-
-def first(filename):
-    try:
-        with open(filename, "x") as _:
-            return True
-    except FileExistsError:
-        return False
-
 class CachedPickledDataset(PickledDataset):
     def __init__(self, filename, local_scratch=""):
         super().__init__(filename)
         local_scratch = local_scratch or os.environ.get('LOCALSCRATCH', "")
-        self.filename = None
-        if local_scratch and local_scratch not in filename:
-            lock = os.path.join(local_scratch, f"{os.path.basename(filename)}.lock")
-            if first(lock): # First process to reach this point copies the dataset
-                def f():
-                    print(f"Copying dataset to local scratch: {filename} -> {local_scratch}.")
-                    try:
-                        self.filename = shutil.copy(filename, local_scratch)
-                    except:
-                        try:
-                            os.remove(os.path.join(local_scratch, os.path.basename(filename)))
-                        except:
-                            pass
-                        print("Failed copying dataset.")
-                        self.query_item = super().query_item
-                    os.remove(lock)
-                self.thread = threading.Thread(target=f)
-                self.thread.start()
-                self.available = lambda: self.filename
-            else: # Other processes wait for the dataset to be copied
-                print(f"Waiting for dataset to be copied to {local_scratch}/ ...")
-                self.filename = os.path.join(local_scratch, os.path.basename(filename))
-                self.available = lambda: not os.path.exists(lock)
-        else:
+        if not local_scratch or local_scratch in filename:
             self.query_item = super().query_item
+            return
+
+        self.filename = os.path.join(local_scratch, os.path.basename(filename))
+        lock = f"{self.filename}.lock"
+        self.available = lambda: not os.path.exists(lock)
+
+        try:
+            with open(lock, "x") as _:
+                pass # First process to reach this point copies the dataset
+        except FileExistsError:
+            return
+
+        if os.path.isfile(self.filename):
+            os.remove(lock)
+            self.reload()
+            return
+
+        def function():
+            logging.info(f"Copying dataset to local scratch: {filename} -> " \
+                f"{self.filename}.")
+            try:
+                shutil.copy(filename, self.filename)
+            except:
+                try:
+                    os.remove(self.filename)
+                except:
+                    pass
+                logging.info("Failed copying dataset.")
+                self.query_item = super().query_item
+            os.remove(lock)
+        self.thread = threading.Thread(target=function, daemon=True)
+        self.thread.start()
+
+    def reload(self):
+        logging.info(f"Reloading dataset from {self.filename}")
+        super().__init__(self.filename)
+        self.query_item = super().query_item
 
     def query_item(self, key):
         if self.available():
-            print(f"Reloading dataset from {self.filename}")
-            super().__init__(self.filename)
-            self.query_item = super().query_item
+            self.reload()
         return super().query_item(key)
 
 
 
-def find(path, dirs=None, verbose=True):
+def find(path, dirs=None, verbose=True, fail=True):
     if os.path.isabs(path):
         if not os.path.isfile(path) and not os.path.isdir(path):
+            if not fail:
+                not verbose or print(f"{path} not found")
+                return None
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
         return path
 
     dirs = dirs or [os.getcwd(), *os.getenv("DATA_PATH", "").split(":")]
     for dirname in dirs:
         if dirname is None:
             continue
         tmp_path = os.path.join(dirname, path)
         if os.path.isfile(tmp_path) or os.path.isdir(tmp_path):
-            if verbose:
-                print("{} found in {}".format(path, tmp_path))
+            not verbose or print("{} found in {}".format(path, tmp_path))
             return tmp_path
 
+    if not fail:
+        not verbose or print(f"{path} not found (searched in {dirs})")
+        return None
     raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
                                 "{} (searched in {})".format(path, dirs))
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/generic_dataset.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/__init__.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/dataset_splitters.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/dataset_splitters.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         random.setstate(random_state)
         testing2_keys = None
         if additional_keys:
             if self.additional_keys_usage == "testing":
                 testing_keys += additional_keys
                 self.testing_arena_labels = self.testing_arena_labels.union(additional_arena_labels)
             elif self.additional_keys_usage == "training":
+                print(f"WARNING: adding {len(additional_keys)} keys to the training set")
                 training_keys += additional_keys
             elif self.additional_keys_usage == "validation":
                 validation_keys += additional_keys
             elif self.additional_keys_usage in ["none", "skip"]:
                 pass
             elif self.additional_keys_usage == "testing2":
                 testing2_keys = additional_keys
@@ -193,15 +194,15 @@
         ]
 
 class TestingArenaLabelsDatasetSplitter():
     def __init__(self, testing_arena_labels, validation_pc=15, repetitions=1):
         self.testing_arena_labels = testing_arena_labels
         self.validation_pc = validation_pc
         self.repetitions = repetitions
-        assert isinstance(self.testing_arena_labels, list)
+        assert isinstance(self.testing_arena_labels, (list, tuple))
 
     def __call__(self, dataset, fold=0):
         testing_keys, remaining_keys = [], []
         for key in dataset.keys:
             (remaining_keys, testing_keys)[key.arena_label in self.testing_arena_labels].append(key)
 
         # Backup random seed
@@ -220,7 +221,33 @@
 
         subsets = [
             Subset(name="training", subset_type=SubsetType.TRAIN, keys=training_keys, dataset=dataset),
             Subset(name="validation", subset_type=SubsetType.EVAL, keys=validation_keys, dataset=dataset, repetitions=self.repetitions),
             Subset(name="testing", subset_type=SubsetType.EVAL, keys=testing_keys, dataset=dataset, repetitions=self.repetitions),
         ]
         return [s for s in subsets if len(s.keys) > 0]
+
+
+
+class TestingValidationArenaLabelsDatasetSplitter():
+    def __init__(self, testing_arena_labels, validation_arena_labels):
+        assert isinstance(testing_arena_labels, (list, tuple))
+        assert isinstance(validation_arena_labels, (list, tuple))
+        self.testing_arena_labels = testing_arena_labels
+        self.validation_arena_labels = validation_arena_labels
+        assert len(set(self.testing_arena_labels).intersection(set(self.validation_arena_labels))) == 0
+
+    def __call__(self, dataset, fold=0):
+        validation_keys, testing_keys, training_keys = [], [], []
+        for key in dataset.keys:
+            if key.arena_label in self.testing_arena_labels:
+                testing_keys.append(key)
+            elif key.arena_label in self.validation_arena_labels:
+                validation_keys.append(key)
+            else:
+                training_keys.append(key)
+        subsets = [
+            Subset(name="training", subset_type=SubsetType.TRAIN, keys=training_keys, dataset=dataset),
+            Subset(name="validation", subset_type=SubsetType.EVAL, keys=validation_keys, dataset=dataset, repetitions=1),
+            Subset(name="testing", subset_type=SubsetType.EVAL, keys=testing_keys, dataset=dataset, repetitions=1),
+        ]
+        return [s for s in subsets if len(s.keys) > 0]
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/instants_dataset.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/instants_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,27 +58,29 @@
             "ball": Ball
         }
         self.annotations = [annotation_map[a['type']](a)for a in (db_item.get('annotations', []) or [])]
 
         self.image_source = db_item.get("image_source", "raw")
         self.court_dim = COURT_DIM[self.rule_type]
         self.court = Court(self.rule_type)
+        self.timestamps = [self.timestamp for _ in range(self.num_cameras)]
 
     def __str__(self):
         return "({}[{:5d}]@{})".format(self.arena_label, self.game_id, self.timestamp)
 
     def get_filekey(self, prefix, suffix):
         return os.path.join(self.arena_label, str(self.game_id), "{}{}{}".format(prefix, self.timestamp, suffix))
 
     @cached_property
     def calibs(self):
         return [self.__load_calib(c) for c in range(self.num_cameras)]
 
     @cached_property
     def all_images(self):
+        _ = self.calibs # triggers calib loading
         all_images = {}
         for c in range(self.num_cameras):
             for idx, offset in enumerate(self.offsets):
                 if     (idx == 0) \
                     or (idx == 1 and self.download_flags & DownloadFlags.WITH_FOLLOWING_IMAGE) \
                     or (self.download_flags & DownloadFlags.WITH_ALL_IMAGES):
                     try:
@@ -275,14 +277,15 @@
     def __repr__(self):
         return "Ball(" + ",".join([
             f"origin='{self.origin}', " \
             f"center=({self.center.x:.01f}, {self.center.y:.01f}, {self.center.z:.01f})" \
         ]) + ")"
 
 class BallAnnotation(Ball):
+    origin = "annotation"
     pass # retro-compatibility
 
 
 class Player():
     def __init__(self, data):
         self.type = "player"
         self.origin = data.get('origin', "annotation")
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/instants_transforms.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/instants_transforms.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/mod_source.c` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/mod_source.c`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/views_dataset.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/views_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,23 +242,26 @@
             if not instant.calibs[ball.camera].projects_in(ball.center):
                 continue
             keypoints = [ball.center]
             c = int(ball.camera)
             timestamp = getattr(instant, "timestamps", [instant.timestamp]*instant.num_cameras)[c] # timestamps may be different for each camera
             yield ViewDescription(c, idx, self.compute_box(keypoints, instant.calibs[c]), ball=ball, timestamp=timestamp)
 
-
 class BuildBallViewsWithRandom(BuildBallViews):
     """ random: a proportion of random views that are at least `margin` away from any created view.
     """
     def __init__(self, *args, random: float=0, **kwargs):
         assert 0 <= random < 1, "random must be in [0,1["
         super().__init__(*args, **kwargs)
         self.random = random
         self.record = {True: 0, False: 0}
+    def compute_box(self, point3D_list: list, calib: Calib):
+        if self.margin == np.inf:
+            return BoundingBox(0, 0, calib.width, calib.height)
+        return super().compute_box(point3D_list, calib)
     def __call__(self, instant_key: InstantKey, instant: Instant):
         idx = 0
         boxes = {}
         for view_description in super().__call__(instant_key, instant):
             yield view_description
             idx = view_description.index + 1
             boxes.setdefault(view_description.camera, []).append(view_description.box)
@@ -293,16 +296,14 @@
             keypoints = [point3D]
             c = int(ball.camera)
             timestamp = getattr(instant, "timestamps", [instant.timestamp]*instant.num_cameras)[c] # timestamps may be different for each camera
             yield ViewDescription(c, idx, self.compute_box(keypoints, instant.calibs[c]), ball=ball, timestamp=timestamp)
             idx += 1
             self.record[False] += 1
 
-
-
 class BuildHeadsViews(ViewBuilder):
     def __call__(self, instant_key: InstantKey, instant: Instant):
         for idx, player in enumerate([a for a in instant.annotations if a.type == "player"]):
             c = int(player.camera)
             keypoints = [player.head]
             yield ViewDescription(c, idx, self.compute_box(keypoints, instant.calibs[c]), annotation=player)
 
@@ -312,58 +313,64 @@
             instants_dataset   - the InstantDataset from which views are built
             view_builder       - the ViewBuilder dictating what type of view is to be created
             output_shape       - view aspect ratio (or exact dimension if 'rescale' is given)
             rescale            - tells whether the view should be rescaled to output_shape size
             crop               - tells whether the original image should be cropped or a rectangle
                                  should be drawn instead (for debug purposes)
     """
-    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True):
+    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
         super().__init__(instants_dataset)
         self.view_builder = view_builder
         self.output_shape = output_shape
         self.rescale = rescale
         self.crop = crop
+        self.debug = debug
 
     def _crop_view(self, view_description: ViewDescription, instant: Instant, **kwargs):
         padding = self.view_builder.padding
         c = view_description.camera
         input_height, input_width, _ = instant.images[c].shape
         aspect_ratio = self.output_shape[0]/self.output_shape[1] if self.output_shape else None
         x_slice, y_slice = view_description.box.increase_box(
             max_width=input_width,
             max_height=input_height,
             aspect_ratio=aspect_ratio,
             padding=self.view_builder.padding
         )
-        all_images = []
 
         if self.crop:
+            all_images = []
             for offset in instant.offsets:
                 index = (c,offset)
                 if index not in instant.all_images:
                     continue # that offset was not downloaded with the download flag of instants dataset
                 image = crop_padded(instant.all_images[index], x_slice, y_slice, padding)
-                if self.rescale and self.output_shape:
+                height, width, _ = image.shape
+                if self.rescale and self.output_shape and (width, height) != self.output_shape:
                     image = cv2.resize(image, self.output_shape)
                 all_images.append(image)
             calib = instant.calibs[c].crop(x_slice, y_slice) # handles negative `slice.start` positions
             if self.rescale and self.output_shape:
                 calib = calib.scale(*self.output_shape)
             if instant.download_flags & DownloadFlags.WITH_HUMAN_SEGMENTATION_MASKS and instant.human_masks:
                 human_masks = crop_padded(instant.human_masks[c], x_slice, y_slice, padding)
                 if self.rescale and self.output_shape:
                     human_masks = cv2.resize(human_masks, self.output_shape)
             else:
                 human_masks = None
         else:
-            for offset in instant.offsets:
-                # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
-                raise NotImplementedError("TODO: check rectangle coordinates")
-                image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
-                all_images.append(image)
+            if self.debug:
+                all_images = []
+                for offset in instant.offsets:
+                    # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
+                    raise NotImplementedError("TODO: check rectangle coordinates")
+                    image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
+                    all_images.append(image)
+            else:
+                all_images = instant.all_images
             calib = instant.calibs[c]
             human_masks = instant.human_masks[c]
 
         return View(all_images, calib, instant.annotations, rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
     def augment(self, instant_key: InstantKey, instant: Instant):
         random_state = np.random.get_state()
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/ds/instants_dataset/views_transforms.py` & `deepsport_utilities-4.9.0/deepsport_utilities/ds/instants_dataset/views_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,14 +160,28 @@
         start = top_edge[0][0][0]
         stop = top_edge[1][0][0]
         x = np.random.beta(2, 2)*(stop-start)+start
         y = np.random.beta(2, 2)*court.h/2+court.h/4
         z = 0
         return Point3D(x,y,z)
 
+    def _apply_transformation(self, view, A):
+        # rectify warp caused by projection on a plane
+        center = view.__shear_center
+        vector = Point2D(center.x - view.calib.K[0,2], center.y - view.calib.K[1,2])
+        R1 = np.eye(3)
+        R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(), np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K[0,0]))
+        T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+        S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+        R2 = np.eye(3)
+        R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+        return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
     def _get_current_parameters(self, view_key, view):
         ball = getattr(view, "ball", None)
         if ball is None:
             warning.warn("No ball annotation found, using random ball position")
 
         # If not `on_ball` use the ball anyway half of the samples
         if random.random() < self.on_ball and ball is not None:
@@ -187,14 +201,15 @@
             size = 1
         else:
             point3D = ball.center if ball is not None else keypoint
             size = float(view.calib.compute_length2D(point3D, self.true_size))
 
         keypoint = view.calib.project_3D_to_2D(keypoint)
         input_shape = view.calib.width, view.calib.height
+        view.__shear_center = keypoint
         return keypoint, size, input_shape
 
 
 class CleverViewRandomCropperTransform(BallViewRandomCropperTransform):
     def __init__(self, def_min=60, def_max=160, **kwargs):
         super().__init__(on_ball=0, def_min=def_min, def_max=def_max, **kwargs)
 
@@ -225,23 +240,51 @@
         margin = float(view.calib.compute_length2D(Point3D(np.mean(keypoints, axis=1)), self.margin))
         size = float(view.calib.compute_length2D(Point3D(np.mean(keypoints, axis=1)), 100))
         keypoints = view.calib.project_3D_to_2D(keypoints)
         input_shape = view.calib.width, view.calib.height
         return keypoints, size, input_shape
 
 class AddBallSizeFactory(Transform):
+    def __init__(self, origins=['annotation', 'interpolation']):
+        self.origins = origins
     def __call__(self, view_key, view):
         ball = view.ball
-        predicate = lambda ball: ball.origin in ['annotation', 'interpolation'] and ball.visible is not False and view.calib.projects_in(ball.center)
+        predicate = lambda ball:    ball.origin in self.origins         \
+                                and ball.visible is not False           \
+                                and view.calib.projects_in(ball.center) \
+                                and ball.center.z < -10
         return {"ball_size": view.calib.compute_length2D(ball.center, BALL_DIAMETER)[0] if predicate(ball) else np.nan}
 
+class AddBallHeightFactory(Transform):
+    """ Ball hidden are considered
+    """
+    def __call__(self, view_key, view):
+        ball = view.ball
+        predicate = lambda ball: ball.origin in ['annotation', 'interpolation'] and view.calib.projects_in(ball.center)
+        center2D = view.calib.project_3D_to_2D(ball.center)
+        ground2D = view.calib.project_3D_to_2D(Point3D(ball.center.x, ball.center.y, 0))
+        return {"ball_height": np.linalg.norm(center2D - ground2D) if predicate(ball) else np.nan}
+
+class AddIsBallTargetFactory(Transform):
+    def __call__(self, view_key: ViewKey, view: View):
+        return {"is_ball": 1 if view.ball.origin in ['annotation', 'interpolation'] else 0}
+
 class AddBallStateFactory(Transform):
+    def __init__(self, state_mapping=None):
+        self.state_mapping = state_mapping or {state: np.eye(len(BallState))[s] for s, state in enumerate(BallState)}
     def __call__(self, view_key, view):
-        predicate = lambda ball: view.calib.projects_in(ball.center) and ball.visible is not False
-        return {"ball_state": view.ball.state if predicate(view.ball) else BallState.NONE}
+        if not view.calib.projects_in(view.ball.center):
+            raise KeyError
+        if view.ball.visible is False:
+            raise KeyError
+        if view.ball.state not in self.state_mapping:
+            raise KeyError
+        #state = view.ball.state if predicate(view.ball) else BallState.NONE
+        #state = state if state in self.state_mapping else BallState.NONE
+        return {"ball_state": self.state_mapping.get(view.ball.state)}
 
 class AddBallPositionFactory(Transform):
     def __call__(self, view_key, view):
         return {"ball_position": view.ball.center}
 
 class AddBallFactory(Transform):
     def __call__(self, view_key, view):
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/transforms.py` & `deepsport_utilities-4.9.0/deepsport_utilities/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,20 +73,20 @@
                 output_shape: Tuple(int, int) final shape of image-like data.
                 size_min: (int) lower bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
                 size_max: (int) upper bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
-                max_angle: (degrees) positive and negative bounds for random
-                    rotation
+                max_angle: (int) positive and negative bounds for random
+                    rotation (in degrees)
                 do_flip: (bool) tells if random flip should be applied
-                padding: (px) amount of padding
-                margin: (px) minimum margin between keypoints and output image
-                    border
+                padding: (int) amount of padding (in pixels) in input image
+                margin: (int) minimum margin (in pixels) between keypoints and
+                    output image border
                 debug: (bool) if `True`, doesn't actually crop but display
                     debug information on image instead.
                 regenerate: (bool) if `True`, items are (deep)-copied before
                     calling `_apply_transformation`. Else, transformation can
                     occur in-place.
         """
         self.output_shape = output_shape
@@ -109,14 +109,20 @@
         size_max = size_max or self.size_max
 
         if size_min > size_max:
             raise IncompatibleCropException("Impossible to crop image with object in the given size range")
         target_size = self.random_size(size_min, size_max) if size_min and size_max else actual_size
         ratio = target_size/actual_size
         tmp_width, tmp_height = [int(x/ratio) for x in self.output_shape]
+        if tmp_width == 0 or tmp_height == 0:
+            print("actual_size", actual_size)
+            print("target_size", target_size)
+            print("tmp_width, tmp_height", tmp_width, tmp_height)
+            print("self.output_shape", self.output_shape)
+            raise
         input_width, input_height = input_shape
 
         # If target size makes the output image bigger than input image, try with a lower size
         if tmp_width >= input_width + 2*self.padding or tmp_height >= input_height + 2*self.padding:
             if not size_min or not size_max:
                 raise IncompatibleCropException("Impossible to crop image with object in the given size range")
             return self.compute(input_shape, keypoints, actual_size, size_min=target_size*1.1, size_max=size_max)
@@ -199,11 +205,11 @@
             return None
         data = {}
         for factory in self.factories:
             if factory is None:
                 continue
             try:
                 data.update(**factory(key, item))
-            except:
-                print(factory)
+            except BaseException as e:
+                print(factory, "failed", e)
                 raise
         return data
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities/utils.py` & `deepsport_utilities-4.9.0/deepsport_utilities/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,18 @@
         left  = max(-padding,           int(self.x-margin))
         right = min(max_width+padding,  int(self.x+self.w+margin))
 
         if aspect_ratio is None:
             return slice(left, right, None), slice(top, bot, None)
 
         if padding:
-            raise NotImplementedError("increase_box method doesn't support padding when aspect ratio is given")
+            try:
+                raise NotImplementedError("increase_box method doesn't support padding when aspect ratio is given")
+            except:
+                pass
 
         w = right - left
         h = bot - top
         if w/h > aspect_ratio: # box is wider
             h = int(w/aspect_ratio)
             if h > max_height: # box is too wide
                 h = max_height
```

### Comparing `deepsport_utilities-4.8.2/deepsport_utilities.egg-info/SOURCES.txt` & `deepsport_utilities-4.9.0/deepsport_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/calib.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/calib.html`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/court.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/court.html`

 * *Files 2% similar despite different names*

```diff
@@ -323,24 +323,63 @@
         pd.fill_polygon(image, self.right_board)
 
 def sort_points_clockwise(data):
     assert data.size != 0, &#34;Empty input data&#34;
     mean = np.mean(data, axis=0) # center of mass of the points
     angles = np.arctan2((data-mean)[:, 1], (data-mean)[:, 0])
     angles[angles &lt; 0] = angles[angles &lt; 0] + 2 * np.pi # Transform angles from [-pi,pi] -&gt; [0, 2*pi]
-    return data[np.argsort(angles)]</code></pre>
+    return data[np.argsort(angles)]
+
+
+def draw_ball(image, calib: Calib, center: Point3D, color=(0,0,255), cross=True, label=None, thickness=1, fontsize=10):
+    pd = ProjectiveDrawer(calib, color, thickness=thickness)
+    ground3D = Point3D(center.x, center.y, 0)
+    pd.draw_line(image, center, ground3D, lineType=cv2.LINE_AA, color=color)
+    if cross:
+        pd.draw_line(image, ground3D+Point3D(100,0,0), ground3D-Point3D(100,0,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+        pd.draw_line(image, ground3D+Point3D(0,100,0), ground3D-Point3D(0,100,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+    radius = pd.calib.compute_length2D(center, BALL_DIAMETER/2)[0]
+    x, y = pd.calib.project_3D_to_2D(center).to_int_tuple()
+
+    cv2.circle(image, (x, y), int(radius), color, 1)
+    if label is not None:
+        cv2.putText(image, label, (x, y - 10), cv2.FONT_HERSHEY_SIMPLEX, fontsize, color, 2, lineType=cv2.LINE_AA)</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 <h2 class="section-title" id="header-functions">Functions</h2>
 <dl>
+<dt id="deepsport_utilities.court.draw_ball"><code class="name flex">
+<span>def <span class="ident">draw_ball</span></span>(<span>image, calib: calib3d.calib.Calib, center: calib3d.points.Point3D, color=(0, 0, 255), cross=True, label=None, thickness=1, fontsize=10)</span>
+</code></dt>
+<dd>
+<div class="desc"></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def draw_ball(image, calib: Calib, center: Point3D, color=(0,0,255), cross=True, label=None, thickness=1, fontsize=10):
+    pd = ProjectiveDrawer(calib, color, thickness=thickness)
+    ground3D = Point3D(center.x, center.y, 0)
+    pd.draw_line(image, center, ground3D, lineType=cv2.LINE_AA, color=color)
+    if cross:
+        pd.draw_line(image, ground3D+Point3D(100,0,0), ground3D-Point3D(100,0,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+        pd.draw_line(image, ground3D+Point3D(0,100,0), ground3D-Point3D(0,100,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+    radius = pd.calib.compute_length2D(center, BALL_DIAMETER/2)[0]
+    x, y = pd.calib.project_3D_to_2D(center).to_int_tuple()
+
+    cv2.circle(image, (x, y), int(radius), color, 1)
+    if label is not None:
+        cv2.putText(image, label, (x, y - 10), cv2.FONT_HERSHEY_SIMPLEX, fontsize, color, 2, lineType=cv2.LINE_AA)</code></pre>
+</details>
+</dd>
 <dt id="deepsport_utilities.court.sort_points_clockwise"><code class="name flex">
 <span>def <span class="ident">sort_points_clockwise</span></span>(<span>data)</span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
@@ -978,14 +1017,15 @@
 <li><h3>Super-module</h3>
 <ul>
 <li><code><a title="deepsport_utilities" href="index.html">deepsport_utilities</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-functions">Functions</a></h3>
 <ul class="">
+<li><code><a title="deepsport_utilities.court.draw_ball" href="#deepsport_utilities.court.draw_ball">draw_ball</a></code></li>
 <li><code><a title="deepsport_utilities.court.sort_points_clockwise" href="#deepsport_utilities.court.sort_points_clockwise">sort_points_clockwise</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
 <h4><code><a title="deepsport_utilities.court.Court" href="#deepsport_utilities.court.Court">Court</a></code></h4>
```

#### html2text {}

```diff
@@ -417,15 +417,56 @@
     assert data.size != 0, "Empty input data"
     mean = np.mean(data, axis=0) # center of mass of the points
     angles = np.arctan2((data-mean)[:, 1], (data-mean)[:, 0])
     angles[angles < 0] = angles[angles < 0] + 2 * np.pi # Transform angles from
 [-pi,pi] -> [0, 2*pi]
     return data[np.argsort(angles)]
 
+
+def draw_ball(image, calib: Calib, center: Point3D, color=(0,0,255),
+cross=True, label=None, thickness=1, fontsize=10):
+    pd = ProjectiveDrawer(calib, color, thickness=thickness)
+    ground3D = Point3D(center.x, center.y, 0)
+    pd.draw_line(image, center, ground3D, lineType=cv2.LINE_AA, color=color)
+    if cross:
+        pd.draw_line(image, ground3D+Point3D(100,0,0), ground3D-Point3D
+(100,0,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+        pd.draw_line(image, ground3D+Point3D(0,100,0), ground3D-Point3D
+(0,100,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+    radius = pd.calib.compute_length2D(center, BALL_DIAMETER/2)[0]
+    x, y = pd.calib.project_3D_to_2D(center).to_int_tuple()
+
+    cv2.circle(image, (x, y), int(radius), color, 1)
+    if label is not None:
+        cv2.putText(image, label, (x, y - 10), cv2.FONT_HERSHEY_SIMPLEX,
+fontsize, color, 2, lineType=cv2.LINE_AA)
+
 ***** Functions *****
+  def draw_ball(image, calib:Â calib3d.calib.Calib, center:
+  Â calib3d.points.Point3D, color=(0, 0, 255), cross=True, label=None,
+  thickness=1, fontsize=10)
+        Expand source code
+      def draw_ball(image, calib: Calib, center: Point3D, color=(0,0,255),
+      cross=True, label=None, thickness=1, fontsize=10):
+          pd = ProjectiveDrawer(calib, color, thickness=thickness)
+          ground3D = Point3D(center.x, center.y, 0)
+          pd.draw_line(image, center, ground3D, lineType=cv2.LINE_AA,
+      color=color)
+          if cross:
+              pd.draw_line(image, ground3D+Point3D(100,0,0), ground3D-Point3D
+      (100,0,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+              pd.draw_line(image, ground3D+Point3D(0,100,0), ground3D-Point3D
+      (0,100,0), lineType=cv2.LINE_AA, thickness=1, color=color)
+          radius = pd.calib.compute_length2D(center, BALL_DIAMETER/2)[0]
+          x, y = pd.calib.project_3D_to_2D(center).to_int_tuple()
+
+          cv2.circle(image, (x, y), int(radius), color, 1)
+          if label is not None:
+              cv2.putText(image, label, (x, y - 10), cv2.FONT_HERSHEY_SIMPLEX,
+      fontsize, color, 2, lineType=cv2.LINE_AA)
   def sort_points_clockwise(data)
         Expand source code
       def sort_points_clockwise(data):
           assert data.size != 0, "Empty input data"
           mean = np.mean(data, axis=0) # center of mass of the points
           angles = np.arctan2((data-mean)[:, 1], (data-mean)[:, 0])
           angles[angles < 0] = angles[angles < 0] + 2 * np.pi # Transform
@@ -1035,14 +1076,15 @@
         var width :Â float
             Alias for field number 0
 
 ****** Index ******
     * **** Super-module ****
           o deepsport_utilities
     * **** Functions ****
+          o draw_ball
           o sort_points_clockwise
     * **** Classes ****
           o *** Court ***
                 # corners
                 # draw_lines
                 # draw_net
                 # draw_poles
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/dataset.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/dataset.html`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">import dataclasses
 from enum import IntFlag
 import errno
+import logging
 import os
 import random
 import shutil
 import threading
 
 import numpy as np
 
@@ -274,77 +275,86 @@
 
 #     def query_item(self, key):
 #         if self.filename:
 #             super().__init__(self.filename)
 #             self.query_item = super().query_item
 #         return super().query_item(key)
 
-
-def first(filename):
-    try:
-        with open(filename, &#34;x&#34;) as _:
-            return True
-    except FileExistsError:
-        return False
-
 class CachedPickledDataset(PickledDataset):
     def __init__(self, filename, local_scratch=&#34;&#34;):
         super().__init__(filename)
         local_scratch = local_scratch or os.environ.get(&#39;LOCALSCRATCH&#39;, &#34;&#34;)
-        self.filename = None
-        if local_scratch and local_scratch not in filename:
-            lock = os.path.join(local_scratch, f&#34;{os.path.basename(filename)}.lock&#34;)
-            if first(lock): # First process to reach this point copies the dataset
-                def f():
-                    print(f&#34;Copying dataset to local scratch: {filename} -&gt; {local_scratch}.&#34;)
-                    try:
-                        self.filename = shutil.copy(filename, local_scratch)
-                    except:
-                        try:
-                            os.remove(os.path.join(local_scratch, os.path.basename(filename)))
-                        except:
-                            pass
-                        print(&#34;Failed copying dataset.&#34;)
-                        self.query_item = super().query_item
-                    os.remove(lock)
-                self.thread = threading.Thread(target=f)
-                self.thread.start()
-                self.available = lambda: self.filename
-            else: # Other processes wait for the dataset to be copied
-                print(f&#34;Waiting for dataset to be copied to {local_scratch}/ ...&#34;)
-                self.filename = os.path.join(local_scratch, os.path.basename(filename))
-                self.available = lambda: not os.path.exists(lock)
-        else:
+        if not local_scratch or local_scratch in filename:
             self.query_item = super().query_item
+            return
+
+        self.filename = os.path.join(local_scratch, os.path.basename(filename))
+        lock = f&#34;{self.filename}.lock&#34;
+        self.available = lambda: not os.path.exists(lock)
+
+        try:
+            with open(lock, &#34;x&#34;) as _:
+                pass # First process to reach this point copies the dataset
+        except FileExistsError:
+            return
+
+        if os.path.isfile(self.filename):
+            os.remove(lock)
+            self.reload()
+            return
+
+        def function():
+            logging.info(f&#34;Copying dataset to local scratch: {filename} -&gt; &#34; \
+                f&#34;{self.filename}.&#34;)
+            try:
+                shutil.copy(filename, self.filename)
+            except:
+                try:
+                    os.remove(self.filename)
+                except:
+                    pass
+                logging.info(&#34;Failed copying dataset.&#34;)
+                self.query_item = super().query_item
+            os.remove(lock)
+        self.thread = threading.Thread(target=function, daemon=True)
+        self.thread.start()
+
+    def reload(self):
+        logging.info(f&#34;Reloading dataset from {self.filename}&#34;)
+        super().__init__(self.filename)
+        self.query_item = super().query_item
 
     def query_item(self, key):
         if self.available():
-            print(f&#34;Reloading dataset from {self.filename}&#34;)
-            super().__init__(self.filename)
-            self.query_item = super().query_item
+            self.reload()
         return super().query_item(key)
 
 
 
-def find(path, dirs=None, verbose=True):
+def find(path, dirs=None, verbose=True, fail=True):
     if os.path.isabs(path):
         if not os.path.isfile(path) and not os.path.isdir(path):
+            if not fail:
+                not verbose or print(f&#34;{path} not found&#34;)
+                return None
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
         return path
 
     dirs = dirs or [os.getcwd(), *os.getenv(&#34;DATA_PATH&#34;, &#34;&#34;).split(&#34;:&#34;)]
     for dirname in dirs:
         if dirname is None:
             continue
         tmp_path = os.path.join(dirname, path)
         if os.path.isfile(tmp_path) or os.path.isdir(tmp_path):
-            if verbose:
-                print(&#34;{} found in {}&#34;.format(path, tmp_path))
+            not verbose or print(&#34;{} found in {}&#34;.format(path, tmp_path))
             return tmp_path
 
+    if not fail:
+        not verbose or print(f&#34;{path} not found (searched in {dirs})&#34;)
+        return None
     raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
                                 &#34;{} (searched in {})&#34;.format(path, dirs))</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
@@ -362,59 +372,47 @@
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def collate_fn(items):
     return {f&#34;batch_{k}&#34;: v for k,v in batchify(items).items()}</code></pre>
 </details>
 </dd>
 <dt id="deepsport_utilities.dataset.find"><code class="name flex">
-<span>def <span class="ident">find</span></span>(<span>path, dirs=None, verbose=True)</span>
+<span>def <span class="ident">find</span></span>(<span>path, dirs=None, verbose=True, fail=True)</span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def find(path, dirs=None, verbose=True):
+<pre><code class="python">def find(path, dirs=None, verbose=True, fail=True):
     if os.path.isabs(path):
         if not os.path.isfile(path) and not os.path.isdir(path):
+            if not fail:
+                not verbose or print(f&#34;{path} not found&#34;)
+                return None
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
         return path
 
     dirs = dirs or [os.getcwd(), *os.getenv(&#34;DATA_PATH&#34;, &#34;&#34;).split(&#34;:&#34;)]
     for dirname in dirs:
         if dirname is None:
             continue
         tmp_path = os.path.join(dirname, path)
         if os.path.isfile(tmp_path) or os.path.isdir(tmp_path):
-            if verbose:
-                print(&#34;{} found in {}&#34;.format(path, tmp_path))
+            not verbose or print(&#34;{} found in {}&#34;.format(path, tmp_path))
             return tmp_path
 
+    if not fail:
+        not verbose or print(f&#34;{path} not found (searched in {dirs})&#34;)
+        return None
     raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
                                 &#34;{} (searched in {})&#34;.format(path, dirs))</code></pre>
 </details>
 </dd>
-<dt id="deepsport_utilities.dataset.first"><code class="name flex">
-<span>def <span class="ident">first</span></span>(<span>filename)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def first(filename):
-    try:
-        with open(filename, &#34;x&#34;) as _:
-            return True
-    except FileExistsError:
-        return False</code></pre>
-</details>
-</dd>
 <dt id="deepsport_utilities.dataset.split_equally"><code class="name flex">
 <span>def <span class="ident">split_equally</span></span>(<span>d, K)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>splits equally the keys of d given their values
 arguments:
 d (dict) - A dict {"label1": 30, "label2": 45, "label3": 22, &hellip; "label<N>": 14}
@@ -579,45 +577,57 @@
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class CachedPickledDataset(PickledDataset):
     def __init__(self, filename, local_scratch=&#34;&#34;):
         super().__init__(filename)
         local_scratch = local_scratch or os.environ.get(&#39;LOCALSCRATCH&#39;, &#34;&#34;)
-        self.filename = None
-        if local_scratch and local_scratch not in filename:
-            lock = os.path.join(local_scratch, f&#34;{os.path.basename(filename)}.lock&#34;)
-            if first(lock): # First process to reach this point copies the dataset
-                def f():
-                    print(f&#34;Copying dataset to local scratch: {filename} -&gt; {local_scratch}.&#34;)
-                    try:
-                        self.filename = shutil.copy(filename, local_scratch)
-                    except:
-                        try:
-                            os.remove(os.path.join(local_scratch, os.path.basename(filename)))
-                        except:
-                            pass
-                        print(&#34;Failed copying dataset.&#34;)
-                        self.query_item = super().query_item
-                    os.remove(lock)
-                self.thread = threading.Thread(target=f)
-                self.thread.start()
-                self.available = lambda: self.filename
-            else: # Other processes wait for the dataset to be copied
-                print(f&#34;Waiting for dataset to be copied to {local_scratch}/ ...&#34;)
-                self.filename = os.path.join(local_scratch, os.path.basename(filename))
-                self.available = lambda: not os.path.exists(lock)
-        else:
+        if not local_scratch or local_scratch in filename:
             self.query_item = super().query_item
+            return
+
+        self.filename = os.path.join(local_scratch, os.path.basename(filename))
+        lock = f&#34;{self.filename}.lock&#34;
+        self.available = lambda: not os.path.exists(lock)
+
+        try:
+            with open(lock, &#34;x&#34;) as _:
+                pass # First process to reach this point copies the dataset
+        except FileExistsError:
+            return
+
+        if os.path.isfile(self.filename):
+            os.remove(lock)
+            self.reload()
+            return
+
+        def function():
+            logging.info(f&#34;Copying dataset to local scratch: {filename} -&gt; &#34; \
+                f&#34;{self.filename}.&#34;)
+            try:
+                shutil.copy(filename, self.filename)
+            except:
+                try:
+                    os.remove(self.filename)
+                except:
+                    pass
+                logging.info(&#34;Failed copying dataset.&#34;)
+                self.query_item = super().query_item
+            os.remove(lock)
+        self.thread = threading.Thread(target=function, daemon=True)
+        self.thread.start()
+
+    def reload(self):
+        logging.info(f&#34;Reloading dataset from {self.filename}&#34;)
+        super().__init__(self.filename)
+        self.query_item = super().query_item
 
     def query_item(self, key):
         if self.available():
-            print(f&#34;Reloading dataset from {self.filename}&#34;)
-            super().__init__(self.filename)
-            self.query_item = super().query_item
+            self.reload()
         return super().query_item(key)</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>mlworkflow.datasets.PickledDataset</li>
 <li>mlworkflow.datasets.Dataset</li>
 </ul>
@@ -630,20 +640,33 @@
 <div class="desc"><p>Returns a tuple for one item, typically (Xi, Yi), or (Xi,)</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def query_item(self, key):
     if self.available():
-        print(f&#34;Reloading dataset from {self.filename}&#34;)
-        super().__init__(self.filename)
-        self.query_item = super().query_item
+        self.reload()
     return super().query_item(key)</code></pre>
 </details>
 </dd>
+<dt id="deepsport_utilities.dataset.CachedPickledDataset.reload"><code class="name flex">
+<span>def <span class="ident">reload</span></span>(<span>self)</span>
+</code></dt>
+<dd>
+<div class="desc"></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def reload(self):
+    logging.info(f&#34;Reloading dataset from {self.filename}&#34;)
+    super().__init__(self.filename)
+    self.query_item = super().query_item</code></pre>
+</details>
+</dd>
 </dl>
 </dd>
 <dt id="deepsport_utilities.dataset.CombinedSubset"><code class="flex name class">
 <span>class <span class="ident">CombinedSubset</span></span>
 <span>(</span><span>name, *subsets)</span>
 </code></dt>
 <dd>
@@ -1138,15 +1161,14 @@
 <li><code><a title="deepsport_utilities" href="index.html">deepsport_utilities</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-functions">Functions</a></h3>
 <ul class="">
 <li><code><a title="deepsport_utilities.dataset.collate_fn" href="#deepsport_utilities.dataset.collate_fn">collate_fn</a></code></li>
 <li><code><a title="deepsport_utilities.dataset.find" href="#deepsport_utilities.dataset.find">find</a></code></li>
-<li><code><a title="deepsport_utilities.dataset.first" href="#deepsport_utilities.dataset.first">first</a></code></li>
 <li><code><a title="deepsport_utilities.dataset.split_equally" href="#deepsport_utilities.dataset.split_equally">split_equally</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
 <h4><code><a title="deepsport_utilities.dataset.BalancedSubest" href="#deepsport_utilities.dataset.BalancedSubest">BalancedSubest</a></code></h4>
@@ -1161,14 +1183,15 @@
 <li><code><a title="deepsport_utilities.dataset.BasicDatasetSplitter.validation_pc" href="#deepsport_utilities.dataset.BasicDatasetSplitter.validation_pc">validation_pc</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.dataset.CachedPickledDataset" href="#deepsport_utilities.dataset.CachedPickledDataset">CachedPickledDataset</a></code></h4>
 <ul class="">
 <li><code><a title="deepsport_utilities.dataset.CachedPickledDataset.query_item" href="#deepsport_utilities.dataset.CachedPickledDataset.query_item">query_item</a></code></li>
+<li><code><a title="deepsport_utilities.dataset.CachedPickledDataset.reload" href="#deepsport_utilities.dataset.CachedPickledDataset.reload">reload</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.dataset.CombinedSubset" href="#deepsport_utilities.dataset.CombinedSubset">CombinedSubset</a></code></h4>
 <ul class="">
 <li><code><a title="deepsport_utilities.dataset.CombinedSubset.batches" href="#deepsport_utilities.dataset.CombinedSubset.batches">batches</a></code></li>
 </ul>
```

#### html2text {}

```diff
@@ -5,14 +5,15 @@
 
 
 ****** Module deepsport_utilities.dataset ******
     Expand source code
 import dataclasses
 from enum import IntFlag
 import errno
+import logging
 import os
 import random
 import shutil
 import threading
 
 import numpy as np
 
@@ -271,121 +272,121 @@
 
 #     def query_item(self, key):
 #         if self.filename:
 #             super().__init__(self.filename)
 #             self.query_item = super().query_item
 #         return super().query_item(key)
 
-
-def first(filename):
-    try:
-        with open(filename, "x") as _:
-            return True
-    except FileExistsError:
-        return False
-
 class CachedPickledDataset(PickledDataset):
     def __init__(self, filename, local_scratch=""):
         super().__init__(filename)
         local_scratch = local_scratch or os.environ.get('LOCALSCRATCH', "")
-        self.filename = None
-        if local_scratch and local_scratch not in filename:
-            lock = os.path.join(local_scratch, f"{os.path.basename
-(filename)}.lock")
-            if first(lock): # First process to reach this point copies the
-dataset
-                def f():
-                    print(f"Copying dataset to local scratch: {filename} ->
-{local_scratch}.")
-                    try:
-                        self.filename = shutil.copy(filename, local_scratch)
-                    except:
-                        try:
-                            os.remove(os.path.join(local_scratch,
-os.path.basename(filename)))
-                        except:
-                            pass
-                        print("Failed copying dataset.")
-                        self.query_item = super().query_item
-                    os.remove(lock)
-                self.thread = threading.Thread(target=f)
-                self.thread.start()
-                self.available = lambda: self.filename
-            else: # Other processes wait for the dataset to be copied
-                print(f"Waiting for dataset to be copied to {local_scratch}/
-...")
-                self.filename = os.path.join(local_scratch, os.path.basename
-(filename))
-                self.available = lambda: not os.path.exists(lock)
-        else:
+        if not local_scratch or local_scratch in filename:
             self.query_item = super().query_item
+            return
+
+        self.filename = os.path.join(local_scratch, os.path.basename(filename))
+        lock = f"{self.filename}.lock"
+        self.available = lambda: not os.path.exists(lock)
+
+        try:
+            with open(lock, "x") as _:
+                pass # First process to reach this point copies the dataset
+        except FileExistsError:
+            return
+
+        if os.path.isfile(self.filename):
+            os.remove(lock)
+            self.reload()
+            return
+
+        def function():
+            logging.info(f"Copying dataset to local scratch: {filename} -> " \
+                f"{self.filename}.")
+            try:
+                shutil.copy(filename, self.filename)
+            except:
+                try:
+                    os.remove(self.filename)
+                except:
+                    pass
+                logging.info("Failed copying dataset.")
+                self.query_item = super().query_item
+            os.remove(lock)
+        self.thread = threading.Thread(target=function, daemon=True)
+        self.thread.start()
+
+    def reload(self):
+        logging.info(f"Reloading dataset from {self.filename}")
+        super().__init__(self.filename)
+        self.query_item = super().query_item
 
     def query_item(self, key):
         if self.available():
-            print(f"Reloading dataset from {self.filename}")
-            super().__init__(self.filename)
-            self.query_item = super().query_item
+            self.reload()
         return super().query_item(key)
 
 
 
-def find(path, dirs=None, verbose=True):
+def find(path, dirs=None, verbose=True, fail=True):
     if os.path.isabs(path):
         if not os.path.isfile(path) and not os.path.isdir(path):
+            if not fail:
+                not verbose or print(f"{path} not found")
+                return None
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
 path)
         return path
 
     dirs = dirs or [os.getcwd(), *os.getenv("DATA_PATH", "").split(":")]
     for dirname in dirs:
         if dirname is None:
             continue
         tmp_path = os.path.join(dirname, path)
         if os.path.isfile(tmp_path) or os.path.isdir(tmp_path):
-            if verbose:
-                print("{} found in {}".format(path, tmp_path))
+            not verbose or print("{} found in {}".format(path, tmp_path))
             return tmp_path
 
+    if not fail:
+        not verbose or print(f"{path} not found (searched in {dirs})")
+        return None
     raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
                                 "{} (searched in {})".format(path, dirs))
 
 ***** Functions *****
   def collate_fn(items)
         Expand source code
       def collate_fn(items):
           return {f"batch_{k}": v for k,v in batchify(items).items()}
-  def find(path, dirs=None, verbose=True)
+  def find(path, dirs=None, verbose=True, fail=True)
         Expand source code
-      def find(path, dirs=None, verbose=True):
+      def find(path, dirs=None, verbose=True, fail=True):
           if os.path.isabs(path):
               if not os.path.isfile(path) and not os.path.isdir(path):
+                  if not fail:
+                      not verbose or print(f"{path} not found")
+                      return None
                   raise FileNotFoundError(errno.ENOENT, os.strerror
       (errno.ENOENT), path)
               return path
 
           dirs = dirs or [os.getcwd(), *os.getenv("DATA_PATH", "").split(":")]
           for dirname in dirs:
               if dirname is None:
                   continue
               tmp_path = os.path.join(dirname, path)
               if os.path.isfile(tmp_path) or os.path.isdir(tmp_path):
-                  if verbose:
-                      print("{} found in {}".format(path, tmp_path))
+                  not verbose or print("{} found in {}".format(path, tmp_path))
                   return tmp_path
 
+          if not fail:
+              not verbose or print(f"{path} not found (searched in {dirs})")
+              return None
           raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
                                       "{} (searched in {})".format(path, dirs))
-  def first(filename)
-        Expand source code
-      def first(filename):
-          try:
-              with open(filename, "x") as _:
-                  return True
-          except FileExistsError:
-              return False
   def split_equally(d, K)
       splits equally the keys of d given their values arguments: d (dict) - A
       dict {"label1": 30, "label2": 45, "label3": 22, … "label": 14} K (int) -
       The number of split to make returns: A list of 'K' lists splitting
       equally the values of 'd': e.g. [[label1, label12, label19], [label2,
       label15], [label3, label10, label11], …] where d["label1"]+d["label12"]+d
       ["label19"] ~= d["label2"]+d["label15"] ~= d["label3"]+d["label10"]+d
@@ -491,66 +492,78 @@
           model.fit(X, Y)
         Expand source code
       class CachedPickledDataset(PickledDataset):
           def __init__(self, filename, local_scratch=""):
               super().__init__(filename)
               local_scratch = local_scratch or os.environ.get('LOCALSCRATCH',
       "")
-              self.filename = None
-              if local_scratch and local_scratch not in filename:
-                  lock = os.path.join(local_scratch, f"{os.path.basename
-      (filename)}.lock")
-                  if first(lock): # First process to reach this point copies
-      the dataset
-                      def f():
-                          print(f"Copying dataset to local scratch: {filename}
-      -> {local_scratch}.")
-                          try:
-                              self.filename = shutil.copy(filename,
-      local_scratch)
-                          except:
-                              try:
-                                  os.remove(os.path.join(local_scratch,
-      os.path.basename(filename)))
-                              except:
-                                  pass
-                              print("Failed copying dataset.")
-                              self.query_item = super().query_item
-                          os.remove(lock)
-                      self.thread = threading.Thread(target=f)
-                      self.thread.start()
-                      self.available = lambda: self.filename
-                  else: # Other processes wait for the dataset to be copied
-                      print(f"Waiting for dataset to be copied to
-      {local_scratch}/ ...")
-                      self.filename = os.path.join(local_scratch,
-      os.path.basename(filename))
-                      self.available = lambda: not os.path.exists(lock)
-              else:
+              if not local_scratch or local_scratch in filename:
                   self.query_item = super().query_item
+                  return
+
+              self.filename = os.path.join(local_scratch, os.path.basename
+      (filename))
+              lock = f"{self.filename}.lock"
+              self.available = lambda: not os.path.exists(lock)
+
+              try:
+                  with open(lock, "x") as _:
+                      pass # First process to reach this point copies the
+      dataset
+              except FileExistsError:
+                  return
+
+              if os.path.isfile(self.filename):
+                  os.remove(lock)
+                  self.reload()
+                  return
+
+              def function():
+                  logging.info(f"Copying dataset to local scratch: {filename} -
+      > " \
+                      f"{self.filename}.")
+                  try:
+                      shutil.copy(filename, self.filename)
+                  except:
+                      try:
+                          os.remove(self.filename)
+                      except:
+                          pass
+                      logging.info("Failed copying dataset.")
+                      self.query_item = super().query_item
+                  os.remove(lock)
+              self.thread = threading.Thread(target=function, daemon=True)
+              self.thread.start()
+
+          def reload(self):
+              logging.info(f"Reloading dataset from {self.filename}")
+              super().__init__(self.filename)
+              self.query_item = super().query_item
 
           def query_item(self, key):
               if self.available():
-                  print(f"Reloading dataset from {self.filename}")
-                  super().__init__(self.filename)
-                  self.query_item = super().query_item
+                  self.reload()
               return super().query_item(key)
       **** Ancestors ****
           * mlworkflow.datasets.PickledDataset
           * mlworkflow.datasets.Dataset
       **** Methods ****
         def query_item(self, key)
             Returns a tuple for one item, typically (Xi, Yi), or (Xi,)
               Expand source code
             def query_item(self, key):
                 if self.available():
-                    print(f"Reloading dataset from {self.filename}")
-                    super().__init__(self.filename)
-                    self.query_item = super().query_item
+                    self.reload()
                 return super().query_item(key)
+        def reload(self)
+              Expand source code
+            def reload(self):
+                logging.info(f"Reloading dataset from {self.filename}")
+                super().__init__(self.filename)
+                self.query_item = super().query_item
   class CombinedSubset (name, *subsets)
         Expand source code
       class CombinedSubset(Subset):
           def __init__(self, name, *subsets):
               self.subsets = subsets
               self.name = name
               assert len(set(subset.type for subset in subsets)) == 1,
@@ -847,24 +860,24 @@
 
 ****** Index ******
     * **** Super-module ****
           o deepsport_utilities
     * **** Functions ****
           o collate_fn
           o find
-          o first
           o split_equally
     * **** Classes ****
           o *** BalancedSubest ***
                 # shuffled_keys
           o *** BasicDatasetSplitter ***
                 # testing_pc
                 # validation_pc
           o *** CachedPickledDataset ***
                 # query_item
+                # reload
           o *** CombinedSubset ***
                 # batches
           o *** DatasetSamplerDataset ***
                 # query_item
                 # yield_keys
           o *** FastFilteredDataset ***
                 # query_item
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/generic_dataset.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/generic_dataset.html`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/index.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/index.html`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/dataset_splitters.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/dataset_splitters.html`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         random.setstate(random_state)
         testing2_keys = None
         if additional_keys:
             if self.additional_keys_usage == &#34;testing&#34;:
                 testing_keys += additional_keys
                 self.testing_arena_labels = self.testing_arena_labels.union(additional_arena_labels)
             elif self.additional_keys_usage == &#34;training&#34;:
+                print(f&#34;WARNING: adding {len(additional_keys)} keys to the training set&#34;)
                 training_keys += additional_keys
             elif self.additional_keys_usage == &#34;validation&#34;:
                 validation_keys += additional_keys
             elif self.additional_keys_usage in [&#34;none&#34;, &#34;skip&#34;]:
                 pass
             elif self.additional_keys_usage == &#34;testing2&#34;:
                 testing2_keys = additional_keys
@@ -222,15 +223,15 @@
         ]
 
 class TestingArenaLabelsDatasetSplitter():
     def __init__(self, testing_arena_labels, validation_pc=15, repetitions=1):
         self.testing_arena_labels = testing_arena_labels
         self.validation_pc = validation_pc
         self.repetitions = repetitions
-        assert isinstance(self.testing_arena_labels, list)
+        assert isinstance(self.testing_arena_labels, (list, tuple))
 
     def __call__(self, dataset, fold=0):
         testing_keys, remaining_keys = [], []
         for key in dataset.keys:
             (remaining_keys, testing_keys)[key.arena_label in self.testing_arena_labels].append(key)
 
         # Backup random seed
@@ -248,14 +249,40 @@
         np.random.set_state(np_random_state)
 
         subsets = [
             Subset(name=&#34;training&#34;, subset_type=SubsetType.TRAIN, keys=training_keys, dataset=dataset),
             Subset(name=&#34;validation&#34;, subset_type=SubsetType.EVAL, keys=validation_keys, dataset=dataset, repetitions=self.repetitions),
             Subset(name=&#34;testing&#34;, subset_type=SubsetType.EVAL, keys=testing_keys, dataset=dataset, repetitions=self.repetitions),
         ]
+        return [s for s in subsets if len(s.keys) &gt; 0]
+
+
+
+class TestingValidationArenaLabelsDatasetSplitter():
+    def __init__(self, testing_arena_labels, validation_arena_labels):
+        assert isinstance(testing_arena_labels, (list, tuple))
+        assert isinstance(validation_arena_labels, (list, tuple))
+        self.testing_arena_labels = testing_arena_labels
+        self.validation_arena_labels = validation_arena_labels
+        assert len(set(self.testing_arena_labels).intersection(set(self.validation_arena_labels))) == 0
+
+    def __call__(self, dataset, fold=0):
+        validation_keys, testing_keys, training_keys = [], [], []
+        for key in dataset.keys:
+            if key.arena_label in self.testing_arena_labels:
+                testing_keys.append(key)
+            elif key.arena_label in self.validation_arena_labels:
+                validation_keys.append(key)
+            else:
+                training_keys.append(key)
+        subsets = [
+            Subset(name=&#34;training&#34;, subset_type=SubsetType.TRAIN, keys=training_keys, dataset=dataset),
+            Subset(name=&#34;validation&#34;, subset_type=SubsetType.EVAL, keys=validation_keys, dataset=dataset, repetitions=1),
+            Subset(name=&#34;testing&#34;, subset_type=SubsetType.EVAL, keys=testing_keys, dataset=dataset, repetitions=1),
+        ]
         return [s for s in subsets if len(s.keys) &gt; 0]</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
@@ -410,14 +437,15 @@
         random.setstate(random_state)
         testing2_keys = None
         if additional_keys:
             if self.additional_keys_usage == &#34;testing&#34;:
                 testing_keys += additional_keys
                 self.testing_arena_labels = self.testing_arena_labels.union(additional_arena_labels)
             elif self.additional_keys_usage == &#34;training&#34;:
+                print(f&#34;WARNING: adding {len(additional_keys)} keys to the training set&#34;)
                 training_keys += additional_keys
             elif self.additional_keys_usage == &#34;validation&#34;:
                 validation_keys += additional_keys
             elif self.additional_keys_usage in [&#34;none&#34;, &#34;skip&#34;]:
                 pass
             elif self.additional_keys_usage == &#34;testing2&#34;:
                 testing2_keys = additional_keys
@@ -511,14 +539,15 @@
     random.setstate(random_state)
     testing2_keys = None
     if additional_keys:
         if self.additional_keys_usage == &#34;testing&#34;:
             testing_keys += additional_keys
             self.testing_arena_labels = self.testing_arena_labels.union(additional_arena_labels)
         elif self.additional_keys_usage == &#34;training&#34;:
+            print(f&#34;WARNING: adding {len(additional_keys)} keys to the training set&#34;)
             training_keys += additional_keys
         elif self.additional_keys_usage == &#34;validation&#34;:
             validation_keys += additional_keys
         elif self.additional_keys_usage in [&#34;none&#34;, &#34;skip&#34;]:
             pass
         elif self.additional_keys_usage == &#34;testing2&#34;:
             testing2_keys = additional_keys
@@ -698,15 +727,15 @@
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class TestingArenaLabelsDatasetSplitter():
     def __init__(self, testing_arena_labels, validation_pc=15, repetitions=1):
         self.testing_arena_labels = testing_arena_labels
         self.validation_pc = validation_pc
         self.repetitions = repetitions
-        assert isinstance(self.testing_arena_labels, list)
+        assert isinstance(self.testing_arena_labels, (list, tuple))
 
     def __call__(self, dataset, fold=0):
         testing_keys, remaining_keys = [], []
         for key in dataset.keys:
             (remaining_keys, testing_keys)[key.arena_label in self.testing_arena_labels].append(key)
 
         # Backup random seed
@@ -727,14 +756,49 @@
             Subset(name=&#34;training&#34;, subset_type=SubsetType.TRAIN, keys=training_keys, dataset=dataset),
             Subset(name=&#34;validation&#34;, subset_type=SubsetType.EVAL, keys=validation_keys, dataset=dataset, repetitions=self.repetitions),
             Subset(name=&#34;testing&#34;, subset_type=SubsetType.EVAL, keys=testing_keys, dataset=dataset, repetitions=self.repetitions),
         ]
         return [s for s in subsets if len(s.keys) &gt; 0]</code></pre>
 </details>
 </dd>
+<dt id="deepsport_utilities.ds.instants_dataset.dataset_splitters.TestingValidationArenaLabelsDatasetSplitter"><code class="flex name class">
+<span>class <span class="ident">TestingValidationArenaLabelsDatasetSplitter</span></span>
+<span>(</span><span>testing_arena_labels, validation_arena_labels)</span>
+</code></dt>
+<dd>
+<div class="desc"></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">class TestingValidationArenaLabelsDatasetSplitter():
+    def __init__(self, testing_arena_labels, validation_arena_labels):
+        assert isinstance(testing_arena_labels, (list, tuple))
+        assert isinstance(validation_arena_labels, (list, tuple))
+        self.testing_arena_labels = testing_arena_labels
+        self.validation_arena_labels = validation_arena_labels
+        assert len(set(self.testing_arena_labels).intersection(set(self.validation_arena_labels))) == 0
+
+    def __call__(self, dataset, fold=0):
+        validation_keys, testing_keys, training_keys = [], [], []
+        for key in dataset.keys:
+            if key.arena_label in self.testing_arena_labels:
+                testing_keys.append(key)
+            elif key.arena_label in self.validation_arena_labels:
+                validation_keys.append(key)
+            else:
+                training_keys.append(key)
+        subsets = [
+            Subset(name=&#34;training&#34;, subset_type=SubsetType.TRAIN, keys=training_keys, dataset=dataset),
+            Subset(name=&#34;validation&#34;, subset_type=SubsetType.EVAL, keys=validation_keys, dataset=dataset, repetitions=1),
+            Subset(name=&#34;testing&#34;, subset_type=SubsetType.EVAL, keys=testing_keys, dataset=dataset, repetitions=1),
+        ]
+        return [s for s in subsets if len(s.keys) &gt; 0]</code></pre>
+</details>
+</dd>
 </dl>
 </section>
 </article>
 <nav id="sidebar">
 <h1>Index</h1>
 <div class="toc">
 <ul></ul>
@@ -792,14 +856,17 @@
 <li><code><a title="deepsport_utilities.ds.instants_dataset.dataset_splitters.SingleArenaDatasetSplitter.folds" href="#deepsport_utilities.ds.instants_dataset.dataset_splitters.SingleArenaDatasetSplitter.folds">folds</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.dataset_splitters.SingleArenaDatasetSplitter.validation_pc" href="#deepsport_utilities.ds.instants_dataset.dataset_splitters.SingleArenaDatasetSplitter.validation_pc">validation_pc</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.dataset_splitters.TestingArenaLabelsDatasetSplitter" href="#deepsport_utilities.ds.instants_dataset.dataset_splitters.TestingArenaLabelsDatasetSplitter">TestingArenaLabelsDatasetSplitter</a></code></h4>
 </li>
+<li>
+<h4><code><a title="deepsport_utilities.ds.instants_dataset.dataset_splitters.TestingValidationArenaLabelsDatasetSplitter" href="#deepsport_utilities.ds.instants_dataset.dataset_splitters.TestingValidationArenaLabelsDatasetSplitter">TestingValidationArenaLabelsDatasetSplitter</a></code></h4>
+</li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
```

#### html2text {}

```diff
@@ -65,14 +65,16 @@
         testing2_keys = None
         if additional_keys:
             if self.additional_keys_usage == "testing":
                 testing_keys += additional_keys
                 self.testing_arena_labels = self.testing_arena_labels.union
 (additional_arena_labels)
             elif self.additional_keys_usage == "training":
+                print(f"WARNING: adding {len(additional_keys)} keys to the
+training set")
                 training_keys += additional_keys
             elif self.additional_keys_usage == "validation":
                 validation_keys += additional_keys
             elif self.additional_keys_usage in ["none", "skip"]:
                 pass
             elif self.additional_keys_usage == "testing2":
                 testing2_keys = additional_keys
@@ -241,15 +243,15 @@
         ]
 
 class TestingArenaLabelsDatasetSplitter():
     def __init__(self, testing_arena_labels, validation_pc=15, repetitions=1):
         self.testing_arena_labels = testing_arena_labels
         self.validation_pc = validation_pc
         self.repetitions = repetitions
-        assert isinstance(self.testing_arena_labels, list)
+        assert isinstance(self.testing_arena_labels, (list, tuple))
 
     def __call__(self, dataset, fold=0):
         testing_keys, remaining_keys = [], []
         for key in dataset.keys:
             (remaining_keys, testing_keys)[key.arena_label in
 self.testing_arena_labels].append(key)
 
@@ -275,14 +277,44 @@
             Subset(name="validation", subset_type=SubsetType.EVAL,
 keys=validation_keys, dataset=dataset, repetitions=self.repetitions),
             Subset(name="testing", subset_type=SubsetType.EVAL,
 keys=testing_keys, dataset=dataset, repetitions=self.repetitions),
         ]
         return [s for s in subsets if len(s.keys) > 0]
 
+
+
+class TestingValidationArenaLabelsDatasetSplitter():
+    def __init__(self, testing_arena_labels, validation_arena_labels):
+        assert isinstance(testing_arena_labels, (list, tuple))
+        assert isinstance(validation_arena_labels, (list, tuple))
+        self.testing_arena_labels = testing_arena_labels
+        self.validation_arena_labels = validation_arena_labels
+        assert len(set(self.testing_arena_labels).intersection(set
+(self.validation_arena_labels))) == 0
+
+    def __call__(self, dataset, fold=0):
+        validation_keys, testing_keys, training_keys = [], [], []
+        for key in dataset.keys:
+            if key.arena_label in self.testing_arena_labels:
+                testing_keys.append(key)
+            elif key.arena_label in self.validation_arena_labels:
+                validation_keys.append(key)
+            else:
+                training_keys.append(key)
+        subsets = [
+            Subset(name="training", subset_type=SubsetType.TRAIN,
+keys=training_keys, dataset=dataset),
+            Subset(name="validation", subset_type=SubsetType.EVAL,
+keys=validation_keys, dataset=dataset, repetitions=1),
+            Subset(name="testing", subset_type=SubsetType.EVAL,
+keys=testing_keys, dataset=dataset, repetitions=1),
+        ]
+        return [s for s in subsets if len(s.keys) > 0]
+
 ***** Functions *****
   def count_keys_per_arena_label(keys)
       returns a dict of (arena_label: number of keys of that arena)
         Expand source code
       def count_keys_per_arena_label(keys):
           """returns a dict of (arena_label: number of keys of that arena)"""
           bins = {}
@@ -405,14 +437,16 @@
               testing2_keys = None
               if additional_keys:
                   if self.additional_keys_usage == "testing":
                       testing_keys += additional_keys
                       self.testing_arena_labels =
       self.testing_arena_labels.union(additional_arena_labels)
                   elif self.additional_keys_usage == "training":
+                      print(f"WARNING: adding {len(additional_keys)} keys to
+      the training set")
                       training_keys += additional_keys
                   elif self.additional_keys_usage == "validation":
                       validation_keys += additional_keys
                   elif self.additional_keys_usage in ["none", "skip"]:
                       pass
                   elif self.additional_keys_usage == "testing2":
                       testing2_keys = additional_keys
@@ -497,14 +531,16 @@
                 testing2_keys = None
                 if additional_keys:
                     if self.additional_keys_usage == "testing":
                         testing_keys += additional_keys
                         self.testing_arena_labels =
             self.testing_arena_labels.union(additional_arena_labels)
                     elif self.additional_keys_usage == "training":
+                        print(f"WARNING: adding {len(additional_keys)} keys to
+            the training set")
                         training_keys += additional_keys
                     elif self.additional_keys_usage == "validation":
                         validation_keys += additional_keys
                     elif self.additional_keys_usage in ["none", "skip"]:
                         pass
                     elif self.additional_keys_usage == "testing2":
                         testing2_keys = additional_keys
@@ -642,15 +678,15 @@
         Expand source code
       class TestingArenaLabelsDatasetSplitter():
           def __init__(self, testing_arena_labels, validation_pc=15,
       repetitions=1):
               self.testing_arena_labels = testing_arena_labels
               self.validation_pc = validation_pc
               self.repetitions = repetitions
-              assert isinstance(self.testing_arena_labels, list)
+              assert isinstance(self.testing_arena_labels, (list, tuple))
 
           def __call__(self, dataset, fold=0):
               testing_keys, remaining_keys = [], []
               for key in dataset.keys:
                   (remaining_keys, testing_keys)[key.arena_label in
       self.testing_arena_labels].append(key)
 
@@ -675,14 +711,44 @@
       keys=training_keys, dataset=dataset),
                   Subset(name="validation", subset_type=SubsetType.EVAL,
       keys=validation_keys, dataset=dataset, repetitions=self.repetitions),
                   Subset(name="testing", subset_type=SubsetType.EVAL,
       keys=testing_keys, dataset=dataset, repetitions=self.repetitions),
               ]
               return [s for s in subsets if len(s.keys) > 0]
+  class TestingValidationArenaLabelsDatasetSplitter (testing_arena_labels,
+  validation_arena_labels)
+        Expand source code
+      class TestingValidationArenaLabelsDatasetSplitter():
+          def __init__(self, testing_arena_labels, validation_arena_labels):
+              assert isinstance(testing_arena_labels, (list, tuple))
+              assert isinstance(validation_arena_labels, (list, tuple))
+              self.testing_arena_labels = testing_arena_labels
+              self.validation_arena_labels = validation_arena_labels
+              assert len(set(self.testing_arena_labels).intersection(set
+      (self.validation_arena_labels))) == 0
+
+          def __call__(self, dataset, fold=0):
+              validation_keys, testing_keys, training_keys = [], [], []
+              for key in dataset.keys:
+                  if key.arena_label in self.testing_arena_labels:
+                      testing_keys.append(key)
+                  elif key.arena_label in self.validation_arena_labels:
+                      validation_keys.append(key)
+                  else:
+                      training_keys.append(key)
+              subsets = [
+                  Subset(name="training", subset_type=SubsetType.TRAIN,
+      keys=training_keys, dataset=dataset),
+                  Subset(name="validation", subset_type=SubsetType.EVAL,
+      keys=validation_keys, dataset=dataset, repetitions=1),
+                  Subset(name="testing", subset_type=SubsetType.EVAL,
+      keys=testing_keys, dataset=dataset, repetitions=1),
+              ]
+              return [s for s in subsets if len(s.keys) > 0]
 
 ****** Index ******
     * **** Super-module ****
           o deepsport_utilities.ds.instants_dataset
     * **** Functions ****
           o count_keys_per_arena_label
           o count_keys_per_game_id
@@ -704,9 +770,10 @@
                 # eval_folds
                 # folds
           o *** SingleArenaDatasetSplitter ***
                 # additional_keys_usage
                 # folds
                 # validation_pc
           o *** TestingArenaLabelsDatasetSplitter ***
+          o *** TestingValidationArenaLabelsDatasetSplitter ***
 
 Generated by pdoc0.10.0.
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/index.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -380,20 +380,20 @@
 <p>output_shape: Tuple(int, int) final shape of image-like data.
 size_min: (int) lower bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
 size_max: (int) upper bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
-max_angle: (degrees) positive and negative bounds for random
-rotation
+max_angle: (int) positive and negative bounds for random
+rotation (in degrees)
 do_flip: (bool) tells if random flip should be applied
-padding: (px) amount of padding
-margin: (px) minimum margin between keypoints and output image
-border
+padding: (int) amount of padding (in pixels) in input image
+margin: (int) minimum margin (in pixels) between keypoints and
+output image border
 debug: (bool) if <code>True</code>, doesn't actually crop but display
 debug information on image instead.
 regenerate: (bool) if <code>True</code>, items are (deep)-copied before
 calling <code>_apply_transformation</code>. Else, transformation can
 occur in-place.</p></div>
 <details class="source">
 <summary>
@@ -449,14 +449,28 @@
         start = top_edge[0][0][0]
         stop = top_edge[1][0][0]
         x = np.random.beta(2, 2)*(stop-start)+start
         y = np.random.beta(2, 2)*court.h/2+court.h/4
         z = 0
         return Point3D(x,y,z)
 
+    def _apply_transformation(self, view, A):
+        # rectify warp caused by projection on a plane
+        center = view.__shear_center
+        vector = Point2D(center.x - view.calib.K[0,2], center.y - view.calib.K[1,2])
+        R1 = np.eye(3)
+        R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(), np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K[0,0]))
+        T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+        S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+        R2 = np.eye(3)
+        R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+        return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
     def _get_current_parameters(self, view_key, view):
         ball = getattr(view, &#34;ball&#34;, None)
         if ball is None:
             warning.warn(&#34;No ball annotation found, using random ball position&#34;)
 
         # If not `on_ball` use the ball anyway half of the samples
         if random.random() &lt; self.on_ball and ball is not None:
@@ -476,14 +490,15 @@
             size = 1
         else:
             point3D = ball.center if ball is not None else keypoint
             size = float(view.calib.compute_length2D(point3D, self.true_size))
 
         keypoint = view.calib.project_3D_to_2D(keypoint)
         input_shape = view.calib.width, view.calib.height
+        view.__shear_center = keypoint
         return keypoint, size, input_shape</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.ViewRandomCropperTransform" href="views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.ViewRandomCropperTransform">ViewRandomCropperTransform</a></li>
 <li><a title="deepsport_utilities.transforms.RandomCropperTransform" href="../../transforms.html#deepsport_utilities.transforms.RandomCropperTransform">RandomCropperTransform</a></li>
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
@@ -618,14 +633,18 @@
     &#34;&#34;&#34; random: a proportion of random views that are at least `margin` away from any created view.
     &#34;&#34;&#34;
     def __init__(self, *args, random: float=0, **kwargs):
         assert 0 &lt;= random &lt; 1, &#34;random must be in [0,1[&#34;
         super().__init__(*args, **kwargs)
         self.random = random
         self.record = {True: 0, False: 0}
+    def compute_box(self, point3D_list: list, calib: Calib):
+        if self.margin == np.inf:
+            return BoundingBox(0, 0, calib.width, calib.height)
+        return super().compute_box(point3D_list, calib)
     def __call__(self, instant_key: InstantKey, instant: Instant):
         idx = 0
         boxes = {}
         for view_description in super().__call__(instant_key, instant):
             yield view_description
             idx = view_description.index + 1
             boxes.setdefault(view_description.camera, []).append(view_description.box)
@@ -680,14 +699,32 @@
 <div class="desc"></div>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.padding"><code class="name">var <span class="ident">padding</span> : int</code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 </dl>
+<h3>Methods</h3>
+<dl>
+<dt id="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.compute_box"><code class="name flex">
+<span>def <span class="ident">compute_box</span></span>(<span>self, point3D_list: list, calib: <a title="deepsport_utilities.calib.Calib" href="../../calib.html#deepsport_utilities.calib.Calib">Calib</a>)</span>
+</code></dt>
+<dd>
+<div class="desc"></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def compute_box(self, point3D_list: list, calib: Calib):
+    if self.margin == np.inf:
+        return BoundingBox(0, 0, calib.width, calib.height)
+    return super().compute_box(point3D_list, calib)</code></pre>
+</details>
+</dd>
+</dl>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.BuildCameraViews"><code class="flex name class">
 <span>class <span class="ident">BuildCameraViews</span></span>
 <span>(</span><span>margin: float = 0, padding: int = None, margin_in_pixels: bool = False)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Builds a view for each camera (margin parameter is useless)</p></div>
@@ -1135,14 +1172,15 @@
         random.setstate(random_state)
         testing2_keys = None
         if additional_keys:
             if self.additional_keys_usage == &#34;testing&#34;:
                 testing_keys += additional_keys
                 self.testing_arena_labels = self.testing_arena_labels.union(additional_arena_labels)
             elif self.additional_keys_usage == &#34;training&#34;:
+                print(f&#34;WARNING: adding {len(additional_keys)} keys to the training set&#34;)
                 training_keys += additional_keys
             elif self.additional_keys_usage == &#34;validation&#34;:
                 validation_keys += additional_keys
             elif self.additional_keys_usage in [&#34;none&#34;, &#34;skip&#34;]:
                 pass
             elif self.additional_keys_usage == &#34;testing2&#34;:
                 testing2_keys = additional_keys
@@ -1236,14 +1274,15 @@
     random.setstate(random_state)
     testing2_keys = None
     if additional_keys:
         if self.additional_keys_usage == &#34;testing&#34;:
             testing_keys += additional_keys
             self.testing_arena_labels = self.testing_arena_labels.union(additional_arena_labels)
         elif self.additional_keys_usage == &#34;training&#34;:
+            print(f&#34;WARNING: adding {len(additional_keys)} keys to the training set&#34;)
             training_keys += additional_keys
         elif self.additional_keys_usage == &#34;validation&#34;:
             validation_keys += additional_keys
         elif self.additional_keys_usage in [&#34;none&#34;, &#34;skip&#34;]:
             pass
         elif self.additional_keys_usage == &#34;testing2&#34;:
             testing2_keys = additional_keys
@@ -1454,27 +1493,29 @@
             &#34;ball&#34;: Ball
         }
         self.annotations = [annotation_map[a[&#39;type&#39;]](a)for a in (db_item.get(&#39;annotations&#39;, []) or [])]
 
         self.image_source = db_item.get(&#34;image_source&#34;, &#34;raw&#34;)
         self.court_dim = COURT_DIM[self.rule_type]
         self.court = Court(self.rule_type)
+        self.timestamps = [self.timestamp for _ in range(self.num_cameras)]
 
     def __str__(self):
         return &#34;({}[{:5d}]@{})&#34;.format(self.arena_label, self.game_id, self.timestamp)
 
     def get_filekey(self, prefix, suffix):
         return os.path.join(self.arena_label, str(self.game_id), &#34;{}{}{}&#34;.format(prefix, self.timestamp, suffix))
 
     @cached_property
     def calibs(self):
         return [self.__load_calib(c) for c in range(self.num_cameras)]
 
     @cached_property
     def all_images(self):
+        _ = self.calibs # triggers calib loading
         all_images = {}
         for c in range(self.num_cameras):
             for idx, offset in enumerate(self.offsets):
                 if     (idx == 0) \
                     or (idx == 1 and self.download_flags &amp; DownloadFlags.WITH_FOLLOWING_IMAGE) \
                     or (self.download_flags &amp; DownloadFlags.WITH_ALL_IMAGES):
                     try:
@@ -1994,15 +2035,15 @@
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class TestingArenaLabelsDatasetSplitter():
     def __init__(self, testing_arena_labels, validation_pc=15, repetitions=1):
         self.testing_arena_labels = testing_arena_labels
         self.validation_pc = validation_pc
         self.repetitions = repetitions
-        assert isinstance(self.testing_arena_labels, list)
+        assert isinstance(self.testing_arena_labels, (list, tuple))
 
     def __call__(self, dataset, fold=0):
         testing_keys, remaining_keys = [], []
         for key in dataset.keys:
             (remaining_keys, testing_keys)[key.arena_label in self.testing_arena_labels].append(key)
 
         # Backup random seed
@@ -2228,20 +2269,20 @@
 <p>output_shape: Tuple(int, int) final shape of image-like data.
 size_min: (int) lower bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
 size_max: (int) upper bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
-max_angle: (degrees) positive and negative bounds for random
-rotation
+max_angle: (int) positive and negative bounds for random
+rotation (in degrees)
 do_flip: (bool) tells if random flip should be applied
-padding: (px) amount of padding
-margin: (px) minimum margin between keypoints and output image
-border
+padding: (int) amount of padding (in pixels) in input image
+margin: (int) minimum margin (in pixels) between keypoints and
+output image border
 debug: (bool) if <code>True</code>, doesn't actually crop but display
 debug information on image instead.
 regenerate: (bool) if <code>True</code>, items are (deep)-copied before
 calling <code>_apply_transformation</code>. Else, transformation can
 occur in-place.</p></div>
 <details class="source">
 <summary>
@@ -2282,15 +2323,15 @@
 <li><code><a title="deepsport_utilities.transforms.RandomCropperTransform.random_size" href="../../transforms.html#deepsport_utilities.transforms.RandomCropperTransform.random_size">random_size</a></code></li>
 </ul>
 </li>
 </ul>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.ViewsDataset"><code class="flex name class">
 <span>class <span class="ident">ViewsDataset</span></span>
-<span>(</span><span>instants_dataset: <a title="deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset" href="instants_dataset.html#deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset">InstantsDataset</a>, view_builder: <a title="deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder" href="views_dataset.html#deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder">ViewBuilder</a>, output_shape=None, rescale=True, crop=True)</span>
+<span>(</span><span>instants_dataset: <a title="deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset" href="instants_dataset.html#deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset">InstantsDataset</a>, view_builder: <a title="deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder" href="views_dataset.html#deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder">ViewBuilder</a>, output_shape=None, rescale=True, crop=True, debug=False)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Dataset of views built according the given ViewBuilder, extracted from the given InstantDataset.</p>
 <h2 id="arguments">Arguments</h2>
 <p>instants_dataset
 - the InstantDataset from which views are built
 view_builder
@@ -2312,58 +2353,64 @@
             instants_dataset   - the InstantDataset from which views are built
             view_builder       - the ViewBuilder dictating what type of view is to be created
             output_shape       - view aspect ratio (or exact dimension if &#39;rescale&#39; is given)
             rescale            - tells whether the view should be rescaled to output_shape size
             crop               - tells whether the original image should be cropped or a rectangle
                                  should be drawn instead (for debug purposes)
     &#34;&#34;&#34;
-    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True):
+    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
         super().__init__(instants_dataset)
         self.view_builder = view_builder
         self.output_shape = output_shape
         self.rescale = rescale
         self.crop = crop
+        self.debug = debug
 
     def _crop_view(self, view_description: ViewDescription, instant: Instant, **kwargs):
         padding = self.view_builder.padding
         c = view_description.camera
         input_height, input_width, _ = instant.images[c].shape
         aspect_ratio = self.output_shape[0]/self.output_shape[1] if self.output_shape else None
         x_slice, y_slice = view_description.box.increase_box(
             max_width=input_width,
             max_height=input_height,
             aspect_ratio=aspect_ratio,
             padding=self.view_builder.padding
         )
-        all_images = []
 
         if self.crop:
+            all_images = []
             for offset in instant.offsets:
                 index = (c,offset)
                 if index not in instant.all_images:
                     continue # that offset was not downloaded with the download flag of instants dataset
                 image = crop_padded(instant.all_images[index], x_slice, y_slice, padding)
-                if self.rescale and self.output_shape:
+                height, width, _ = image.shape
+                if self.rescale and self.output_shape and (width, height) != self.output_shape:
                     image = cv2.resize(image, self.output_shape)
                 all_images.append(image)
             calib = instant.calibs[c].crop(x_slice, y_slice) # handles negative `slice.start` positions
             if self.rescale and self.output_shape:
                 calib = calib.scale(*self.output_shape)
             if instant.download_flags &amp; DownloadFlags.WITH_HUMAN_SEGMENTATION_MASKS and instant.human_masks:
                 human_masks = crop_padded(instant.human_masks[c], x_slice, y_slice, padding)
                 if self.rescale and self.output_shape:
                     human_masks = cv2.resize(human_masks, self.output_shape)
             else:
                 human_masks = None
         else:
-            for offset in instant.offsets:
-                # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
-                raise NotImplementedError(&#34;TODO: check rectangle coordinates&#34;)
-                image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
-                all_images.append(image)
+            if self.debug:
+                all_images = []
+                for offset in instant.offsets:
+                    # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
+                    raise NotImplementedError(&#34;TODO: check rectangle coordinates&#34;)
+                    image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
+                    all_images.append(image)
+            else:
+                all_images = instant.all_images
             calib = instant.calibs[c]
             human_masks = instant.human_masks[c]
 
         return View(all_images, calib, instant.annotations, rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
     def augment(self, instant_key: InstantKey, instant: Instant):
         random_state = np.random.get_state()
@@ -2483,14 +2530,15 @@
 <li><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViews.margin_in_pixels" href="#deepsport_utilities.ds.instants_dataset.BuildBallViews.margin_in_pixels">margin_in_pixels</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViews.padding" href="#deepsport_utilities.ds.instants_dataset.BuildBallViews.padding">padding</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom" href="#deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom">BuildBallViewsWithRandom</a></code></h4>
 <ul class="">
+<li><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.compute_box" href="#deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.compute_box">compute_box</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.margin" href="#deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.margin">margin</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.margin_in_pixels" href="#deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.margin_in_pixels">margin_in_pixels</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.padding" href="#deepsport_utilities.ds.instants_dataset.BuildBallViewsWithRandom.padding">padding</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.BuildCameraViews" href="#deepsport_utilities.ds.instants_dataset.BuildCameraViews">BuildCameraViews</a></code></h4>
```

#### html2text {}

```diff
@@ -212,21 +212,22 @@
       size_min and size_max (At each call, the current keypoint size is
       returned by _get_current_parameters).
       ***** Arguments *****
       output_shape: Tuple(int, int) final shape of image-like data. size_min:
       (int) lower bound of keypoints random size. If 0 size_min and size_max
       are ignored and no random scaling is applied. size_max: (int) upper bound
       of keypoints random size. If 0 size_min and size_max are ignored and no
-      random scaling is applied. max_angle: (degrees) positive and negative
-      bounds for random rotation do_flip: (bool) tells if random flip should be
-      applied padding: (px) amount of padding margin: (px) minimum margin
-      between keypoints and output image border debug: (bool) if True, doesn't
-      actually crop but display debug information on image instead. regenerate:
-      (bool) if True, items are (deep)-copied before calling
-      _apply_transformation. Else, transformation can occur in-place.
+      random scaling is applied. max_angle: (int) positive and negative bounds
+      for random rotation (in degrees) do_flip: (bool) tells if random flip
+      should be applied padding: (int) amount of padding (in pixels) in input
+      image margin: (int) minimum margin (in pixels) between keypoints and
+      output image border debug: (bool) if True, doesn't actually crop but
+      display debug information on image instead. regenerate: (bool) if True,
+      items are (deep)-copied before calling _apply_transformation. Else,
+      transformation can occur in-place.
         Expand source code
       class BallViewRandomCropperTransform(ViewRandomCropperTransform):
           """ Create random crops with annotated balls visible in them.
               If [min_size, max_size] range is given, scale factor is chosen
       s.t. ball
               size is in the [min_size, max_size] range.
               If [def_min, def_max] range is given, scale factor is chosen s.t.
@@ -294,14 +295,32 @@
               start = top_edge[0][0][0]
               stop = top_edge[1][0][0]
               x = np.random.beta(2, 2)*(stop-start)+start
               y = np.random.beta(2, 2)*court.h/2+court.h/4
               z = 0
               return Point3D(x,y,z)
 
+          def _apply_transformation(self, view, A):
+              # rectify warp caused by projection on a plane
+              center = view.__shear_center
+              vector = Point2D(center.x - view.calib.K[0,2], center.y -
+      view.calib.K[1,2])
+              R1 = np.eye(3)
+              R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(),
+      np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+              scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K
+      [0,0]))
+              T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+              S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+              R2 = np.eye(3)
+              R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y,
+      vector.x)*180/np.pi, 1.0)
+              T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+              return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
           def _get_current_parameters(self, view_key, view):
               ball = getattr(view, "ball", None)
               if ball is None:
                   warning.warn("No ball annotation found, using random ball
       position")
 
               # If not `on_ball` use the ball anyway half of the samples
@@ -324,14 +343,15 @@
               else:
                   point3D = ball.center if ball is not None else keypoint
                   size = float(view.calib.compute_length2D(point3D,
       self.true_size))
 
               keypoint = view.calib.project_3D_to_2D(keypoint)
               input_shape = view.calib.width, view.calib.height
+              view.__shear_center = keypoint
               return keypoint, size, input_shape
       **** Ancestors ****
           * ViewRandomCropperTransform
           * RandomCropperTransform
           * Transform
       **** Subclasses ****
           * CleverViewRandomCropperTransform
@@ -411,14 +431,18 @@
       away from any created view.
           """
           def __init__(self, *args, random: float=0, **kwargs):
               assert 0 <= random < 1, "random must be in [0,1["
               super().__init__(*args, **kwargs)
               self.random = random
               self.record = {True: 0, False: 0}
+          def compute_box(self, point3D_list: list, calib: Calib):
+              if self.margin == np.inf:
+                  return BoundingBox(0, 0, calib.width, calib.height)
+              return super().compute_box(point3D_list, calib)
           def __call__(self, instant_key: InstantKey, instant: Instant):
               idx = 0
               boxes = {}
               for view_description in super().__call__(instant_key, instant):
                   yield view_description
                   idx = view_description.index + 1
                   boxes.setdefault(view_description.camera, []).append
@@ -466,14 +490,21 @@
       **** Ancestors ****
           * BuildBallViews
           * ViewBuilder
       **** Class variables ****
         var margin :Â float
         var margin_in_pixels :Â bool
         var padding :Â int
+      **** Methods ****
+        def compute_box(self, point3D_list:Â list, calib:Â Calib)
+              Expand source code
+            def compute_box(self, point3D_list: list, calib: Calib):
+                if self.margin == np.inf:
+                    return BoundingBox(0, 0, calib.width, calib.height)
+                return super().compute_box(point3D_list, calib)
   class BuildCameraViews (margin:Â floatÂ =Â 0, padding:Â intÂ =Â None,
   margin_in_pixels:Â boolÂ =Â False)
       Builds a view for each camera (margin parameter is useless)
         Expand source code
       class BuildCameraViews(ViewBuilder):
           """ Builds a view for each camera (margin parameter is useless)
           """
@@ -795,14 +826,16 @@
               testing2_keys = None
               if additional_keys:
                   if self.additional_keys_usage == "testing":
                       testing_keys += additional_keys
                       self.testing_arena_labels =
       self.testing_arena_labels.union(additional_arena_labels)
                   elif self.additional_keys_usage == "training":
+                      print(f"WARNING: adding {len(additional_keys)} keys to
+      the training set")
                       training_keys += additional_keys
                   elif self.additional_keys_usage == "validation":
                       validation_keys += additional_keys
                   elif self.additional_keys_usage in ["none", "skip"]:
                       pass
                   elif self.additional_keys_usage == "testing2":
                       testing2_keys = additional_keys
@@ -887,14 +920,16 @@
                 testing2_keys = None
                 if additional_keys:
                     if self.additional_keys_usage == "testing":
                         testing_keys += additional_keys
                         self.testing_arena_labels =
             self.testing_arena_labels.union(additional_arena_labels)
                     elif self.additional_keys_usage == "training":
+                        print(f"WARNING: adding {len(additional_keys)} keys to
+            the training set")
                         training_keys += additional_keys
                     elif self.additional_keys_usage == "validation":
                         validation_keys += additional_keys
                     elif self.additional_keys_usage in ["none", "skip"]:
                         pass
                     elif self.additional_keys_usage == "testing2":
                         testing2_keys = additional_keys
@@ -1034,14 +1069,16 @@
               }
               self.annotations = [annotation_map[a['type']](a)for a in
       (db_item.get('annotations', []) or [])]
 
               self.image_source = db_item.get("image_source", "raw")
               self.court_dim = COURT_DIM[self.rule_type]
               self.court = Court(self.rule_type)
+              self.timestamps = [self.timestamp for _ in range
+      (self.num_cameras)]
 
           def __str__(self):
               return "({}[{:5d}]@{})".format(self.arena_label, self.game_id,
       self.timestamp)
 
           def get_filekey(self, prefix, suffix):
               return os.path.join(self.arena_label, str(self.game_id), "{}{}
@@ -1049,14 +1086,15 @@
 
           @cached_property
           def calibs(self):
               return [self.__load_calib(c) for c in range(self.num_cameras)]
 
           @cached_property
           def all_images(self):
+              _ = self.calibs # triggers calib loading
               all_images = {}
               for c in range(self.num_cameras):
                   for idx, offset in enumerate(self.offsets):
                       if     (idx == 0) \
                           or (idx == 1 and self.download_flags &
       DownloadFlags.WITH_FOLLOWING_IMAGE) \
                           or (self.download_flags &
@@ -1512,15 +1550,15 @@
         Expand source code
       class TestingArenaLabelsDatasetSplitter():
           def __init__(self, testing_arena_labels, validation_pc=15,
       repetitions=1):
               self.testing_arena_labels = testing_arena_labels
               self.validation_pc = validation_pc
               self.repetitions = repetitions
-              assert isinstance(self.testing_arena_labels, list)
+              assert isinstance(self.testing_arena_labels, (list, tuple))
 
           def __call__(self, dataset, fold=0):
               testing_keys, remaining_keys = [], []
               for key in dataset.keys:
                   (remaining_keys, testing_keys)[key.arena_label in
       self.testing_arena_labels].append(key)
 
@@ -1682,21 +1720,22 @@
       size_min and size_max (At each call, the current keypoint size is
       returned by _get_current_parameters).
       ***** Arguments *****
       output_shape: Tuple(int, int) final shape of image-like data. size_min:
       (int) lower bound of keypoints random size. If 0 size_min and size_max
       are ignored and no random scaling is applied. size_max: (int) upper bound
       of keypoints random size. If 0 size_min and size_max are ignored and no
-      random scaling is applied. max_angle: (degrees) positive and negative
-      bounds for random rotation do_flip: (bool) tells if random flip should be
-      applied padding: (px) amount of padding margin: (px) minimum margin
-      between keypoints and output image border debug: (bool) if True, doesn't
-      actually crop but display debug information on image instead. regenerate:
-      (bool) if True, items are (deep)-copied before calling
-      _apply_transformation. Else, transformation can occur in-place.
+      random scaling is applied. max_angle: (int) positive and negative bounds
+      for random rotation (in degrees) do_flip: (bool) tells if random flip
+      should be applied padding: (int) amount of padding (in pixels) in input
+      image margin: (int) minimum margin (in pixels) between keypoints and
+      output image border debug: (bool) if True, doesn't actually crop but
+      display debug information on image instead. regenerate: (bool) if True,
+      items are (deep)-copied before calling _apply_transformation. Else,
+      transformation can occur in-place.
         Expand source code
       class ViewRandomCropperTransform(RandomCropperTransform):
           def _apply_transformation(self, view, A):
               if self.debug:
                   w, h = self.output_shape
                   points = Point2D(np.linalg.inv(A)@Point2D([0,0,w,w],
       [0,h,h,0]).H)
@@ -1725,15 +1764,15 @@
           * BallViewRandomCropperTransform
           * NaiveViewRandomCropperTransform
           * PlayerViewRandomCropperTransform
       **** Inherited members ****
           * RandomCropperTransform:
                 o random_size
   class ViewsDataset (instants_dataset:Â InstantsDataset, view_builder:
-  Â ViewBuilder, output_shape=None, rescale=True, crop=True)
+  Â ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False)
       Dataset of views built according the given ViewBuilder, extracted from
       the given InstantDataset.
       ***** Arguments *****
       instants_dataset - the InstantDataset from which views are built
       view_builder - the ViewBuilder dictating what type of view is to be
       created output_shape - view aspect ratio (or exact dimension if 'rescale'
       is given) rescale - tells whether the view should be rescaled to
@@ -1754,45 +1793,48 @@
       rescaled to output_shape size
                   crop               - tells whether the original image should
       be cropped or a rectangle
                                        should be drawn instead (for debug
       purposes)
           """
           def __init__(self, instants_dataset: InstantsDataset, view_builder:
-      ViewBuilder, output_shape=None, rescale=True, crop=True):
+      ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
               super().__init__(instants_dataset)
               self.view_builder = view_builder
               self.output_shape = output_shape
               self.rescale = rescale
               self.crop = crop
+              self.debug = debug
 
           def _crop_view(self, view_description: ViewDescription, instant:
       Instant, **kwargs):
               padding = self.view_builder.padding
               c = view_description.camera
               input_height, input_width, _ = instant.images[c].shape
               aspect_ratio = self.output_shape[0]/self.output_shape[1] if
       self.output_shape else None
               x_slice, y_slice = view_description.box.increase_box(
                   max_width=input_width,
                   max_height=input_height,
                   aspect_ratio=aspect_ratio,
                   padding=self.view_builder.padding
               )
-              all_images = []
 
               if self.crop:
+                  all_images = []
                   for offset in instant.offsets:
                       index = (c,offset)
                       if index not in instant.all_images:
                           continue # that offset was not downloaded with the
       download flag of instants dataset
                       image = crop_padded(instant.all_images[index], x_slice,
       y_slice, padding)
-                      if self.rescale and self.output_shape:
+                      height, width, _ = image.shape
+                      if self.rescale and self.output_shape and (width, height)
+      != self.output_shape:
                           image = cv2.resize(image, self.output_shape)
                       all_images.append(image)
                   calib = instant.calibs[c].crop(x_slice, y_slice) # handles
       negative `slice.start` positions
                   if self.rescale and self.output_shape:
                       calib = calib.scale(*self.output_shape)
                   if instant.download_flags &
@@ -1801,23 +1843,27 @@
       x_slice, y_slice, padding)
                       if self.rescale and self.output_shape:
                           human_masks = cv2.resize(human_masks,
       self.output_shape)
                   else:
                       human_masks = None
               else:
-                  for offset in instant.offsets:
-                      # the coordinates of the rectangle below are probably
+                  if self.debug:
+                      all_images = []
+                      for offset in instant.offsets:
+                          # the coordinates of the rectangle below are probably
       wrong see documentation of cv2.rectangle
-                      raise NotImplementedError("TODO: check rectangle
+                          raise NotImplementedError("TODO: check rectangle
       coordinates")
-                      image = cv2.rectangle(instant.all_images[(c, offset)],
-      (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0),
-      10)
-                      all_images.append(image)
+                          image = cv2.rectangle(instant.all_images[(c,
+      offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop),
+      (255,0,0), 10)
+                          all_images.append(image)
+                  else:
+                      all_images = instant.all_images
                   calib = instant.calibs[c]
                   human_masks = instant.human_masks[c]
 
               return View(all_images, calib, instant.annotations,
       rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
           def augment(self, instant_key: InstantKey, instant: Instant):
@@ -1882,14 +1928,15 @@
                 # random_ball_position
           o *** BayeringTransform ***
           o *** BuildBallViews ***
                 # margin
                 # margin_in_pixels
                 # padding
           o *** BuildBallViewsWithRandom ***
+                # compute_box
                 # margin
                 # margin_in_pixels
                 # padding
           o *** BuildCameraViews ***
                 # margin
                 # margin_in_pixels
                 # padding
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/instants_dataset.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/instants_dataset.html`

 * *Files 1% similar despite different names*

```diff
@@ -87,27 +87,29 @@
             &#34;ball&#34;: Ball
         }
         self.annotations = [annotation_map[a[&#39;type&#39;]](a)for a in (db_item.get(&#39;annotations&#39;, []) or [])]
 
         self.image_source = db_item.get(&#34;image_source&#34;, &#34;raw&#34;)
         self.court_dim = COURT_DIM[self.rule_type]
         self.court = Court(self.rule_type)
+        self.timestamps = [self.timestamp for _ in range(self.num_cameras)]
 
     def __str__(self):
         return &#34;({}[{:5d}]@{})&#34;.format(self.arena_label, self.game_id, self.timestamp)
 
     def get_filekey(self, prefix, suffix):
         return os.path.join(self.arena_label, str(self.game_id), &#34;{}{}{}&#34;.format(prefix, self.timestamp, suffix))
 
     @cached_property
     def calibs(self):
         return [self.__load_calib(c) for c in range(self.num_cameras)]
 
     @cached_property
     def all_images(self):
+        _ = self.calibs # triggers calib loading
         all_images = {}
         for c in range(self.num_cameras):
             for idx, offset in enumerate(self.offsets):
                 if     (idx == 0) \
                     or (idx == 1 and self.download_flags &amp; DownloadFlags.WITH_FOLLOWING_IMAGE) \
                     or (self.download_flags &amp; DownloadFlags.WITH_ALL_IMAGES):
                     try:
@@ -304,14 +306,15 @@
     def __repr__(self):
         return &#34;Ball(&#34; + &#34;,&#34;.join([
             f&#34;origin=&#39;{self.origin}&#39;, &#34; \
             f&#34;center=({self.center.x:.01f}, {self.center.y:.01f}, {self.center.z:.01f})&#34; \
         ]) + &#34;)&#34;
 
 class BallAnnotation(Ball):
+    origin = &#34;annotation&#34;
     pass # retro-compatibility
 
 
 class Player():
     def __init__(self, data):
         self.type = &#34;player&#34;
         self.origin = data.get(&#39;origin&#39;, &#34;annotation&#34;)
@@ -474,20 +477,28 @@
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class BallAnnotation(Ball):
+    origin = &#34;annotation&#34;
     pass # retro-compatibility</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.Ball" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.Ball">Ball</a></li>
 </ul>
+<h3>Class variables</h3>
+<dl>
+<dt id="deepsport_utilities.ds.instants_dataset.instants_dataset.BallAnnotation.origin"><code class="name">var <span class="ident">origin</span></code></dt>
+<dd>
+<div class="desc"></div>
+</dd>
+</dl>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.instants_dataset.BallState"><code class="flex name class">
 <span>class <span class="ident">BallState</span></span>
 <span>(</span><span>value, names=None, *, module=None, qualname=None, type=None, start=1)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>An enumeration.</p></div>
@@ -651,27 +662,29 @@
             &#34;ball&#34;: Ball
         }
         self.annotations = [annotation_map[a[&#39;type&#39;]](a)for a in (db_item.get(&#39;annotations&#39;, []) or [])]
 
         self.image_source = db_item.get(&#34;image_source&#34;, &#34;raw&#34;)
         self.court_dim = COURT_DIM[self.rule_type]
         self.court = Court(self.rule_type)
+        self.timestamps = [self.timestamp for _ in range(self.num_cameras)]
 
     def __str__(self):
         return &#34;({}[{:5d}]@{})&#34;.format(self.arena_label, self.game_id, self.timestamp)
 
     def get_filekey(self, prefix, suffix):
         return os.path.join(self.arena_label, str(self.game_id), &#34;{}{}{}&#34;.format(prefix, self.timestamp, suffix))
 
     @cached_property
     def calibs(self):
         return [self.__load_calib(c) for c in range(self.num_cameras)]
 
     @cached_property
     def all_images(self):
+        _ = self.calibs # triggers calib loading
         all_images = {}
         for c in range(self.num_cameras):
             for idx, offset in enumerate(self.offsets):
                 if     (idx == 0) \
                     or (idx == 1 and self.download_flags &amp; DownloadFlags.WITH_FOLLOWING_IMAGE) \
                     or (self.download_flags &amp; DownloadFlags.WITH_ALL_IMAGES):
                     try:
@@ -1174,14 +1187,17 @@
 <li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.Ball.to_dict" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.Ball.to_dict">to_dict</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.Ball.value" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.Ball.value">value</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.Ball.visible" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.Ball.visible">visible</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.BallAnnotation" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.BallAnnotation">BallAnnotation</a></code></h4>
+<ul class="">
+<li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.BallAnnotation.origin" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.BallAnnotation.origin">origin</a></code></li>
+</ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.BallState" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.BallState">BallState</a></code></h4>
 <ul class="">
 <li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.BallState.CONSTRAINT" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.BallState.CONSTRAINT">CONSTRAINT</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.BallState.DRIBBLING" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.BallState.DRIBBLING">DRIBBLING</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.instants_dataset.BallState.FLYING" href="#deepsport_utilities.ds.instants_dataset.instants_dataset.BallState.FLYING">FLYING</a></code></li>
```

#### html2text {}

```diff
@@ -69,14 +69,15 @@
         }
         self.annotations = [annotation_map[a['type']](a)for a in (db_item.get
 ('annotations', []) or [])]
 
         self.image_source = db_item.get("image_source", "raw")
         self.court_dim = COURT_DIM[self.rule_type]
         self.court = Court(self.rule_type)
+        self.timestamps = [self.timestamp for _ in range(self.num_cameras)]
 
     def __str__(self):
         return "({}[{:5d}]@{})".format(self.arena_label, self.game_id,
 self.timestamp)
 
     def get_filekey(self, prefix, suffix):
         return os.path.join(self.arena_label, str(self.game_id), "{}{}
@@ -84,14 +85,15 @@
 
     @cached_property
     def calibs(self):
         return [self.__load_calib(c) for c in range(self.num_cameras)]
 
     @cached_property
     def all_images(self):
+        _ = self.calibs # triggers calib loading
         all_images = {}
         for c in range(self.num_cameras):
             for idx, offset in enumerate(self.offsets):
                 if     (idx == 0) \
                     or (idx == 1 and self.download_flags &
 DownloadFlags.WITH_FOLLOWING_IMAGE) \
                     or (self.download_flags & DownloadFlags.WITH_ALL_IMAGES):
@@ -317,14 +319,15 @@
         return "Ball(" + ",".join([
             f"origin='{self.origin}', " \
             f"center=({self.center.x:.01f}, {self.center.y:.01f},
 {self.center.z:.01f})" \
         ]) + ")"
 
 class BallAnnotation(Ball):
+    origin = "annotation"
     pass # retro-compatibility
 
 
 class Player():
     def __init__(self, data):
         self.type = "player"
         self.origin = data.get('origin', "annotation")
@@ -430,17 +433,20 @@
                     "visible": self.visible,
                     "state": self.state,
                     "value": self.value
                 }
   class BallAnnotation (data)
         Expand source code
       class BallAnnotation(Ball):
+          origin = "annotation"
           pass # retro-compatibility
       **** Ancestors ****
           * Ball
+      **** Class variables ****
+        var origin
   class BallState (value, names=None, *, module=None, qualname=None, type=None,
   start=1)
       An enumeration.
         Expand source code
       class BallState(IntEnum):
           NONE = 0
           FLYING = 1
@@ -532,14 +538,16 @@
               }
               self.annotations = [annotation_map[a['type']](a)for a in
       (db_item.get('annotations', []) or [])]
 
               self.image_source = db_item.get("image_source", "raw")
               self.court_dim = COURT_DIM[self.rule_type]
               self.court = Court(self.rule_type)
+              self.timestamps = [self.timestamp for _ in range
+      (self.num_cameras)]
 
           def __str__(self):
               return "({}[{:5d}]@{})".format(self.arena_label, self.game_id,
       self.timestamp)
 
           def get_filekey(self, prefix, suffix):
               return os.path.join(self.arena_label, str(self.game_id), "{}{}
@@ -547,14 +555,15 @@
 
           @cached_property
           def calibs(self):
               return [self.__load_calib(c) for c in range(self.num_cameras)]
 
           @cached_property
           def all_images(self):
+              _ = self.calibs # triggers calib loading
               all_images = {}
               for c in range(self.num_cameras):
                   for idx, offset in enumerate(self.offsets):
                       if     (idx == 0) \
                           or (idx == 1 and self.download_flags &
       DownloadFlags.WITH_FOLLOWING_IMAGE) \
                           or (self.download_flags &
@@ -976,14 +985,15 @@
     * **** Classes ****
           o *** Ball ***
                 # state
                 # to_dict
                 # value
                 # visible
           o *** BallAnnotation ***
+                # origin
           o *** BallState ***
                 # CONSTRAINT
                 # DRIBBLING
                 # FLYING
                 # NONE
           o *** DownloadFlags ***
                 # ALL
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/instants_transforms.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/instants_transforms.html`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/views_dataset.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/views_dataset.html`

 * *Files 2% similar despite different names*

```diff
@@ -271,23 +271,26 @@
             if not instant.calibs[ball.camera].projects_in(ball.center):
                 continue
             keypoints = [ball.center]
             c = int(ball.camera)
             timestamp = getattr(instant, &#34;timestamps&#34;, [instant.timestamp]*instant.num_cameras)[c] # timestamps may be different for each camera
             yield ViewDescription(c, idx, self.compute_box(keypoints, instant.calibs[c]), ball=ball, timestamp=timestamp)
 
-
 class BuildBallViewsWithRandom(BuildBallViews):
     &#34;&#34;&#34; random: a proportion of random views that are at least `margin` away from any created view.
     &#34;&#34;&#34;
     def __init__(self, *args, random: float=0, **kwargs):
         assert 0 &lt;= random &lt; 1, &#34;random must be in [0,1[&#34;
         super().__init__(*args, **kwargs)
         self.random = random
         self.record = {True: 0, False: 0}
+    def compute_box(self, point3D_list: list, calib: Calib):
+        if self.margin == np.inf:
+            return BoundingBox(0, 0, calib.width, calib.height)
+        return super().compute_box(point3D_list, calib)
     def __call__(self, instant_key: InstantKey, instant: Instant):
         idx = 0
         boxes = {}
         for view_description in super().__call__(instant_key, instant):
             yield view_description
             idx = view_description.index + 1
             boxes.setdefault(view_description.camera, []).append(view_description.box)
@@ -322,16 +325,14 @@
             keypoints = [point3D]
             c = int(ball.camera)
             timestamp = getattr(instant, &#34;timestamps&#34;, [instant.timestamp]*instant.num_cameras)[c] # timestamps may be different for each camera
             yield ViewDescription(c, idx, self.compute_box(keypoints, instant.calibs[c]), ball=ball, timestamp=timestamp)
             idx += 1
             self.record[False] += 1
 
-
-
 class BuildHeadsViews(ViewBuilder):
     def __call__(self, instant_key: InstantKey, instant: Instant):
         for idx, player in enumerate([a for a in instant.annotations if a.type == &#34;player&#34;]):
             c = int(player.camera)
             keypoints = [player.head]
             yield ViewDescription(c, idx, self.compute_box(keypoints, instant.calibs[c]), annotation=player)
 
@@ -341,58 +342,64 @@
             instants_dataset   - the InstantDataset from which views are built
             view_builder       - the ViewBuilder dictating what type of view is to be created
             output_shape       - view aspect ratio (or exact dimension if &#39;rescale&#39; is given)
             rescale            - tells whether the view should be rescaled to output_shape size
             crop               - tells whether the original image should be cropped or a rectangle
                                  should be drawn instead (for debug purposes)
     &#34;&#34;&#34;
-    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True):
+    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
         super().__init__(instants_dataset)
         self.view_builder = view_builder
         self.output_shape = output_shape
         self.rescale = rescale
         self.crop = crop
+        self.debug = debug
 
     def _crop_view(self, view_description: ViewDescription, instant: Instant, **kwargs):
         padding = self.view_builder.padding
         c = view_description.camera
         input_height, input_width, _ = instant.images[c].shape
         aspect_ratio = self.output_shape[0]/self.output_shape[1] if self.output_shape else None
         x_slice, y_slice = view_description.box.increase_box(
             max_width=input_width,
             max_height=input_height,
             aspect_ratio=aspect_ratio,
             padding=self.view_builder.padding
         )
-        all_images = []
 
         if self.crop:
+            all_images = []
             for offset in instant.offsets:
                 index = (c,offset)
                 if index not in instant.all_images:
                     continue # that offset was not downloaded with the download flag of instants dataset
                 image = crop_padded(instant.all_images[index], x_slice, y_slice, padding)
-                if self.rescale and self.output_shape:
+                height, width, _ = image.shape
+                if self.rescale and self.output_shape and (width, height) != self.output_shape:
                     image = cv2.resize(image, self.output_shape)
                 all_images.append(image)
             calib = instant.calibs[c].crop(x_slice, y_slice) # handles negative `slice.start` positions
             if self.rescale and self.output_shape:
                 calib = calib.scale(*self.output_shape)
             if instant.download_flags &amp; DownloadFlags.WITH_HUMAN_SEGMENTATION_MASKS and instant.human_masks:
                 human_masks = crop_padded(instant.human_masks[c], x_slice, y_slice, padding)
                 if self.rescale and self.output_shape:
                     human_masks = cv2.resize(human_masks, self.output_shape)
             else:
                 human_masks = None
         else:
-            for offset in instant.offsets:
-                # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
-                raise NotImplementedError(&#34;TODO: check rectangle coordinates&#34;)
-                image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
-                all_images.append(image)
+            if self.debug:
+                all_images = []
+                for offset in instant.offsets:
+                    # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
+                    raise NotImplementedError(&#34;TODO: check rectangle coordinates&#34;)
+                    image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
+                    all_images.append(image)
+            else:
+                all_images = instant.all_images
             calib = instant.calibs[c]
             human_masks = instant.human_masks[c]
 
         return View(all_images, calib, instant.annotations, rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
     def augment(self, instant_key: InstantKey, instant: Instant):
         random_state = np.random.get_state()
@@ -590,14 +597,18 @@
     &#34;&#34;&#34; random: a proportion of random views that are at least `margin` away from any created view.
     &#34;&#34;&#34;
     def __init__(self, *args, random: float=0, **kwargs):
         assert 0 &lt;= random &lt; 1, &#34;random must be in [0,1[&#34;
         super().__init__(*args, **kwargs)
         self.random = random
         self.record = {True: 0, False: 0}
+    def compute_box(self, point3D_list: list, calib: Calib):
+        if self.margin == np.inf:
+            return BoundingBox(0, 0, calib.width, calib.height)
+        return super().compute_box(point3D_list, calib)
     def __call__(self, instant_key: InstantKey, instant: Instant):
         idx = 0
         boxes = {}
         for view_description in super().__call__(instant_key, instant):
             yield view_description
             idx = view_description.index + 1
             boxes.setdefault(view_description.camera, []).append(view_description.box)
@@ -652,14 +663,32 @@
 <div class="desc"></div>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.padding"><code class="name">var <span class="ident">padding</span> : int</code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 </dl>
+<h3>Methods</h3>
+<dl>
+<dt id="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.compute_box"><code class="name flex">
+<span>def <span class="ident">compute_box</span></span>(<span>self, point3D_list: list, calib: <a title="deepsport_utilities.calib.Calib" href="../../calib.html#deepsport_utilities.calib.Calib">Calib</a>)</span>
+</code></dt>
+<dd>
+<div class="desc"></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def compute_box(self, point3D_list: list, calib: Calib):
+    if self.margin == np.inf:
+        return BoundingBox(0, 0, calib.width, calib.height)
+    return super().compute_box(point3D_list, calib)</code></pre>
+</details>
+</dd>
+</dl>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_dataset.BuildCameraViews"><code class="flex name class">
 <span>class <span class="ident">BuildCameraViews</span></span>
 <span>(</span><span>margin: float = 0, padding: int = None, margin_in_pixels: bool = False)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Builds a view for each camera (margin parameter is useless)</p></div>
@@ -1271,15 +1300,15 @@
     return self.instant_key.timestamp</code></pre>
 </details>
 </dd>
 </dl>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_dataset.ViewsDataset"><code class="flex name class">
 <span>class <span class="ident">ViewsDataset</span></span>
-<span>(</span><span>instants_dataset: <a title="deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset" href="instants_dataset.html#deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset">InstantsDataset</a>, view_builder: <a title="deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder" href="#deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder">ViewBuilder</a>, output_shape=None, rescale=True, crop=True)</span>
+<span>(</span><span>instants_dataset: <a title="deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset" href="instants_dataset.html#deepsport_utilities.ds.instants_dataset.instants_dataset.InstantsDataset">InstantsDataset</a>, view_builder: <a title="deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder" href="#deepsport_utilities.ds.instants_dataset.views_dataset.ViewBuilder">ViewBuilder</a>, output_shape=None, rescale=True, crop=True, debug=False)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Dataset of views built according the given ViewBuilder, extracted from the given InstantDataset.</p>
 <h2 id="arguments">Arguments</h2>
 <p>instants_dataset
 - the InstantDataset from which views are built
 view_builder
@@ -1301,58 +1330,64 @@
             instants_dataset   - the InstantDataset from which views are built
             view_builder       - the ViewBuilder dictating what type of view is to be created
             output_shape       - view aspect ratio (or exact dimension if &#39;rescale&#39; is given)
             rescale            - tells whether the view should be rescaled to output_shape size
             crop               - tells whether the original image should be cropped or a rectangle
                                  should be drawn instead (for debug purposes)
     &#34;&#34;&#34;
-    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True):
+    def __init__(self, instants_dataset: InstantsDataset, view_builder: ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
         super().__init__(instants_dataset)
         self.view_builder = view_builder
         self.output_shape = output_shape
         self.rescale = rescale
         self.crop = crop
+        self.debug = debug
 
     def _crop_view(self, view_description: ViewDescription, instant: Instant, **kwargs):
         padding = self.view_builder.padding
         c = view_description.camera
         input_height, input_width, _ = instant.images[c].shape
         aspect_ratio = self.output_shape[0]/self.output_shape[1] if self.output_shape else None
         x_slice, y_slice = view_description.box.increase_box(
             max_width=input_width,
             max_height=input_height,
             aspect_ratio=aspect_ratio,
             padding=self.view_builder.padding
         )
-        all_images = []
 
         if self.crop:
+            all_images = []
             for offset in instant.offsets:
                 index = (c,offset)
                 if index not in instant.all_images:
                     continue # that offset was not downloaded with the download flag of instants dataset
                 image = crop_padded(instant.all_images[index], x_slice, y_slice, padding)
-                if self.rescale and self.output_shape:
+                height, width, _ = image.shape
+                if self.rescale and self.output_shape and (width, height) != self.output_shape:
                     image = cv2.resize(image, self.output_shape)
                 all_images.append(image)
             calib = instant.calibs[c].crop(x_slice, y_slice) # handles negative `slice.start` positions
             if self.rescale and self.output_shape:
                 calib = calib.scale(*self.output_shape)
             if instant.download_flags &amp; DownloadFlags.WITH_HUMAN_SEGMENTATION_MASKS and instant.human_masks:
                 human_masks = crop_padded(instant.human_masks[c], x_slice, y_slice, padding)
                 if self.rescale and self.output_shape:
                     human_masks = cv2.resize(human_masks, self.output_shape)
             else:
                 human_masks = None
         else:
-            for offset in instant.offsets:
-                # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
-                raise NotImplementedError(&#34;TODO: check rectangle coordinates&#34;)
-                image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
-                all_images.append(image)
+            if self.debug:
+                all_images = []
+                for offset in instant.offsets:
+                    # the coordinates of the rectangle below are probably wrong see documentation of cv2.rectangle
+                    raise NotImplementedError(&#34;TODO: check rectangle coordinates&#34;)
+                    image = cv2.rectangle(instant.all_images[(c, offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
+                    all_images.append(image)
+            else:
+                all_images = instant.all_images
             calib = instant.calibs[c]
             human_masks = instant.human_masks[c]
 
         return View(all_images, calib, instant.annotations, rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
     def augment(self, instant_key: InstantKey, instant: Instant):
         random_state = np.random.get_state()
@@ -1424,14 +1459,15 @@
 <li><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViews.margin_in_pixels" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViews.margin_in_pixels">margin_in_pixels</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViews.padding" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViews.padding">padding</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom">BuildBallViewsWithRandom</a></code></h4>
 <ul class="">
+<li><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.compute_box" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.compute_box">compute_box</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.margin" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.margin">margin</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.margin_in_pixels" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.margin_in_pixels">margin_in_pixels</a></code></li>
 <li><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.padding" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildBallViewsWithRandom.padding">padding</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_dataset.BuildCameraViews" href="#deepsport_utilities.ds.instants_dataset.views_dataset.BuildCameraViews">BuildCameraViews</a></code></h4>
```

#### html2text {}

```diff
@@ -286,24 +286,27 @@
             c = int(ball.camera)
             timestamp = getattr(instant, "timestamps",
 [instant.timestamp]*instant.num_cameras)[c] # timestamps may be different for
 each camera
             yield ViewDescription(c, idx, self.compute_box(keypoints,
 instant.calibs[c]), ball=ball, timestamp=timestamp)
 
-
 class BuildBallViewsWithRandom(BuildBallViews):
     """ random: a proportion of random views that are at least `margin` away
 from any created view.
     """
     def __init__(self, *args, random: float=0, **kwargs):
         assert 0 <= random < 1, "random must be in [0,1["
         super().__init__(*args, **kwargs)
         self.random = random
         self.record = {True: 0, False: 0}
+    def compute_box(self, point3D_list: list, calib: Calib):
+        if self.margin == np.inf:
+            return BoundingBox(0, 0, calib.width, calib.height)
+        return super().compute_box(point3D_list, calib)
     def __call__(self, instant_key: InstantKey, instant: Instant):
         idx = 0
         boxes = {}
         for view_description in super().__call__(instant_key, instant):
             yield view_description
             idx = view_description.index + 1
             boxes.setdefault(view_description.camera, []).append
@@ -344,16 +347,14 @@
 [instant.timestamp]*instant.num_cameras)[c] # timestamps may be different for
 each camera
             yield ViewDescription(c, idx, self.compute_box(keypoints,
 instant.calibs[c]), ball=ball, timestamp=timestamp)
             idx += 1
             self.record[False] += 1
 
-
-
 class BuildHeadsViews(ViewBuilder):
     def __call__(self, instant_key: InstantKey, instant: Instant):
         for idx, player in enumerate([a for a in instant.annotations if a.type
 == "player"]):
             c = int(player.camera)
             keypoints = [player.head]
             yield ViewDescription(c, idx, self.compute_box(keypoints,
@@ -371,45 +372,48 @@
             rescale            - tells whether the view should be rescaled to
 output_shape size
             crop               - tells whether the original image should be
 cropped or a rectangle
                                  should be drawn instead (for debug purposes)
     """
     def __init__(self, instants_dataset: InstantsDataset, view_builder:
-ViewBuilder, output_shape=None, rescale=True, crop=True):
+ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
         super().__init__(instants_dataset)
         self.view_builder = view_builder
         self.output_shape = output_shape
         self.rescale = rescale
         self.crop = crop
+        self.debug = debug
 
     def _crop_view(self, view_description: ViewDescription, instant: Instant,
 **kwargs):
         padding = self.view_builder.padding
         c = view_description.camera
         input_height, input_width, _ = instant.images[c].shape
         aspect_ratio = self.output_shape[0]/self.output_shape[1] if
 self.output_shape else None
         x_slice, y_slice = view_description.box.increase_box(
             max_width=input_width,
             max_height=input_height,
             aspect_ratio=aspect_ratio,
             padding=self.view_builder.padding
         )
-        all_images = []
 
         if self.crop:
+            all_images = []
             for offset in instant.offsets:
                 index = (c,offset)
                 if index not in instant.all_images:
                     continue # that offset was not downloaded with the download
 flag of instants dataset
                 image = crop_padded(instant.all_images[index], x_slice,
 y_slice, padding)
-                if self.rescale and self.output_shape:
+                height, width, _ = image.shape
+                if self.rescale and self.output_shape and (width, height) !=
+self.output_shape:
                     image = cv2.resize(image, self.output_shape)
                 all_images.append(image)
             calib = instant.calibs[c].crop(x_slice, y_slice) # handles negative
 `slice.start` positions
             if self.rescale and self.output_shape:
                 calib = calib.scale(*self.output_shape)
             if instant.download_flags &
@@ -417,21 +421,26 @@
                 human_masks = crop_padded(instant.human_masks[c], x_slice,
 y_slice, padding)
                 if self.rescale and self.output_shape:
                     human_masks = cv2.resize(human_masks, self.output_shape)
             else:
                 human_masks = None
         else:
-            for offset in instant.offsets:
-                # the coordinates of the rectangle below are probably wrong see
-documentation of cv2.rectangle
-                raise NotImplementedError("TODO: check rectangle coordinates")
-                image = cv2.rectangle(instant.all_images[(c, offset)],
+            if self.debug:
+                all_images = []
+                for offset in instant.offsets:
+                    # the coordinates of the rectangle below are probably wrong
+see documentation of cv2.rectangle
+                    raise NotImplementedError("TODO: check rectangle
+coordinates")
+                    image = cv2.rectangle(instant.all_images[(c, offset)],
 (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0), 10)
-                all_images.append(image)
+                    all_images.append(image)
+            else:
+                all_images = instant.all_images
             calib = instant.calibs[c]
             human_masks = instant.human_masks[c]
 
         return View(all_images, calib, instant.annotations,
 rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
     def augment(self, instant_key: InstantKey, instant: Instant):
@@ -585,14 +594,18 @@
       away from any created view.
           """
           def __init__(self, *args, random: float=0, **kwargs):
               assert 0 <= random < 1, "random must be in [0,1["
               super().__init__(*args, **kwargs)
               self.random = random
               self.record = {True: 0, False: 0}
+          def compute_box(self, point3D_list: list, calib: Calib):
+              if self.margin == np.inf:
+                  return BoundingBox(0, 0, calib.width, calib.height)
+              return super().compute_box(point3D_list, calib)
           def __call__(self, instant_key: InstantKey, instant: Instant):
               idx = 0
               boxes = {}
               for view_description in super().__call__(instant_key, instant):
                   yield view_description
                   idx = view_description.index + 1
                   boxes.setdefault(view_description.camera, []).append
@@ -640,14 +653,21 @@
       **** Ancestors ****
           * BuildBallViews
           * ViewBuilder
       **** Class variables ****
         var margin :Â float
         var margin_in_pixels :Â bool
         var padding :Â int
+      **** Methods ****
+        def compute_box(self, point3D_list:Â list, calib:Â Calib)
+              Expand source code
+            def compute_box(self, point3D_list: list, calib: Calib):
+                if self.margin == np.inf:
+                    return BoundingBox(0, 0, calib.width, calib.height)
+                return super().compute_box(point3D_list, calib)
   class BuildCameraViews (margin:Â floatÂ =Â 0, padding:Â intÂ =Â None,
   margin_in_pixels:Â boolÂ =Â False)
       Builds a view for each camera (margin parameter is useless)
         Expand source code
       class BuildCameraViews(ViewBuilder):
           """ Builds a view for each camera (margin parameter is useless)
           """
@@ -1074,15 +1094,15 @@
             Alias for field number 0
         var timestamp
               Expand source code
             @property
             def timestamp(self):
                 return self.instant_key.timestamp
   class ViewsDataset (instants_dataset:Â InstantsDataset, view_builder:
-  Â ViewBuilder, output_shape=None, rescale=True, crop=True)
+  Â ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False)
       Dataset of views built according the given ViewBuilder, extracted from
       the given InstantDataset.
       ***** Arguments *****
       instants_dataset - the InstantDataset from which views are built
       view_builder - the ViewBuilder dictating what type of view is to be
       created output_shape - view aspect ratio (or exact dimension if 'rescale'
       is given) rescale - tells whether the view should be rescaled to
@@ -1103,45 +1123,48 @@
       rescaled to output_shape size
                   crop               - tells whether the original image should
       be cropped or a rectangle
                                        should be drawn instead (for debug
       purposes)
           """
           def __init__(self, instants_dataset: InstantsDataset, view_builder:
-      ViewBuilder, output_shape=None, rescale=True, crop=True):
+      ViewBuilder, output_shape=None, rescale=True, crop=True, debug=False):
               super().__init__(instants_dataset)
               self.view_builder = view_builder
               self.output_shape = output_shape
               self.rescale = rescale
               self.crop = crop
+              self.debug = debug
 
           def _crop_view(self, view_description: ViewDescription, instant:
       Instant, **kwargs):
               padding = self.view_builder.padding
               c = view_description.camera
               input_height, input_width, _ = instant.images[c].shape
               aspect_ratio = self.output_shape[0]/self.output_shape[1] if
       self.output_shape else None
               x_slice, y_slice = view_description.box.increase_box(
                   max_width=input_width,
                   max_height=input_height,
                   aspect_ratio=aspect_ratio,
                   padding=self.view_builder.padding
               )
-              all_images = []
 
               if self.crop:
+                  all_images = []
                   for offset in instant.offsets:
                       index = (c,offset)
                       if index not in instant.all_images:
                           continue # that offset was not downloaded with the
       download flag of instants dataset
                       image = crop_padded(instant.all_images[index], x_slice,
       y_slice, padding)
-                      if self.rescale and self.output_shape:
+                      height, width, _ = image.shape
+                      if self.rescale and self.output_shape and (width, height)
+      != self.output_shape:
                           image = cv2.resize(image, self.output_shape)
                       all_images.append(image)
                   calib = instant.calibs[c].crop(x_slice, y_slice) # handles
       negative `slice.start` positions
                   if self.rescale and self.output_shape:
                       calib = calib.scale(*self.output_shape)
                   if instant.download_flags &
@@ -1150,23 +1173,27 @@
       x_slice, y_slice, padding)
                       if self.rescale and self.output_shape:
                           human_masks = cv2.resize(human_masks,
       self.output_shape)
                   else:
                       human_masks = None
               else:
-                  for offset in instant.offsets:
-                      # the coordinates of the rectangle below are probably
+                  if self.debug:
+                      all_images = []
+                      for offset in instant.offsets:
+                          # the coordinates of the rectangle below are probably
       wrong see documentation of cv2.rectangle
-                      raise NotImplementedError("TODO: check rectangle
+                          raise NotImplementedError("TODO: check rectangle
       coordinates")
-                      image = cv2.rectangle(instant.all_images[(c, offset)],
-      (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop), (255,0,0),
-      10)
-                      all_images.append(image)
+                          image = cv2.rectangle(instant.all_images[(c,
+      offset)], (x_slice.start, x_slice.stop), (y_slice.start, y_slice.stop),
+      (255,0,0), 10)
+                          all_images.append(image)
+                  else:
+                      all_images = instant.all_images
                   calib = instant.calibs[c]
                   human_masks = instant.human_masks[c]
 
               return View(all_images, calib, instant.annotations,
       rule_type=instant.rule_type, human_masks=human_masks, **kwargs)
 
           def augment(self, instant_key: InstantKey, instant: Instant):
@@ -1209,14 +1236,15 @@
           o get_court_keypoints
     * **** Classes ****
           o *** BuildBallViews ***
                 # margin
                 # margin_in_pixels
                 # padding
           o *** BuildBallViewsWithRandom ***
+                # compute_box
                 # margin
                 # margin_in_pixels
                 # padding
           o *** BuildCameraViews ***
                 # margin
                 # margin_in_pixels
                 # padding
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/ds/instants_dataset/views_transforms.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/ds/instants_dataset/views_transforms.html`

 * *Files 5% similar despite different names*

```diff
@@ -189,14 +189,28 @@
         start = top_edge[0][0][0]
         stop = top_edge[1][0][0]
         x = np.random.beta(2, 2)*(stop-start)+start
         y = np.random.beta(2, 2)*court.h/2+court.h/4
         z = 0
         return Point3D(x,y,z)
 
+    def _apply_transformation(self, view, A):
+        # rectify warp caused by projection on a plane
+        center = view.__shear_center
+        vector = Point2D(center.x - view.calib.K[0,2], center.y - view.calib.K[1,2])
+        R1 = np.eye(3)
+        R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(), np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K[0,0]))
+        T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+        S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+        R2 = np.eye(3)
+        R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+        return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
     def _get_current_parameters(self, view_key, view):
         ball = getattr(view, &#34;ball&#34;, None)
         if ball is None:
             warning.warn(&#34;No ball annotation found, using random ball position&#34;)
 
         # If not `on_ball` use the ball anyway half of the samples
         if random.random() &lt; self.on_ball and ball is not None:
@@ -216,14 +230,15 @@
             size = 1
         else:
             point3D = ball.center if ball is not None else keypoint
             size = float(view.calib.compute_length2D(point3D, self.true_size))
 
         keypoint = view.calib.project_3D_to_2D(keypoint)
         input_shape = view.calib.width, view.calib.height
+        view.__shear_center = keypoint
         return keypoint, size, input_shape
 
 
 class CleverViewRandomCropperTransform(BallViewRandomCropperTransform):
     def __init__(self, def_min=60, def_max=160, **kwargs):
         super().__init__(on_ball=0, def_min=def_min, def_max=def_max, **kwargs)
 
@@ -254,23 +269,51 @@
         margin = float(view.calib.compute_length2D(Point3D(np.mean(keypoints, axis=1)), self.margin))
         size = float(view.calib.compute_length2D(Point3D(np.mean(keypoints, axis=1)), 100))
         keypoints = view.calib.project_3D_to_2D(keypoints)
         input_shape = view.calib.width, view.calib.height
         return keypoints, size, input_shape
 
 class AddBallSizeFactory(Transform):
+    def __init__(self, origins=[&#39;annotation&#39;, &#39;interpolation&#39;]):
+        self.origins = origins
     def __call__(self, view_key, view):
         ball = view.ball
-        predicate = lambda ball: ball.origin in [&#39;annotation&#39;, &#39;interpolation&#39;] and ball.visible is not False and view.calib.projects_in(ball.center)
+        predicate = lambda ball:    ball.origin in self.origins         \
+                                and ball.visible is not False           \
+                                and view.calib.projects_in(ball.center) \
+                                and ball.center.z &lt; -10
         return {&#34;ball_size&#34;: view.calib.compute_length2D(ball.center, BALL_DIAMETER)[0] if predicate(ball) else np.nan}
 
+class AddBallHeightFactory(Transform):
+    &#34;&#34;&#34; Ball hidden are considered
+    &#34;&#34;&#34;
+    def __call__(self, view_key, view):
+        ball = view.ball
+        predicate = lambda ball: ball.origin in [&#39;annotation&#39;, &#39;interpolation&#39;] and view.calib.projects_in(ball.center)
+        center2D = view.calib.project_3D_to_2D(ball.center)
+        ground2D = view.calib.project_3D_to_2D(Point3D(ball.center.x, ball.center.y, 0))
+        return {&#34;ball_height&#34;: np.linalg.norm(center2D - ground2D) if predicate(ball) else np.nan}
+
+class AddIsBallTargetFactory(Transform):
+    def __call__(self, view_key: ViewKey, view: View):
+        return {&#34;is_ball&#34;: 1 if view.ball.origin in [&#39;annotation&#39;, &#39;interpolation&#39;] else 0}
+
 class AddBallStateFactory(Transform):
+    def __init__(self, state_mapping=None):
+        self.state_mapping = state_mapping or {state: np.eye(len(BallState))[s] for s, state in enumerate(BallState)}
     def __call__(self, view_key, view):
-        predicate = lambda ball: view.calib.projects_in(ball.center) and ball.visible is not False
-        return {&#34;ball_state&#34;: view.ball.state if predicate(view.ball) else BallState.NONE}
+        if not view.calib.projects_in(view.ball.center):
+            raise KeyError
+        if view.ball.visible is False:
+            raise KeyError
+        if view.ball.state not in self.state_mapping:
+            raise KeyError
+        #state = view.ball.state if predicate(view.ball) else BallState.NONE
+        #state = state if state in self.state_mapping else BallState.NONE
+        return {&#34;ball_state&#34;: self.state_mapping.get(view.ball.state)}
 
 class AddBallPositionFactory(Transform):
     def __call__(self, view_key, view):
         return {&#34;ball_position&#34;: view.ball.center}
 
 class AddBallFactory(Transform):
     def __call__(self, view_key, view):
@@ -435,14 +478,38 @@
         return {&#34;ball&#34;: view.ball}</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
 </ul>
 </dd>
+<dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallHeightFactory"><code class="flex name class">
+<span>class <span class="ident">AddBallHeightFactory</span></span>
+</code></dt>
+<dd>
+<div class="desc"><p>Ball hidden are considered</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">class AddBallHeightFactory(Transform):
+    &#34;&#34;&#34; Ball hidden are considered
+    &#34;&#34;&#34;
+    def __call__(self, view_key, view):
+        ball = view.ball
+        predicate = lambda ball: ball.origin in [&#39;annotation&#39;, &#39;interpolation&#39;] and view.calib.projects_in(ball.center)
+        center2D = view.calib.project_3D_to_2D(ball.center)
+        ground2D = view.calib.project_3D_to_2D(Point3D(ball.center.x, ball.center.y, 0))
+        return {&#34;ball_height&#34;: np.linalg.norm(center2D - ground2D) if predicate(ball) else np.nan}</code></pre>
+</details>
+<h3>Ancestors</h3>
+<ul class="hlist">
+<li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
+</ul>
+</dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallPositionFactory"><code class="flex name class">
 <span>class <span class="ident">AddBallPositionFactory</span></span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
@@ -482,45 +549,61 @@
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
 </ul>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSizeFactory"><code class="flex name class">
 <span>class <span class="ident">AddBallSizeFactory</span></span>
+<span>(</span><span>origins=['annotation', 'interpolation'])</span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class AddBallSizeFactory(Transform):
+    def __init__(self, origins=[&#39;annotation&#39;, &#39;interpolation&#39;]):
+        self.origins = origins
     def __call__(self, view_key, view):
         ball = view.ball
-        predicate = lambda ball: ball.origin in [&#39;annotation&#39;, &#39;interpolation&#39;] and ball.visible is not False and view.calib.projects_in(ball.center)
+        predicate = lambda ball:    ball.origin in self.origins         \
+                                and ball.visible is not False           \
+                                and view.calib.projects_in(ball.center) \
+                                and ball.center.z &lt; -10
         return {&#34;ball_size&#34;: view.calib.compute_length2D(ball.center, BALL_DIAMETER)[0] if predicate(ball) else np.nan}</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
 </ul>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallStateFactory"><code class="flex name class">
 <span>class <span class="ident">AddBallStateFactory</span></span>
+<span>(</span><span>state_mapping=None)</span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class AddBallStateFactory(Transform):
+    def __init__(self, state_mapping=None):
+        self.state_mapping = state_mapping or {state: np.eye(len(BallState))[s] for s, state in enumerate(BallState)}
     def __call__(self, view_key, view):
-        predicate = lambda ball: view.calib.projects_in(ball.center) and ball.visible is not False
-        return {&#34;ball_state&#34;: view.ball.state if predicate(view.ball) else BallState.NONE}</code></pre>
+        if not view.calib.projects_in(view.ball.center):
+            raise KeyError
+        if view.ball.visible is False:
+            raise KeyError
+        if view.ball.state not in self.state_mapping:
+            raise KeyError
+        #state = view.ball.state if predicate(view.ball) else BallState.NONE
+        #state = state if state in self.state_mapping else BallState.NONE
+        return {&#34;ball_state&#34;: self.state_mapping.get(view.ball.state)}</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
 </ul>
 </dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallVisibilityFactory"><code class="flex name class">
@@ -672,14 +755,32 @@
         return {&#34;input_image&#34;: view.image}</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
 </ul>
 </dd>
+<dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddIsBallTargetFactory"><code class="flex name class">
+<span>class <span class="ident">AddIsBallTargetFactory</span></span>
+</code></dt>
+<dd>
+<div class="desc"></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">class AddIsBallTargetFactory(Transform):
+    def __call__(self, view_key: ViewKey, view: View):
+        return {&#34;is_ball&#34;: 1 if view.ball.origin in [&#39;annotation&#39;, &#39;interpolation&#39;] else 0}</code></pre>
+</details>
+<h3>Ancestors</h3>
+<ul class="hlist">
+<li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
+</ul>
+</dd>
 <dt id="deepsport_utilities.ds.instants_dataset.views_transforms.AddNextImageFactory"><code class="flex name class">
 <span>class <span class="ident">AddNextImageFactory</span></span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
@@ -722,20 +823,20 @@
 <p>output_shape: Tuple(int, int) final shape of image-like data.
 size_min: (int) lower bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
 size_max: (int) upper bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
-max_angle: (degrees) positive and negative bounds for random
-rotation
+max_angle: (int) positive and negative bounds for random
+rotation (in degrees)
 do_flip: (bool) tells if random flip should be applied
-padding: (px) amount of padding
-margin: (px) minimum margin between keypoints and output image
-border
+padding: (int) amount of padding (in pixels) in input image
+margin: (int) minimum margin (in pixels) between keypoints and
+output image border
 debug: (bool) if <code>True</code>, doesn't actually crop but display
 debug information on image instead.
 regenerate: (bool) if <code>True</code>, items are (deep)-copied before
 calling <code>_apply_transformation</code>. Else, transformation can
 occur in-place.</p></div>
 <details class="source">
 <summary>
@@ -791,14 +892,28 @@
         start = top_edge[0][0][0]
         stop = top_edge[1][0][0]
         x = np.random.beta(2, 2)*(stop-start)+start
         y = np.random.beta(2, 2)*court.h/2+court.h/4
         z = 0
         return Point3D(x,y,z)
 
+    def _apply_transformation(self, view, A):
+        # rectify warp caused by projection on a plane
+        center = view.__shear_center
+        vector = Point2D(center.x - view.calib.K[0,2], center.y - view.calib.K[1,2])
+        R1 = np.eye(3)
+        R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(), np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K[0,0]))
+        T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+        S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+        R2 = np.eye(3)
+        R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+        T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+        return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
     def _get_current_parameters(self, view_key, view):
         ball = getattr(view, &#34;ball&#34;, None)
         if ball is None:
             warning.warn(&#34;No ball annotation found, using random ball position&#34;)
 
         # If not `on_ball` use the ball anyway half of the samples
         if random.random() &lt; self.on_ball and ball is not None:
@@ -818,14 +933,15 @@
             size = 1
         else:
             point3D = ball.center if ball is not None else keypoint
             size = float(view.calib.compute_length2D(point3D, self.true_size))
 
         keypoint = view.calib.project_3D_to_2D(keypoint)
         input_shape = view.calib.width, view.calib.height
+        view.__shear_center = keypoint
         return keypoint, size, input_shape</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.ViewRandomCropperTransform" href="#deepsport_utilities.ds.instants_dataset.views_transforms.ViewRandomCropperTransform">ViewRandomCropperTransform</a></li>
 <li><a title="deepsport_utilities.transforms.RandomCropperTransform" href="../../transforms.html#deepsport_utilities.transforms.RandomCropperTransform">RandomCropperTransform</a></li>
 <li><a title="deepsport_utilities.transforms.Transform" href="../../transforms.html#deepsport_utilities.transforms.Transform">Transform</a></li>
@@ -925,20 +1041,20 @@
 <p>output_shape: Tuple(int, int) final shape of image-like data.
 size_min: (int) lower bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
 size_max: (int) upper bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
-max_angle: (degrees) positive and negative bounds for random
-rotation
+max_angle: (int) positive and negative bounds for random
+rotation (in degrees)
 do_flip: (bool) tells if random flip should be applied
-padding: (px) amount of padding
-margin: (px) minimum margin between keypoints and output image
-border
+padding: (int) amount of padding (in pixels) in input image
+margin: (int) minimum margin (in pixels) between keypoints and
+output image border
 debug: (bool) if <code>True</code>, doesn't actually crop but display
 debug information on image instead.
 regenerate: (bool) if <code>True</code>, items are (deep)-copied before
 calling <code>_apply_transformation</code>. Else, transformation can
 occur in-place.</p></div>
 <details class="source">
 <summary>
@@ -1195,20 +1311,20 @@
 <p>output_shape: Tuple(int, int) final shape of image-like data.
 size_min: (int) lower bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
 size_max: (int) upper bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
-max_angle: (degrees) positive and negative bounds for random
-rotation
+max_angle: (int) positive and negative bounds for random
+rotation (in degrees)
 do_flip: (bool) tells if random flip should be applied
-padding: (px) amount of padding
-margin: (px) minimum margin between keypoints and output image
-border
+padding: (int) amount of padding (in pixels) in input image
+margin: (int) minimum margin (in pixels) between keypoints and
+output image border
 debug: (bool) if <code>True</code>, doesn't actually crop but display
 debug information on image instead.
 regenerate: (bool) if <code>True</code>, items are (deep)-copied before
 calling <code>_apply_transformation</code>. Else, transformation can
 occur in-place.</p></div>
 <details class="source">
 <summary>
@@ -1270,14 +1386,17 @@
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallAnnotation" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallAnnotation">AddBallAnnotation</a></code></h4>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallFactory">AddBallFactory</a></code></h4>
 </li>
 <li>
+<h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallHeightFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallHeightFactory">AddBallHeightFactory</a></code></h4>
+</li>
+<li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallPositionFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallPositionFactory">AddBallPositionFactory</a></code></h4>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSegmentationTargetViewFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSegmentationTargetViewFactory">AddBallSegmentationTargetViewFactory</a></code></h4>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSizeFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSizeFactory">AddBallSizeFactory</a></code></h4>
@@ -1303,14 +1422,17 @@
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddHumansSegmentationTargetViewFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddHumansSegmentationTargetViewFactory">AddHumansSegmentationTargetViewFactory</a></code></h4>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddImageFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddImageFactory">AddImageFactory</a></code></h4>
 </li>
 <li>
+<h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddIsBallTargetFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddIsBallTargetFactory">AddIsBallTargetFactory</a></code></h4>
+</li>
+<li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddNextImageFactory" href="#deepsport_utilities.ds.instants_dataset.views_transforms.AddNextImageFactory">AddNextImageFactory</a></code></h4>
 </li>
 <li>
 <h4><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.BallViewRandomCropperTransform" href="#deepsport_utilities.ds.instants_dataset.views_transforms.BallViewRandomCropperTransform">BallViewRandomCropperTransform</a></code></h4>
 <ul class="">
 <li><code><a title="deepsport_utilities.ds.instants_dataset.views_transforms.BallViewRandomCropperTransform.random_ball_position" href="#deepsport_utilities.ds.instants_dataset.views_transforms.BallViewRandomCropperTransform.random_ball_position">random_ball_position</a></code></li>
 </ul>
```

#### html2text {}

```diff
@@ -193,14 +193,31 @@
         start = top_edge[0][0][0]
         stop = top_edge[1][0][0]
         x = np.random.beta(2, 2)*(stop-start)+start
         y = np.random.beta(2, 2)*court.h/2+court.h/4
         z = 0
         return Point3D(x,y,z)
 
+    def _apply_transformation(self, view, A):
+        # rectify warp caused by projection on a plane
+        center = view.__shear_center
+        vector = Point2D(center.x - view.calib.K[0,2], center.y - view.calib.K
+[1,2])
+        R1 = np.eye(3)
+        R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(), np.arctan2
+(vector.y, vector.x)*180/np.pi, 1.0)
+        scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K[0,0]))
+        T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+        S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+        R2 = np.eye(3)
+        R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y,
+vector.x)*180/np.pi, 1.0)
+        T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+        return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
     def _get_current_parameters(self, view_key, view):
         ball = getattr(view, "ball", None)
         if ball is None:
             warning.warn("No ball annotation found, using random ball
 position")
 
         # If not `on_ball` use the ball anyway half of the samples
@@ -222,14 +239,15 @@
             size = 1
         else:
             point3D = ball.center if ball is not None else keypoint
             size = float(view.calib.compute_length2D(point3D, self.true_size))
 
         keypoint = view.calib.project_3D_to_2D(keypoint)
         input_shape = view.calib.width, view.calib.height
+        view.__shear_center = keypoint
         return keypoint, size, input_shape
 
 
 class CleverViewRandomCropperTransform(BallViewRandomCropperTransform):
     def __init__(self, def_min=60, def_max=160, **kwargs):
         super().__init__(on_ball=0, def_min=def_min, def_max=def_max, **kwargs)
 
@@ -267,27 +285,57 @@
         size = float(view.calib.compute_length2D(Point3D(np.mean(keypoints,
 axis=1)), 100))
         keypoints = view.calib.project_3D_to_2D(keypoints)
         input_shape = view.calib.width, view.calib.height
         return keypoints, size, input_shape
 
 class AddBallSizeFactory(Transform):
+    def __init__(self, origins=['annotation', 'interpolation']):
+        self.origins = origins
     def __call__(self, view_key, view):
         ball = view.ball
-        predicate = lambda ball: ball.origin in ['annotation', 'interpolation']
-and ball.visible is not False and view.calib.projects_in(ball.center)
+        predicate = lambda ball:    ball.origin in self.origins         \
+                                and ball.visible is not False           \
+                                and view.calib.projects_in(ball.center) \
+                                and ball.center.z < -10
         return {"ball_size": view.calib.compute_length2D(ball.center,
 BALL_DIAMETER)[0] if predicate(ball) else np.nan}
 
-class AddBallStateFactory(Transform):
+class AddBallHeightFactory(Transform):
+    """ Ball hidden are considered
+    """
     def __call__(self, view_key, view):
-        predicate = lambda ball: view.calib.projects_in(ball.center) and
-ball.visible is not False
-        return {"ball_state": view.ball.state if predicate(view.ball) else
-BallState.NONE}
+        ball = view.ball
+        predicate = lambda ball: ball.origin in ['annotation', 'interpolation']
+and view.calib.projects_in(ball.center)
+        center2D = view.calib.project_3D_to_2D(ball.center)
+        ground2D = view.calib.project_3D_to_2D(Point3D(ball.center.x,
+ball.center.y, 0))
+        return {"ball_height": np.linalg.norm(center2D - ground2D) if predicate
+(ball) else np.nan}
+
+class AddIsBallTargetFactory(Transform):
+    def __call__(self, view_key: ViewKey, view: View):
+        return {"is_ball": 1 if view.ball.origin in ['annotation',
+'interpolation'] else 0}
+
+class AddBallStateFactory(Transform):
+    def __init__(self, state_mapping=None):
+        self.state_mapping = state_mapping or {state: np.eye(len(BallState))[s]
+for s, state in enumerate(BallState)}
+    def __call__(self, view_key, view):
+        if not view.calib.projects_in(view.ball.center):
+            raise KeyError
+        if view.ball.visible is False:
+            raise KeyError
+        if view.ball.state not in self.state_mapping:
+            raise KeyError
+        #state = view.ball.state if predicate(view.ball) else BallState.NONE
+        #state = state if state in self.state_mapping else BallState.NONE
+        return {"ball_state": self.state_mapping.get(view.ball.state)}
 
 class AddBallPositionFactory(Transform):
     def __call__(self, view_key, view):
         return {"ball_position": view.ball.center}
 
 class AddBallFactory(Transform):
     def __call__(self, view_key, view):
@@ -432,14 +480,31 @@
   class AddBallFactory
         Expand source code
       class AddBallFactory(Transform):
           def __call__(self, view_key, view):
               return {"ball": view.ball}
       **** Ancestors ****
           * Transform
+  class AddBallHeightFactory
+      Ball hidden are considered
+        Expand source code
+      class AddBallHeightFactory(Transform):
+          """ Ball hidden are considered
+          """
+          def __call__(self, view_key, view):
+              ball = view.ball
+              predicate = lambda ball: ball.origin in ['annotation',
+      'interpolation'] and view.calib.projects_in(ball.center)
+              center2D = view.calib.project_3D_to_2D(ball.center)
+              ground2D = view.calib.project_3D_to_2D(Point3D(ball.center.x,
+      ball.center.y, 0))
+              return {"ball_height": np.linalg.norm(center2D - ground2D) if
+      predicate(ball) else np.nan}
+      **** Ancestors ****
+          * Transform
   class AddBallPositionFactory
         Expand source code
       class AddBallPositionFactory(Transform):
           def __call__(self, view_key, view):
               return {"ball_position": view.ball.center}
       **** Ancestors ****
           * Transform
@@ -458,34 +523,46 @@
                   target[skimage.draw.disk(center.flatten()[::-1], radius=float
       (diameter/2), shape=target.shape)] = 1
               return {
                   "target": target
               }
       **** Ancestors ****
           * Transform
-  class AddBallSizeFactory
+  class AddBallSizeFactory (origins=['annotation', 'interpolation'])
         Expand source code
       class AddBallSizeFactory(Transform):
+          def __init__(self, origins=['annotation', 'interpolation']):
+              self.origins = origins
           def __call__(self, view_key, view):
               ball = view.ball
-              predicate = lambda ball: ball.origin in ['annotation',
-      'interpolation'] and ball.visible is not False and view.calib.projects_in
-      (ball.center)
+              predicate = lambda ball:    ball.origin in self.origins         \
+                                      and ball.visible is not False           \
+                                      and view.calib.projects_in(ball.center) \
+                                      and ball.center.z < -10
               return {"ball_size": view.calib.compute_length2D(ball.center,
       BALL_DIAMETER)[0] if predicate(ball) else np.nan}
       **** Ancestors ****
           * Transform
-  class AddBallStateFactory
+  class AddBallStateFactory (state_mapping=None)
         Expand source code
       class AddBallStateFactory(Transform):
-          def __call__(self, view_key, view):
-              predicate = lambda ball: view.calib.projects_in(ball.center) and
-      ball.visible is not False
-              return {"ball_state": view.ball.state if predicate(view.ball)
-      else BallState.NONE}
+          def __init__(self, state_mapping=None):
+              self.state_mapping = state_mapping or {state: np.eye(len
+      (BallState))[s] for s, state in enumerate(BallState)}
+          def __call__(self, view_key, view):
+              if not view.calib.projects_in(view.ball.center):
+                  raise KeyError
+              if view.ball.visible is False:
+                  raise KeyError
+              if view.ball.state not in self.state_mapping:
+                  raise KeyError
+              #state = view.ball.state if predicate(view.ball) else
+      BallState.NONE
+              #state = state if state in self.state_mapping else BallState.NONE
+              return {"ball_state": self.state_mapping.get(view.ball.state)}
       **** Ancestors ****
           * Transform
   class AddBallVisibilityFactory
         Expand source code
       class AddBallVisibilityFactory(Transform):
           def __call__(self, view_key, view):
               return {"ball_visible": view.ball.visible}
@@ -556,14 +633,22 @@
   class AddImageFactory
         Expand source code
       class AddImageFactory(Transform):
           def __call__(self, view_key, view):
               return {"input_image": view.image}
       **** Ancestors ****
           * Transform
+  class AddIsBallTargetFactory
+        Expand source code
+      class AddIsBallTargetFactory(Transform):
+          def __call__(self, view_key: ViewKey, view: View):
+              return {"is_ball": 1 if view.ball.origin in ['annotation',
+      'interpolation'] else 0}
+      **** Ancestors ****
+          * Transform
   class AddNextImageFactory
         Expand source code
       class AddNextImageFactory(Transform):
           def __call__(self, view_key, view):
               return {"input_image2": view.all_images[1]}
       **** Ancestors ****
           * Transform
@@ -589,21 +674,22 @@
       size_min and size_max (At each call, the current keypoint size is
       returned by _get_current_parameters).
       ***** Arguments *****
       output_shape: Tuple(int, int) final shape of image-like data. size_min:
       (int) lower bound of keypoints random size. If 0 size_min and size_max
       are ignored and no random scaling is applied. size_max: (int) upper bound
       of keypoints random size. If 0 size_min and size_max are ignored and no
-      random scaling is applied. max_angle: (degrees) positive and negative
-      bounds for random rotation do_flip: (bool) tells if random flip should be
-      applied padding: (px) amount of padding margin: (px) minimum margin
-      between keypoints and output image border debug: (bool) if True, doesn't
-      actually crop but display debug information on image instead. regenerate:
-      (bool) if True, items are (deep)-copied before calling
-      _apply_transformation. Else, transformation can occur in-place.
+      random scaling is applied. max_angle: (int) positive and negative bounds
+      for random rotation (in degrees) do_flip: (bool) tells if random flip
+      should be applied padding: (int) amount of padding (in pixels) in input
+      image margin: (int) minimum margin (in pixels) between keypoints and
+      output image border debug: (bool) if True, doesn't actually crop but
+      display debug information on image instead. regenerate: (bool) if True,
+      items are (deep)-copied before calling _apply_transformation. Else,
+      transformation can occur in-place.
         Expand source code
       class BallViewRandomCropperTransform(ViewRandomCropperTransform):
           """ Create random crops with annotated balls visible in them.
               If [min_size, max_size] range is given, scale factor is chosen
       s.t. ball
               size is in the [min_size, max_size] range.
               If [def_min, def_max] range is given, scale factor is chosen s.t.
@@ -671,14 +757,32 @@
               start = top_edge[0][0][0]
               stop = top_edge[1][0][0]
               x = np.random.beta(2, 2)*(stop-start)+start
               y = np.random.beta(2, 2)*court.h/2+court.h/4
               z = 0
               return Point3D(x,y,z)
 
+          def _apply_transformation(self, view, A):
+              # rectify warp caused by projection on a plane
+              center = view.__shear_center
+              vector = Point2D(center.x - view.calib.K[0,2], center.y -
+      view.calib.K[1,2])
+              R1 = np.eye(3)
+              R1[0:2,:] = cv2.getRotationMatrix2D(center.to_int_tuple(),
+      np.arctan2(vector.y, vector.x)*180/np.pi, 1.0)
+              scale = np.cos(np.arctan(np.linalg.norm(vector)/view.calib.K
+      [0,0]))
+              T1 = np.array([[1, 0, -center.x], [0, 1, -center.y], [0, 0, 1]])
+              S = np.array([[scale, 0, 0], [0, 1, 0], [0, 0, 1]])
+              R2 = np.eye(3)
+              R2[0:2,:] = cv2.getRotationMatrix2D((0, 0), -np.arctan2(vector.y,
+      vector.x)*180/np.pi, 1.0)
+              T2 = np.array([[1, 0,  center.x], [0, 1,  center.y], [0, 0, 1]])
+              return super()._apply_transformation(view, A@T2@R2@S@T1@R1)
+
           def _get_current_parameters(self, view_key, view):
               ball = getattr(view, "ball", None)
               if ball is None:
                   warning.warn("No ball annotation found, using random ball
       position")
 
               # If not `on_ball` use the ball anyway half of the samples
@@ -701,14 +805,15 @@
               else:
                   point3D = ball.center if ball is not None else keypoint
                   size = float(view.calib.compute_length2D(point3D,
       self.true_size))
 
               keypoint = view.calib.project_3D_to_2D(keypoint)
               input_shape = view.calib.width, view.calib.height
+              view.__shear_center = keypoint
               return keypoint, size, input_shape
       **** Ancestors ****
           * ViewRandomCropperTransform
           * RandomCropperTransform
           * Transform
       **** Subclasses ****
           * CleverViewRandomCropperTransform
@@ -769,21 +874,22 @@
       size_min and size_max (At each call, the current keypoint size is
       returned by _get_current_parameters).
       ***** Arguments *****
       output_shape: Tuple(int, int) final shape of image-like data. size_min:
       (int) lower bound of keypoints random size. If 0 size_min and size_max
       are ignored and no random scaling is applied. size_max: (int) upper bound
       of keypoints random size. If 0 size_min and size_max are ignored and no
-      random scaling is applied. max_angle: (degrees) positive and negative
-      bounds for random rotation do_flip: (bool) tells if random flip should be
-      applied padding: (px) amount of padding margin: (px) minimum margin
-      between keypoints and output image border debug: (bool) if True, doesn't
-      actually crop but display debug information on image instead. regenerate:
-      (bool) if True, items are (deep)-copied before calling
-      _apply_transformation. Else, transformation can occur in-place.
+      random scaling is applied. max_angle: (int) positive and negative bounds
+      for random rotation (in degrees) do_flip: (bool) tells if random flip
+      should be applied padding: (int) amount of padding (in pixels) in input
+      image margin: (int) minimum margin (in pixels) between keypoints and
+      output image border debug: (bool) if True, doesn't actually crop but
+      display debug information on image instead. regenerate: (bool) if True,
+      items are (deep)-copied before calling _apply_transformation. Else,
+      transformation can occur in-place.
         Expand source code
       class CleverViewRandomCropperTransform(BallViewRandomCropperTransform):
           def __init__(self, def_min=60, def_max=160, **kwargs):
               super().__init__(on_ball=0, def_min=def_min, def_max=def_max,
       **kwargs)
       **** Ancestors ****
           * BallViewRandomCropperTransform
@@ -945,21 +1051,22 @@
       size_min and size_max (At each call, the current keypoint size is
       returned by _get_current_parameters).
       ***** Arguments *****
       output_shape: Tuple(int, int) final shape of image-like data. size_min:
       (int) lower bound of keypoints random size. If 0 size_min and size_max
       are ignored and no random scaling is applied. size_max: (int) upper bound
       of keypoints random size. If 0 size_min and size_max are ignored and no
-      random scaling is applied. max_angle: (degrees) positive and negative
-      bounds for random rotation do_flip: (bool) tells if random flip should be
-      applied padding: (px) amount of padding margin: (px) minimum margin
-      between keypoints and output image border debug: (bool) if True, doesn't
-      actually crop but display debug information on image instead. regenerate:
-      (bool) if True, items are (deep)-copied before calling
-      _apply_transformation. Else, transformation can occur in-place.
+      random scaling is applied. max_angle: (int) positive and negative bounds
+      for random rotation (in degrees) do_flip: (bool) tells if random flip
+      should be applied padding: (int) amount of padding (in pixels) in input
+      image margin: (int) minimum margin (in pixels) between keypoints and
+      output image border debug: (bool) if True, doesn't actually crop but
+      display debug information on image instead. regenerate: (bool) if True,
+      items are (deep)-copied before calling _apply_transformation. Else,
+      transformation can occur in-place.
         Expand source code
       class ViewRandomCropperTransform(RandomCropperTransform):
           def _apply_transformation(self, view, A):
               if self.debug:
                   w, h = self.output_shape
                   points = Point2D(np.linalg.inv(A)@Point2D([0,0,w,w],
       [0,h,h,0]).H)
@@ -994,25 +1101,27 @@
 
 ****** Index ******
     * **** Super-module ****
           o deepsport_utilities.ds.instants_dataset
     * **** Classes ****
           o *** AddBallAnnotation ***
           o *** AddBallFactory ***
+          o *** AddBallHeightFactory ***
           o *** AddBallPositionFactory ***
           o *** AddBallSegmentationTargetViewFactory ***
           o *** AddBallSizeFactory ***
           o *** AddBallStateFactory ***
           o *** AddBallVisibilityFactory ***
           o *** AddCalibFactory ***
                 # to_basic_dict
           o *** AddCourtFactory ***
           o *** AddDiffFactory ***
           o *** AddHumansSegmentationTargetViewFactory ***
           o *** AddImageFactory ***
+          o *** AddIsBallTargetFactory ***
           o *** AddNextImageFactory ***
           o *** BallViewRandomCropperTransform ***
                 # random_ball_position
           o *** BayeringTransform ***
           o *** CleverViewRandomCropperTransform ***
           o *** ComputeDiff ***
           o *** GameGammaColorTransform ***
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/index.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/index.html`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/transforms.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/transforms.html`

 * *Files 3% similar despite different names*

```diff
@@ -102,20 +102,20 @@
                 output_shape: Tuple(int, int) final shape of image-like data.
                 size_min: (int) lower bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
                 size_max: (int) upper bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
-                max_angle: (degrees) positive and negative bounds for random
-                    rotation
+                max_angle: (int) positive and negative bounds for random
+                    rotation (in degrees)
                 do_flip: (bool) tells if random flip should be applied
-                padding: (px) amount of padding
-                margin: (px) minimum margin between keypoints and output image
-                    border
+                padding: (int) amount of padding (in pixels) in input image
+                margin: (int) minimum margin (in pixels) between keypoints and
+                    output image border
                 debug: (bool) if `True`, doesn&#39;t actually crop but display
                     debug information on image instead.
                 regenerate: (bool) if `True`, items are (deep)-copied before
                     calling `_apply_transformation`. Else, transformation can
                     occur in-place.
         &#34;&#34;&#34;
         self.output_shape = output_shape
@@ -138,14 +138,20 @@
         size_max = size_max or self.size_max
 
         if size_min &gt; size_max:
             raise IncompatibleCropException(&#34;Impossible to crop image with object in the given size range&#34;)
         target_size = self.random_size(size_min, size_max) if size_min and size_max else actual_size
         ratio = target_size/actual_size
         tmp_width, tmp_height = [int(x/ratio) for x in self.output_shape]
+        if tmp_width == 0 or tmp_height == 0:
+            print(&#34;actual_size&#34;, actual_size)
+            print(&#34;target_size&#34;, target_size)
+            print(&#34;tmp_width, tmp_height&#34;, tmp_width, tmp_height)
+            print(&#34;self.output_shape&#34;, self.output_shape)
+            raise
         input_width, input_height = input_shape
 
         # If target size makes the output image bigger than input image, try with a lower size
         if tmp_width &gt;= input_width + 2*self.padding or tmp_height &gt;= input_height + 2*self.padding:
             if not size_min or not size_max:
                 raise IncompatibleCropException(&#34;Impossible to crop image with object in the given size range&#34;)
             return self.compute(input_shape, keypoints, actual_size, size_min=target_size*1.1, size_max=size_max)
@@ -228,16 +234,16 @@
             return None
         data = {}
         for factory in self.factories:
             if factory is None:
                 continue
             try:
                 data.update(**factory(key, item))
-            except:
-                print(factory)
+            except BaseException as e:
+                print(factory, &#34;failed&#34;, e)
                 raise
         return data</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
@@ -265,16 +271,16 @@
             return None
         data = {}
         for factory in self.factories:
             if factory is None:
                 continue
             try:
                 data.update(**factory(key, item))
-            except:
-                print(factory)
+            except BaseException as e:
+                print(factory, &#34;failed&#34;, e)
                 raise
         return data</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="deepsport_utilities.transforms.Transform" href="#deepsport_utilities.transforms.Transform">Transform</a></li>
 </ul>
@@ -387,20 +393,20 @@
 <p>output_shape: Tuple(int, int) final shape of image-like data.
 size_min: (int) lower bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
 size_max: (int) upper bound of keypoints random size. If <code>0</code>
 <code>size_min</code> and <code>size_max</code> are ignored and no random scaling
 is applied.
-max_angle: (degrees) positive and negative bounds for random
-rotation
+max_angle: (int) positive and negative bounds for random
+rotation (in degrees)
 do_flip: (bool) tells if random flip should be applied
-padding: (px) amount of padding
-margin: (px) minimum margin between keypoints and output image
-border
+padding: (int) amount of padding (in pixels) in input image
+margin: (int) minimum margin (in pixels) between keypoints and
+output image border
 debug: (bool) if <code>True</code>, doesn't actually crop but display
 debug information on image instead.
 regenerate: (bool) if <code>True</code>, items are (deep)-copied before
 calling <code>_apply_transformation</code>. Else, transformation can
 occur in-place.</p></div>
 <details class="source">
 <summary>
@@ -419,20 +425,20 @@
                 output_shape: Tuple(int, int) final shape of image-like data.
                 size_min: (int) lower bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
                 size_max: (int) upper bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
-                max_angle: (degrees) positive and negative bounds for random
-                    rotation
+                max_angle: (int) positive and negative bounds for random
+                    rotation (in degrees)
                 do_flip: (bool) tells if random flip should be applied
-                padding: (px) amount of padding
-                margin: (px) minimum margin between keypoints and output image
-                    border
+                padding: (int) amount of padding (in pixels) in input image
+                margin: (int) minimum margin (in pixels) between keypoints and
+                    output image border
                 debug: (bool) if `True`, doesn&#39;t actually crop but display
                     debug information on image instead.
                 regenerate: (bool) if `True`, items are (deep)-copied before
                     calling `_apply_transformation`. Else, transformation can
                     occur in-place.
         &#34;&#34;&#34;
         self.output_shape = output_shape
@@ -455,14 +461,20 @@
         size_max = size_max or self.size_max
 
         if size_min &gt; size_max:
             raise IncompatibleCropException(&#34;Impossible to crop image with object in the given size range&#34;)
         target_size = self.random_size(size_min, size_max) if size_min and size_max else actual_size
         ratio = target_size/actual_size
         tmp_width, tmp_height = [int(x/ratio) for x in self.output_shape]
+        if tmp_width == 0 or tmp_height == 0:
+            print(&#34;actual_size&#34;, actual_size)
+            print(&#34;target_size&#34;, target_size)
+            print(&#34;tmp_width, tmp_height&#34;, tmp_width, tmp_height)
+            print(&#34;self.output_shape&#34;, self.output_shape)
+            raise
         input_width, input_height = input_shape
 
         # If target size makes the output image bigger than input image, try with a lower size
         if tmp_width &gt;= input_width + 2*self.padding or tmp_height &gt;= input_height + 2*self.padding:
             if not size_min or not size_max:
                 raise IncompatibleCropException(&#34;Impossible to crop image with object in the given size range&#34;)
             return self.compute(input_shape, keypoints, actual_size, size_min=target_size*1.1, size_max=size_max)
@@ -571,14 +583,20 @@
     size_max = size_max or self.size_max
 
     if size_min &gt; size_max:
         raise IncompatibleCropException(&#34;Impossible to crop image with object in the given size range&#34;)
     target_size = self.random_size(size_min, size_max) if size_min and size_max else actual_size
     ratio = target_size/actual_size
     tmp_width, tmp_height = [int(x/ratio) for x in self.output_shape]
+    if tmp_width == 0 or tmp_height == 0:
+        print(&#34;actual_size&#34;, actual_size)
+        print(&#34;target_size&#34;, target_size)
+        print(&#34;tmp_width, tmp_height&#34;, tmp_width, tmp_height)
+        print(&#34;self.output_shape&#34;, self.output_shape)
+        raise
     input_width, input_height = input_shape
 
     # If target size makes the output image bigger than input image, try with a lower size
     if tmp_width &gt;= input_width + 2*self.padding or tmp_height &gt;= input_height + 2*self.padding:
         if not size_min or not size_max:
             raise IncompatibleCropException(&#34;Impossible to crop image with object in the given size range&#34;)
         return self.compute(input_shape, keypoints, actual_size, size_min=target_size*1.1, size_max=size_max)
@@ -746,24 +764,26 @@
 <li><a title="deepsport_utilities.ds.instants_dataset.instants_transforms.EnhanceColorTransform" href="ds/instants_dataset/instants_transforms.html#deepsport_utilities.ds.instants_dataset.instants_transforms.EnhanceColorTransform">EnhanceColorTransform</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.instants_transforms.GammaCorrectionTransform" href="ds/instants_dataset/instants_transforms.html#deepsport_utilities.ds.instants_dataset.instants_transforms.GammaCorrectionTransform">GammaCorrectionTransform</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.instants_transforms.ProjectBall" href="ds/instants_dataset/instants_transforms.html#deepsport_utilities.ds.instants_dataset.instants_transforms.ProjectBall">ProjectBall</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.instants_transforms.RemoveAnnotationMetadata" href="ds/instants_dataset/instants_transforms.html#deepsport_utilities.ds.instants_dataset.instants_transforms.RemoveAnnotationMetadata">RemoveAnnotationMetadata</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.instants_transforms.RemoveGroundTruth" href="ds/instants_dataset/instants_transforms.html#deepsport_utilities.ds.instants_dataset.instants_transforms.RemoveGroundTruth">RemoveGroundTruth</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallAnnotation" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallAnnotation">AddBallAnnotation</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallFactory">AddBallFactory</a></li>
+<li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallHeightFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallHeightFactory">AddBallHeightFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallPositionFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallPositionFactory">AddBallPositionFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSegmentationTargetViewFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSegmentationTargetViewFactory">AddBallSegmentationTargetViewFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSizeFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallSizeFactory">AddBallSizeFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallStateFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallStateFactory">AddBallStateFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddBallVisibilityFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddBallVisibilityFactory">AddBallVisibilityFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddCalibFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddCalibFactory">AddCalibFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddCourtFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddCourtFactory">AddCourtFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddDiffFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddDiffFactory">AddDiffFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddHumansSegmentationTargetViewFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddHumansSegmentationTargetViewFactory">AddHumansSegmentationTargetViewFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddImageFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddImageFactory">AddImageFactory</a></li>
+<li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddIsBallTargetFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddIsBallTargetFactory">AddIsBallTargetFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.AddNextImageFactory" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.AddNextImageFactory">AddNextImageFactory</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.BayeringTransform" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.BayeringTransform">BayeringTransform</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.ComputeDiff" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.ComputeDiff">ComputeDiff</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.GameGammaColorTransform" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.GameGammaColorTransform">GameGammaColorTransform</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.GameRGBColorTransform" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.GameRGBColorTransform">GameRGBColorTransform</a></li>
 <li><a title="deepsport_utilities.ds.instants_dataset.views_transforms.UndistortTransform" href="ds/instants_dataset/views_transforms.html#deepsport_utilities.ds.instants_dataset.views_transforms.UndistortTransform">UndistortTransform</a></li>
 <li><a title="deepsport_utilities.transforms.DataExtractorTransform" href="#deepsport_utilities.transforms.DataExtractorTransform">DataExtractorTransform</a></li>
```

#### html2text {}

```diff
@@ -85,20 +85,20 @@
                 output_shape: Tuple(int, int) final shape of image-like data.
                 size_min: (int) lower bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
                 size_max: (int) upper bound of keypoints random size. If `0`
                     `size_min` and `size_max` are ignored and no random scaling
                     is applied.
-                max_angle: (degrees) positive and negative bounds for random
-                    rotation
+                max_angle: (int) positive and negative bounds for random
+                    rotation (in degrees)
                 do_flip: (bool) tells if random flip should be applied
-                padding: (px) amount of padding
-                margin: (px) minimum margin between keypoints and output image
-                    border
+                padding: (int) amount of padding (in pixels) in input image
+                margin: (int) minimum margin (in pixels) between keypoints and
+                    output image border
                 debug: (bool) if `True`, doesn't actually crop but display
                     debug information on image instead.
                 regenerate: (bool) if `True`, items are (deep)-copied before
                     calling `_apply_transformation`. Else, transformation can
                     occur in-place.
         """
         self.output_shape = output_shape
@@ -125,14 +125,20 @@
         if size_min > size_max:
             raise IncompatibleCropException("Impossible to crop image with
 object in the given size range")
         target_size = self.random_size(size_min, size_max) if size_min and
 size_max else actual_size
         ratio = target_size/actual_size
         tmp_width, tmp_height = [int(x/ratio) for x in self.output_shape]
+        if tmp_width == 0 or tmp_height == 0:
+            print("actual_size", actual_size)
+            print("target_size", target_size)
+            print("tmp_width, tmp_height", tmp_width, tmp_height)
+            print("self.output_shape", self.output_shape)
+            raise
         input_width, input_height = input_shape
 
         # If target size makes the output image bigger than input image, try
 with a lower size
         if tmp_width >= input_width + 2*self.padding or tmp_height >=
 input_height + 2*self.padding:
             if not size_min or not size_max:
@@ -230,16 +236,16 @@
             return None
         data = {}
         for factory in self.factories:
             if factory is None:
                 continue
             try:
                 data.update(**factory(key, item))
-            except:
-                print(factory)
+            except BaseException as e:
+                print(factory, "failed", e)
                 raise
         return data
 
 ***** Classes *****
   class DataExtractorTransform (*factories)
         Expand source code
       class DataExtractorTransform(Transform):
@@ -250,16 +256,16 @@
                   return None
               data = {}
               for factory in self.factories:
                   if factory is None:
                       continue
                   try:
                       data.update(**factory(key, item))
-                  except:
-                      print(factory)
+                  except BaseException as e:
+                      print(factory, "failed", e)
                       raise
               return data
       **** Ancestors ****
           * Transform
   class DeclutterItems (drop)
       Drops attributes from dataset items. Attributes to drop are given by the
       'drop' argument.
@@ -319,21 +325,22 @@
       size_min and size_max (At each call, the current keypoint size is
       returned by _get_current_parameters).
       ***** Arguments *****
       output_shape: Tuple(int, int) final shape of image-like data. size_min:
       (int) lower bound of keypoints random size. If 0 size_min and size_max
       are ignored and no random scaling is applied. size_max: (int) upper bound
       of keypoints random size. If 0 size_min and size_max are ignored and no
-      random scaling is applied. max_angle: (degrees) positive and negative
-      bounds for random rotation do_flip: (bool) tells if random flip should be
-      applied padding: (px) amount of padding margin: (px) minimum margin
-      between keypoints and output image border debug: (bool) if True, doesn't
-      actually crop but display debug information on image instead. regenerate:
-      (bool) if True, items are (deep)-copied before calling
-      _apply_transformation. Else, transformation can occur in-place.
+      random scaling is applied. max_angle: (int) positive and negative bounds
+      for random rotation (in degrees) do_flip: (bool) tells if random flip
+      should be applied padding: (int) amount of padding (in pixels) in input
+      image margin: (int) minimum margin (in pixels) between keypoints and
+      output image border debug: (bool) if True, doesn't actually crop but
+      display debug information on image instead. regenerate: (bool) if True,
+      items are (deep)-copied before calling _apply_transformation. Else,
+      transformation can occur in-place.
         Expand source code
       class RandomCropperTransform(Transform, metaclass=abc.ABCMeta):
           linewidth = 4
           random_size = np.random.uniform
           def __init__(self, output_shape, size_min, size_max, max_angle=0,
       do_flip=False, padding=0, margin=0, debug=False, regenerate=False):
               """ Randomly scale, crop and rotate dataset items. The scale
@@ -353,22 +360,22 @@
       scaling
                           is applied.
                       size_max: (int) upper bound of keypoints random size. If
       `0`
                           `size_min` and `size_max` are ignored and no random
       scaling
                           is applied.
-                      max_angle: (degrees) positive and negative bounds for
-      random
-                          rotation
+                      max_angle: (int) positive and negative bounds for random
+                          rotation (in degrees)
                       do_flip: (bool) tells if random flip should be applied
-                      padding: (px) amount of padding
-                      margin: (px) minimum margin between keypoints and output
+                      padding: (int) amount of padding (in pixels) in input
       image
-                          border
+                      margin: (int) minimum margin (in pixels) between
+      keypoints and
+                          output image border
                       debug: (bool) if `True`, doesn't actually crop but
       display
                           debug information on image instead.
                       regenerate: (bool) if `True`, items are (deep)-copied
       before
                           calling `_apply_transformation`. Else, transformation
       can
@@ -399,14 +406,20 @@
               if size_min > size_max:
                   raise IncompatibleCropException("Impossible to crop image
       with object in the given size range")
               target_size = self.random_size(size_min, size_max) if size_min
       and size_max else actual_size
               ratio = target_size/actual_size
               tmp_width, tmp_height = [int(x/ratio) for x in self.output_shape]
+              if tmp_width == 0 or tmp_height == 0:
+                  print("actual_size", actual_size)
+                  print("target_size", target_size)
+                  print("tmp_width, tmp_height", tmp_width, tmp_height)
+                  print("self.output_shape", self.output_shape)
+                  raise
               input_width, input_height = input_shape
 
               # If target size makes the output image bigger than input image,
       try with a lower size
               if tmp_width >= input_width + 2*self.padding or tmp_height >=
       input_height + 2*self.padding:
                   if not size_min or not size_max:
@@ -530,24 +543,26 @@
           * EnhanceColorTransform
           * GammaCorrectionTransform
           * ProjectBall
           * RemoveAnnotationMetadata
           * RemoveGroundTruth
           * AddBallAnnotation
           * AddBallFactory
+          * AddBallHeightFactory
           * AddBallPositionFactory
           * AddBallSegmentationTargetViewFactory
           * AddBallSizeFactory
           * AddBallStateFactory
           * AddBallVisibilityFactory
           * AddCalibFactory
           * AddCourtFactory
           * AddDiffFactory
           * AddHumansSegmentationTargetViewFactory
           * AddImageFactory
+          * AddIsBallTargetFactory
           * AddNextImageFactory
           * BayeringTransform
           * ComputeDiff
           * GameGammaColorTransform
           * GameRGBColorTransform
           * UndistortTransform
           * DataExtractorTransform
```

### Comparing `deepsport_utilities-4.8.2/docs/deepsport_utilities/utils.html` & `deepsport_utilities-4.9.0/docs/deepsport_utilities/utils.html`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,18 @@
         left  = max(-padding,           int(self.x-margin))
         right = min(max_width+padding,  int(self.x+self.w+margin))
 
         if aspect_ratio is None:
             return slice(left, right, None), slice(top, bot, None)
 
         if padding:
-            raise NotImplementedError(&#34;increase_box method doesn&#39;t support padding when aspect ratio is given&#34;)
+            try:
+                raise NotImplementedError(&#34;increase_box method doesn&#39;t support padding when aspect ratio is given&#34;)
+            except:
+                pass
 
         w = right - left
         h = bot - top
         if w/h &gt; aspect_ratio: # box is wider
             h = int(w/aspect_ratio)
             if h &gt; max_height: # box is too wide
                 h = max_height
@@ -561,15 +564,18 @@
         left  = max(-padding,           int(self.x-margin))
         right = min(max_width+padding,  int(self.x+self.w+margin))
 
         if aspect_ratio is None:
             return slice(left, right, None), slice(top, bot, None)
 
         if padding:
-            raise NotImplementedError(&#34;increase_box method doesn&#39;t support padding when aspect ratio is given&#34;)
+            try:
+                raise NotImplementedError(&#34;increase_box method doesn&#39;t support padding when aspect ratio is given&#34;)
+            except:
+                pass
 
         w = right - left
         h = bot - top
         if w/h &gt; aspect_ratio: # box is wider
             h = int(w/aspect_ratio)
             if h &gt; max_height: # box is too wide
                 h = max_height
@@ -692,15 +698,18 @@
     left  = max(-padding,           int(self.x-margin))
     right = min(max_width+padding,  int(self.x+self.w+margin))
 
     if aspect_ratio is None:
         return slice(left, right, None), slice(top, bot, None)
 
     if padding:
-        raise NotImplementedError(&#34;increase_box method doesn&#39;t support padding when aspect ratio is given&#34;)
+        try:
+            raise NotImplementedError(&#34;increase_box method doesn&#39;t support padding when aspect ratio is given&#34;)
+        except:
+            pass
 
     w = right - left
     h = bot - top
     if w/h &gt; aspect_ratio: # box is wider
         h = int(w/aspect_ratio)
         if h &gt; max_height: # box is too wide
             h = max_height
```

#### html2text {}

```diff
@@ -226,16 +226,19 @@
         left  = max(-padding,           int(self.x-margin))
         right = min(max_width+padding,  int(self.x+self.w+margin))
 
         if aspect_ratio is None:
             return slice(left, right, None), slice(top, bot, None)
 
         if padding:
-            raise NotImplementedError("increase_box method doesn't support
+            try:
+                raise NotImplementedError("increase_box method doesn't support
 padding when aspect ratio is given")
+            except:
+                pass
 
         w = right - left
         h = bot - top
         if w/h > aspect_ratio: # box is wider
             h = int(w/aspect_ratio)
             if h > max_height: # box is too wide
                 h = max_height
@@ -479,16 +482,19 @@
               left  = max(-padding,           int(self.x-margin))
               right = min(max_width+padding,  int(self.x+self.w+margin))
 
               if aspect_ratio is None:
                   return slice(left, right, None), slice(top, bot, None)
 
               if padding:
-                  raise NotImplementedError("increase_box method doesn't
+                  try:
+                      raise NotImplementedError("increase_box method doesn't
       support padding when aspect ratio is given")
+                  except:
+                      pass
 
               w = right - left
               h = bot - top
               if w/h > aspect_ratio: # box is wider
                   h = int(w/aspect_ratio)
                   if h > max_height: # box is too wide
                       h = max_height
@@ -578,16 +584,19 @@
                 left  = max(-padding,           int(self.x-margin))
                 right = min(max_width+padding,  int(self.x+self.w+margin))
 
                 if aspect_ratio is None:
                     return slice(left, right, None), slice(top, bot, None)
 
                 if padding:
-                    raise NotImplementedError("increase_box method doesn't
+                    try:
+                        raise NotImplementedError("increase_box method doesn't
             support padding when aspect ratio is given")
+                    except:
+                        pass
 
                 w = right - left
                 h = bot - top
                 if w/h > aspect_ratio: # box is wider
                     h = int(w/aspect_ratio)
                     if h > max_height: # box is too wide
                         h = max_height
```

### Comparing `deepsport_utilities-4.8.2/examples/create_camera_views_dataset.py` & `deepsport_utilities-4.9.0/examples/create_camera_views_dataset.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/examples/import_instants_dataset.py` & `deepsport_utilities-4.9.0/examples/import_instants_dataset.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/release.sh` & `deepsport_utilities-4.9.0/release.sh`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/setup.py` & `deepsport_utilities-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     python_requires='>=3.8',
     # 3.8 required for
     #    - PEP 572 – Assignment Expressions (:=)
     #    - `functools.cached_property` (although `mlworkflow.lazyproperty` could be used for older python versions)
     # 3.7 required for
     #    - EvalAI ... but we don't care anymore, do we?
     description="",
-    version='4.8.2',
+    version='4.9.0',
     packages=find_packages(),
     install_requires=[
         "numpy", # was >=1.20", ... but I don't understand why
         "scipy",
         "opencv-python",
         "imageio",
         "m3u8",
```

### Comparing `deepsport_utilities-4.8.2/tests/groundtruths/ball_view.png` & `deepsport_utilities-4.9.0/tests/groundtruths/ball_view.png`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/tests/input_imgs/game_94132_frame_idx_0.png` & `deepsport_utilities-4.9.0/tests/input_imgs/game_94132_frame_idx_0.png`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/tests/test_calib.py` & `deepsport_utilities-4.9.0/tests/test_calib.py`

 * *Files identical despite different names*

### Comparing `deepsport_utilities-4.8.2/tests/test_court.py` & `deepsport_utilities-4.9.0/tests/test_court.py`

 * *Files identical despite different names*

