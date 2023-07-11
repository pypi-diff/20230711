# Comparing `tmp/yeastvision-0.1.6.tar.gz` & `tmp/yeastvision-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeastvision-0.1.6.tar", last modified: Thu Jun 29 18:29:07 2023, max compression
+gzip compressed data, was "yeastvision-0.1.7.tar", last modified: Tue Jul 11 03:12:40 2023, max compression
```

## Comparing `yeastvision-0.1.6.tar` & `yeastvision-0.1.7.tar`

### file list

```diff
@@ -1,81 +1,96 @@
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.426939 yeastvision-0.1.6/
--rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.6/LICENSE
--rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-29 18:29:07.426659 yeastvision-0.1.6/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     3290 2023-06-21 06:06:54.000000 yeastvision-0.1.6/README.md
--rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-29 18:29:07.427034 yeastvision-0.1.6/setup.cfg
--rw-r--r--   0 berk       (502) staff       (20)     1750 2023-06-29 18:28:24.000000 yeastvision-0.1.6/setup.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.406439 yeastvision-0.1.6/yeastvision/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.6/yeastvision/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)    80318 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/__main__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.409163 yeastvision-0.1.6/yeastvision/disk/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.6/yeastvision/disk/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.6/yeastvision/disk/io.py
--rw-r--r--   0 berk       (502) staff       (20)    10218 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/disk/reader.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.410106 yeastvision-0.1.6/yeastvision/flou/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.6/yeastvision/flou/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.6/yeastvision/flou/blob_detect.py
--rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.6/yeastvision/flou/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     2688 2023-06-20 19:25:38.000000 yeastvision-0.1.6/yeastvision/ims.py
--rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.6/yeastvision/install_weights.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.412016 yeastvision-0.1.6/yeastvision/models/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.413180 yeastvision-0.1.6/yeastvision/models/YeaZ/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/segment.py
--rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.6/yeastvision/models/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.413820 yeastvision-0.1.6/yeastvision/models/artilife/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.6/yeastvision/models/artilife/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.414472 yeastvision-0.1.6/yeastvision/models/artilife/budSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.6/yeastvision/models/artilife/budSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.6/yeastvision/models/artilife/budSeg/model.py
--rw-r--r--   0 berk       (502) staff       (20)     9519 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/models/artilife/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.415076 yeastvision-0.1.6/yeastvision/models/budNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.6/yeastvision/models/budNET/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.6/yeastvision/models/budNET/model.py
--rw-r--r--   0 berk       (502) staff       (20)     3833 2023-06-27 20:12:02.000000 yeastvision-0.1.6/yeastvision/models/cp.py
--rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.6/yeastvision/models/eval.py
--rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.6/yeastvision/models/loss.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.415952 yeastvision-0.1.6/yeastvision/models/matSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.6/yeastvision/models/matSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.6/yeastvision/models/matSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.6/yeastvision/models/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.416449 yeastvision-0.1.6/yeastvision/models/tetradSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.6/yeastvision/models/tetradSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.6/yeastvision/models/tetradSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.6/yeastvision/models/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.6/yeastvision/models/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.417075 yeastvision-0.1.6/yeastvision/models/vacNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.6/yeastvision/models/vacNET/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.6/yeastvision/models/vacNET/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.419845 yeastvision-0.1.6/yeastvision/parts/
--rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.6/yeastvision/parts/canvas.py
--rw-r--r--   0 berk       (502) staff       (20)    31747 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/parts/dialogs.py
--rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.6/yeastvision/parts/guiparts.py
--rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.6/yeastvision/parts/menu.py
--rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.6/yeastvision/parts/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     2734 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/parts/workers.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.421779 yeastvision-0.1.6/yeastvision/plot/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.6/yeastvision/plot/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3461 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/cell_table.py
--rw-r--r--   0 berk       (502) staff       (20)    12653 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/plot.py
--rw-r--r--   0 berk       (502) staff       (20)     5056 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/types.py
--rw-r--r--   0 berk       (502) staff       (20)      391 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.426042 yeastvision-0.1.6/yeastvision/track/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.6/yeastvision/track/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     6286 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/cell.py
--rw-r--r--   0 berk       (502) staff       (20)     8241 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/data.py
--rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.6/yeastvision/track/hungarian_track.py
--rw-r--r--   0 berk       (502) staff       (20)        4 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/lc.py
--rw-r--r--   0 berk       (502) staff       (20)     8413 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/lineage.py
--rw-r--r--   0 berk       (502) staff       (20)    18443 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/mat.py
--rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.6/yeastvision/track/track.py
--rw-r--r--   0 berk       (502) staff       (20)     4574 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     5523 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.408427 yeastvision-0.1.6/yeastvision.egg-info/
--rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-29 18:29:06.000000 yeastvision-0.1.6/yeastvision.egg-info/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     1875 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/SOURCES.txt
--rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-29 18:29:06.000000 yeastvision-0.1.6/yeastvision.egg-info/dependency_links.txt
--rw-r--r--   0 berk       (502) staff       (20)      115 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/entry_points.txt
--rw-r--r--   0 berk       (502) staff       (20)      287 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/requires.txt
--rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/top_level.txt
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.216730 yeastvision-0.1.7/
+-rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.7/LICENSE
+-rw-r--r--   0 berk       (502) staff       (20)     3635 2023-07-11 03:12:40.216031 yeastvision-0.1.7/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     3287 2023-07-11 03:08:39.000000 yeastvision-0.1.7/README.md
+-rw-r--r--   0 berk       (502) staff       (20)       38 2023-07-11 03:12:40.216921 yeastvision-0.1.7/setup.cfg
+-rw-r--r--   0 berk       (502) staff       (20)     1798 2023-07-11 03:12:14.000000 yeastvision-0.1.7/setup.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.142601 yeastvision-0.1.7/yeastvision/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.7/yeastvision/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)    81437 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/__main__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.149281 yeastvision-0.1.7/yeastvision/disk/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.7/yeastvision/disk/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.7/yeastvision/disk/io.py
+-rw-r--r--   0 berk       (502) staff       (20)    13015 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/disk/reader.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.151588 yeastvision-0.1.7/yeastvision/flou/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.7/yeastvision/flou/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.7/yeastvision/flou/blob_detect.py
+-rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.7/yeastvision/flou/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.153324 yeastvision-0.1.7/yeastvision/ims/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     2688 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/im_funcs.py
+-rw-r--r--   0 berk       (502) staff       (20)     3907 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/interpolate.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.162021 yeastvision-0.1.7/yeastvision/ims/rife_model/
+-rw-r--r--   0 berk       (502) staff       (20)     4518 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet.py
+-rw-r--r--   0 berk       (502) staff       (20)     4509 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet_2R.py
+-rw-r--r--   0 berk       (502) staff       (20)     4716 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/IFNet_m.py
+-rw-r--r--   0 berk       (502) staff       (20)     3518 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/RIFE.py
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3850 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/interpolate.py
+-rw-r--r--   0 berk       (502) staff       (20)     2187 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/laplacian.py
+-rw-r--r--   0 berk       (502) staff       (20)     4641 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/loss.py
+-rw-r--r--   0 berk       (502) staff       (20)     3219 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/refine.py
+-rw-r--r--   0 berk       (502) staff       (20)     3286 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/refine_2R.py
+-rw-r--r--   0 berk       (502) staff       (20)     1058 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/ims/rife_model/warplayer.py
+-rw-r--r--   0 berk       (502) staff       (20)     2419 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/install_weights.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.168913 yeastvision-0.1.7/yeastvision/models/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.173158 yeastvision-0.1.7/yeastvision/models/YeaZ/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/segment.py
+-rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.7/yeastvision/models/YeaZ/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.7/yeastvision/models/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.174327 yeastvision-0.1.7/yeastvision/models/artilife/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.7/yeastvision/models/artilife/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.175936 yeastvision-0.1.7/yeastvision/models/artilife/budSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.7/yeastvision/models/artilife/budSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.7/yeastvision/models/artilife/budSeg/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     9519 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/models/artilife/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.177044 yeastvision-0.1.7/yeastvision/models/budNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.7/yeastvision/models/budNET/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.7/yeastvision/models/budNET/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     3833 2023-06-27 20:12:02.000000 yeastvision-0.1.7/yeastvision/models/cp.py
+-rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.7/yeastvision/models/eval.py
+-rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.7/yeastvision/models/loss.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.178176 yeastvision-0.1.7/yeastvision/models/matSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.7/yeastvision/models/matSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.7/yeastvision/models/matSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.7/yeastvision/models/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.179368 yeastvision-0.1.7/yeastvision/models/tetradSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.7/yeastvision/models/tetradSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.7/yeastvision/models/tetradSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.7/yeastvision/models/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.7/yeastvision/models/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.180471 yeastvision-0.1.7/yeastvision/models/vacNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.7/yeastvision/models/vacNET/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.7/yeastvision/models/vacNET/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.186965 yeastvision-0.1.7/yeastvision/parts/
+-rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.7/yeastvision/parts/canvas.py
+-rw-r--r--   0 berk       (502) staff       (20)    31747 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/parts/dialogs.py
+-rw-r--r--   0 berk       (502) staff       (20)    12008 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/parts/guiparts.py
+-rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.7/yeastvision/parts/menu.py
+-rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.7/yeastvision/parts/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     3502 2023-07-11 03:02:20.000000 yeastvision-0.1.7/yeastvision/parts/workers.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.191258 yeastvision-0.1.7/yeastvision/plot/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.7/yeastvision/plot/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3461 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/cell_table.py
+-rw-r--r--   0 berk       (502) staff       (20)    12653 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/plot.py
+-rw-r--r--   0 berk       (502) staff       (20)     5056 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/types.py
+-rw-r--r--   0 berk       (502) staff       (20)      391 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/plot/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.211297 yeastvision-0.1.7/yeastvision/track/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.7/yeastvision/track/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     6286 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/cell.py
+-rw-r--r--   0 berk       (502) staff       (20)     8241 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/data.py
+-rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.7/yeastvision/track/hungarian_track.py
+-rw-r--r--   0 berk       (502) staff       (20)        4 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/lc.py
+-rw-r--r--   0 berk       (502) staff       (20)     8413 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/lineage.py
+-rw-r--r--   0 berk       (502) staff       (20)    18443 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/mat.py
+-rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.7/yeastvision/track/track.py
+-rw-r--r--   0 berk       (502) staff       (20)     4574 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/track/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     5523 2023-06-29 18:12:58.000000 yeastvision-0.1.7/yeastvision/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-07-11 03:12:40.147281 yeastvision-0.1.7/yeastvision.egg-info/
+-rw-r--r--   0 berk       (502) staff       (20)     3635 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     2364 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/SOURCES.txt
+-rw-r--r--   0 berk       (502) staff       (20)        1 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/dependency_links.txt
+-rw-r--r--   0 berk       (502) staff       (20)      116 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/entry_points.txt
+-rw-r--r--   0 berk       (502) staff       (20)      273 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/requires.txt
+-rw-r--r--   0 berk       (502) staff       (20)       12 2023-07-11 03:12:40.000000 yeastvision-0.1.7/yeastvision.egg-info/top_level.txt
```

### Comparing `yeastvision-0.1.6/LICENSE` & `yeastvision-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/PKG-INFO` & `yeastvision-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.6
+Version: 0.1.7
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 Yeastvision is ready to go for cpu-usage as soon as it downloaded. GPU-usage requires some additional steps after download. To download:
 
 1. Install an [Anaconda](https://www.anaconda.com/products/distribution) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
 2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
 3. Create a new environment with `conda create --name yeastvision python=3.10.o`. 
 4. Activate this new environment by running `conda activate yeastvision`
 5. Run `python -m pip install yeastvision` to download our package plus all dependencies
-6. Download the weights [online](https://drive.google.com/file/d/1J3R4JKILkQNM0Ap-MKxqv61oAxObSjBo/view?usp=drive_link). 
+6. Download the weights [online](https://drive.google.com/file/d/1Zl3b00eSbe3wbxpYOknEP5q0A86XtEfL/view?usp=sharing). 
 7. Run `install-weights` in the same directory as the *yeastvision_weights.zip* file
 
 
 You should upgrade yeastvision (package [here](https://pypi.org/project/yeastvision/)) periodically as it is still in development. To do so, run the following in the environment:
 
 ~~~sh
 python -m pip install yeastvision --upgrade
```

### Comparing `yeastvision-0.1.6/README.md` & `yeastvision-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Yeastvision is ready to go for cpu-usage as soon as it downloaded. GPU-usage requires some additional steps after download. To download:
 
 1. Install an [Anaconda](https://www.anaconda.com/products/distribution) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
 2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
 3. Create a new environment with `conda create --name yeastvision python=3.10.o`. 
 4. Activate this new environment by running `conda activate yeastvision`
 5. Run `python -m pip install yeastvision` to download our package plus all dependencies
-6. Download the weights [online](https://drive.google.com/file/d/1J3R4JKILkQNM0Ap-MKxqv61oAxObSjBo/view?usp=drive_link). 
+6. Download the weights [online](https://drive.google.com/file/d/1Zl3b00eSbe3wbxpYOknEP5q0A86XtEfL/view?usp=sharing). 
 7. Run `install-weights` in the same directory as the *yeastvision_weights.zip* file
 
 
 You should upgrade yeastvision (package [here](https://pypi.org/project/yeastvision/)) periodically as it is still in development. To do so, run the following in the environment:
 
 ~~~sh
 python -m pip install yeastvision --upgrade
```

### Comparing `yeastvision-0.1.6/setup.py` & `yeastvision-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,26 +26,26 @@
         requires.remove("torch==1.12.1")
 except:
     pass
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-packages = ["yeastvision", "yeastvision.plot", "yeastvision.track", "yeastvision.models", 
+packages = ["yeastvision", "yeastvision.plot", "yeastvision.track", "yeastvision.models", "yeastvision.ims", "yeastvision.ims.rife_model",
             "yeastvision.parts", "yeastvision.flou", "yeastvision.disk", 
             "yeastvision.models.artilife", "yeastvision.models.artilife.budSeg",
             "yeastvision.models.matSeg", "yeastvision.models.tetradSeg", "yeastvision.models.budNET", 
             "yeastvision.models.vacNET", "yeastvision.models.YeaZ"]
 
 
 
 
 setup(
     name = "yeastvision",
-    version = "0.1.6",
+    version = "0.1.7",
     description = "Deep learning-enabled image analysis of the yeast full life cycle",
     author = "Berk Yalcinkaya",
     url = "https://github.com/berkyalcinkaya/yeastvision",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email="berkyalcinkaya55@gmail.com",
     license = "BSD",
```

### Comparing `yeastvision-0.1.6/yeastvision/__main__.py` & `yeastvision-0.1.7/yeastvision/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 tic = process_time()
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2' 
 from PyQt5 import QtWidgets, QtGui, QtCore
 from PyQt5.QtWidgets import (QApplication, QStyle, QMainWindow, QGroupBox, QPushButton, QDialog,
                             QDialogButtonBox, QLineEdit, QFormLayout, QMessageBox,QErrorMessage, QStatusBar, 
                              QFileDialog, QVBoxLayout, QCheckBox, QFrame, QSpinBox, QLabel, QWidget, QComboBox, QSizePolicy, QGridLayout)
-from PyQt5.QtCore import Qt, QThread
+from PyQt5.QtCore import Qt, QThread, QMutex, pyqtSignal
 import pyqtgraph as pg
 import numpy as np
 import matplotlib.pyplot as plt
 from yeastvision.parts.canvas import ImageDraw, ViewBoxNoRightDrag
 from yeastvision.parts.guiparts import *
-from yeastvision.parts.workers import SegmentWorker, TrackWorker
+from yeastvision.parts.workers import SegmentWorker, TrackWorker, InterpolationWorker
 from yeastvision.parts.dialogs import *
 from yeastvision.track.track import track_to_cell, trackYeasts
 from yeastvision.track.data import LineageData, TimeSeriesData
 from yeastvision.track.lineage import LineageConstruction
 from yeastvision.track.cell import LABEL_PROPS, IM_PROPS, EXTRA_IM_PROPS, getCellData, exportCellData, getHeatMaps, getDaughterMatrix
 import cv2
 from yeastvision.disk.reader import loadPkl, ImageData, MaskData
@@ -28,58 +28,30 @@
 import glob
 from os.path import join
 from datetime import datetime
 import pandas as pd
 import yeastvision.plot.plot as plot
 from yeastvision.flou.blob_detect import Blob
 from yeastvision.utils import *
-import yeastvision.ims as im_funcs
+import yeastvision.ims.im_funcs as im_funcs
+from yeastvision.ims.interpolate import interpolate
 import math
 import pickle
 from skimage.io import imread, imsave
 from cellpose.metrics import average_precision
 from tqdm import tqdm
+from memory_profiler import profile
+from functools import partial
 
-class QHLine(QFrame):
-    def __init__(self):
-        super(QHLine, self).__init__()
-        self.setFrameShape(QFrame.HLine)
-        self.setFrameShadow(QFrame.Sunken)
-
-
-class QVLine(QFrame):
-    def __init__(self):
-        super(QVLine, self).__init__()
-        self.setFrameShape(QFrame.VLine)
-        self.setFrameShadow(QFrame.Sunken)
-
-
-class Worker(QtCore.QObject):
-    '''Handles Multithreading'''
-    finished = QtCore.pyqtSignal()
-    def __init__(self, parent, process, button = None):
-        super(Worker,self).__init__()
-        self.parent = parent
-        self.process = process
-        self.button = button
-        self.error = False
-        
-    def run(self):
-        #try:
-        self.process()
-        self.finished.emit()
-        # except:
-        #     self.error = True
-        #     self.finished.emit()
 
 class MainWindow(QtWidgets.QMainWindow):
     def __init__(self, thread, imPaths = None, labelPaths = None):
         super(MainWindow, self).__init__()
         pg.setConfigOption('imageAxisOrder', 'row-major')
-        self.setGeometry(50, 50, 1000, 1000)
+        self.setGeometry(50, 50, 1300, 1300)
         self.setAcceptDrops(True)
 
         #self.idealThreadCount  = thread.idealThreadCount()//2
         self.idealThreadCount = 2
 
         self.sessionId = self.getCurrTimeStr()
         
@@ -110,20 +82,20 @@
         self.firstMaskLoad = True
         self.getModelNames()
         self.setStyleSheet("QMainWindow {background: 'black';}")
         self.cwidget = QWidget(self)
         self.l = QGridLayout()
         self.cwidget.setLayout(self.l)
         self.setCentralWidget(self.cwidget)
-        self.l.setSpacing(3)
+        self.l.setSpacing(1)
 
         self.win = pg.GraphicsLayoutWidget()
         self.mainViewRows = 30
-        self.mainViewCols  = 19
-        self.l.addWidget(self.win, 1,0, self.mainViewRows, self.mainViewCols)
+        self.mainViewCols  = 21
+        self.l.addWidget(self.win, 0,0, self.mainViewRows, self.mainViewCols)
         self.make_viewbox()
 
         self.labelX, self.labelY = None, None
         self.currMaskDtype = "uint8"
         self.currImDtype = "uint8"
 
         self.threads = []
@@ -390,14 +362,15 @@
     
 
     def getCellColors(self,im):
         return np.take(self.maskColors, np.unique(im), 0)
 
     def build_widgets(self):
         rowspace = self.mainViewRows
+        cspace = 2
         self.labelstyle = """QLabel{
                             color: white
                             } 
                          QToolTip { 
                            background-color: black; 
                            color: white; 
                            border: black solid 1px
@@ -411,15 +384,14 @@
                         "background-color: rgb(40,40,40);"
                         "selection-color: white;"
                         "selection-background-color: rgb(50,100,50);")
         self.checkstyle = "color: rgb(190,190,190);"
 
         self.statusBar = QStatusBar()
         self.statusBar.setFont(self.medfont)
-
         self.statusBar.setStyleSheet(self.statusbarstyle)
         self.setStatusBar(self.statusBar)
         self.gpuDisplayTorch = ReadOnlyCheckBox("gpu - torch  |  ")
         self.gpuDisplayTF= ReadOnlyCheckBox("gpu - tf")
         self.gpuDisplayTF.setFont(self.smallfont)
         self.gpuDisplayTorch.setFont(self.smallfont)
         self.gpuDisplayTF.setStyleSheet(self.checkstyle)
@@ -443,225 +415,239 @@
         self.hasLineageBox = ReadOnlyCheckBox("lineage data")
         self.hasCellDataBox = ReadOnlyCheckBox("cell data")
         for display in [self.hasLineageBox,self.hasCellDataBox]:
             display.setFont(self.smallfont)
             display.setStyleSheet(self.checkstyle)
             display.setChecked(False)
 
-        self.statusBarLayout.addWidget(self.cpuCoreDisplay, 0, 0, 1,1 )
-        self.statusBarLayout.addWidget(self.gpuDisplayTF, 0, 1, 1, 1)
-        self.statusBarLayout.addWidget(self.gpuDisplayTorch, 0, 2, 1, 1)
-        self.statusBarLayout.addWidget(self.hasLineageBox, 0,3,1,1)
-        self.statusBarLayout.addWidget(self.hasCellDataBox,0,4,1,1)
+        self.statusBarLayout.addWidget(self.cpuCoreDisplay, 0, 1, 1,1, alignment=(QtCore.Qt.AlignCenter))
+        self.statusBarLayout.addWidget(self.gpuDisplayTF, 0, 2, 1, 1)
+        self.statusBarLayout.addWidget(self.gpuDisplayTorch, 0, 3, 1, 1)
+        self.statusBarLayout.addWidget(self.hasLineageBox, 0,4,1,1)
+        self.statusBarLayout.addWidget(self.hasCellDataBox,0,5,1,1)
         self.statusBar.addPermanentWidget(self.statusBarWidget)
         
         self.dataDisplay = QLabel("")
         self.dataDisplay.setMinimumWidth(300)
         # self.dataDisplay.setMaximumWidth(300)
         self.dataDisplay.setStyleSheet(self.labelstyle)
         self.dataDisplay.setFont(self.smallfont)
         self.dataDisplay.setAlignment(QtCore.Qt.AlignLeft | QtCore.Qt.AlignBottom)
         self.updateDataDisplay()
-        self.l.addWidget(self.dataDisplay, rowspace-1,0,1,20)
+        self.l.addWidget(self.dataDisplay, rowspace-1,cspace+1,1,20)
 
         label = QLabel('Drawing:')#[\u2191 \u2193]')
         label.setStyleSheet(self.headings)
         label.setFont(self.boldfont)
-        self.l.addWidget(label, rowspace,0,1,5)
+        self.l.addWidget(label, rowspace,1,1,5)
 
         label = QLabel("Brush Type:")
         label.setStyleSheet(self.labelstyle)
         label.setFont(self.medfont)
-        self.l.addWidget(label,rowspace+1,0,1,2)
+        self.l.addWidget(label,rowspace+1,1,1,2)
         self.brushTypeSelect = QComboBox()
         self.brushTypeSelect.addItems(["Eraser", "Brush", "Outline"])
         self.brushTypeSelect.setCurrentIndex(-1)
         self.brushTypeSelect.currentIndexChanged.connect(self.brushTypeChoose)
         self.brushTypeSelect.setStyleSheet(self.dropdowns)
         self.brushTypeSelect.setFont(self.medfont)
         self.brushTypeSelect.setCurrentText("")
         self.brushTypeSelect.setFocusPolicy(QtCore.Qt.NoFocus)
         self.brushTypeSelect.setEnabled(False)
         self.brushTypeSelect.setFixedWidth(90)
         self.brushTypeSelect.setEnabled(False)
-        self.l.addWidget(self.brushTypeSelect, rowspace+1,2,1,1)
+        self.l.addWidget(self.brushTypeSelect, rowspace+1,3,1,1)
 
         
         label = QLabel("Brush Size")
         label.setStyleSheet(self.labelstyle)
         label.setFont(self.medfont)
-        self.l.addWidget(label, rowspace+2,0,1,2)
+        self.l.addWidget(label, rowspace+2,1,1,2)
         self.brush_size = 3
         self.brushSelect = QSpinBox()
         self.brushSelect.setMinimum(1)
         self.brushSelect.setValue(self.brush_size)
         self.brushSelect.valueChanged.connect(self.brushSizeChoose)
         self.brushSelect.setFixedWidth(90)
         self.brushSelect.setStyleSheet(self.dropdowns)
         self.brushSelect.setFont(self.medfont)
         edit = self.brushSelect.lineEdit()
         edit.setFocusPolicy(QtCore.Qt.NoFocus)
         self.brushSelect.setEnabled(False)
-        self.l.addWidget(self.brushSelect, rowspace+2,2,1,1)
+        self.l.addWidget(self.brushSelect, rowspace+2,3,1,1)
 
         line = QVLine()
         line.setStyleSheet('color:white;')
-        self.l.addWidget(line, rowspace,3,6,1)
+        self.l.addWidget(line, rowspace,4,6,1)
 
         label = QLabel('Tracking')#[\u2191 \u2193]')
         label.setStyleSheet(self.headings)
         label.setFont(self.boldfont)
-        self.l.addWidget(label, rowspace,4,1,4)
+        self.l.addWidget(label, rowspace,5,1,4)
 
         self.cellNumButton = QCheckBox("cell nums")
         self.cellNumButton.setStyleSheet(self.checkstyle)
         self.cellNumButton.setFont(self.medfont)
         self.cellNumButton.stateChanged.connect(self.toggleCellNums)
         self.cellNumButton.setEnabled(False)
-        self.l.addWidget(self.cellNumButton, rowspace+1, 4, 1,2)
+        self.l.addWidget(self.cellNumButton, rowspace+1, 5, 1,2)
 
         self.showLineageButton = QCheckBox("lineages")
         self.showLineageButton.setStyleSheet(self.checkstyle)
         self.showLineageButton.setFont(self.medfont)
         self.showLineageButton.stateChanged.connect(self.toggleLineages)
         self.showLineageButton.setEnabled(False)
-        self.l.addWidget(self.showLineageButton, rowspace+1, 6, 1,2)
+        self.l.addWidget(self.showLineageButton, rowspace+1, 7, 1,2)
 
         self.trackButton = QPushButton('track cells')
-        self.trackButton.setFixedWidth(90)
-        self.trackButton.setFixedHeight(20)
+        #self.trackButton.setFixedWidth(90)
+        #self.trackButton.setFixedHeight(20)
         self.trackButton.setStyleSheet(self.styleInactive)
         self.trackButton.setFont(self.medfont)
         self.trackButton.clicked.connect(self.trackButtonClick)
         self.trackButton.setEnabled(False)
         self.trackButton.setToolTip("Track current cell labels")
-        self.l.addWidget(self.trackButton, rowspace+2, 4,1,2)
+        self.l.addWidget(self.trackButton, rowspace+2, 5,1,2)
 
         self.trackObjButton = QPushButton('track to cell')
-        self.trackObjButton.setFixedWidth(90)
-        self.trackObjButton.setFixedHeight(20)
+        #self.trackObjButton.setFixedWidth(90)
+        #self.trackObjButton.setFixedHeight(20)
         self.trackObjButton.setFont(self.medfont)
         self.trackObjButton.setStyleSheet(self.styleInactive)
         self.trackObjButton.clicked.connect(self.trackObjButtonClick)
         self.trackObjButton.setEnabled(False)
         self.trackObjButton.setToolTip("Track current non-cytoplasmic label to a cellular label")
-        self.l.addWidget(self.trackObjButton, rowspace+2, 6,1,2)
+        self.l.addWidget(self.trackObjButton, rowspace+2, 7,1,2)
 
         self.lineageButton = QPushButton("get lineages")
         self.lineageButton.setStyleSheet(self.styleInactive)
-        self.lineageButton.setFixedWidth(90)
-        self.lineageButton.setFixedHeight(18)
+        #self.lineageButton.setFixedWidth(90)
+        #self.lineageButton.setFixedHeight(18)
         self.lineageButton.setFont(self.medfont)
         self.lineageButton.setToolTip("Use current budNET mask to assign lineages to a cellular label")
         self.lineageButton.setEnabled(False)
         self.showMotherDaughters = False
         self.showLineages = False
         self.lineageButton.clicked.connect(self.getLineages)
-        self.l.addWidget(self.lineageButton, rowspace+3, 4,1,2, Qt.AlignBottom)
+        self.l.addWidget(self.lineageButton, rowspace+3, 5,1,2, Qt.AlignBottom)
 
         self.showMotherDaughtersButton = QCheckBox("mother-daughters")
         self.showMotherDaughtersButton.setStyleSheet(self.checkstyle)
         self.showMotherDaughtersButton.setFont(self.medfont)
         self.showMotherDaughtersButton.stateChanged.connect(self.toggleMotherDaughters)
         self.showMotherDaughtersButton.setEnabled(False)
-        self.l.addWidget(self.showMotherDaughtersButton, rowspace+3, 6, 1,2)
+        self.l.addWidget(self.showMotherDaughtersButton, rowspace+3, 7, 1,2)
+
+        self.interpolateButton = QPushButton("Enhance Tracking Through Frame Interpolation")
+        self.interpolateButton.setStyleSheet(self.styleInactive)
+        self.interpolateButton.setFont(self.medfont)
+        self.interpolateButton.setEnabled(False)
+        self.interpolateButton.clicked.connect(self.interpolateButtonClicked)
+        self.l.addWidget(self.interpolateButton, rowspace+4, 5,1,4)
+
 
         line = QVLine()
         line.setStyleSheet('color:white;')
-        self.l.addWidget(line, rowspace,8,6,1)
+        self.l.addWidget(line, rowspace,9,6,1)
     
         label = QLabel('Segmentation')#[\u2191 \u2193]')
         label.setStyleSheet(self.headings)
         label.setFont(self.boldfont)
-        self.l.addWidget(label, rowspace,9,1,5)
+        self.l.addWidget(label, rowspace,10,1,5)
         
         #----------UNETS-----------
         self.GB = QGroupBox("Unets")
         self.GB.setStyleSheet("QGroupBox { border: 1px solid white; color:white; padding: 10px 0px;}")
         self.GBLayout = QGridLayout()
         self.GB.setLayout(self.GBLayout)
         self.GB.setToolTip("Select Unet(s) to be used for segmenting channel")
     
         self.getModels()
         self.modelChoose = QComboBox()
         self.modelChoose.addItems(sorted(self.modelNames, key = lambda x: x[0]))
             #self.modelChoose.setItemChecked(i, False)
-        self.modelChoose.setFixedWidth(180)
+        #self.modelChoose.setFixedWidth(180)
         self.modelChoose.setStyleSheet(self.dropdowns)
         self.modelChoose.setFont(self.medfont)
         self.modelChoose.setFocusPolicy(QtCore.Qt.NoFocus)
         self.modelChoose.setCurrentIndex(-1)
         self.GBLayout.addWidget(self.modelChoose, 0,0,1,7)
 
         self.modelButton = QPushButton(u'run model')
         self.modelButton.clicked.connect(self.computeModels)
         self.GBLayout.addWidget(self.modelButton, 0,7,1,2)
         self.modelButton.setEnabled(False)
         self.modelButton.setStyleSheet(self.styleInactive)
-        self.l.addWidget(self.GB, rowspace+1,9,3,5, Qt.AlignTop | Qt.AlignHCenter)
+        self.l.addWidget(self.GB, rowspace+1,10,3,5, Qt.AlignTop | Qt.AlignHCenter)
 
         #------Flourescence Segmentation -----------pp-p-
         self.segButton = QPushButton(u'blob detection')
         self.segButton.setEnabled(False)
         self.segButton.clicked.connect(self.doFlou)
         self.segButton.setStyleSheet(self.styleInactive)
-        self.l.addWidget(self.segButton, rowspace+1+3,9,3,5, Qt.AlignTop | Qt.AlignLeft)
+        self.l.addWidget(self.segButton, rowspace+1+2,10,3,5, Qt.AlignTop | Qt.AlignLeft)
 
-        #-----------------------------------------------
+        #----------------------------------s-------------
 
         line = QVLine()
         line.setStyleSheet('color:white;')
-        self.l.addWidget(line, rowspace,14,6,1)
+        self.l.addWidget(line, rowspace,15,6,1)
 
         label = QLabel('Display')#[\u2191 \u2193]')
         label.setStyleSheet(self.headings)
         label.setFont(self.boldfont)
-        self.l.addWidget(label, rowspace,15,1,5)
+        self.l.addWidget(label, rowspace,16,1,5)
 
         self.contourButton = QCheckBox("Show Contours")
         self.contourButton.setStyleSheet(self.checkstyle)
         self.contourButton.setFont(self.medfont)
         self.contourButton.stateChanged.connect(self.toggleContours)
         self.contourButton.setShortcut(QtCore.Qt.Key_C)
         self.contourButton.setEnabled(False)
-        self.l.addWidget(self.contourButton, rowspace+1, 15,1,2)
+        self.l.addWidget(self.contourButton, rowspace+1, 16,1,2)
 
         self.plotButton = QCheckBox("Show Plot Window")
         self.plotButton.setStyleSheet(self.checkstyle)
         self.plotButton.setFont(self.medfont)
         self.plotButton.stateChanged.connect(self.togglePlotWindow)
         self.plotButton.setShortcut(QtCore.Qt.Key_P)
-        self.l.addWidget(self.plotButton, rowspace+1, 17, 1,2)
+        self.l.addWidget(self.plotButton, rowspace+1, 18, 1,2)
 
         self.channelSelect = QComboBox()
         self.channelSelect.setStyleSheet(self.dropdowns)
         self.channelSelect.setFont(self.medfont)
         self.channelSelect.setCurrentText("")
         self.channelSelect.currentIndexChanged.connect(self.channelSelectIndexChange)
         self.channelSelect.setEditable(True)
         self.channelSelect.editTextChanged.connect(self.channelSelectEdit)
-        self.channelSelect.setFixedWidth(120)
-        self.l.addWidget(self.channelSelect, rowspace+2,15,1,2)
+        self.channelSelect.setEnabled(False)
+        self.l.addWidget(self.channelSelect, rowspace+2,16,1,2)
         self.l.setAlignment(self.channelSelect, QtCore.Qt.AlignLeft)
+        self.channelSelect.setMinimumWidth(200)
+        self.channelSelect.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
+        self.channelSelect.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         setattr(self.channelSelect, "items", lambda: [self.channelSelect.itemText(i) for i in range(self.channelSelect.count())])
 
         self.labelSelect = QComboBox()
         self.labelSelect.setStyleSheet(self.dropdowns)
         self.labelSelect.setFont(self.medfont)
         self.labelSelect.setCurrentText("")
         self.labelSelect.currentIndexChanged.connect(self.labelSelectIndexChange)
         self.labelSelect.setEditable(True)
         self.labelSelect.editTextChanged.connect(self.labelSelectEdit)
-        self.labelSelect.setFixedWidth(120)
+        self.labelSelect.setMinimumWidth(200)
         self.labelSelect.setEnabled(False)
-        self.l.addWidget(self.labelSelect, rowspace+2,17,1,2)
+        
+        self.l.addWidget(self.labelSelect, rowspace+2,18,1,2)
         self.l.setAlignment(self.labelSelect, QtCore.Qt.AlignLeft)
         setattr(self.labelSelect, "items", lambda: [self.labelSelect.itemText(i) for i in range(self.labelSelect.count())])
+        self.labelSelect.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
+        self.labelSelect.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
-        self.maskTypeSelect  = MaskTypeButtons(parent=self, row = rowspace+3, col = 15)
+        self.maskTypeSelect  = MaskTypeButtons(parent=self, row = rowspace+3, col = 16)
 
         # self.autoSaturationButton = QPushButton("Auto")
         # self.autoSaturationButton.setFixedWidth(45)
         # self.autoSaturationButton.setEnabled(True)
         # self.autoSaturationButton.setStyleSheet(self.styleInactive)
         # self.autoSaturationButton.setEnabled(False)
         # self.autoSaturationButton.clicked.connect(self.resetAutoSaturation)
@@ -671,14 +657,19 @@
         # self.saturationSlider.setMaximum(255)
         # self.saturationSlider.setLow(self.saturation[0])
         # self.saturationSlider.setHigh(self.saturation[-1])
         # self.saturationSlider.setTickPosition(QSlider.TicksRight)
         # self.saturationSlider.setFocusPolicy(QtCore.Qt.NoFocus)
         # self.saturationSlider.setEnabled(False)
         # self.l.addWidget(self.saturationSlider, rowspace+4, 22,1,3)
+        for i in range(self.mainViewRows):
+            self.l.setRowStretch(i, 10)
+
+        self.l.setColumnStretch(21,2)
+        self.l.setColumnStretch(0,2)
     
     def updateThreadDisplay(self):
         threadCount = len(self.threads)+1
         self.cpuCoreDisplay.setText(f"{threadCount}/{self.idealThreadCount} cores |")
 
     def enableMaskOperations(self):
         self.contourButton.setEnabled(True)
@@ -698,14 +689,17 @@
         #self.saturationSlider.setEnabled(True)
         #self.autoSaturationButton.setEnabled(True)
         #self.autoSaturationButton.setStyleSheet(self.styleUnpressed)
         self.modelButton.setEnabled(True)
         self.modelButton.setStyleSheet(self.styleUnpressed)
         self.segButton.setEnabled(True)
         self.segButton.setStyleSheet(self.styleUnpressed)
+        self.interpolateButton.setEnabled(True)
+        self.interpolateButton.setStyleSheet(self.styleUnpressed)
+        self.channelSelect.setEnabled(True)
     
     def toggleDrawing(self,b):
         if b:
             idx = 0
         else:
             idx = -1
         self.brushTypeSelect.setCurrentIndex(idx)
@@ -783,61 +777,57 @@
         labelsToTrack =  self.labelSelect.currentText()
         dlg  = GeneralParamDialog({}, [], f"Track {labelsToTrack}", self, labelSelects=["Cytoplasm Label"])
 
         if dlg.exec():
             self.deactivateButton(self.trackObjButton)
             data = dlg.getData()
 
+
             cellIdx = self.labelSelect.findText(data["Cytoplasm Label"])
             cells = self.maskData.channels[cellIdx][0, :, :,:].copy()
             obj = self.maskData.channels[self.maskZ][0, :, :,:].copy()
 
-            task = lambda: track_to_cell(obj, cells)
-            worker = TrackWorker(self, task, cellIdx)            
-            self.runLongTask(worker, worker.run, self.trackObjFinished, self.trackObjButton)
+            task = partial(track_to_cell, obj, cells)
+            worker = TrackWorker(task, cells, cellIdx, obj)            
+            self.runLongTask(worker,self.trackObjFinished, self.trackObjButton)
 
         else:
             return
     
     def trackObjFinished(self, tracked, z):
-        self.activateButton(self.trackObjButton)
         self.maskData.channels[z][0,:,:,:] = tracked
         contours = self.getCurrContourSet()
         newContours = tracked.copy()
         newContours[np.logical_not(contours>0)] = 0
         self.maskData.contours[z] = newContours
         self.updateCellData(idx = z)
-        self.handleFinished()
         self.maskZ = z
         self.drawMask()
     
     def trackFinished(self, z, tracked):
-        self.activateButton(self.trackButton)
-        self.handleFinished()
 
-        print(type(tracked))
         if isinstance(tracked, np.ndarray):
             self.maskData.channels[z][0,:,:,:] = tracked
             contours = self.getCurrContourSet()
             newContours = tracked.copy()
             newContours[np.logical_not(contours>0)] = 0
             self.maskData.contours[z] = newContours
             self.updateCellData(idx = z)
             self.maskZ = z
             self.drawMask()
         
 
     def trackButtonClick(self):
-        self.deactivateButton(self.trackButton)
 
         idxToTrack = self.maskZ
         cells = self.getCurrMaskSet().copy()
-        task = lambda: trackYeasts(cells)
-        worker = TrackWorker(self, task, idxToTrack)            
-        self.runLongTask(worker, worker.run, self.trackFinished, self.trackButton)
+        task = trackYeasts
+        worker = TrackWorker(task, cells, idxToTrack)     
+    
+        self.runLongTask(worker,self.trackFinished, self.trackButton)
 
         
     def updateCellData(self, idx = None):
         if not self.maskLoaded:
             return
   
         if idx:
@@ -1710,17 +1700,14 @@
             for i in [0,1]:
                 template = np.zeros_like(ims, dtype = output[i].dtype)
                 template[tStart:tStop+1] = output[i]
                 templates.append(template)
             outputTup = (templates[0], templates[1])
             self.loadMasks(outputTup, name = f"{imName}_{modelType}_{tStart}-{tStop}")
         
-        self.activateButton(self.modelButton)
-        self.handleFinished()
-        
     def evaluate(self):
         if not self.maskLoaded:
             return
         params = {label: False for label in self.labelSelect.items()}
         paramtypes = [bool] * len(params)
         labelSelects = ["validation"]
         evalDlg = GeneralParamDialog(params, paramtypes, "Evaluate Predictions", self, labelSelects = labelSelects)
@@ -1775,27 +1762,34 @@
             return potentialName
         n = (np.char.find(np.array(allNames), potentialName)+1).sum()
         if n>0:
             return f"{potentialName}-n"
         else:
             return potentialName
     
-    def runLongTask(self, worker, task, finished, button):
+    def runLongTask(self, worker, finished, button):
         if len(self.threads)+1>self.idealThreadCount:
             self.showError("Too Many Threads Running At This Time")
             self.activateButton(button)
             return
         
         thread = QThread()
-        self.threads.append(thread)
-        thread.started.connect(task)
+
         self.workers.append(worker)
+        self.threads.append(thread)
+
         worker.moveToThread(thread)
+        # Step 5: Connect signals and slots
+        thread.started.connect(worker.run)
         worker.finished.connect(finished)
+        worker.finished.connect(thread.quit)
+        worker.finished.connect(self.handleFinished)
         thread.start()
+        self.deactivateButton(button)
+        thread.finished.connect(lambda: self.activateButton(button))
         self.updateThreadDisplay()
 
 
     def computeModels(self):
         weightName = self.modelChoose.currentText() 
         if weightName == '':
             return
@@ -1811,23 +1805,40 @@
         dlg = dlgCls(modelClass.hyperparams, modelClass.types, modelType, self)
         
         if dlg.exec():
             params = dlg.getData()
             channel = params["Channel"]
             channelIndex = self.channelSelect.findText(channel)
             ims = self.imData.channels[channelIndex]
-
-            worker = SegmentWorker(self)
+            worker = SegmentWorker(modelClass,ims, params, weightPath, modelType)
             self.runLongTask(worker, 
-                             lambda: worker.run(modelClass,ims, params, weightPath, modelType),
                              self.segment,
                              self.modelButton)
+    
+    def interpolateButtonClicked(self):
+        dlg = GeneralParamDialog({"2x":False, "4x": False, "8x": False, "16x": False}, [bool,bool,bool,bool], "choose interpolation level", self)
+        if dlg.exec():
+            data = dlg.getData()
+            exp = None
+            for data, isChecked in data.items():
+                if isChecked:
+                    exp = int(data[0])/2
+                    break
         else:
-            self.activateButton(self.modelButton)
             return
+    
+        if exp:
+            ims = self.getCurrImSet().copy()
+            files = self.imData.files[self.imZ]
+            currName = self.channelSelect.currentText()
+            worker = InterpolationWorker(ims, files, f"{currName}_{data}interp", interpolate, np.uint8, exp)
+        else:
+            return
+
+        self.runLongTask(worker, self.addProcessedIms, self.interpolateButton)
 
     def doAdaptHist(self):
         files = self.imData.files[self.imZ]
         currName = self.channelSelect.currentText()
         newIms = im_funcs.do_adapt_hist(self.getCurrImSet())
         self.addProcessedIms(newIms, files, currName+"-adaptHist", dtype = np.float32)
     
@@ -2110,14 +2121,15 @@
     def checkDataAvailibility(self):
         hasLineages = self.hasLineageData()
         self.hasLineageBox.setChecked(hasLineages)
         self.hasCellDataBox.setChecked(self.hasCellData())
         self.showMotherDaughtersButton.setEnabled(hasLineages)
         self.showLineageButton.setEnabled(hasLineages)
 
+@profile
 def main():
     print("running main")
     app = QApplication([])
     im_path = "test_phase.tif"
     mask_path = "test_mask.tif"
     cdc_path = "test_cdc.tif"
     mainThread = app.instance().thread()
```

### Comparing `yeastvision-0.1.6/yeastvision/disk/io.py` & `yeastvision-0.1.7/yeastvision/disk/io.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/disk/reader.py` & `yeastvision-0.1.7/yeastvision/disk/reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,102 @@
 from skimage.measure import label
 from yeastvision.utils import get_mask_contour
 import pickle
 import pandas as pd
 from tqdm import tqdm
 from os.path import splitext, basename
 
+def get_channels_from_dir(dir, num_channels):
+    '''Loads images seperately by channel 
+    
+    Parameters
+    ----------
+    
+    dir: string 
+        The directory from which to load each set of channels. All files should be image files and should be named such that the first num_chhanels images below to distinct channel groups
+    
+    num_channels: int
+        Number of channels to load
+        
+    Returns
+    -------
+    
+    channels: a 4d Ndarray np.uint16 whose last dimension is the channels
+        Loaded image data. Has shape (num_ims/num_channels, test_im.shape[0], test_im.shape[1], num_channels)
+    
+    files: list[list[string]]
+        nested list structure containing all filepaths 
+    
+    names: list[string]
+        list of length num_channels of channel id strings obtained by splitting all letters after the last _ in filenames'''
+
+    all_files = sorted(glob.glob(os.path.join(dir, "*")))
+    num_ims = len(all_files)
+
+    if num_ims % num_channels != 0:
+        raise IndexError
+
+    test_im = imread(all_files[0])
+    im_shape = (num_ims/num_channels, test_im.shape[0], test_im.shape[1], num_channels)
+    channels = np.zeros(im_shape)
+    files = [[]*num_channels]
+    names = []
+    
+    for i in range(num_channels):
+        names.append(all_files[i].split("_")[-1])
+        for n in range(i,num_ims, num_channels):
+            channels[n,:,:,i] = imread(all_files[n])
+            files[i].append(all_files[n])
+
+    return channels, files, names
+
+def get_channel_files_from_dir(dir, num_channels):
+    '''Loads images seperately by channel 
+    
+    Parameters
+    ----------
+    
+    dir: string 
+        The directory from which to load each set of channels. All files should be image files and should be named such that the first num_chhanels images below to distinct channel groups
+    
+    num_channels: int
+        Number of channels to load
+        
+    Returns
+    -------
+    
+    channels: a 4d Ndarray np.uint16 whose last dimension is the channels
+        Loaded image data. Has shape (num_ims/num_channels, test_im.shape[0], test_im.shape[1], num_channels)
+    
+    files: list[list[string]]
+        nested list structure containing all filepaths 
+    
+    names: list[string]
+        list of length num_channels of channel id strings obtained by splitting all letters after the last _ in filenames'''
+
+    all_files = sorted(glob.glob(os.path.join(dir, "*")))
+    num_ims = len(all_files)
+
+    if num_ims % num_channels != 0:
+        raise IndexError
+
+    test_im = imread(all_files[0])
+    files = [[]*num_channels]
+    names = []
+    
+    for i in range(num_channels):
+        names.append(all_files[i].split("_")[-1])
+        for n in range(i,num_ims, num_channels):
+            files[i].append(all_files[n])
+
+    return files, names
+    
+
+
+
 def loadPkl(path, parent):
     '''data keys
     [Images, Saturation, Masks, Contours, Channels, Labels, Cells, Lineages]
     '''
     parent.overrideNpyPath = path
     parent.sessionId = splitext(basename(path))[0]
     with open(path, "rb") as f:
```

### Comparing `yeastvision-0.1.6/yeastvision/flou/blob_detect.py` & `yeastvision-0.1.7/yeastvision/flou/blob_detect.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/flou/utils.py` & `yeastvision-0.1.7/yeastvision/flou/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/ims.py` & `yeastvision-0.1.7/yeastvision/ims/im_funcs.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/install_weights.py` & `yeastvision-0.1.7/yeastvision/install_weights.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import zipfile
 import shutil
 import os
 from yeastvision.models.utils import MODEL_DIR
 from os.path import join
+from yeastvision.ims.interpolate import RIFE_DIR
 
 def do_install():
     current_directory = os.getcwd()
     folder_path = "yeastvision_weights.zip"
     models = [model for model in os.listdir(MODEL_DIR) if os.path.isdir(join(MODEL_DIR, model)) and model != "__pycache__"]
     print("Extracting weights for the following models", models)
 
@@ -23,15 +24,19 @@
 
             if "._" not in file_name:
                 # Get the name of the file without the extension
                 file_name_without_extension = os.path.splitext(file_name)[0]
 
                 if file_name_without_extension == "Bud_Seg":
                     destination_directory = join(MODEL_DIR, "artilife/budSeg")
-                    print("\tocated BudSeg weights - moving to", destination_directory)
+                    print("\tlocated BudSeg weights -- moving to", destination_directory)
+                
+                elif file_name_without_extension == "flownet":
+                    destination_directory = RIFE_DIR
+                    print("\tlocated weights for movie interpolation -- moving to", destination_directory)
 
                 else:
                     destination_name = ""
                     for model in models:
                         if model in file_name_without_extension:
                             destination_name = model
                             print("\tfound", file_name, "belong to", model)
```

### Comparing `yeastvision-0.1.6/yeastvision/models/YeaZ/model.py` & `yeastvision-0.1.7/yeastvision/models/YeaZ/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/YeaZ/segment.py` & `yeastvision-0.1.7/yeastvision/models/YeaZ/segment.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/YeaZ/unet.py` & `yeastvision-0.1.7/yeastvision/models/YeaZ/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/artilife/budSeg/model.py` & `yeastvision-0.1.7/yeastvision/models/artilife/budSeg/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/artilife/model.py` & `yeastvision-0.1.7/yeastvision/models/artilife/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/budNET/model.py` & `yeastvision-0.1.7/yeastvision/models/budNET/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/cp.py` & `yeastvision-0.1.7/yeastvision/models/cp.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/model.py` & `yeastvision-0.1.7/yeastvision/models/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/unet.py` & `yeastvision-0.1.7/yeastvision/models/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/models/utils.py` & `yeastvision-0.1.7/yeastvision/models/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/parts/canvas.py` & `yeastvision-0.1.7/yeastvision/parts/canvas.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/parts/dialogs.py` & `yeastvision-0.1.7/yeastvision/parts/dialogs.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/parts/guiparts.py` & `yeastvision-0.1.7/yeastvision/parts/guiparts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 from PyQt5 import QtGui, QtCore
-
 from PyQt5.QtGui import QPainter
-from PyQt5.QtWidgets import (QApplication,QSlider, QStyle, QStyleOptionSlider, QPushButton, QDialog,
-                            QDialogButtonBox, QLineEdit, QFormLayout, QCheckBox,  QSpinBox, QLabel, 
-                            QWidget, QComboBox, QGridLayout, QHBoxLayout)
+from PyQt5.QtWidgets import (QApplication,QSlider, QStyle, QStyleOptionSlider, QPushButton,QCheckBox, QComboBox, QFrame)
 from PyQt5.QtCore import Qt
 
 
+class QHLine(QFrame):
+    def __init__(self):
+        super(QHLine, self).__init__()
+        self.setFrameShape(QFrame.HLine)
+        self.setFrameShadow(QFrame.Sunken)
+
+
+class QVLine(QFrame):
+    def __init__(self):
+        super(QVLine, self).__init__()
+        self.setFrameShape(QFrame.VLine)
+        self.setFrameShadow(QFrame.Sunken)
+
+
 class ReadOnlyCheckBox(QCheckBox):
     def __init__(self, parent=None):
         super().__init__(parent)
     
     def mousePressEvent(self, event):
         event.ignore()
```

### Comparing `yeastvision-0.1.6/yeastvision/parts/menu.py` & `yeastvision-0.1.7/yeastvision/parts/menu.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/plot/cell_table.py` & `yeastvision-0.1.7/yeastvision/plot/cell_table.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/plot/plot.py` & `yeastvision-0.1.7/yeastvision/plot/plot.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/plot/types.py` & `yeastvision-0.1.7/yeastvision/plot/types.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/cell.py` & `yeastvision-0.1.7/yeastvision/track/cell.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/data.py` & `yeastvision-0.1.7/yeastvision/track/data.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/hungarian_track.py` & `yeastvision-0.1.7/yeastvision/track/hungarian_track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/lineage.py` & `yeastvision-0.1.7/yeastvision/track/lineage.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/mat.py` & `yeastvision-0.1.7/yeastvision/track/mat.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/track.py` & `yeastvision-0.1.7/yeastvision/track/track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/track/utils.py` & `yeastvision-0.1.7/yeastvision/track/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision/utils.py` & `yeastvision-0.1.7/yeastvision/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.6/yeastvision.egg-info/PKG-INFO` & `yeastvision-0.1.7/yeastvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.6
+Version: 0.1.7
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 Yeastvision is ready to go for cpu-usage as soon as it downloaded. GPU-usage requires some additional steps after download. To download:
 
 1. Install an [Anaconda](https://www.anaconda.com/products/distribution) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
 2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
 3. Create a new environment with `conda create --name yeastvision python=3.10.o`. 
 4. Activate this new environment by running `conda activate yeastvision`
 5. Run `python -m pip install yeastvision` to download our package plus all dependencies
-6. Download the weights [online](https://drive.google.com/file/d/1J3R4JKILkQNM0Ap-MKxqv61oAxObSjBo/view?usp=drive_link). 
+6. Download the weights [online](https://drive.google.com/file/d/1Zl3b00eSbe3wbxpYOknEP5q0A86XtEfL/view?usp=sharing). 
 7. Run `install-weights` in the same directory as the *yeastvision_weights.zip* file
 
 
 You should upgrade yeastvision (package [here](https://pypi.org/project/yeastvision/)) periodically as it is still in development. To do so, run the following in the environment:
 
 ~~~sh
 python -m pip install yeastvision --upgrade
```

### Comparing `yeastvision-0.1.6/yeastvision.egg-info/SOURCES.txt` & `yeastvision-0.1.7/yeastvision.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 LICENSE
 README.md
 setup.py
 yeastvision/__init__.py
 yeastvision/__main__.py
-yeastvision/ims.py
 yeastvision/install_weights.py
 yeastvision/utils.py
 yeastvision.egg-info/PKG-INFO
 yeastvision.egg-info/SOURCES.txt
 yeastvision.egg-info/dependency_links.txt
 yeastvision.egg-info/entry_points.txt
 yeastvision.egg-info/requires.txt
 yeastvision.egg-info/top_level.txt
 yeastvision/disk/__init__.py
 yeastvision/disk/io.py
 yeastvision/disk/reader.py
 yeastvision/flou/__init__.py
 yeastvision/flou/blob_detect.py
 yeastvision/flou/utils.py
+yeastvision/ims/__init__.py
+yeastvision/ims/im_funcs.py
+yeastvision/ims/interpolate.py
+yeastvision/ims/rife_model/IFNet.py
+yeastvision/ims/rife_model/IFNet_2R.py
+yeastvision/ims/rife_model/IFNet_m.py
+yeastvision/ims/rife_model/RIFE.py
+yeastvision/ims/rife_model/__init__.py
+yeastvision/ims/rife_model/interpolate.py
+yeastvision/ims/rife_model/laplacian.py
+yeastvision/ims/rife_model/loss.py
+yeastvision/ims/rife_model/refine.py
+yeastvision/ims/rife_model/refine_2R.py
+yeastvision/ims/rife_model/warplayer.py
 yeastvision/models/__init__.py
 yeastvision/models/cp.py
 yeastvision/models/eval.py
 yeastvision/models/loss.py
 yeastvision/models/model.py
 yeastvision/models/unet.py
 yeastvision/models/utils.py
```

