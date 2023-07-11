# Comparing `tmp/icepy4d-1.6.2.tar.gz` & `tmp/icepy4d-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icepy4d-1.6.2.tar", last modified: Tue Apr 25 16:21:23 2023, max compression
+gzip compressed data, was "icepy4d-1.7.0.tar", last modified: Tue Jul 11 09:06:11 2023, max compression
```

## Comparing `icepy4d-1.6.2.tar` & `icepy4d-1.7.0.tar`

### file list

```diff
@@ -1,140 +1,131 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1558 2023-04-20 09:19:34.000000 icepy4d-1.6.2/LICENSE.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4168 2023-04-25 16:21:23.911137 icepy4d-1.6.2/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1765 2023-04-25 16:19:58.000000 icepy4d-1.6.2/README.md
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1623 2023-04-25 16:20:56.000000 icepy4d-1.6.2/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-25 16:21:23.911137 icepy4d-1.6.2/setup.cfg
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/icepy4d/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       55 2023-04-25 16:20:56.000000 icepy4d-1.6.2/src/icepy4d/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      244 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/__main__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/classes/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      235 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    17269 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/camera.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/dsm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/epoch.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    26531 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    19126 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/images.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/ortophoto.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6786 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/point_cloud.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18374 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/points.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3262 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/solution.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11317 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/targets.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      789 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/typed_dict_classes.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/io/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/__init__.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22889 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3709 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build_windows_app.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4731 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/bundler_to_ply.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2622 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/clang_format_code.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5565 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/crawl_camera_specs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15026 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/database.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3389 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_matches.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3237 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_pairs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6730 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_bundler.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6402 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_visualsfm.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6297 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/flickr_downloader.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5996 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/h5_to_db.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2692 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/merge_ply_files.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4743 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/nvm_to_ply.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    25506 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/plyfile.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5172 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_dense.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5230 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_fused_vis.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22035 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_model.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     7069 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/visualize_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9057 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/io/export2bundler.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2922 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/export2calge.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4751 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/export2colmap.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2995 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/export2textfile.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1617 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/importing.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/least_squares/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/least_squares/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4184 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/least_squares/absolute_orientation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2845 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/least_squares/rototra3d.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2761 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/least_squares/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/matching/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11728 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/match_by_preselection.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13660 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/match_pairs.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7602 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/matching_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1656 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/retrieve_matches_from_npz.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4096 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/matching/superglue_match_simple_old.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14690 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/superglue_matcher.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13481 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/matching/superglue_tracker.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15735 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/templatematch.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16743 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/track_matches.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18706 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/track_matches_bk.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3438 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/tracking_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5879 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/metashape/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/metashape/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20168 2023-04-25 16:04:33.000000 icepy4d-1.6.2/src/icepy4d/metashape/metashape.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18623 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/metashape/metashape_core.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7242 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/cloudcompare_fun.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12502 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/open3d_fun.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      974 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/sfm/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      218 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10834 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/sfm/absolute_orientation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4404 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/interpolate_colors.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1333 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/reconstruction.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6341 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/sfm/triangulation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8073 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/two_view_geometry.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/thirdparty/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3419 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11869 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8350 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20648 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10683 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    18127 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3417 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11781 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8142 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20039 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11815 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/templatematch_pyimgraft.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/transformations.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10133 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/triangulation.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      295 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13046 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/binned_stats.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7091 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/dsm_orthophoto.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      951 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/homography.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12345 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/initialization.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5957 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/logger.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3670 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/math.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1552 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/sensor_width_database.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3783 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/spatial_funs.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7325 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/tiles.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1662 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/timer.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16090 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/tracking_features_utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6354 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/utils/transformations.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/visualization/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       29 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/visualization/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    27688 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/visualization/visualization.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/icepy4d.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4168 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4573 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      246 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/top_level.txt
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/tests/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8220 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1484 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_image.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2394 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_initialization.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      775 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2032 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_point_cloud.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2742 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_sfm_geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      518 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1457 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_utils_spatial.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1558 2023-07-07 16:21:27.000000 icepy4d-1.7.0/LICENSE.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4168 2023-07-11 09:06:11.366039 icepy4d-1.7.0/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1765 2023-07-07 16:21:27.000000 icepy4d-1.7.0/README.md
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1635 2023-07-11 09:03:42.000000 icepy4d-1.7.0/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-07-11 09:06:11.366039 icepy4d-1.7.0/setup.cfg
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.362039 icepy4d-1.7.0/src/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.362039 icepy4d-1.7.0/src/icepy4d/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       55 2023-07-11 09:03:42.000000 icepy4d-1.7.0/src/icepy4d/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      244 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/__main__.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.362039 icepy4d-1.7.0/src/icepy4d/classes/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      759 2023-07-11 07:55:42.000000 icepy4d-1.7.0/src/icepy4d/classes/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6796 2023-07-11 08:52:20.000000 icepy4d-1.7.0/src/icepy4d/classes/calibration.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    17267 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/classes/camera.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/classes/dsm.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11136 2023-07-11 08:20:23.000000 icepy4d-1.7.0/src/icepy4d/classes/epoch.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    26531 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/classes/features.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    22425 2023-07-10 18:43:47.000000 icepy4d-1.7.0/src/icepy4d/classes/images.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/classes/ortophoto.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6786 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/classes/point_cloud.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18222 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/classes/points.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1648 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/classes/sensor_width_database.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11317 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/classes/targets.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      995 2023-07-10 19:20:23.000000 icepy4d-1.7.0/src/icepy4d/classes/typed_dict_classes_old.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.362039 icepy4d-1.7.0/src/icepy4d/io/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/__init__.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/__init__.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22889 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/build.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3709 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/build_windows_app.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4731 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2622 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/clang_format_code.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5565 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15026 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/database.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3389 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3237 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6730 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_to_bundler.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6402 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6297 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/flickr_downloader.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5996 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/h5_to_db.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2692 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/merge_ply_files.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4743 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    25506 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/plyfile.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5172 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/read_write_dense.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5230 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22035 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/read_write_model.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     7069 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/colmap_utils/visualize_model.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     9017 2023-07-10 18:50:01.000000 icepy4d-1.7.0/src/icepy4d/io/export2bundler.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2922 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/export2calge.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4734 2023-07-10 18:41:13.000000 icepy4d-1.7.0/src/icepy4d/io/export2colmap.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2995 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/io/export2textfile.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/least_squares/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/least_squares/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4184 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/least_squares/absolute_orientation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2845 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/least_squares/rototra3d.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2761 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/least_squares/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/matching/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11684 2023-07-10 19:27:51.000000 icepy4d-1.7.0/src/icepy4d/matching/match_by_preselection.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13660 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/match_pairs.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8963 2023-07-10 16:34:54.000000 icepy4d-1.7.0/src/icepy4d/matching/matching_base.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1656 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/retrieve_matches_from_npz.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4096 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/superglue_match_simple_old.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14690 2023-07-10 16:34:54.000000 icepy4d-1.7.0/src/icepy4d/matching/superglue_matcher.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13481 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/superglue_tracker.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    15735 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/templatematch.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16741 2023-07-11 07:36:27.000000 icepy4d-1.7.0/src/icepy4d/matching/track_matches.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18706 2023-07-07 17:53:42.000000 icepy4d-1.7.0/src/icepy4d/matching/track_matches_bk.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3428 2023-07-10 17:04:29.000000 icepy4d-1.7.0/src/icepy4d/matching/tracking_base.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5879 2023-07-10 19:27:39.000000 icepy4d-1.7.0/src/icepy4d/matching/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/metashape/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/metashape/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20175 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/metashape/metashape.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20138 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/metashape/metashape_core.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/point_cloud_proc/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/point_cloud_proc/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7242 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    12500 2023-07-11 07:36:27.000000 icepy4d-1.7.0/src/icepy4d/point_cloud_proc/open3d_fun.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      974 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/point_cloud_proc/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/sfm/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      218 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/sfm/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    10834 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/sfm/absolute_orientation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/sfm/geometry.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4404 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/sfm/interpolate_colors.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1333 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/sfm/reconstruction.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6341 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/sfm/triangulation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8073 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/sfm/two_view_geometry.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/thirdparty/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.362039 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3419 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11869 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/superglue.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8350 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/superpoint.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20648 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11815 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/transformations.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    10133 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/thirdparty/triangulation.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/utils/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      295 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/utils/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13046 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/utils/binned_stats.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7098 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/utils/dsm_orthophoto.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3783 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/utils/geospatial.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1446 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/utils/homography.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16068 2023-07-11 08:24:07.000000 icepy4d-1.7.0/src/icepy4d/utils/initialization.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5944 2023-07-11 07:51:46.000000 icepy4d-1.7.0/src/icepy4d/utils/logger.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3606 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/utils/math.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8192 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/utils/tiles.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1662 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/utils/timer.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16096 2023-07-11 07:36:27.000000 icepy4d-1.7.0/src/icepy4d/utils/tracking_features_utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7704 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/utils/transformations.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/src/icepy4d/visualization/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       29 2023-07-07 16:21:27.000000 icepy4d-1.7.0/src/icepy4d/visualization/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    27598 2023-07-07 18:02:33.000000 icepy4d-1.7.0/src/icepy4d/visualization/visualization.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.362039 icepy4d-1.7.0/src/icepy4d.egg-info/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4168 2023-07-11 09:06:11.000000 icepy4d-1.7.0/src/icepy4d.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4107 2023-07-11 09:06:11.000000 icepy4d-1.7.0/src/icepy4d.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-07-11 09:06:11.000000 icepy4d-1.7.0/src/icepy4d.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      251 2023-07-11 09:06:11.000000 icepy4d-1.7.0/src/icepy4d.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-07-11 09:06:11.000000 icepy4d-1.7.0/src/icepy4d.egg-info/top_level.txt
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-07-11 09:06:11.366039 icepy4d-1.7.0/tests/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8220 2023-07-07 16:21:27.000000 icepy4d-1.7.0/tests/test_features.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1484 2023-07-07 16:21:27.000000 icepy4d-1.7.0/tests/test_image.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2394 2023-07-07 16:21:27.000000 icepy4d-1.7.0/tests/test_initialization.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      775 2023-07-07 16:21:27.000000 icepy4d-1.7.0/tests/test_matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2032 2023-07-07 16:21:27.000000 icepy4d-1.7.0/tests/test_point_cloud.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2742 2023-07-07 16:21:27.000000 icepy4d-1.7.0/tests/test_sfm_geometry.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1295 2023-07-07 18:02:33.000000 icepy4d-1.7.0/tests/test_transformations.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      482 2023-07-11 07:38:03.000000 icepy4d-1.7.0/tests/test_utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1455 2023-07-11 07:38:26.000000 icepy4d-1.7.0/tests/test_utils_geospatial.py
```

### Comparing `icepy4d-1.6.2/LICENSE.txt` & `icepy4d-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/PKG-INFO` & `icepy4d-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icepy4d
-Version: 1.6.2
+Version: 1.7.0
 Summary: 4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
         All rights reserved.
