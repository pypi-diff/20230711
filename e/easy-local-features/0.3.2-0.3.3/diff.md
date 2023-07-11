# Comparing `tmp/easy_local_features-0.3.2.tar.gz` & `tmp/easy_local_features-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.3.2.tar", last modified: Wed Jul  5 12:51:57 2023, max compression
+gzip compressed data, was "easy_local_features-0.3.3.tar", last modified: Tue Jul 11 16:39:47 2023, max compression
```

## Comparing `easy_local_features-0.3.2.tar` & `easy_local_features-0.3.3.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    32722 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/LICENSE_DISK.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    21121 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/LICENSE_R2D2.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     7009 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/LICENSE_SUPERGLUE.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1942 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1690 2023-07-05 12:20:10.000000 easy_local_features-0.3.2/README.md
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.798528 easy_local_features-0.3.2/easy_local_features/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/__init__.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.798528 easy_local_features-0.3.2/easy_local_features/datasets/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/datasets/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/datasets/download.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/feature/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34250 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_dalf.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2624 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_deal.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6746 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_disk.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6012 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_r2d2.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2857 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_superpoint.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/matching/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2103 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/baseline_loftr.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5116 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/baseline_superglue.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/core.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/__init__.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/__init__.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       24 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/__init__.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2652 2023-07-05 12:00:59.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/structs.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       79 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      291 2023-07-05 12:01:08.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2096 2023-07-05 12:01:56.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/epi.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3406 2023-07-05 12:02:13.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/pose.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      113 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2732 2023-07-05 12:02:43.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2566 2023-07-05 12:03:01.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5454 2023-07-05 12:04:18.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/detector.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2177 2023-07-05 12:05:58.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/disk.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      865 2023-07-05 12:04:30.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/nms.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      249 2023-07-05 10:39:12.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4159 2023-07-05 11:59:54.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/blocks.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2070 2023-07-05 10:39:12.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/ops.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3289 2023-07-05 12:00:26.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/unet.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1291 2023-07-05 10:39:12.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/utils.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6223 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     9927 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract_kapture.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2360 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1720 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/losses.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     7158 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/patchnet.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1760 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2006 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    15031 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/sampler.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1080 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/common.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    14318 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/dataloader.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2208 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/trainer.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    18298 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     7160 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5647 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/viz.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5018 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/train.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4203 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/__init__.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3417 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/matching.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    11537 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superglue.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     8092 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superpoint.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    20039 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/utils.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/utils/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:28:06.000000 easy_local_features-0.3.2/easy_local_features/utils/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      293 2023-07-05 10:29:53.000000 easy_local_features-0.3.2/easy_local_features/utils/generic_match.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.798528 easy_local_features-0.3.2/easy_local_features.egg-info/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1942 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3607 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/SOURCES.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/dependency_links.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       68 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/requires.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/top_level.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/setup.cfg
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      910 2023-07-05 12:51:15.000000 easy_local_features-0.3.2/setup.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.866134 easy_local_features-0.3.3/
+-rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.3/LICENSE_DISK.txt
+-rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.3/LICENSE_R2D2.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.3/LICENSE_SUPERGLUE.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     2023 2023-07-11 16:39:47.865922 easy_local_features-0.3.3/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     1771 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/README.md
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.847938 easy_local_features-0.3.3/easy_local_features/
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.3/easy_local_features/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.850061 easy_local_features-0.3.3/easy_local_features/datasets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.3/easy_local_features/datasets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    10235 2023-07-11 16:37:31.000000 easy_local_features-0.3.3/easy_local_features/datasets/augmentor.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.3/easy_local_features/datasets/download.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.851981 easy_local_features-0.3.3/easy_local_features/feature/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    34684 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_superpoint.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.852959 easy_local_features-0.3.3/easy_local_features/matching/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.3/easy_local_features/matching/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2103 2023-07-04 22:47:59.000000 easy_local_features-0.3.3/easy_local_features/matching/baseline_loftr.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.3/easy_local_features/matching/baseline_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.3/easy_local_features/matching/core.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853072 easy_local_features-0.3.3/easy_local_features/submodules/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.3/easy_local_features/submodules/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853186 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853302 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/
+-rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853906 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2652 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/structs.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.855327 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/
+-rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      291 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2096 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/epi.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3406 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/pose.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.856653 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/
+-rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2732 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2566 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5454 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/detector.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2177 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      865 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/nms.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.857757 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/
+-rw-r--r--   0 cadar      (501) staff       (20)      249 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4159 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/blocks.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2070 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/ops.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3289 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/unet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1291 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.859159 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract.py
+-rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract_kapture.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.861444 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/losses.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/patchnet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/sampler.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.863207 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/common.py
+-rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/dataloader.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/trainer.py
+-rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/viz.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/train.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.863465 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.864874 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/matching.py
+-rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superpoint.py
+-rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.865448 easy_local_features-0.3.3/easy_local_features/utils/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/utils/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      293 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/utils/generic_match.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.849012 easy_local_features-0.3.3/easy_local_features.egg-info/
+-rw-r--r--   0 cadar      (501) staff       (20)     2023 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     3649 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/SOURCES.txt
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/dependency_links.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       68 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/requires.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/top_level.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-11 16:39:47.866195 easy_local_features-0.3.3/setup.cfg
+-rw-r--r--   0 cadar      (501) staff       (20)      910 2023-07-11 16:39:34.000000 easy_local_features-0.3.3/setup.py
```

### Comparing `easy_local_features-0.3.2/LICENSE_DISK.txt` & `easy_local_features-0.3.3/LICENSE_DISK.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/LICENSE_R2D2.txt` & `easy_local_features-0.3.3/LICENSE_R2D2.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/LICENSE_SUPERGLUE.txt` & `easy_local_features-0.3.3/LICENSE_SUPERGLUE.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/PKG-INFO` & `easy_local_features-0.3.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: easy_local_features
-Version: 0.3.2
-Author: eucadar
-Author-email: python@eucadar.com
-Description-Content-Type: text/markdown
-License-File: LICENSE_DISK.txt
-License-File: LICENSE_R2D2.txt
-License-File: LICENSE_SUPERGLUE.txt
-
 # easy-local-features-baselines
 
 Just some scripts to make things easier for the local features baselines.
 
 # Installation
 
 
