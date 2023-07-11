# Comparing `tmp/nkululeko-0.52.0.tar.gz` & `tmp/nkululeko-0.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.52.0.tar", last modified: Thu Jul  6 09:40:19 2023, max compression
+gzip compressed data, was "nkululeko-0.53.0.tar", last modified: Tue Jul 11 17:20:59 2023, max compression
```

## Comparing `nkululeko-0.52.0.tar` & `nkululeko-0.53.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-06 09:40:19.769135 nkululeko-0.52.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6975 2023-07-06 09:40:02.000000 nkululeko-0.52.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.52.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18774 2023-07-06 09:40:19.769135 nkululeko-0.52.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.52.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-06 09:40:19.769135 nkululeko-0.52.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.52.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.52.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.52.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.52.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.52.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.52.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.52.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.52.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.52.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.52.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21545 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.52.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.52.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.52.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.52.0/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.52.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.52.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.52.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.52.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.52.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.52.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.52.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.52.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.52.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.52.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.52.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6665 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.52.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.52.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.52.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.52.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.52.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.52.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.52.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.52.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.52.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.52.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.52.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.52.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.52.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.52.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.52.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.52.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.52.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.52.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.52.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.52.0/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.52.0/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.52.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.52.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.52.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.52.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.52.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.52.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.52.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10463 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-06 09:40:19.769135 nkululeko-0.52.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18774 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.52.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-06 09:40:19.769135 nkululeko-0.52.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.52.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-11 17:20:59.162757 nkululeko-0.53.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7166 2023-07-11 17:19:19.000000 nkululeko-0.53.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.53.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18965 2023-07-11 17:20:59.162757 nkululeko-0.53.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.53.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-11 17:20:59.158756 nkululeko-0.53.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.53.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.53.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.53.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.53.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.53.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-11 17:19:50.000000 nkululeko-0.53.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.53.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.53.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.53.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.53.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.53.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21808 2023-07-11 17:10:58.000000 nkululeko-0.53.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.53.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.53.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.53.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.53.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.53.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.53.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.53.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.53.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.53.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.53.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.53.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.53.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.53.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.53.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.53.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3510 2023-07-11 17:13:59.000000 nkululeko-0.53.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6717 2023-07-11 16:16:04.000000 nkululeko-0.53.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.53.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.53.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.53.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.53.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.53.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.53.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.53.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.53.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.53.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.53.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.53.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.53.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.53.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.53.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.53.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.53.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.53.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.53.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.53.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.53.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.53.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.53.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.53.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.53.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.53.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.53.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.53.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.53.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.53.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10463 2023-07-06 09:40:02.000000 nkululeko-0.53.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-11 17:20:59.162757 nkululeko-0.53.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18965 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1675 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.53.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-11 17:20:59.162757 nkululeko-0.53.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.53.0/setup.py
```

### Comparing `nkululeko-0.52.0/CHANGELOG.md` & `nkululeko-0.53.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 0.53.0
+--------------
+* added file checks: size in bytes and voice activity detection with silero
+
+Version 0.52.1
+--------------
+* bugfix: min/max duration_of_sample was not working
+
 Version 0.52.0
 --------------
 * added flexible value distribution plots
 
 Version 0.51.0
 --------------
 * added datafilter
```

### Comparing `nkululeko-0.52.0/LICENSE` & `nkululeko-0.53.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/PKG-INFO` & `nkululeko-0.53.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.52.0
+Version: 0.53.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -211,14 +211,22 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.53.0
+--------------
+* added file checks: size in bytes and voice activity detection with silero
+
+Version 0.52.1
+--------------
+* bugfix: min/max duration_of_sample was not working
+
 Version 0.52.0
 --------------
 * added flexible value distribution plots
 
 Version 0.51.0
 --------------
 * added datafilter
```

### Comparing `nkululeko-0.52.0/README.md` & `nkululeko-0.53.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/augment.py` & `nkululeko-0.53.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/augmenter.py` & `nkululeko-0.53.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/cacheddataset.py` & `nkululeko-0.53.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/dataset.py` & `nkululeko-0.53.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/dataset_csv.py` & `nkululeko-0.53.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.53.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/demo.py` & `nkululeko-0.53.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/demo_predictor.py` & `nkululeko-0.53.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/experiment.py` & `nkululeko-0.53.0/nkululeko/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nkululeko.runmanager import Runmanager
 from nkululeko.test_predictor import Test_predictor
 from nkululeko.feats_analyser import FeatureAnalyser
 from nkululeko.util import Util
 from nkululeko.feature_extractor import FeatureExtractor
 from nkululeko.plots import Plots
 from nkululeko.filter_data import DataFilter
+from nkululeko.file_checker import FileChecker
 import nkululeko.glob_conf as glob_conf
 from nkululeko.demo_predictor import Demo_predictor
 import ast # To convert strings to objects
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 from nkululeko.scaler import Scaler
 import pickle
@@ -175,14 +176,20 @@
             storage_test = f'{store}testdf.csv'
             storage_train = f'{store}traindf.csv'
             self.df_test.to_csv(storage_test)
             self.df_train.to_csv(storage_train)
 
         self.util.copy_flags(self, self.df_test)
         self.util.copy_flags(self, self.df_train)