```

### Comparing `icepy4d-1.6.2/README.md` & `icepy4d-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/pyproject.toml` & `icepy4d-1.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icepy4d"
-version = "1.6.2"
+version = "1.7.0"
 description = "4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry."
 readme = "README.md"
 authors = [{ name = "Francesco Ioli", email = "francesco.ioli@polimi.it" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,14 +27,15 @@
     "exifread",
     "tqdm",
     "laspy",
     "pyyaml",
     "easydict",
     "kornia",
     "lmfit",
+    "h5py",
 ]
 requires-python = ">=3.8"
 
 
 [project.optional-dependencies]
 dev = ["flake8", "black", "bumpver", "isort", "pip-tools", "pytest", "bumpver", "mkdocs", "mkdocs-material", "mkdocstrings[python]", "pre-commit", "nbstripout", "build", "twine"]
 
@@ -45,15 +46,15 @@
 addopts = [
     "--import-mode=importlib",
 ]
 
 [tool.isort]
 profile = "black"
 [tool.bumpver]
-current_version = "1.6.2"
+current_version = "1.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/camera.py` & `icepy4d-1.7.0/src/icepy4d/classes/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import cv2
 import logging
 
 from typing import List, Union, Tuple
 from scipy import linalg
 from pathlib import Path
 
-from ..io.importing import read_opencv_calibration
+from .calibration import read_opencv_calibration
 
 
 class Camera:
     """Class to manage Pinhole Cameras.
 
     Attributes:
         _w (int): Image width in pixels.
```

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/dsm.py` & `icepy4d-1.7.0/src/icepy4d/classes/dsm.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/epoch.py` & `icepy4d-1.7.0/src/icepy4d/classes/ortophoto.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/features.py` & `icepy4d-1.7.0/src/icepy4d/classes/features.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/images.py` & `icepy4d-1.7.0/src/icepy4d/classes/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import os
 import logging
+import os
+from datetime import datetime
 from pathlib import Path
 from typing import List, Union
-from datetime import datetime
 
 import cv2
 import exifread
 import numpy as np
 
-from icepy4d.classes.camera import Camera
-from icepy4d.utils.sensor_width_database import SensorWidthDatabase
-from ..sfm.geometry import undistort_image
+from .camera import Camera
+from .sensor_width_database import SensorWidthDatabase
+
+
 
 # @TODO: remove variable number of outputs
 def read_image(
     path: Union[str, Path],
     color: bool = True,
     resize: List[int] = [-1],
     crop: List[int] = None,
@@ -211,14 +212,29 @@
         if self._date_time is not None:
             return self._date_time.strftime("%H:%M:%S")
         else:
             logging.error("No exif data available.")
             return None
 
     @property
+    def datetime(self) -> datetime:
+        """
+        Returns the date and time of the image in a string format.
+        If the information is not available in the EXIF metadata, it returns None.
+
+        Returns:
+            datetime: The date and time of the image as datetime object
+        """
+        if self._date_time is not None:
+            return self._date_time
+        else:
+            logging.error("No exif data available.")
+            return
+
+    @property
     def value(self) -> np.ndarray:
         """
         Returns the image (pixel values) as numpy array
         """
         if self._value_array is not None:
             return self._value_array
         else:
@@ -240,22 +256,24 @@
 
     def read_image(
         self,
         # path: Union[str, Path],
         col: bool = True,
         resize: List[int] = [-1],
         crop: List[int] = None,
-    ) -> None:
+    ) -> np.ndarray:
         """Wrapper around the function read_image to be a class method."""
         # path = Path(path)
         if self.path.exists():
             self._value_array = read_image(self.path, col, resize, crop)
             self.read_exif()
+            return self._value_array
         else:
             logging.error(f"Input paht {self.path} not valid.")
+            return None
 
     def reset_image(self) -> None:
         self._value_array = None
 
     def read_exif(self) -> None:
         """Read image exif with exifread and store them in a dictionary"""
         try:
@@ -374,160 +392,276 @@
             camera (Camera): Camera object containing K and dist arrays.
             out_path (str, optional): Path for writing the undistorted image to disk. If out_path is None, undistorted image is not saved to disk. Defaults to None.
 
         Returns:
             np.ndarray: undistored image
         """
         self.read_image()
-        und_imge = undistort_image(
-            cv2.cvtColor(self._value_array, cv2.COLOR_RGB2BGR), camera, out_path
+
+        und_imge = cv2.undistort(
+            cv2.cvtColor(self._value_array, cv2.COLOR_RGB2BGR),
+            camera.K,
+            camera.dist,
+            None,
+            camera.K,
         )
+        if out_path is not None:
+            cv2.imwrite(out_path, und_imge)
+
         return und_imge
 
 
 class ImageDS:
     """
     Class to manage Image datasets for multi epoch
-
     """
 
     def __init__(
         self,
-        folder: Union[str, Path],
+        path: Union[str, Path, List[Path]],
         ext: str = None,
         recursive: bool = False,
     ) -> None:
         """
-        __init__ _summary_
+        Initializes an ImageDS object.
 
         Args:
-            folder (Union[str, Path]): Path to the image folder
+            path (Union[str, Path]): Path to the image folder or list of paths of the images.
             ext (str, optional): Image extension for filtering files. If None is provided, all files in 'folder' are read. Defaults to None.
-            recursive (bool, optional): Read files recurevely. Defaults to False.
+            recursive (bool, optional): Read files recursively. Defaults to False.
 
         Raises:
-            IsADirectoryError: _description_
+            IsADirectoryError: If the input path is invalid.
         """
-        self.reset_imageds()
-
-        self.folder = Path(folder)
-        if not self.folder.exists():
-            msg = f"Error: invalid input path {self.folder}"
-            logging.error(msg)
-            raise IsADirectoryError(msg)
-        if ext is not None:
-            self.ext = ext
-        self.recursive = recursive
+        self._files = None
+        self._datetimes = {}
+        self._folder = None
+        self._ext = None
+        self._elem = 0
 
-        self.read_image_list(self.folder)
+        if isinstance(path, list):
+            assert all(
+                [isinstance(x, Path) for x in path]
+            ), "If a list is provided, all elements must be of type Path"
+            self._files = path
+        else:
+            self._folder = Path(path)
+            if not self._folder.exists():
+                msg = f"Error: invalid input path {self._folder}"
+                logging.error(msg)
+                raise IsADirectoryError(msg)
+            if ext is not None:
+                self._ext = ext
+            self._recursive = recursive
+            self._read_image_list(self._folder)
+        try:
+            self._read_dates()
+        except RuntimeError as err:
+            logging.exception(err)
 
     def __len__(self) -> int:
-        """Get number of images in the datastore"""
-        return len(self.files)
+        """
+        Returns the number of images in the datastore.
+        """
+        return len(self._files)
 
     def __contains__(self, name: str) -> bool:
-        """Check if an image is in the datastore, given the image name"""
-        files = [x.name for x in self.files]
+        """
+        Checks if an image is in the datastore, given the image name.
+
+        Args:
+            name (str): The name of the image.
+
+        Returns:
+            bool: True if the image is in the datastore, False otherwise.
+        """
+        files = [x.name for x in self._files]
         return name in files
 
     def __getitem__(self, idx: int) -> str:
-        """Return image name (including extension) at position idx in datastore"""
-        return self.files[idx].name
+        """
+        Returns the image name (including extension) at position idx in the datastore.
+
+        Args:
+            idx (int): The index of the image.
+
+        Returns:
+            str: The name of the image.
+        """
+        return self._files[idx].name
 
     def __iter__(self):
+        """
+        Initializes the iterator for iterating over the images in the datastore.
+
+        Returns:
+            ImageDS: The iterator object.
+        """
         self._elem = 0
         return self
 
     def __next__(self):
+        """
+        Returns the next image file in the iteration.
+
+        Returns:
+            Path: The next image file.
+
+        Raises:
+            StopIteration: If there are no more images in the datastore.
+        """
         while self._elem < len(self):
-            file = self.files[self._elem]
+            file = self._files[self._elem]
             self._elem += 1
             return file
         else:
             self._elem
             raise StopIteration
 
     def reset_imageds(self) -> None:
-        """Initialize image datastore"""
-        self.files = None
-        self.folder = None
-        self.ext = None
+        """
+        Re-initializes the image datastore.
+        """
+        self._files = None
+        self._folder = None
+        self._ext = None
         self._elem = 0
 
-    def read_image_list(self, recursive: bool = None) -> None:
-        assert self.folder.is_dir(), "Error: invalid image directory."
+    @property
+    def files(self) -> List[Path]:
+        """
+        Returns the list of files in the datastore.
+        """
+        return self._files
+
+    @property
+    def folder(self) -> Path:
+        """
+        Returns the folder path of the datastore.
+        """
+        return self._folder
+
+    @property
+    def datetimes(self) -> List[datetime]:
+        """
+        Returns the list of datetimes of images in the datastore.
+        """
+        return list(self._datetimes.values())
+
+    def _read_image_list(self, recursive: bool = None) -> None:
+        """
+        Reads the list of image files in the datastore.
+
+        Args:
+            recursive (bool, optional): Read files recursively. Defaults to None.
+
+        Raises:
+            AssertionError: If the image directory is invalid.
+        """
+        assert self._folder.is_dir(), "Error: invalid image directory."
 
         if recursive is not None:
-            self.recursive = recursive
-        if self.recursive:
+            self._recursive = recursive
+        if self._recursive:
             rec_patt = "**/"
         else:
             rec_patt = ""
-        if self.ext is not None:
-            ext_patt = f".{self.ext}"
+        if self._ext is not None:
+            ext_patt = f".{self._ext}"
         else:
             ext_patt = ""
         pattern = f"{rec_patt}*{ext_patt}"
 
-        self.files = sorted(self.folder.glob(pattern))
+        self._files = sorted(self._folder.glob(pattern))
 
-        if len(self.files) == 0:
-            logging.error(f"No images found in folder {self.folder}")
+        if len(self._files) == 0:
+            logging.error(f"No images found in folder {self._folder}")
             return
-        try:
-            self.read_dates()
-        except OSError as err:
-            logging.exception(err)
-
-    def read_image(self, idx: int) -> Image:
-        """Return image at position idx as Image instance, containing both exif and value data (accessible by value proprierty, e.g., image.value)"""
-        image = Image(self.files[idx])
-        image.read_image()
-        return image
 
-    def read_dates(self) -> None:
+    def _read_dates(self) -> None:
         """
-        read_dates Read date and time for all the images in ImageDS from exif.
+        Reads the date and time for all the images in the ImageDS from the EXIF data.
         """
-        assert self.files, "No image in ImageDS. Please read image list first"
+        assert self._files, "No image in ImageDS. Please read image list first"
         self._dates, self._times = {}, {}
         try:
-            for id, im in enumerate(self.files):
+            for id, im in enumerate(self._files):
                 image = Image(im)
+                self._datetimes[id] = image.datetime
+
+                # These are kept only for backward compatibility
                 self._dates[id] = image.date
                 self._times[id] = image.time
         except:
-            logging.error("Unable to read image dates and time from exif.")
+            logging.error("Unable to read image dates and time from EXIF.")
             self._dates, self._times = {}, {}
             return
 
+    def read_image(self, idx: int) -> Image:
+        """
+        Returns the image at the specified position as an Image instance, containing both EXIF and value data.
+
+        Args:
+            idx (int): The index of the image.
+
+        Returns:
+            Image: The Image instance.
+        """
+        image = Image(self._files[idx])
+        image.read_image()
+        return image
+
     def get_image_path(self, idx: int) -> Path:
-        """Return path of the image at position idx in datastore as Pathlib"""
-        return self.files[idx]
+        """
+        Returns the path of the image at the specified position in the datastore.
+
+        Args:
+            idx (int): The index of the image.
+
+        Returns:
+            Path: The path of the image.
+        """
+        return self._files[idx]
 
     def get_image_stem(self, idx: int) -> str:
-        """Return name without extension(stem) of the image at position idx in datastore"""
-        return self.files[idx].stem
+        """
+        Returns the name without extension (stem) of the image at the specified position in the datastore.
+
+        Args:
+            idx (int): The index of the image.
+
+        Returns:
+            str: The name without extension of the image.
+        """
+        return self._files[idx].stem
 
     def get_image_date(self, idx: int) -> str:
-        """Return name without extension(stem) of the image at position idx in datastore"""
+        """
+        Returns the date of the image at the specified position in the datastore.
+
+        Args:
+            idx (int): The index of the image.
+
+        Returns:
+            str: The date of the image.
+        """
         return self._dates[idx]
 
     def get_image_time(self, idx: int) -> str:
         """Return name without extension(stem) of the image at position idx in datastore"""
         return self._times[idx]
 
     def write_exif_to_csv(
         self, filename: str, sep: str = ",", header: bool = True
     ) -> None:
-        assert self.folder.is_dir(), "Empty Image Datastore."
+        assert self._folder.is_dir(), "Empty Image Datastore."
         file = open(filename, "w")
         if header:
             file.write("epoch,name,date,time\n")
-        for i, img_path in enumerate(self.files):
+        for i, img_path in enumerate(self._files):
             img = Image(img_path)
             name = img_path.name
             date = img.date
             time = img.time
             file.write(f"{i}{sep}{name}{sep}{date}{sep}{time}\n")
         file.close()
```

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/point_cloud.py` & `icepy4d-1.7.0/src/icepy4d/classes/point_cloud.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/points.py` & `icepy4d-1.7.0/src/icepy4d/classes/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,16 @@
 import time
 
 from typing import Union, List, Tuple
 from pathlib import Path
 
 from typing import List, Union
 
-if __name__ == "__main__":
-    from src.icepy4d.classes.camera import Camera
-    from src.icepy4d.classes.point_cloud import PointCloud
-else:
-    from .camera import Camera
-    from .point_cloud import PointCloud
+from .camera import Camera
+from .point_cloud import PointCloud
 
 
 def float32_type_check(
     array: np.ndarray, cast_integers: bool = False, verbose: bool = False
 ) -> np.ndarray:
     """
     float32_type_check Check if the numpy array is of type np.float32 and, if possible, return a casted array to np.float32
@@ -358,15 +354,15 @@
                 ids = range(self._last_id + 1, self._last_id + len(coordinates) + 1)
 
         if colors is not None:
             colors = np.float32(colors)
         else:
             colors = [None for _ in range(len(coordinates))]
 
-        for (id, coor, col) in zip(ids, coordinates, colors):
+        for id, coor, col in zip(ids, coordinates, colors):
             self._values[id] = Point(coor, id, color=col)
             self._last_id = id
 
     def to_numpy(self) -> np.ndarray:
         """
         to_numpy Get all points' coordinates stacked as numpy array.
```

### Comparing `icepy4d-1.6.2/src/icepy4d/classes/targets.py` & `icepy4d-1.7.0/src/icepy4d/classes/targets.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/build.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build_windows_app.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/build_windows_app.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/bundler_to_ply.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/clang_format_code.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/clang_format_code.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/crawl_camera_specs.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/database.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/database.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_matches.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_pairs.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_bundler.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_to_bundler.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_visualsfm.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/flickr_downloader.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/flickr_downloader.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/h5_to_db.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/h5_to_db.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/merge_ply_files.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/merge_ply_files.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/nvm_to_ply.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/plyfile.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/plyfile.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_dense.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/read_write_dense.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_fused_vis.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_model.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/read_write_model.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/visualize_model.py` & `icepy4d-1.7.0/src/icepy4d/io/colmap_utils/visualize_model.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/export2bundler.py` & `icepy4d-1.7.0/src/icepy4d/io/export2bundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import numpy as np
-import os
 import logging
-
-from pathlib import Path
+import os
 from copy import deepcopy
+from pathlib import Path
 from shutil import copy as scopy
-from typing import Union, List
+from typing import List, Union
+
+import numpy as np
 
+from ..classes import CamerasDict, FeaturesDict
 from ..classes.point_cloud import PointCloud
 from ..classes.points import Points
 from ..classes.targets import Targets
-from ..classes.typed_dict_classes import FeaturesDictEpoch, CamerasDictEpoch
-
 from ..thirdparty.transformations import euler_from_matrix, euler_matrix
 
 
 def create_directory(path):
     """
     Creates a directory, if it does not exist.
     """
@@ -23,16 +22,16 @@
     path.mkdir(parents=True, exist_ok=True)
     return path
 
 
 def write_bundler_out(
     export_dir: Union[str, Path],
     im_dict: dict,
-    cameras: CamerasDictEpoch,
-    features: FeaturesDictEpoch,
+    cameras: CamerasDict,
+    features: FeaturesDict,
     points: Points,
     targets: Targets = None,
     targets_to_use: List[str] = [],
     targets_enabled: List[bool] = [],
 ) -> None:
     """
     Export solution in Bundler .out format.
```

### Comparing `icepy4d-1.6.2/src/icepy4d/io/export2calge.py` & `icepy4d-1.7.0/src/icepy4d/io/export2calge.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/io/export2colmap.py` & `icepy4d-1.7.0/src/icepy4d/io/export2colmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
-import numpy as np
-
-from typing import Union
-from pathlib import Path
+from collections import defaultdict
+from copy import deepcopy
 from enum import Enum
+from pathlib import Path
+from typing import Union
 
 import h5py
-from collections import defaultdict
+import numpy as np
 import torch
-from copy import deepcopy
 
 import icepy4d.classes as icepy4d_classes
 from icepy4d.thirdparty.transformations import quaternion_from_matrix
 
 
 class CameraModels(Enum):
     PINHOLE = 0
@@ -21,15 +20,15 @@
     FULL_OPENCV = 3
 
 
 MIN_MATCHES = 20
 
 
 def features_to_h5(
-    features: icepy4d_classes.FeaturesDictEpoch, output_dir: Union[str, Path]
+    features: icepy4d_classes.FeaturesDict, output_dir: Union[str, Path]
 ) -> bool:
     key1, key2 = images[cams[0]][epoch], images[cams[1]][epoch]
 
     cams = list(features.keys())
 
     mkpts0 = features[cams[0]].kpts_to_numpy()
     mkpts1 = features[cams[1]].kpts_to_numpy()
@@ -87,20 +86,19 @@
             for k2, match in gr.items():
                 group[k2] = match
 
 
 def export_solution_to_colmap(
     export_dir: Union[str, Path],
     im_dict: dict,
-    cameras: icepy4d_classes.CamerasDictEpoch,
-    features: icepy4d_classes.FeaturesDictEpoch,
+    cameras: icepy4d_classes.CamerasDict,
+    features: icepy4d_classes.FeaturesDict,
     points: icepy4d_classes.Points,
     camera_model: CameraModels = CameraModels.OPENCV,
 ) -> bool:
-
     cams = list(cameras.keys())
     export_dir = Path(export_dir)
     export_dir.mkdir(parents=True, exist_ok=True)
 
     # Write cameras.txt
     file = open(export_dir / f"cameras.txt", "w")
     for cam_id, cam in enumerate(cams):
```

### Comparing `icepy4d-1.6.2/src/icepy4d/io/export2textfile.py` & `icepy4d-1.7.0/src/icepy4d/io/export2textfile.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/least_squares/absolute_orientation.py` & `icepy4d-1.7.0/src/icepy4d/least_squares/absolute_orientation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/least_squares/rototra3d.py` & `icepy4d-1.7.0/src/icepy4d/least_squares/rototra3d.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/least_squares/utils.py` & `icepy4d-1.7.0/src/icepy4d/least_squares/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/match_by_preselection.py` & `icepy4d-1.7.0/src/icepy4d/matching/match_by_preselection.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,30 +59,30 @@
         )
         ax.scatter(centroids[:, 0], centroids[:, 1], c="r")
 
     return (centroids, classes)
 
 
 def find_matches_on_patches(
-    images: icepy4d_classes.ImagesDict,
+    images,
     patches_lim: dict,
     epoch: int,
-    features: icepy4d_classes.FeaturesDict,
+    features,  #: icepy4d_classes.FeaturesDict,
     cfg: dict,
     do_geometric_verification: bool = True,
     geometric_verification_threshold: float = 5,
     viz_results: bool = True,
     fast_viz: bool = True,
     viz_path: Union[Path, str] = None,
 ):
     """
     Find and verify matches between patches of two images.
 
     Args:
-        images (icepy4d_classes.ImagesDict): A dictionary of `ImagesDict` instances, where each instance represents an image captured by a specific camera.
+        images (icepy4d_classes.ImagesDS): A dictionary of `ImagesDS` instances, where each instance represents an image captured by a specific camera.
         patches_lim (dict): A dictionary containing the patch limits (x1, y1, x2, y2) for each camera, where x1 and y1 are the coordinates of the top-left corner of the patch, and x2 and y2 are the coordinates of the bottom-right corner of the patch.
         epoch (int): An integer indicating the epoch number.
         features (icepy4d_classes.FeaturesDict): A dictionary of `FeaturesDict` instances, where each instance represents the detected features in an image captured by a specific camera.
         cfg (dict): A dictionary containing the configuration parameters for the matching algorithm.
         viz_results (bool, optional): A boolean indicating whether to visualize the matched features. Defaults to True.
         fast_viz (bool, optional): A boolean indicating whether to use fast visualization. Defaults to True.
         viz_path (Union[Path, str], optional): A path to the directory where the visualization results will be saved. Defaults to None.
@@ -131,38 +131,38 @@
             descr=descriptors[cam],
             scores=scores[cam],
         )
 
 
 def match_by_preselection(
     images: icepy4d_classes.ImagesDict,
-    features: icepy4d_classes.FeaturesDictEpoch,
+    features: icepy4d_classes.FeaturesDict,
     camera_names: List[str],
     epoch: int,
     cfg: edict,
     out_dir: Union[Path, str],
     n_tiles: int = 8,
     n_dist: int = 2,
     viz_results: bool = True,
     fast_viz: bool = True,
-) -> icepy4d_classes.FeaturesDictEpoch:
+):  # -> icepy4d_classes.FeaturesDict:
     """
     Matches features between two images by preselecting keypoints on downscaled images, and then refining the matches on full-resolution patches of the images.
 
     Args:
         images (icepy4d_classes.ImagesDict): A dictionary of image paths for each camera.
-        features (icepy4d_classes.FeaturesDictEpoch): A dictionary of features for each camera.
+        features (icepy4d_classes.FeaturesDict): A dictionary of features for each camera.
         epoch (int): The index of the epoch to process.
         cfg (edict): A dictionary with configuration parameters.
         n_tiles (int, optional): The number of tiles to divide the images into. Defaults to 8.
         n_dist (int, optional): The number of times the average point distance of each cluster has to be multiplied with to get the tile size. Defaults to 2.
         viz_results (bool, optional): Whether to visualize the results. Defaults to True.
         fast_viz (bool, optional): Make plot faster with opencv (it uses matplotlib otherwise). Defaults to True.
     Returns:
-        icepy4d_classes.FeaturesDictEpoch: A dictionary of refined features for each camera.
+        icepy4d_classes.FeaturesDict: A dictionary of refined features for each camera.
     """
 
     if not isinstance(cfg, dict):
         raise TypeError("opt must be a dictionary")
     required_keys = [
         "weights",
         "keypoint_threshold",
```

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/match_pairs.py` & `icepy4d-1.7.0/src/icepy4d/matching/match_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/matching_base.py` & `icepy4d-1.7.0/src/icepy4d/matching/matching_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,43 @@
 import pydegensac
 import logging
 
 from easydict import EasyDict as edict
 from typing import List, Union
 from pathlib import Path
 
-# from .utils import load_matches_from_disk
 from .match_pairs import match_pair
 from .track_matches import track_matches
 
-from ..classes.features import Features
+DEBUG = False
 
-DEBUG = True
+WRITE_RES_STATS = True
+RESULT_FNAME = "res/matching_tracking_results.txt"
+
+if WRITE_RES_STATS and not Path(RESULT_FNAME).exists():
+    sep = ","
+    items = [
+        "epoch",
+        "day_cur",
+        "day_before",
+        "n_tracked",
+        "n_new_matches",
+        "n_valid",
+    ]
+    with open(RESULT_FNAME, "w") as f:
+        f.write(f"{f'{sep}'.join(items)}\n")
 
 
 def MatchingAndTracking(
     cfg: edict,
     epoch: int,
     images: dict,
     features: dict,
     epoch_dict: dict,
 ) -> dict:
-
     epochdir = Path(cfg.paths.results_dir) / f"{epoch_dict[epoch]}/matching"
     cams = cfg.paths.camera_names
 
     # === Track previous matches at current epoch ===#
     if cfg.proc.do_tracking and epoch > 0:
         logging.info(f"Track points from epoch {epoch-1} to epoch {epoch}")
 
@@ -91,14 +103,25 @@
                 tracked_cam1["kpts"][:, 1:2],
                 tracked_cam1["descr"],
                 tracked_cam1["score"],
                 track_ids=tracked_kpts_idx,
                 epoch=epoch - 1,
             )
 
+            # Write tracking stats to file
+            if WRITE_RES_STATS:
+                with open(RESULT_FNAME, "a") as f:
+                    line = [
+                        epoch,
+                        epoch_dict[epoch],
+                        epoch_dict[epoch - 1],
+                        len(tracked_kpts_idx),
+                    ]
+                    f.write(",".join([str(x) for x in line]) + ",")
+
             # For debugging
             if DEBUG:
                 # from ..visualization.visualization import make_matching_plot
 
                 f_list = {
                     epoch: features[epoch][cams[0]]
                     for epoch in range(cfg.proc.epoch_to_process[0], epoch + 1)
@@ -124,14 +147,23 @@
                 #     path="ep180.png",
                 # )
 
         else:
             logging.warning(
                 f"Skipping tracking from epoch {epoch_dict[epoch-1]} to {epoch_dict[epoch]}"
             )
+            if WRITE_RES_STATS:
+                with open(RESULT_FNAME, "a") as f:
+                    line = [
+                        epoch,
+                        epoch_dict[epoch],
+                        epoch_dict[epoch - 1],
+                        "",
+                    ]
+                    f.write(",".join([str(x) for x in line]) + ",")
 
     # -- Find Matches at current epoch --#
     logging.info(f"Run Superglue to find matches at epoch {epoch}")
     cfg.matching.output_dir = epochdir
     pair = [
         images[cams[0]].get_image_path(epoch),
         images[cams[1]].get_image_path(epoch),
@@ -160,14 +192,19 @@
 
     # For debugging
     f_list = {
         epoch: features[epoch][cams[0]]
         for epoch in range(cfg.proc.epoch_to_process[0], epoch + 1)
     }
 
+    if WRITE_RES_STATS:
+        with open(RESULT_FNAME, "a") as f:
+            line = [epoch, len(x)]
+            f.write(f"{len(x)}" + ",")
+
     # Run Pydegensac to estimate F matrix and reject outliers
     logging.info(
         f"Geometric verification of the matches - Pydegensac parameters:  threshold {cfg.matching.pydegensac_threshold} [px], confidence: {cfg.matching.pydegensac_confidence}"
     )
     F, inlMask = pydegensac.findFundamentalMatrix(
         features[epoch][cams[0]].kpts_to_numpy(),
         features[epoch][cams[1]].kpts_to_numpy(),
@@ -182,14 +219,19 @@
     logging.info(
         f"Pydegensac found {inlMask.sum()} inliers ({inlMask.sum()*100/len(features[epoch][cams[0]]):.2f}%)"
     )
 
     features[epoch][cams[0]].filter_feature_by_mask(inlMask)
     features[epoch][cams[1]].filter_feature_by_mask(inlMask)
 
+    if WRITE_RES_STATS:
+        with open(RESULT_FNAME, "a") as f:
+            line = [epoch, len(x)]
+            f.write(f"{len(features[epoch][cams[0]])}" + "\n")
+
     # Write matched points to disk
     im_stems = (
         images[cams[0]].get_image_stem(epoch),
         images[cams[1]].get_image_stem(epoch),
     )
     for jj, cam in enumerate(cams):
         features[epoch][cam].save_as_txt(epochdir / f"{im_stems[jj]}_mktps.txt")
```

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/retrieve_matches_from_npz.py` & `icepy4d-1.7.0/src/icepy4d/matching/retrieve_matches_from_npz.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/superglue_match_simple_old.py` & `icepy4d-1.7.0/src/icepy4d/matching/superglue_match_simple_old.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/superglue_matcher.py` & `icepy4d-1.7.0/src/icepy4d/matching/superglue_matcher.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/superglue_tracker.py` & `icepy4d-1.7.0/src/icepy4d/matching/superglue_tracker.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/templatematch.py` & `icepy4d-1.7.0/src/icepy4d/matching/templatematch.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/track_matches.py` & `icepy4d-1.7.0/src/icepy4d/matching/track_matches.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from icepy4d.thirdparty.SuperGlue.models.utils import (
     make_matching_plot,
     AverageTimer,
     process_resize,
     frame2tensor,
 )
 from icepy4d.utils.tiles import generateTiles
-from icepy4d.utils.spatial_funs import point_in_rect
+from icepy4d.utils.geospatial import point_in_rect
 
 torch.set_grad_enabled(False)
 
 # SuperPoint Parameters
 NMS_RADIUS = 3
 
 # SuperGlue Parameters
```

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/track_matches_bk.py` & `icepy4d-1.7.0/src/icepy4d/matching/track_matches_bk.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/tracking_base.py` & `icepy4d-1.7.0/src/icepy4d/matching/tracking_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 import icepy4d.classes as icepy4d_classes
 from icepy4d.classes.features import Features
 from icepy4d.utils.timer import AverageTimer
 
 
 def tracking_base(
     images: icepy4d_classes.ImagesDict,
-    prev_features: icepy4d_classes.FeaturesDictEpoch,
+    prev_features: icepy4d_classes.FeaturesDict,
     camera_names: List[str],
     epoch_dict: icepy4d_classes.EpochDict,
     epoch: int,
     cfg: edict,
     epoch_dir: Union[Path, str],
-) -> icepy4d_classes.FeaturesDictEpoch:
+) -> icepy4d_classes.FeaturesDict:
     if not isinstance(cfg, dict):
         raise TypeError("opt must be a dictionary")
     required_keys = [
         "weights",
         "keypoint_threshold",
         "max_keypoints",
         "match_threshold",
```

### Comparing `icepy4d-1.6.2/src/icepy4d/matching/utils.py` & `icepy4d-1.7.0/src/icepy4d/matching/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/metashape/metashape.py` & `icepy4d-1.7.0/src/icepy4d/metashape/metashape.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     create_new_project,
     save_project,
     cameras_from_bundler,
     add_markers,
     read_gcp_file,
 )
 from icepy4d.utils.timer import AverageTimer