@@ -55,15 +45,18 @@
 - [ ] Make a general maching class
   - The idea is to have a class that can match images using any local feature extractor and any matching method.
 - [ ] Fix requirements to install automatically with the package (maybe)
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
 - [ ] Add more baselines :)
   - [x] DEAL
+    - [ ] Add LICENSE file
   - [x] R2D2
   - [x] DISK
   - [x] SuperPoin
   - [x] SuperGlue
-  - [x] DELF
+  - [x] DALF
+    - [ ] Add LICENSE file
   - [ ] ASLFeat
   - [x] LoFTR
-  - [ ] DKM
+    - [ ] Add LICENSE file
+  - [ ] DKM
```

### Comparing `easy_local_features-0.3.2/README.md` & `easy_local_features-0.3.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: easy_local_features
+Version: 0.3.3
+Author: eucadar
+Author-email: python@eucadar.com
+Description-Content-Type: text/markdown
+License-File: LICENSE_DISK.txt
+License-File: LICENSE_R2D2.txt
+License-File: LICENSE_SUPERGLUE.txt
+
 # easy-local-features-baselines
 
 Just some scripts to make things easier for the local features baselines.
 
 # Installation
 
 
@@ -45,15 +55,18 @@
 - [ ] Make a general maching class
   - The idea is to have a class that can match images using any local feature extractor and any matching method.
 - [ ] Fix requirements to install automatically with the package (maybe)
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
 - [ ] Add more baselines :)
   - [x] DEAL
+    - [ ] Add LICENSE file
   - [x] R2D2
   - [x] DISK
   - [x] SuperPoin
   - [x] SuperGlue
-  - [x] DELF
+  - [x] DALF
+    - [ ] Add LICENSE file
   - [ ] ASLFeat
   - [x] LoFTR