+        # Try data checks
+        datachecker = FileChecker(self.df_train)
+        self.df_train = datachecker.all_checks()
+        datachecker.set_data(self.df_test)
+        self.df_test = datachecker.all_checks()
+
         # Check for filters
         filter_sample_selection = self.util.config_val('DATA', 'filter.sample_selection', 'all')
         if filter_sample_selection=='all':
             datafilter = DataFilter(self.df_train)
             self.df_train = datafilter.all_filters()
             datafilter = DataFilter(self.df_test)
             self.df_test = datafilter.all_filters()
```

### Comparing `nkululeko-0.52.0/nkululeko/explore.py` & `nkululeko-0.53.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_analyser.py` & `nkululeko-0.53.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_audmodel.py` & `nkululeko-0.53.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.53.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_clap.py` & `nkululeko-0.53.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_import.py` & `nkululeko-0.53.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_mld.py` & `nkululeko-0.53.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_opensmile.py` & `nkululeko-0.53.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_oxbow.py` & `nkululeko-0.53.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_praat.py` & `nkululeko-0.53.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_trill.py` & `nkululeko-0.53.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.53.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feature_extractor.py` & `nkululeko-0.53.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/featureset.py` & `nkululeko-0.53.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/feinberg_praat.py` & `nkululeko-0.53.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/filter_data.py` & `nkululeko-0.53.0/nkululeko/filter_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,30 +70,32 @@
             max_dur = self.util.config_val_data(data_name, 'max_duration_of_sample', False)
         if min_dur or max_dur:
             if not isinstance(self.df.index, pd.MultiIndex):
                 self.util.debug('converting file index to multi index, this might take a while...')
                 self.df.index = audformat.utils.to_segmented_index(self.df.index, allow_nat=False)    
             if min_dur:
                 old_samples = self.df.shape[0]
+                df = self.df.copy()
                 for i in self.df.index:
                     start = i[1]
                     end = i[2]
                     dur = (end - start).total_seconds()
                     if dur < float(min_dur):
-                        df = self.df.drop(i, axis=0)
-                self.util.debug(f'{data_name}: filtered samples less than {min_dur} seconds, reduced samples from {old_samples} to {self.df.shape[0]}')
+                        df = df.drop(i, axis=0)
+                self.util.debug(f'{data_name}: filtered samples less than {min_dur} seconds, reduced samples from {old_samples} to {df.shape[0]}')
             if max_dur:
                 old_samples = self.df.shape[0]
+                df = self.df.copy()
                 for i in self.df.index:
                     start = i[1]
                     end = i[2]
                     dur = (end - start).total_seconds()
                     if dur > float(max_dur):
-                        df = self.df.drop(i, axis=0)
-                self.util.debug(f'{data_name}: filtered samples more than {max_dur} seconds, reduced samples from {old_samples} to {self.df.shape[0]}')
+                        df = df.drop(i, axis=0)
+                self.util.debug(f'{data_name}: filtered samples more than {max_dur} seconds, reduced samples from {old_samples} to {df.shape[0]}')
             self.util.copy_flags(self.df, df)   
             self.df = df
             return df
         else:
             return self.df
     
     def filter_value(self, data_name=''):
```

### Comparing `nkululeko-0.52.0/nkululeko/loss_ccc.py` & `nkululeko-0.53.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.53.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model.py` & `nkululeko-0.53.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_cnn.py` & `nkululeko-0.53.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_gmm.py` & `nkululeko-0.53.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_knn.py` & `nkululeko-0.53.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_knn_reg.py` & `nkululeko-0.53.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_mlp.py` & `nkululeko-0.53.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.53.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/model_svm.py` & `nkululeko-0.53.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/modelrunner.py` & `nkululeko-0.53.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/nkululeko.py` & `nkululeko-0.53.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/plots.py` & `nkululeko-0.53.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/randomsplicer.py` & `nkululeko-0.53.0/nkululeko/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/randomsplicing.py` & `nkululeko-0.53.0/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/reporter.py` & `nkululeko-0.53.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/runmanager.py` & `nkululeko-0.53.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/scaler.py` & `nkululeko-0.53.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.53.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/test.py` & `nkululeko-0.53.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/test_predictor.py` & `nkululeko-0.53.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko/util.py` & `nkululeko-0.53.0/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.52.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.53.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.52.0
+Version: 0.53.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -211,14 +211,22 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.53.0
+--------------
+* added file checks: size in bytes and voice activity detection with silero
+
+Version 0.52.1
+--------------
+* bugfix: min/max duration_of_sample was not working
+
 Version 0.52.0
 --------------
 * added flexible value distribution plots
 
 Version 0.51.0
 --------------
 * added datafilter
```

### Comparing `nkululeko-0.52.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.53.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 nkululeko/feats_oxbow.py
 nkululeko/feats_praat.py
 nkululeko/feats_trill.py
 nkululeko/feats_wav2vec2.py
 nkululeko/feature_extractor.py
 nkululeko/featureset.py
 nkululeko/feinberg_praat.py
+nkululeko/file_checker.py
 nkululeko/filter_data.py
 nkululeko/glob_conf.py
 nkululeko/loss_ccc.py
 nkululeko/loss_softf1loss.py
 nkululeko/model.py
 nkululeko/model_bayes.py
 nkululeko/model_cnn.py
```

### Comparing `nkululeko-0.52.0/setup.cfg` & `nkululeko-0.53.0/setup.cfg`

 * *Files identical despite different names*