-from icepy4d.io.importing import read_opencv_calibration
+from icepy4d.classes.calibration import read_opencv_calibration
 
 REGION_RESIZE_FCT = 10.0
 
 
 def build_metashape_cfg(cfg: edict, epoch_dict: dict, cur_epoch: int) -> edict:
     """
     # build_metashape_cfg Build metashape configuration dictionary, starting from global configuration dictionary.
```

### Comparing `icepy4d-1.6.2/src/icepy4d/metashape/metashape_core.py` & `icepy4d-1.7.0/src/icepy4d/metashape/metashape_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import numpy as np
 import logging
 
 from typing import List
 from typing import Union
 from pathlib import Path
 
-from ..io.importing import read_opencv_calibration
+from icepy4d.classes.calibration import read_opencv_calibration
 
 """ License """
 
 
 def check_license() -> None:
     if Metashape.app.activated:
         logging.info("Metashape is activated: ", Metashape.app.activated)
@@ -181,14 +181,54 @@
         )
     return gcps
 
 
 """Output"""
 
 
+def export_tie_points_world(
+    chunk: Metashape.Chunk,
+    file_name: str,
+    expot_covariance_mat: bool = False,
+) -> None:
+    """Export tie points in world coordinates to a file.
+
+    Args:
+        chunk: A Metashape Chunk object containing the tie points.
+        file_name: A string specifying the name of the output file.
+        export_covariance_mat: A boolean indicating whether to export covariance matrix. If false, export only standard deviation of 3D coordinates of each point. Default is False.
+
+    Returns:
+        None
+
+
+    """
+    with open(file_name, "w") as f:
+        if expot_covariance_mat:
+            f.write("track_id,x,y,z,c11,c12,c13,c21,c22,c23,c31,c32,c33\n")
+        else:
+            f.write("track_id,x,y,z,sx,sy,sz\n")
+        for point in chunk.point_cloud.points:
+            track_id = point.track_id
+            valid = point.valid
+            if not valid:
+                continue
+            coord = point.coord
+            cov = point.cov
+            f.write(f"{track_id},{coord[0]},{coord[1]},{coord[2]},")
+            if expot_covariance_mat:
+                f.write(f"{cov[0,0]},{cov[0,1]},{cov[0,2]},")
+                f.write(f"{cov[1,0]},{cov[1,1]},{cov[1,2]},")
+                f.write(f"{cov[2,0]},{cov[2,1]},{cov[2,2]},")
+            else:
+                f.write(f"{np.sqrt(cov[0,0])},{np.sqrt(cov[1,1])},{np.sqrt(cov[2,2])},")
+            f.write("\n")
+    print(f"Tie points exported to {file_name}.")
+
+
 def write_markers_by_camera(
     chunk: Metashape.Chunk,
     file_name: str,
     convert_to_micron: bool = False,
 ) -> None:
     """Write Marker image coordinates to csv file,
     sort by camera, as follows:
```

### Comparing `icepy4d-1.6.2/src/icepy4d/point_cloud_proc/cloudcompare_fun.py` & `icepy4d-1.7.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/point_cloud_proc/open3d_fun.py` & `icepy4d-1.7.0/src/icepy4d/point_cloud_proc/open3d_fun.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Union, List
 
 import numpy as np
 import open3d as o3d
 from easydict import EasyDict as edict
 from matplotlib import path as mpath
 
-from icepy4d.utils.spatial_funs import ccw_sort_points, point_in_hull
+from icepy4d.utils.geospatial import ccw_sort_points, point_in_hull
 from icepy4d.utils.timer import AverageTimer
 
 # def filter_mesh_by_convex_hull(mesh, pcd):
 #     convex_hull = pcd.compute_convex_hull()
 
 #     keep = point_in_hull(np.asarray(mesh.vertices), np.asarray(convex_hull.vertices))
 #     idx = list(compress(range(len(keep)), keep))
```

### Comparing `icepy4d-1.6.2/src/icepy4d/point_cloud_proc/utils.py` & `icepy4d-1.7.0/src/icepy4d/point_cloud_proc/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/sfm/absolute_orientation.py` & `icepy4d-1.7.0/src/icepy4d/sfm/absolute_orientation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/sfm/geometry.py` & `icepy4d-1.7.0/src/icepy4d/sfm/geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/sfm/reconstruction.py` & `icepy4d-1.7.0/src/icepy4d/sfm/reconstruction.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/sfm/triangulation.py` & `icepy4d-1.7.0/src/icepy4d/sfm/triangulation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/sfm/two_view_geometry.py` & `icepy4d-1.7.0/src/icepy4d/sfm/two_view_geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/matching.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/matching.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/superglue.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/superglue.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/superpoint.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/utils.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/SuperGlue/models/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/templatematch_pyimgraft.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/transformations.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/transformations.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/thirdparty/triangulation.py` & `icepy4d-1.7.0/src/icepy4d/thirdparty/triangulation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/binned_stats.py` & `icepy4d-1.7.0/src/icepy4d/utils/binned_stats.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import numpy as np
-import cv2
 import logging