-  - [ ] DKM
+    - [ ] Add LICENSE file
+  - [ ] DKM
```

### Comparing `easy_local_features-0.3.2/easy_local_features/datasets/download.py` & `easy_local_features-0.3.3/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/feature/baseline_dalf.py` & `easy_local_features-0.3.3/easy_local_features/feature/baseline_dalf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 '''
   - This script contains the model definitions for detection of kps trained with policy gradient;
   - Description is performed by the deformation-aware network and optimized with hard triplet loss;
   - Detection and description are simulateously optimized to be deformation-aware.
+
+    @author: Guilherme Potje
+    @cite: @INPROCEEDINGS{potje2023cvpr,
+            author={Guilherme {Potje} and and Felipe {Cadar} and Andre {Araujo} and Renato {Martins} and Erickson R. {Nascimento}},
+            booktitle={2023 IEEE / CVF Computer Vision and Pattern Recognition (CVPR)}, 
+            title={Enhancing Deformable Local Features by Jointly Learning to Detect and Describe Keypoints}, 
+            year={2023}
+    }
+
 '''
 
 import torch
 from torch import nn
 from torch import optim
 import torch.nn.functional as F
 import math
```

### Comparing `easy_local_features-0.3.2/easy_local_features/feature/baseline_deal.py` & `easy_local_features-0.3.3/easy_local_features/feature/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/feature/baseline_disk.py` & `easy_local_features-0.3.3/easy_local_features/feature/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/feature/baseline_r2d2.py` & `easy_local_features-0.3.3/easy_local_features/feature/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/feature/baseline_superpoint.py` & `easy_local_features-0.3.3/easy_local_features/feature/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/matching/baseline_loftr.py` & `easy_local_features-0.3.3/easy_local_features/matching/baseline_loftr.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/matching/baseline_superglue.py` & `easy_local_features-0.3.3/easy_local_features/matching/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/structs.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/structs.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/epi.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/epi.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/pose.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/pose.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/detector.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/detector.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/disk.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/nms.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/nms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/blocks.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/blocks.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/ops.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/ops.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/unet.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/unet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/utils.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract_kapture.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract_kapture.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/ap_loss.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/ap_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/losses.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/losses.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/patchnet.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/patchnet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/sampler.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/sampler.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/common.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/common.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/dataloader.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/dataloader.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/trainer.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/viz.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/viz.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/train.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/train.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/viz_heatmaps.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/viz_heatmaps.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/matching.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/matching.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superglue.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superpoint.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/utils.py` & `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.2/easy_local_features.egg-info/PKG-INFO` & `easy_local_features-0.3.3/easy_local_features.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-local-features
-Version: 0.3.2
+Version: 0.3.3
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
 
@@ -55,15 +55,18 @@
 - [ ] Make a general maching class
   - The idea is to have a class that can match images using any local feature extractor and any matching method.
 - [ ] Fix requirements to install automatically with the package (maybe)
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
 - [ ] Add more baselines :)
   - [x] DEAL
+    - [ ] Add LICENSE file
   - [x] R2D2
   - [x] DISK
   - [x] SuperPoin
   - [x] SuperGlue
-  - [x] DELF
+  - [x] DALF
+    - [ ] Add LICENSE file
   - [ ] ASLFeat
   - [x] LoFTR
+    - [ ] Add LICENSE file
   - [ ] DKM
```

### Comparing `easy_local_features-0.3.2/easy_local_features.egg-info/SOURCES.txt` & `easy_local_features-0.3.3/easy_local_features.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 easy_local_features/__init__.py
 easy_local_features.egg-info/PKG-INFO
 easy_local_features.egg-info/SOURCES.txt
 easy_local_features.egg-info/dependency_links.txt
 easy_local_features.egg-info/requires.txt
 easy_local_features.egg-info/top_level.txt
 easy_local_features/datasets/__init__.py
+easy_local_features/datasets/augmentor.py
 easy_local_features/datasets/download.py
 easy_local_features/feature/__init__.py
 easy_local_features/feature/baseline_dalf.py
 easy_local_features/feature/baseline_deal.py
 easy_local_features/feature/baseline_disk.py
 easy_local_features/feature/baseline_r2d2.py
 easy_local_features/feature/baseline_superpoint.py
```

### Comparing `easy_local_features-0.3.2/setup.py` & `easy_local_features-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         long_description = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='easy_local_features',
-    version='0.3.2',
+    version='0.3.3',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets')),
     include_package_data=True,
     install_requires=[
         'numpy',
         'scipy',
```