-
-from pathlib import Path
-from matplotlib import pyplot as plt
 from datetime import datetime
+from pathlib import Path
 from typing import List, Tuple
+
+import cv2
+import numpy as np
+from matplotlib import pyplot as plt
 from scipy.stats import binned_statistic_2d, binned_statistic_dd
 
 
 def bins_from_nodes(x_nodes: List, y_nodes: List) -> Tuple[List]:
     """Divides a 2D space into bins based on the x and y coordinates of the nodes.
 
     Args:
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/dsm_orthophoto.py` & `icepy4d-1.7.0/src/icepy4d/utils/dsm_orthophoto.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         # plt.show()
         if save_path is not None:
             plt.savefig(save_fld.joinpath(save_stem + "_plot.png"), bbox_inches="tight")
 
     # Save dsm as GeoTIff
     if save_path is not None:
         save_path = Path(save_path)
-        save_path.mkdir(parents=True, exist_ok=True)
+        save_path.parent.mkdir(parents=True, exist_ok=True)
         rater_origin = [xlim[0] - dsm_step / 2, ylim[0] - dsm_step / 2]
         transform = Affine.translation(rater_origin[0], rater_origin[1]) * Affine.scale(
             dsm_step, -dsm_step
         )
         mask = np.invert(np.isnan(dsm_grid))
         rater_origin = [grid_x[0, 0], grid_y[0, 0]]
         transform = Affine.translation(rater_origin[0], rater_origin[1]) * Affine.scale(
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/initialization.py` & `icepy4d-1.7.0/src/icepy4d/utils/initialization.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,34 +18,40 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import numpy as np
-import yaml
+import argparse
 import logging
 import sys
-import argparse
-
-from easydict import EasyDict as edict
-from pathlib import Path
-from typing import List, Union, Tuple, TypedDict
 from datetime import datetime
+from pathlib import Path
 from pprint import pprint
+from typing import List, Tuple, TypedDict, Union
 
-from icepy4d.classes.camera import Camera
-from icepy4d.classes.features import Features
-from icepy4d.classes.points import Points
-from icepy4d.classes.point_cloud import PointCloud
-from icepy4d.classes.images import Image, ImageDS
-from icepy4d.classes.targets import Targets
-from icepy4d.classes.typed_dict_classes import *
+import numpy as np
+import yaml
+from easydict import EasyDict as edict
 
+from icepy4d.classes import (
+    Calibration,
+    Camera,
+    CamerasDict,
+    Epoch,
+    Features,
+    FeaturesDict,
+    Image,
+    ImageDS,
+    ImagesDict,
+    PointCloud,
+    Points,
+    Targets,
+)
 
 """ 
 This file defines the dictionary cfg which includes the default parameters of the pipeline.
 The dictionary is updated/extended at runtime with the parameters defined by the user in the input yaml config file
 """
 
 
@@ -138,49 +144,64 @@
         edict: A dictionary-like object containing the configuration parameters.
     """
 
     cfg_file = Path(cfg_file)
     if not cfg_file.exists():
         sys.exit("Configuration file does not exist! Aborting.")
 
-    with open(cfg_file) as file:
-        cfg = edict(yaml.safe_load(file))
-    assert isinstance(
-        cfg, edict
-    ), "Unable to create valid cfg dictionary from yaml file"
+    try:
+        with open(cfg_file) as file:
+            cfg = edict(yaml.safe_load(file))
+    except:
+        raise RuntimeError("Unable to create valid cfg dictionary from yaml file")
+
+    # Camera names
+    cfg.cams = cfg.paths.camera_names
 
     # - Data paths
     root_path = Path().absolute()
     cfg.paths.root_path = root_path
     cfg.paths.image_dir = root_path / Path(cfg.paths.image_dir)
     cfg.paths.calibration_dir = root_path / Path(cfg.paths.calibration_dir)
     cfg.paths.results_dir = root_path / Path(cfg.paths.results_dir)
 
+    # - Result paths
+    cfg.camea_estimated_fname = cfg.paths.results_dir / "camera_info_est.txt"
+    cfg.residuals_fname = cfg.paths.results_dir / "residuals_image.txt"
+    cfg.matching_stats_fname = cfg.paths.results_dir / "matching_tracking_results.txt"
+
+    # remove files if they already exist
+    if cfg.camea_estimated_fname.exists():
+        cfg.camea_estimated_fname.unlink()
+    if cfg.residuals_fname.exists():
+        cfg.residuals_fname.unlink()
+    if cfg.matching_stats_fname.exists():
+        cfg.matching_stats_fname.unlink()
+
     # - Processing options
     if cfg.proc.do_matching == False and cfg.proc.do_tracking == True:
         logging.warning(
             "Invalid combination of Matching and Tracking options. Tracking was se to enabled, but Matching was not. Disabling Tracking."
         )
         cfg.proc.do_tracking == False
 
     # - Image-realted options
     cfg.images.mask_bounding_box = np.array(cfg.images.mask_bounding_box).astype("int")
 
     # - Georef options
     cfg.georef.camera_centers_world = np.array(cfg.georef.camera_centers_world)
     cfg.georef.target_dir = Path(cfg.georef.target_dir)
 
-    # Check and expand epoches to be processed
+    # - Check and expand epoches to be processed
     if cfg.proc.epoch_to_process == "all":
         logging.info(
             "Epoch_to_process set to 'all'. Expanding it based on the images found in image folder."
         )
-        cams = cfg.paths.camera_names
-        img_ds = dict.fromkeys(cams)
-        img_ds = ImageDS(cfg.paths.image_dir / cams[0])
+        img_ds = dict.fromkeys(cfg.cams)
+        img_ds = ImageDS(cfg.paths.image_dir / cfg.cams[0])
         n_images = len(img_ds)
         cfg.proc.epoch_to_process = [x for x in range(n_images)]
     elif len(cfg.proc.epoch_to_process) == 2:
         logging.info(
             f"Epoch_to_process set to a pair of values. Expanding it for a range of epoches from epoch {cfg.proc.epoch_to_process[0]} to {cfg.proc.epoch_to_process[1]}."
         )
         ep_ini = cfg.proc.epoch_to_process[0]
@@ -223,14 +244,15 @@
     pprint(dict(cfg), indent=2)
 
 
 def download_model():
     """
     Download the model from the internet.
     """
+    pass
 
 
 class Inizializer:
     def __init__(
         self,
         cfg: edict,
     ) -> None:
@@ -245,82 +267,196 @@
 
         self.cfg = cfg
         assert (
             "camera_names" in self.cfg.paths
         ), "Camera names not available in cfg file."
         self.cams = self.cfg.paths.camera_names
 
-    def init_image_ds(self) -> ImagesDict:
+    def init_image_ds(self):
         """
         init_image_ds _summary_
 
         Returns:
             ImagesDict: _description_
         """
-        self.images: ImagesDict = {
+        self.images = {
             cam: ImageDS(self.cfg.paths.image_dir / cam) for cam in self.cams
         }
         for cam in self.cams:
             self.images[cam].write_exif_to_csv(
                 self.cfg.paths.image_dir / f"image_list_{cam}.csv"
             )
-
         return self.images
 
-    def init_epoch_dict(self) -> EpochDict:
+    def init_epoch_dict(self):
         """
         init_epoch_dict Build dictonary containing pairs of epoch and dates, as follows:
         {0: "2021_01_01", 1: "2021_01_02" ...}
 
         Returns:
             EpochDict: epoc_dict
         """
-        self.epoch_dict: EpochDict = {}
+        self.epoch_dict = {}
         for epoch in range(len(self.images[self.cams[0]])):
             date_str = self.images[self.cams[0]].get_image_date(epoch)
             date = datetime.strptime(date_str, "%Y:%m:%d")
             self.epoch_dict[epoch] = f"{date.year}_{date.month:02}_{date.day:02}"
         return self.epoch_dict
 
-    def init_cameras(self) -> CamerasDict:
+    def init_features(self):
+        """
+        init_features _summary_
+
+        Returns:
+            _type_: _description_
+
+        NOTE: This function is deprecated. It is kept for backward compatibility with the function MatchingAndTracking that require the full dictionary of features as input. It will be removed in future versions.
+        """
+        logging.warning(
+            "This function is deprecated. It is kept for backward compatibility with the function MatchingAndTracking that require the full dictionary of features as input. It will be removed in future versions."
+        )
+        self.features = {}
+        for epoch in self.cfg.proc.epoch_to_process:
+            self.features[epoch] = {cam: Features() for cam in self.cams}
+
+        return self.features
+
+    def init_epoch(self, epoch_id: int, epoch_dir: Union[Path, str] = None):
+        """
+        init_epoch _summary_
+
+        Returns:
+            Epoch: _description_
+        """
+
+        # Build dictionary of Images for the current epoch
+        im_epoch: ImagesDict = {
+            cam: Image(self.images[cam].get_image_path(epoch_id)) for cam in self.cams
+        }
+
+        # Load cameras
+        cams_ep: CamerasDict = {}
+        for cam in self.cams:
+            calib = Calibration(self.cfg.paths.calibration_dir / f"{cam}.txt")
+            cams_ep[cam] = calib.to_camera()
+
+        # Load targets
+        target_paths = [
+            self.cfg.georef.target_dir
+            / (im_epoch[cam].stem + self.cfg.georef.target_file_ext)
+            for cam in self.cams
+        ]
+        targ_ep = Targets(
+            im_file_path=target_paths,
+            obj_file_path=self.cfg.georef.target_dir
+            / self.cfg.georef.target_world_file,
+        )
 
+        # init empty features and points
+        feat_ep = {cam: Features() for cam in self.cams}
+        pts_ep = Points()
+
+        epoch = Epoch(
+            im_epoch[self.cams[0]].datetime,
+            images=im_epoch,
+            cameras=cams_ep,
+            features=feat_ep,
+            points=pts_ep,
+            targets=targ_ep,
+            point_cloud=None,
+            epoch_dir=epoch_dir,
+        )
+        return epoch
+
+
+class Inizializer_old:
+    def __init__(
+        self,
+        cfg: edict,
+    ) -> None:
+        """
+        __init__ initialization class
+
+        Args:
+            cfg (edict): dictionary (as EasyDict object) containing all the configuration parameters.
+
+        NOTE: This old class do not use Epoch as main container for all the variables. Use Inizializer instead
+        """
+
+        print_welcome_msg()
+
+        self.cfg = cfg
+        assert (
+            "camera_names" in self.cfg.paths
+        ), "Camera names not available in cfg file."
+        self.cams = self.cfg.paths.camera_names
+
+    def init_image_ds(self):  # -> ImagesDict:
+        """
+        init_image_ds _summary_
+
+        Returns:
+            ImagesDict: _description_
+        """
+        self.images = {
+            cam: ImageDS(self.cfg.paths.image_dir / cam) for cam in self.cams
+        }
+        for cam in self.cams:
+            self.images[cam].write_exif_to_csv(
+                self.cfg.paths.image_dir / f"image_list_{cam}.csv"
+            )
+        return self.images
+
+    def init_epoch_dict(self):
+        """
+        init_epoch_dict Build dictonary containing pairs of epoch and dates, as follows:
+        {0: "2021_01_01", 1: "2021_01_02" ...}
+
+        Returns:
+            EpochDict: epoc_dict
+        """
+        self.epoch_dict = {}
+        for epoch in range(len(self.images[self.cams[0]])):
+            date_str = self.images[self.cams[0]].get_image_date(epoch)
+            date = datetime.strptime(date_str, "%Y:%m:%d")
+            self.epoch_dict[epoch] = f"{date.year}_{date.month:02}_{date.day:02}"
+        return self.epoch_dict
+
+    def init_cameras(self):
         assert hasattr(
             self, "images"
         ), "Images datastore not available yet. Inizialize images first"
         img = Image(self.images[self.cams[0]].get_image_path(0))
         im_height, im_width = img.height, img.width
 
         # Inizialize Camera Intrinsics at every epoch setting them equal to the those of the reference cameras.
-        self.cameras: CamerasDict = {}
+        self.cameras = {}
         for epoch in self.cfg.proc.epoch_to_process:
-            self.cameras[epoch]: CamerasDictEpoch = {
+            self.cameras[epoch] = {
                 cam: Camera(
                     width=im_width,
                     height=im_height,
                     calib_path=self.cfg.paths.calibration_dir / f"{cam}.txt",
                 )
                 for cam in self.cams
             }
 
         return self.cameras
 
-    def init_features(self) -> FeaturesDict:
-        self.features: FeaturesDict = {}
+    def init_features(self):
+        self.features = {}
         for epoch in self.cfg.proc.epoch_to_process:
-            self.features[epoch]: FeaturesDictEpoch = {
-                cam: Features() for cam in self.cams
-            }
+            self.features[epoch] = {cam: Features() for cam in self.cams}
 
         return self.features
 
-    def init_targets(self) -> TargetDict:
+    def init_targets(self):
         # Read target image coordinates and object coordinates
-        self.targets: TargetDict = {}
+        self.targets = {}
         for epoch in self.cfg.proc.epoch_to_process:
-
             p1_path = self.cfg.georef.target_dir / (
                 self.images[self.cams[0]].get_image_stem(epoch)
                 + self.cfg.georef.target_file_ext
             )
 
             p2_path = self.cfg.georef.target_dir / (
                 self.images[self.cams[1]].get_image_stem(epoch)
@@ -331,43 +467,29 @@
                 im_file_path=[p1_path, p2_path],
                 obj_file_path=self.cfg.georef.target_dir
                 / self.cfg.georef.target_world_file,
             )
 
         return self.targets
 
-    def init_points(self) -> PointsDict:
-        self.points: PointsDict = {
-            ep: Points() for ep in self.cfg.proc.epoch_to_process
-        }
+    def init_points(self):
+        self.points = {ep: Points() for ep in self.cfg.proc.epoch_to_process}
         return self.points
 
-    def init_point_cloud(self) -> PointCloudDict:
-        self.point_clouds: PointCloudDict = {
-            ep: None for ep in self.cfg.proc.epoch_to_process
-        }
+    def init_point_cloud(self):
+        self.point_clouds = {ep: None for ep in self.cfg.proc.epoch_to_process}
         return self.point_clouds
 
     def init_focals_dict(self) -> dict:
         self.focals_dict = dict.fromkeys(self.cams)
         for cam in self.cams:
             self.focals_dict[cam] = {}
 
-    def inizialize_icepy4d(self) -> dict:
-        self.init_image_ds()
-        self.init_epoch_dict()
-        self.init_cameras()
-        self.init_features()
-        self.init_targets()
-        self.init_points()
-        self.init_focals_dict()
-
 
 if __name__ == "__main__":
-
     cfg_file = "./config/config_base.yaml"
     cfg = parse_yaml_cfg(cfg_file)
 
     print(cfg)
 
     init = Inizializer(cfg)
     init.init_image_ds()
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/logger.py` & `icepy4d-1.7.0/src/icepy4d/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 #  Based on:                                                                   -
 #  https://stackoverflow.com/a/13733863/1976617
 #  https://uran198.github.io/en/python/2016/07/12/colorful-python-logging.html
 #  https://en.wikipedia.org/wiki/ANSI_escape_code#Colors
 #
 # -------------------------------------------------------------------------------
 
-# Imports
-import sys
 import logging
-
+import sys
 from datetime import date, datetime
 from pathlib import Path
 
+
 # Logging formatter supporting colorized output
 class LogFormatter(logging.Formatter):
-
     COLOR_CODES = {
         logging.CRITICAL: "\033[1;35m",  # bright/bold magenta
         logging.ERROR: "\033[1;31m",  # bright/bold red
         logging.WARNING: "\033[1;33m",  # bright/bold yellow
         logging.INFO: "\033[0;37m",  # white / light gray
         logging.DEBUG: "\033[1;30m",  # bright/bold black / dark gray
     }
@@ -53,15 +51,14 @@
     console_log_level,
     console_log_color,
     logfile_file,
     logfile_log_level,
     logfile_log_color,
     log_line_template,
 ):
-
     # Create logger
     # For simplicity, we use the root logger, i.e. call 'logging.getLogger()'
     # without name argument. This way we can simply use module methods for
     # for logging throughout the script. An alternative would be exporting
     # the logger, i.e. 'global logger; logger = logging.getLogger("<name>")'
     logger = logging.getLogger()
 
@@ -160,15 +157,14 @@
     ):
         print("Failed to setup logging, aborting.")
         raise RuntimeError
 
 
 # Call main function
 if __name__ == "__main__":
-
     CONSOLE_LOG_LEVEL = "info"
     LOGFILE_LEVEL = "debug"
     LOG_FOLDER = "logs"
     LOG_BASE_NAME = "icepy4d"
 
     # Setup logger
     setup_logger(LOG_FOLDER, LOG_BASE_NAME, CONSOLE_LOG_LEVEL, LOGFILE_LEVEL)
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/math.py` & `icepy4d-1.7.0/src/icepy4d/utils/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,16 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import cv2
 import numpy as np
 
-from copy import deepcopy
-from pathlib import Path
-
-
 # --- MAT ---#
 
 
 def convert_to_homogeneous(x):
     """
     Convert 2xn or 3xn vector of n points in euclidean coordinates
     to a 3xn or 4xn vector homogeneous by adding a row of ones
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/sensor_width_database.py` & `icepy4d-1.7.0/src/icepy4d/classes/sensor_width_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 """
 
 import pandas as pd
 
 from pathlib import Path
 
 DEFAULT_SENSOR_DB_PATH = (
-    Path("thirdparty/CameraSensorSizeDatabase") / "sensor_database.csv"
+    Path.cwd() / "src/icepy4d/thirdparty/CameraSensorSizeDatabase/sensor_database.csv"
 )
 
 
 class SensorWidthDatabase:
     """Database class for sensor-width, reading data from a csv file."""
 
     def __init__(self, csv_path: str = DEFAULT_SENSOR_DB_PATH):
         """Initializes the database from a csv file"""
 
+        assert Path(csv_path).exists(), f"csv_path='{csv_path}' does not exist"
+
         self.df = pd.read_csv(csv_path)
 
         # convert string to lower-case
         self.df["CameraMaker"] = self.df["CameraMaker"].str.lower()
         self.df["CameraModel"] = self.df["CameraModel"].str.lower()
 
     def lookup(self, make: str, model: str) -> float:
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/spatial_funs.py` & `icepy4d-1.7.0/src/icepy4d/utils/geospatial.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/tiles.py` & `icepy4d-1.7.0/src/icepy4d/utils/tiles.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,105 +29,152 @@
 import logging
 
 from pathlib import Path
 from typing import List
 
 from icepy4d.classes.images import Image, ImageDS
 
+# TODO: use KORNIA for image tiling
+
+
+import logging
+from typing import List, Dict
+import numpy as np
+import matplotlib.pyplot as plt
+from PIL import Image
+
 
 class Tiler:
     """
     Class for dividing an image into tiles.
     """
 
     def __init__(
         self,
         image: Image,
         grid: List[int] = [1, 1],
         overlap: int = 0,
         origin: List[int] = [0, 0],
     ) -> None:
-        """Initialize class
-        Parameters
-        __________
-        - image (Image):
-        - grid (List[int], default=[1, 1]): List containing the number of rows and number of colums in which to divide the image ([nrows, ncols])
-        - overlap (int, default=0): Number of pixel of overlap between adiacent tiles
-        - origin (List[int], default=[0, 0]): List of coordinates [x,y] of the pixel from which the tiling starts (top-left corner of the first tile)
-        __________
-        Return: None
         """
+        Initialize class.
 
+        Parameters:
+        - image (Image): The input image.
+        - grid (List[int], default=[1, 1]): List containing the number of rows and number of columns in which to divide the image ([nrows, ncols]).
+        - overlap (int, default=0): Number of pixels of overlap between adjacent tiles.
+        - origin (List[int], default=[0, 0]): List of coordinates [x, y] of the pixel from which the tiling starts (top-left corner of the first tile).
+
+        Returns:
+        None
+        """
         self._image = image
         self._im_path = image.path
         self._w = int(self._image.width)
         self._h = int(self._image.height)
         self._origin = origin
         self._overlap = overlap
         self._nrow = grid[0]
         self._ncol = grid[1]
-        self.limits = {}
-        self.tiles = {}
+        self._limits = {}
+        self._tiles = {}
 
     @property
-    def grid(self) -> List:
+    def grid(self) -> List[int]:
+        """
+        Get the grid size.
+
+        Returns:
+        List[int]: The number of rows and number of columns in the grid.
+        """
         return [self._nrow, self._ncol]
 
     @property
-    def tiles_limits(self) -> dict:
-        if not dict:
-            return self.limits
-        else:
-            logging.warning(
+    def limits(self) -> Dict[int, tuple]:
+        """
+        Get the tile limits.
+
+        Returns:
+        dict: A dictionary containing the index of each tile and its bounding box coordinates.
+        """
+        if not self._limits:
+            raise ValueError(
                 "Limits not available, compute them first with compute_limits_by_grid."
             )
+        return self._limits
 
     def compute_limits_by_grid(self) -> None:
-        """Method to compute the limits of each tile (i.e. xmin,ymin,xmax,xmax), given the number or row and columns of the tile grid.
-
-        Returns a dictionary containing the index of the tile (in row-major order, C-style) and a list of the bounding box coordinates as:
-        {0,[xmin, xmax, ymin, ymax]}
-        {1,[xmin, xmax, ymin, ymax]}
-        ....
         """
+        Compute the limits of each tile (i.e., xmin, ymin, xmax, ymax) given the number of rows and columns in the tile grid.
 
+        Returns:
+        None
+        """
         DX = round((self._w - self._origin[0]) / self._ncol / 10) * 10
         DY = round((self._h - self._origin[1]) / self._nrow / 10) * 10
 
         for col in range(self._ncol):
             for row in range(self._nrow):
                 tile_idx = np.ravel_multi_index(
                     (row, col), (self._nrow, self._ncol), order="C"
                 )
                 xmin = max(self._origin[0], col * DX - self._overlap)
                 ymin = max(self._origin[1], row * DY - self._overlap)
                 xmax = xmin + DX + self._overlap - 1
                 ymax = ymin + DY + self._overlap - 1
-                self.limits[tile_idx] = (xmin, ymin, xmax, ymax)
+                self._limits[tile_idx] = (xmin, ymin, xmax, ymax)
 
     def read_all_tiles(self) -> None:
-        """Read all tiles and store them in class instance"""
+        """
+        Read all tiles and store them in the class instance.
+
+        Returns:
+        None
+        """
         assert self._im_path is not None, "Invalid image path"
-        for idx, limit in self.limits.items():
-            self.tiles[idx] = self._image.extract_patch(limit)
+        for idx, limit in self._limits.items():
+            self._tiles[idx] = self._image.extract_patch(limit)
 
     def read_tile(self, idx) -> np.ndarray:
-        """Extract tile given its idx (int) and return it"""
+        """
+        Extract and return a tile given its index.
+
+        Parameters:
+        - idx (int): The index of the tile.
+
+        Returns:
+        np.ndarray: The extracted tile.
+        """
         assert self._im_path is not None, "Invalid image path"
-        return self._image.extract_patch(self.limits[idx])
+        return self._image.extract_patch(self._limits[idx])
+
+    def remove_tiles(self, tile_idx=None) -> None:
+        """
+        Remove tiles from the class instance.
 
-    def remove_tiles(self, tile_idx) -> None:
+        Parameters:
+        - tile_idx: The index of the tile to be removed. If None, remove all tiles.
+
+        Returns:
+        None
+        """
         if tile_idx is None:
-            self.tiles = {}
+            self._tiles = {}
         else:
-            self.tiles[tile_idx] = []
+            self._tiles[tile_idx] = []
 
     def display_tiles(self) -> None:
-        for idx, tile in self.tiles.items():
-            plt.subplot(tile_grid[0], tile_grid[1], idx + 1)
+        """
+        Display all the stored tiles.
+
+        Returns:
+        None
+        """
+        for idx, tile in self._tiles.items():
+            plt.subplot(self.grid[0], self.grid[1], idx + 1)
             plt.imshow(tile)
         plt.show()
 
     # def write_tiles_to_disk(self, ) -> None:
     #             isExist = os.path.exists(out_dir)
     #             if not isExist:
     #                 os.makedirs(out_dir)
@@ -219,11 +266,18 @@
         img,
         grid=tile_grid,
         origin=origin,
     )
 
     tiles.compute_limits_by_grid()
 
-    # t = tiles.read_tile(1)
+    t = tiles.read_tile(1)
 
     tiles.read_all_tiles()
     tiles.display_tiles()
+
+    grid = tiles.grid
+    limits = tiles.limits
+
+    print(grid)
+
+    print("Done")
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/timer.py` & `icepy4d-1.7.0/src/icepy4d/utils/timer.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/tracking_features_utils.py` & `icepy4d-1.7.0/src/icepy4d/utils/tracking_features_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import TypedDict, List, Union
 from pathlib import Path
 from itertools import groupby, product
 
 import icepy4d.classes as icepy4d_classes
 
-from icepy4d.utils.spatial_funs import *
+from icepy4d.utils.geospatial import *
 from icepy4d.utils.timer import timeit
 
 
 class FeaturesDictByCam(TypedDict):
     epoch: icepy4d_classes.Features
 
 
@@ -31,15 +31,15 @@
     Args:
         features (icepy4d_classes.FeaturesDict): A dictionary of features, where the keys are epochs and the values are dictionaries of features for each camera.
         cam (str): The camera identifier to sort the features by.
 
     Returns:
         FeaturesDictByCam: A dictionary of features sorted by camera, where the keys are epochs and the values are the features for the specified camera.
     """
-    f_by_cam: FeaturesDictByCam = {ep: features[ep][cam] for ep in features.keys()}
+    f_by_cam: FeaturesDictByCam = {ep: epoch.features[cam] for ep in features.keys()}
     return f_by_cam
 
 
 # @timeit
 # def tracked_features_time_series(
 #     fdict: FeaturesDictByCam,
 #     min_tracked_epoches: int = 1,
@@ -190,22 +190,22 @@
 
     epoches = list(points.keys())
     pts = {}
     for i, epoch in enumerate(epoches):
         track_ids = points[epoch].get_track_ids()
         for track_id in track_ids:
             if volume is None:
-                out = [ep for ep in epoches[i:] if track_id in points[ep]]
+                out = [ep for ep in epoches[i:] if track_id in epoch.points]
             else:
                 out = [
                     ep
                     for ep in epoches[i:]
                     if (
-                        track_id in points[ep]
-                        and point_in_volume(points[ep][track_id].coordinates, volume)
+                        track_id in epoch.points
+                        and point_in_volume(epoch.points[track_id].coordinates, volume)
                     )
                 ]
             if not out:
                 continue
             if len(out) < min_tracked_epoches:
                 continue
             if track_id not in pts.keys():
```

### Comparing `icepy4d-1.6.2/src/icepy4d/utils/transformations.py` & `icepy4d-1.7.0/src/icepy4d/utils/transformations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,102 +1,35 @@
 import numpy as np
 import pandas as pd
+import open3d as o3d
 
 from pathlib import Path
 from typing import Union, List
 
-" Transformation for Belvedere North-West terminus, from Local RS to WGS84-UTM32N "
-
-
-def belvedere_loc2utm() -> np.ndarray:
-    BELV_LOC2UTM = np.array(
-        [
-            [0.706579327583, -0.70687371492, -0.00012600114, 416614.833],
-            [0.706873714924, 0.706579267979, 0.000202054813, 5090932.706],
-            [-0.00005382637, -0.00023195939, 0.999462246895, 1767.547],
-            [0.0, 0.0, 0.0, 1.0],
-        ]
-    )
-    return BELV_LOC2UTM
-
-
-def belvedere_utm2loc() -> np.ndarray:
-    BELV_UTM2LOC = np.linalg.inv(belvedere_loc2utm())
-    return BELV_UTM2LOC
-
-
-def convert_to_homogeneous(x: np.ndarray) -> np.ndarray:
-    """Converts a 2xn or 3xn vector of n points in euclidean coordinates to a 3xn or 4xn vector in homogeneous coordinates by adding a row of ones.
-
-    Args:
-        x (np.ndarray): A numpy array with shape 2xn or 3xn, representing the euclidean
-            coordinates of n points.
-
-    Returns:
-        np.ndarray: A numpy array with shape 3xn or 4xn, representing the homogeneous
-        coordinates of the same n points.
-    """
-    x = np.array(x)
-    ndim, npts = x.shape
-    if ndim != 2 and ndim != 3:
-        print(
-            "Error: wrong number of dimension of the input vector.\
-            A number of dimensions (rows) of 2 or 3 is required."
-        )
-        return None
-    x1 = np.concatenate((x, np.ones((1, npts), "float32")), axis=0)
-    return x1
-
-
-def convert_from_homogeneous(x: np.ndarray) -> np.ndarray:
-    """
-    Convert 3xn or 4xn vector of n points in homogeneous coordinates
-    to a 2xn or 3xn vector in euclidean coordinates, by dividing by the
-    homogeneous part of the vector (last row) and removing one dimension
-    """
-    x = np.array(x)
-    ndim, npts = x.shape
-    if ndim != 3 and ndim != 4:
-        print(
-            "Error: wrong number of dimension of the input vector.\
-            A number of dimensions (rows) of 2 or 3 is required."
-        )
-        return None
-    x1 = x[: ndim - 1, :] / x[ndim - 1, :]
-    return x1
-
-
-def get_coordinates_from_df(
-    df: pd.DataFrame,
-    to_homogeneous: bool = False,
-) -> np.ndarray:
-    """Extracts the 3D coordinates of a point cloud from a pandas DataFrame.
-
-    Args:
-        df: A pandas DataFrame with columns "X", "Y" and "Z".
-        to_homogeneous: A boolean indicating whether to convert the coordinates
-            to homogeneous coordinates or not.
-
-    Returns:
-        A numpy array with shape mx3 or mx4, representing the 3D coordinates
-        of a point cloud with m points, in euclidean or homogeneous coordinates.
-    """
-    xyz = df[["X", "Y", "Z"]].to_numpy()
-    if to_homogeneous:
-        xyz = np.concatenate((xyz, np.ones((xyz.shape[0], 1))), axis=1)
-    return xyz
+"Transformation for Belvedere North-West terminus, from Local RS to WGS84-UTM32N"
+BELV_LOC2UTM = np.array(
+    [
+        [0.706579327583, -0.70687371492, -0.00012600114, 416614.833],
+        [0.706873714924, 0.706579267979, 0.000202054813, 5090932.706],
+        [-0.00005382637, -0.00023195939, 0.999462246895, 1767.547],
+        [0.0, 0.0, 0.0, 1.0],
+    ]
+)
 
 
 class Rotrotranslation:
     def __init__(self, t_mat: np.ndarray) -> None:
         # TODO: add checks on input T mat
         assert isinstance(
             t_mat, np.ndarray
-        ), "Invalid input for the transformation matrix t_mat. It must be a 4x4 numpy array"
-        assert t_mat.shape == (4, 4), "Error: T mat must be a 4x4 numpy array"
+        ), "Invalid input for the transformation matrix t_mat. It must be a 4x4 numpy array."
+        assert t_mat.shape == (
+            4,
+            4,
+        ), "Error: T mat must be a 4x4 numpy array in homogeneous coordinates."
 
         self._t = t_mat
 
     @classmethod
     def read_T_from_file(cls, file: Union[str, Path]):
         # TODO: implement this function
         T = np.loadtxt(file)
@@ -106,14 +39,23 @@
     def T(self):
         return self._t
 
     @property
     def T_inv(self):
         return np.linalg.inv(self._t)
 
+    @staticmethod
+    def belvedere_loc2utm() -> np.ndarray:
+        return BELV_LOC2UTM
+
+    @staticmethod
+    def belvedere_utm2loc() -> np.ndarray:
+        BELV_UTM2LOC = np.linalg.inv(BELV_LOC2UTM)
+        return BELV_UTM2LOC
+
     def apply_transformation(self, x: np.ndarray) -> np.ndarray:
         """
         Applies a 4x4 transformation matrix in homogeneous coordinates
         to a 4xn numpy array in homogeneous coordinates. If input points are not in homogeneous coordinates, it converts them using convert_to_homogeneous function.
 
         Args:
             x: A 4xn numpy array representing n points in homogeneous coordinates or a 3xn numpy array representing n points in euclidean coordinates .
@@ -158,19 +100,118 @@
             raise ValueError(
                 "Error: x must be a 4xn numpy array in homogeneous coordinates or a 3xn numpy array in euclidean coordinates."
             )
 
         out = self.T_inv @ x
         return convert_from_homogeneous(out)
 
+    def read_pcd(self, fname: Union[str, Path]) -> np.ndarray:
+        """
+        Reads a pcd file by using Open3D
+        """
+        pcd = o3d.io.read_point_cloud(str(fname))
+        return np.asarray(pcd.points)
+
+    def write_pcd(self, fname: Union[str, Path], x: np.ndarray) -> None:
+        """
+        Writes a pcd file by using Open3D
+        """
+        assert isinstance(x, np.ndarray), "x must be a numpy array."
+        assert x.shape[1] == 3, "x must be a nx3 numpy array."
+        pcd = o3d.geometry.PointCloud()
+        pcd.points = o3d.utility.Vector3dVector(x)
+        o3d.io.write_point_cloud(str(fname), pcd)
+
+    def transform_pcd(
+        self,
+        fname: Union[str, Path],
+        save_transformed: bool = True,
+        out_fname: str = None,
+    ):
+        fname = Path(fname)
+        x = self.read_pcd(fname)
+        x_transf = self.apply_transformation(x.T).T
+        if save_transformed:
+            if out_fname is None:
+                out_fname = fname.parent / f"{fname.stem}_transformed.pcd"
+            self.write_pcd(fname, x_transf)
+        else:
+
+            return x_transf
+
     def write_T_mat_to_csv(self, fname: str, sep: str = " "):
         with open(fname, "w") as f:
             for row in self.T:
                 string = f"{sep}".join([f"{x}" for x in row])
                 f.write(f"{string}\n")
 
 
+def convert_to_homogeneous(x: np.ndarray) -> np.ndarray:
+    """Converts a 2xn or 3xn vector of n points in euclidean coordinates to a 3xn or 4xn vector in homogeneous coordinates by adding a row of ones.
+
+    Args:
+        x (np.ndarray): A numpy array with shape 2xn or 3xn, representing the euclidean
+            coordinates of n points.
+
+    Returns:
+        np.ndarray: A numpy array with shape 3xn or 4xn, representing the homogeneous
+        coordinates of the same n points.
+    """
+    x = np.array(x)
+    ndim, npts = x.shape
+    if ndim != 2 and ndim != 3:
+        print(
+            "Error: wrong number of dimension of the input vector.\
+            A number of dimensions (rows) of 2 or 3 is required."
+        )
+        return None
+    x1 = np.concatenate((x, np.ones((1, npts), "float32")), axis=0)
+    return x1
+
+
+def convert_from_homogeneous(x: np.ndarray) -> np.ndarray:
+    """
+    Convert 3xn or 4xn vector of n points in homogeneous coordinates
+    to a 2xn or 3xn vector in euclidean coordinates, by dividing by the
+    homogeneous part of the vector (last row) and removing one dimension
+    """
+    x = np.array(x)
+    ndim, npts = x.shape
+    if ndim != 3 and ndim != 4:
+        print(
+            "Error: wrong number of dimension of the input vector.\
+            A number of dimensions (rows) of 2 or 3 is required."
+        )
+        return None
+    x1 = x[: ndim - 1, :] / x[ndim - 1, :]
+    return x1
+
+
+def get_coordinates_from_df(
+    df: pd.DataFrame,
+    to_homogeneous: bool = False,
+) -> np.ndarray:
+    """Extracts the 3D coordinates of a point cloud from a pandas DataFrame.
+
+    Args:
+        df: A pandas DataFrame with columns "X", "Y" and "Z".
+        to_homogeneous: A boolean indicating whether to convert the coordinates
+            to homogeneous coordinates or not.
+
+    Returns:
+        A numpy array with shape mx3 or mx4, representing the 3D coordinates
+        of a point cloud with m points, in euclidean or homogeneous coordinates.
+    """
+    xyz = df[["X", "Y", "Z"]].to_numpy()
+    if to_homogeneous:
+        xyz = np.concatenate((xyz, np.ones((xyz.shape[0], 1))), axis=1)
+    return xyz
+
+
 if __name__ == "__main__":
-    belv_rotra = Rotrotranslation(belvedere_loc2utm())
+    belv_rotra = Rotrotranslation(Rotrotranslation.belvedere_loc2utm())
     # a = Rotrotranslation.read_T_from_file("scripts/rototranslation/BELV_LOC2UTM.txt")
 
+    pcd_name = "res/monthly_pcd/belvedere2021_densaMedium_lingua_50cm_utm.ply"
+    belv_rotra.transform_pcd(pcd_name)
+
     print("done")
```

### Comparing `icepy4d-1.6.2/src/icepy4d/visualization/visualization.py` & `icepy4d-1.7.0/src/icepy4d/visualization/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 import matplotlib
 import logging
 
 from typing import List, Union, Dict
 from pathlib import Path
 from copy import deepcopy
 
-from icepy4d.classes.camera import Camera
-from icepy4d.classes.features import Features, Feature
-from icepy4d.classes.point_cloud import PointCloud
+from icepy4d.classes import Camera, Feature, Features, PointCloud
 from icepy4d.sfm.geometry import project_points
 
 
 """ Visualization of images"""
 
 
 def imshow_cv2(
@@ -285,17 +283,19 @@
 
     if zoom_to_features:
         w = window_size  # px
         xc = points[:, 0].mean()
         yc = points[:, 1].mean()
         ax.set_xlim([xc - w, xc + w])
         ax.set_ylim([yc - w, yc + w])
+
     if save_path is not None:
         fig.set_size_inches(size_inches[0], size_inches[1])
         fig.savefig(save_path, dpi=dpi)
+
     if hide_fig is True:
         plt.close(fig)
         return None
     else:
         return ax
 
 
@@ -354,15 +354,15 @@
     image: np.ndarray,
     features: Features,
     title: str = None,
     ax=None,
     save_path: Union[str, Path] = None,
     hide_fig: bool = False,
     **kwargs,
-) -> None:
+):
     """Wrapper around plot_points to work if the input is a Features object"""
     xy = features.to_numpy()["kpts"]
     fig = plot_points(
         image,
         points=xy,
         title=title,
         ax=ax,
@@ -766,15 +766,14 @@
 
 def make_camera_angles_plot(
     cameras,
     save_path: Union[str, Path] = None,
     baseline_epoch: int = None,
     current_epoch: int = None,
 ):
-
     cameras_plt = deepcopy(cameras)
 
     if baseline_epoch is not None:
         ep0 = baseline_epoch
     else:
         ep0 = 0
 
@@ -901,15 +900,14 @@
 #         fig.canvas.mpl_disconnect(cid)
 
 #     return coords
 # cid = fig.canvas.mpl_connect('button_press_event', onclick)
 
 
 if __name__ == "__main__":
-
     camera_extrinsics = np.eye(4)
     K = np.array([[4000, 0, 2000], [0, 4000, 3000], [0, 0, 1]])
     cam = Camera(6000, 4000, K, extrinsics=camera_extrinsics)
 
     pyr = make_camera_pyramid(
         cam, color=[1.0, 0.0, 0.0], focal_len_scaled=2, aspect_ratio=0.4
     )
```

### Comparing `icepy4d-1.6.2/src/icepy4d.egg-info/PKG-INFO` & `icepy4d-1.7.0/src/icepy4d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icepy4d
-Version: 1.6.2
+Version: 1.7.0
 Summary: 4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
         All rights reserved.
```

### Comparing `icepy4d-1.6.2/src/icepy4d.egg-info/SOURCES.txt` & `icepy4d-1.7.0/src/icepy4d.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 src/icepy4d/__main__.py
 src/icepy4d.egg-info/PKG-INFO
 src/icepy4d.egg-info/SOURCES.txt
 src/icepy4d.egg-info/dependency_links.txt
 src/icepy4d.egg-info/requires.txt
 src/icepy4d.egg-info/top_level.txt
 src/icepy4d/classes/__init__.py
+src/icepy4d/classes/calibration.py
 src/icepy4d/classes/camera.py
 src/icepy4d/classes/dsm.py
 src/icepy4d/classes/epoch.py
 src/icepy4d/classes/features.py
 src/icepy4d/classes/images.py
 src/icepy4d/classes/ortophoto.py
 src/icepy4d/classes/point_cloud.py
 src/icepy4d/classes/points.py
-src/icepy4d/classes/solution.py
+src/icepy4d/classes/sensor_width_database.py
 src/icepy4d/classes/targets.py
-src/icepy4d/classes/typed_dict_classes.py
+src/icepy4d/classes/typed_dict_classes_old.py
 src/icepy4d/io/__init__.py
 src/icepy4d/io/export2bundler.py
 src/icepy4d/io/export2calge.py
 src/icepy4d/io/export2colmap.py
 src/icepy4d/io/export2textfile.py
-src/icepy4d/io/importing.py
 src/icepy4d/io/colmap_utils/__init__.py
 src/icepy4d/io/colmap_utils/build.py
 src/icepy4d/io/colmap_utils/build_windows_app.py
 src/icepy4d/io/colmap_utils/bundler_to_ply.py
 src/icepy4d/io/colmap_utils/clang_format_code.py
 src/icepy4d/io/colmap_utils/crawl_camera_specs.py
 src/icepy4d/io/colmap_utils/database.py
@@ -82,37 +82,30 @@
 src/icepy4d/thirdparty/transformations.py
 src/icepy4d/thirdparty/triangulation.py
 src/icepy4d/thirdparty/SuperGlue/models/__init__.py
 src/icepy4d/thirdparty/SuperGlue/models/matching.py
 src/icepy4d/thirdparty/SuperGlue/models/superglue.py
 src/icepy4d/thirdparty/SuperGlue/models/superpoint.py
 src/icepy4d/thirdparty/SuperGlue/models/utils.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
-src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
 src/icepy4d/utils/__init__.py
 src/icepy4d/utils/binned_stats.py
 src/icepy4d/utils/dsm_orthophoto.py
+src/icepy4d/utils/geospatial.py
 src/icepy4d/utils/homography.py
 src/icepy4d/utils/initialization.py
 src/icepy4d/utils/logger.py
 src/icepy4d/utils/math.py
-src/icepy4d/utils/sensor_width_database.py
-src/icepy4d/utils/spatial_funs.py
 src/icepy4d/utils/tiles.py
 src/icepy4d/utils/timer.py
 src/icepy4d/utils/tracking_features_utils.py
 src/icepy4d/utils/transformations.py
 src/icepy4d/visualization/__init__.py
 src/icepy4d/visualization/visualization.py
 tests/test_features.py
 tests/test_image.py
 tests/test_initialization.py
 tests/test_matching.py
 tests/test_point_cloud.py
 tests/test_sfm_geometry.py
+tests/test_transformations.py
 tests/test_utils.py
-tests/test_utils_spatial.py
+tests/test_utils_geospatial.py
```

### Comparing `icepy4d-1.6.2/tests/test_features.py` & `icepy4d-1.7.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/tests/test_image.py` & `icepy4d-1.7.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/tests/test_initialization.py` & `icepy4d-1.7.0/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/tests/test_matching.py` & `icepy4d-1.7.0/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/tests/test_point_cloud.py` & `icepy4d-1.7.0/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/tests/test_sfm_geometry.py` & `icepy4d-1.7.0/tests/test_sfm_geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.6.2/tests/test_utils_spatial.py` & `icepy4d-1.7.0/tests/test_utils_geospatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from icepy4d.utils.spatial_funs import *
+from icepy4d.utils.geospatial import *
 
 
 def test_point_in_volume():
     volume = np.array([[0, 0, 0], [1, 1, 1], [1, 0, 0], [0, 1, 0], [0, 0, 1]])
     point = (0.5, 0.5, 0.5)
     assert point_in_volume(point, volume) == True
```

