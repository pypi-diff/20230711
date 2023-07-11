# Comparing `tmp/graphium-2.1.2.tar.gz` & `tmp/graphium-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphium-2.1.2.tar", last modified: Tue Jul 11 19:29:34 2023, max compression
+gzip compressed data, was "graphium-2.1.3.tar", last modified: Tue Jul 11 19:58:50 2023, max compression
```

## Comparing `graphium-2.1.2.tar` & `graphium-2.1.3.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.172443 graphium-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.120440 graphium-2.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.120440 graphium-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-11 19:24:38.000000 graphium-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-11 19:24:38.000000 graphium-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:29:34.172443 graphium-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-11 19:24:38.000000 graphium-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:24:38.000000 graphium-2.1.2/cleanup_files.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 19:24:38.000000 graphium-2.1.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.108440 graphium-2.1.2/docs/_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/_assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/_assets/css/custom-graphium.css
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/_assets/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/_assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/_assets/js/google-analytics.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.config.md
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.data.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.features.md
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.ipu.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/api/graphium.nn/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/architectures.md
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/encoders.md
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/graphium.nn.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/pyg_layers.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.trainer.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.visualization.md
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/baseline.md
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/cli_references.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/datasets.md
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/design.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/datamodule.png
--rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/full_graph_network.png
--rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/pretrained_models.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.112440 graphium-2.1.2/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/tutorials/feature_processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/choosing_parallelization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/csv_to_parquet.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/timing_parallel.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/tutorials/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/gnn/add_new_gnn_layers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/gnn/making_gnn_networks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/gnn/using_gnn_layers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/tutorials/model_training/
--rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/model_training/running-multitask-ipu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/model_training/simple-molecular-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 19:24:38.000000 graphium-2.1.2/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/expts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/expts/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m_mod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_gpspp_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_mpnn_10M_b3lyp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_mpnn_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_mpnn_pcqm4m.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.132441 graphium-2.1.2/expts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/data/micro_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/data/tiny_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/dataset_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_get_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.132441 graphium-2.1.2/expts/neurips2023_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.132441 graphium-2.1.2/expts/neurips2023_configs/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_classifigression_l1000.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_mpnn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_luis_jama.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gated_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_mpnn.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/debug/
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/debug/config_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/run_validation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/graphium/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/config/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/config_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/fake_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/zinc_default_multitask_pyg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/data/L1000/
--rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/QM9/
--rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/QM9/micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/QM9/micro_qm9.parquet
--rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/QM9/norm_micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)   108384 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/make_data_splits/
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/micro_ZINC/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/micro_ZINC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/micro_ZINC/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multilevel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/multitask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/tiny_ZINC_SA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/tiny_ZINC_logp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/tiny_ZINC_score.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/sdf2csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/single_atom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/single_atom_dataset/single_atom_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/smiles_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/expts/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/expts/pyg_batching_sparse.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.148441 graphium-2.1.2/graphium/features/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/commute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/electrostatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/nmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/periodic_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/test_new_pes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/transfer_pos_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.148441 graphium-2.1.2/graphium/ipu/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_simple_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/to_dense_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.148441 graphium-2.1.2/graphium/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.152442 graphium-2.1.2/graphium/nn/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/encoder_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    73133 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/global_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/pyg_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/base_graph_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/base_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.152442 graphium-2.1.2/graphium/nn/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/bessel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/laplace_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/mlp_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/signnet_pos_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.156442 graphium-2.1.2/graphium/nn/pyg_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/dimenet_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gated_gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gin_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gps_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/mpnn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/pna_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/pooling_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.156442 graphium-2.1.2/graphium/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/predictor_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/predictor_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.156442 graphium-2.1.2/graphium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/custom_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/moving_average_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/mup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/safe_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/graphium/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/visualization/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/visualization/vis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/graphium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-11 19:29:34.000000 graphium-2.1.2/graphium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 19:24:38.000000 graphium-2.1.2/lightning.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-11 19:24:38.000000 graphium-2.1.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-datamodule-invalidate-cache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-datamodule-ogb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-datamodule.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-pretrained.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-training-loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/running-fingerprints-from-pretrained-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/running-model-from-config.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/profiling/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/configs_profiling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/profile_mol_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/profile_one_of_k_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/profile_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-11 19:24:38.000000 graphium-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 19:24:38.000000 graphium-2.1.2/requirements_ipu.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-11 19:24:38.000000 graphium-2.1.2/scripts/convert_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:24:38.000000 graphium-2.1.2/scripts/ipu_start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 19:24:38.000000 graphium-2.1.2/scripts/ipu_venv.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:29:34.172443 graphium-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.168443 graphium-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/config_test_ipu_dataloader.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/converted_fake_multilevel_data.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.168443 graphium-2.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/config_micro_ZINC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_corrupt.csv
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/pcqm4mv2-2k.csv
--rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/fake_and_missing_multilevel_data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_base_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_mtl_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_multitask_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_mup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pe_nodepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pe_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pe_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pos_transfer_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_positional_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_positional_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pyg_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.387511 graphium-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.315511 graphium-2.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.315511 graphium-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-11 19:53:38.000000 graphium-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-11 19:53:38.000000 graphium-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:58:50.387511 graphium-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-11 19:53:38.000000 graphium-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:53:38.000000 graphium-2.1.3/cleanup_files.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 19:53:38.000000 graphium-2.1.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.315511 graphium-2.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.307511 graphium-2.1.3/docs/_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/_assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/_assets/css/custom-graphium.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/_assets/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/_assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/_assets/js/google-analytics.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.config.md
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.ipu.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/api/graphium.nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/architectures.md
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/graphium.nn.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/pyg_layers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.trainer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.visualization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/baseline.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/cli_references.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/design.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/datamodule.png
+-rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/full_graph_network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/pretrained_models.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.307511 graphium-2.1.3/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/docs/tutorials/feature_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/choosing_parallelization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/csv_to_parquet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/timing_parallel.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/docs/tutorials/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/gnn/add_new_gnn_layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/gnn/making_gnn_networks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/gnn/using_gnn_layers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/docs/tutorials/model_training/
+-rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/model_training/running-multitask-ipu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/model_training/simple-molecular-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 19:53:38.000000 graphium-2.1.3/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/expts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m_mod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_gpspp_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_mpnn_10M_b3lyp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_mpnn_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_mpnn_pcqm4m.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/data/micro_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/data/tiny_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/dataset_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_get_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/neurips2023_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/neurips2023_configs/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_classifigression_l1000.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_mpnn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_luis_jama.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gated_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_mpnn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/debug/config_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/run_validation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/graphium/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.335511 graphium-2.1.3/graphium/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.339511 graphium-2.1.3/graphium/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/config_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/fake_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/zinc_default_multitask_pyg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.339511 graphium-2.1.3/graphium/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.339511 graphium-2.1.3/graphium/data/L1000/
+-rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/QM9/
+-rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/QM9/micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/QM9/micro_qm9.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/QM9/norm_micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108384 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/make_data_splits/
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/micro_ZINC/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/micro_ZINC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/micro_ZINC/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multilevel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/multitask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/tiny_ZINC_SA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/tiny_ZINC_logp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/tiny_ZINC_score.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/sdf2csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/single_atom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/single_atom_dataset/single_atom_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/smiles_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/expts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/expts/pyg_batching_sparse.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.347511 graphium-2.1.3/graphium/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/commute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/electrostatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/nmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/periodic_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/test_new_pes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/transfer_pos_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.347511 graphium-2.1.3/graphium/ipu/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_simple_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/to_dense_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.351511 graphium-2.1.3/graphium/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.351511 graphium-2.1.3/graphium/nn/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/encoder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73133 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/global_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/pyg_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/base_graph_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/base_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.351511 graphium-2.1.3/graphium/nn/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/bessel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/laplace_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/mlp_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/signnet_pos_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.355511 graphium-2.1.3/graphium/nn/pyg_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/dimenet_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gated_gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gin_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gps_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/mpnn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/pna_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/pooling_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.355511 graphium-2.1.3/graphium/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/predictor_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/predictor_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.359511 graphium-2.1.3/graphium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/custom_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/moving_average_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/safe_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.359511 graphium-2.1.3/graphium/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/visualization/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/visualization/vis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.335511 graphium-2.1.3/graphium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 19:53:38.000000 graphium-2.1.3/lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-11 19:53:38.000000 graphium-2.1.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.363511 graphium-2.1.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-datamodule-invalidate-cache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-datamodule-ogb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-datamodule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-pretrained.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-training-loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/running-fingerprints-from-pretrained-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/running-model-from-config.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.363511 graphium-2.1.3/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/configs_profiling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/profile_mol_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/profile_one_of_k_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/profile_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-11 19:53:38.000000 graphium-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 19:53:38.000000 graphium-2.1.3/requirements_ipu.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.363511 graphium-2.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-11 19:53:38.000000 graphium-2.1.3/scripts/convert_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:53:38.000000 graphium-2.1.3/scripts/ipu_start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 19:53:38.000000 graphium-2.1.3/scripts/ipu_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:58:50.387511 graphium-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.383511 graphium-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/config_test_ipu_dataloader.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/converted_fake_multilevel_data.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.383511 graphium-2.1.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/config_micro_ZINC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_corrupt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_2.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/pcqm4mv2-2k.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/fake_and_missing_multilevel_data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_base_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_mtl_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_multitask_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pe_nodepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pe_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pe_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pos_transfer_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_positional_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_positional_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pyg_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_utils.py
```

### Comparing `graphium-2.1.2/.github/CODE_OF_CONDUCT.md` & `graphium-2.1.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/.github/PULL_REQUEST_TEMPLATE.md` & `graphium-2.1.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/.github/workflows/code-check.yml` & `graphium-2.1.3/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/.github/workflows/doc.yml` & `graphium-2.1.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/.github/workflows/release.yml` & `graphium-2.1.3/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
       - name: Build Changelog
         id: github_release
         uses: mikepenz/release-changelog-builder-action@v4
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           toTag: "main"
-    
+
       - name: Configure git
         run: |
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
       - name: Create and push git tag
         env:
@@ -106,21 +106,21 @@
 
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
-      - name: Create GitHub Release
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
-        with:
-          tag_name: ${{ inputs.release-version }}
-          body: ${{steps.github_release.outputs.changelog}}
-
       - name: Deploy the doc
         run: |
           echo "Get the gh-pages branch"
           git fetch origin gh-pages
 
           echo "Build and deploy the doc on ${{ inputs.release-version }}"
           mike deploy --push --force stable
           mike deploy --push --force ${{ inputs.release-version }}
+
+      - name: Create GitHub Release
+        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        with:
+          tag_name: ${{ inputs.release-version }}
+          body: ${{steps.github_release.outputs.changelog}}
```

### Comparing `graphium-2.1.2/.github/workflows/test.yml` & `graphium-2.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/.gitignore` & `graphium-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/LICENSE` & `graphium-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/PKG-INFO` & `graphium-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.1.2
+Version: 2.1.3
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `graphium-2.1.2/README.md` & `graphium-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/_assets/css/custom-graphium.css` & `graphium-2.1.3/docs/_assets/css/custom-graphium.css`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/_assets/css/custom.css` & `graphium-2.1.3/docs/_assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/api/graphium.features.md` & `graphium-2.1.3/docs/api/graphium.features.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/api/graphium.ipu.md` & `graphium-2.1.3/docs/api/graphium.ipu.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/api/graphium.nn/encoders.md` & `graphium-2.1.3/docs/api/graphium.nn/encoders.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/api/graphium.nn/pyg_layers.md` & `graphium-2.1.3/docs/api/graphium.nn/pyg_layers.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/api/graphium.utils.md` & `graphium-2.1.3/docs/api/graphium.utils.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/baseline.md` & `graphium-2.1.3/docs/baseline.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/datasets.md` & `graphium-2.1.3/docs/datasets.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/design.md` & `graphium-2.1.3/docs/design.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/images/datamodule.png` & `graphium-2.1.3/docs/images/datamodule.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/images/full_graph_network.png` & `graphium-2.1.3/docs/images/full_graph_network.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/images/logo.png` & `graphium-2.1.3/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/images/logo.svg` & `graphium-2.1.3/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/index.md` & `graphium-2.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/pretrained_models.md` & `graphium-2.1.3/docs/pretrained_models.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb` & `graphium-2.1.3/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/feature_processing/choosing_parallelization.ipynb` & `graphium-2.1.3/docs/tutorials/feature_processing/choosing_parallelization.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/feature_processing/csv_to_parquet.ipynb` & `graphium-2.1.3/docs/tutorials/feature_processing/csv_to_parquet.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/feature_processing/timing_parallel.ipynb` & `graphium-2.1.3/docs/tutorials/feature_processing/timing_parallel.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/gnn/add_new_gnn_layers.ipynb` & `graphium-2.1.3/docs/tutorials/gnn/add_new_gnn_layers.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/gnn/making_gnn_networks.ipynb` & `graphium-2.1.3/docs/tutorials/gnn/making_gnn_networks.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/gnn/using_gnn_layers.ipynb` & `graphium-2.1.3/docs/tutorials/gnn/using_gnn_layers.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/model_training/running-multitask-ipu.ipynb` & `graphium-2.1.3/docs/tutorials/model_training/running-multitask-ipu.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/docs/tutorials/model_training/simple-molecular-model.ipynb` & `graphium-2.1.3/docs/tutorials/model_training/simple-molecular-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/env.yml` & `graphium-2.1.3/env.yml`

 * *Files 21% similar despite different names*

```diff
@@ -43,14 +43,15 @@
   # chemistry
   - rdkit
   - datamol >=0.10
 
   # Optional deps
   - sympy
   - tensorboard
+  - pydantic <2  # because of lightning. See https://github.com/Lightning-AI/lightning/issues/18026 and https://github.com/Lightning-AI/lightning/pull/18022
 
   # Dev
   - pytest >=6.0
   - pytest-xdist
   - pytest-cov
   - nbconvert
   - black >=23
```

### Comparing `graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m.yaml` & `graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m_mod.yaml` & `graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m_mod.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/configs/config_gpspp_10M_pcqm4m.yaml` & `graphium-2.1.3/expts/configs/config_gpspp_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/configs/config_mpnn_10M_b3lyp.yaml` & `graphium-2.1.3/expts/configs/config_mpnn_10M_b3lyp.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/configs/config_mpnn_10M_pcqm4m.yaml` & `graphium-2.1.3/expts/configs/config_mpnn_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/configs/config_mpnn_pcqm4m.yaml` & `graphium-2.1.3/expts/configs/config_mpnn_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/data/micro_zinc_splits.csv` & `graphium-2.1.3/expts/data/micro_zinc_splits.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/dataset_benchmark.py` & `graphium-2.1.3/expts/dataset_benchmark.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/main_run_get_fingerprints.py` & `graphium-2.1.3/expts/main_run_get_fingerprints.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/main_run_multitask.py` & `graphium-2.1.3/expts/main_run_multitask.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/main_run_predict.py` & `graphium-2.1.3/expts/main_run_predict.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/main_run_test.py` & `graphium-2.1.3/expts/main_run_test.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml` & `graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml` & `graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml` & `graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_classifigression_l1000.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_classifigression_l1000.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_large_gcn.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_large_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_large_gin.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_large_gin.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_large_gine.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_large_gine.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_large_mpnn.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_large_mpnn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_luis_jama.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_luis_jama.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_small_gated_gcn.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_small_gated_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_small_gcn.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_small_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_small_gine.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_small_gine.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/config_small_mpnn.yaml` & `graphium-2.1.3/expts/neurips2023_configs/config_small_mpnn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/debug/config_debug.yaml` & `graphium-2.1.3/expts/neurips2023_configs/debug/config_debug.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml` & `graphium-2.1.3/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml` & `graphium-2.1.3/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml` & `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/run_validation_test.py` & `graphium-2.1.3/expts/run_validation_test.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/expts/test_yaml.py` & `graphium-2.1.3/expts/test_yaml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/cli/data.py` & `graphium-2.1.3/graphium/cli/data.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/config/_loader.py` & `graphium-2.1.3/graphium/config/_loader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/config/config_convert.py` & `graphium-2.1.3/graphium/config/config_convert.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml` & `graphium-2.1.3/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/config/fake_multilevel_multitask_pyg.yaml` & `graphium-2.1.3/graphium/config/fake_multilevel_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/config/zinc_default_multitask_pyg.yaml` & `graphium-2.1.3/graphium/config/zinc_default_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb` & `graphium-2.1.3/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/QM9/micro_qm9.csv` & `graphium-2.1.3/graphium/data/QM9/micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/QM9/micro_qm9.parquet` & `graphium-2.1.3/graphium/data/QM9/micro_qm9.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/QM9/norm_micro_qm9.csv` & `graphium-2.1.3/graphium/data/QM9/norm_micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/README.md` & `graphium-2.1.3/graphium/data/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/collate.py` & `graphium-2.1.3/graphium/data/collate.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/datamodule.py` & `graphium-2.1.3/graphium/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/dataset.py` & `graphium-2.1.3/graphium/data/dataset.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb` & `graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb` & `graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/micro_ZINC/micro_ZINC.csv` & `graphium-2.1.3/graphium/data/micro_ZINC/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/multilevel_utils.py` & `graphium-2.1.3/graphium/data/multilevel_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/multitask/tiny_ZINC_SA.csv` & `graphium-2.1.3/graphium/data/multitask/tiny_ZINC_SA.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/multitask/tiny_ZINC_logp.csv` & `graphium-2.1.3/graphium/data/multitask/tiny_ZINC_logp.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/multitask/tiny_ZINC_score.csv` & `graphium-2.1.3/graphium/data/multitask/tiny_ZINC_score.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/normalization.py` & `graphium-2.1.3/graphium/data/normalization.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/sdf2csv.py` & `graphium-2.1.3/graphium/data/sdf2csv.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/smiles_transform.py` & `graphium-2.1.3/graphium/data/smiles_transform.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/data/utils.py` & `graphium-2.1.3/graphium/data/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/expts/pyg_batching_sparse.ipynb` & `graphium-2.1.3/graphium/expts/pyg_batching_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/README.md` & `graphium-2.1.3/graphium/features/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/commute.py` & `graphium-2.1.3/graphium/features/commute.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/electrostatic.py` & `graphium-2.1.3/graphium/features/electrostatic.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/featurizer.py` & `graphium-2.1.3/graphium/features/featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/graphormer.py` & `graphium-2.1.3/graphium/features/graphormer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/nmp.py` & `graphium-2.1.3/graphium/features/nmp.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/periodic_table.csv` & `graphium-2.1.3/graphium/features/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/positional_encoding.py` & `graphium-2.1.3/graphium/features/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/properties.py` & `graphium-2.1.3/graphium/features/properties.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/rw.py` & `graphium-2.1.3/graphium/features/rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/spectral.py` & `graphium-2.1.3/graphium/features/spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/test_new_pes.ipynb` & `graphium-2.1.3/graphium/features/test_new_pes.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/features/transfer_pos_level.py` & `graphium-2.1.3/graphium/features/transfer_pos_level.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/ipu_dataloader.py` & `graphium-2.1.3/graphium/ipu/ipu_dataloader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/ipu_losses.py` & `graphium-2.1.3/graphium/ipu/ipu_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/ipu_metrics.py` & `graphium-2.1.3/graphium/ipu/ipu_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/ipu_simple_lightning.py` & `graphium-2.1.3/graphium/ipu/ipu_simple_lightning.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/ipu_utils.py` & `graphium-2.1.3/graphium/ipu/ipu_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/ipu_wrapper.py` & `graphium-2.1.3/graphium/ipu/ipu_wrapper.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/ipu/to_dense_batch.py` & `graphium-2.1.3/graphium/ipu/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/README.md` & `graphium-2.1.3/graphium/nn/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/architectures/encoder_manager.py` & `graphium-2.1.3/graphium/nn/architectures/encoder_manager.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/architectures/global_architectures.py` & `graphium-2.1.3/graphium/nn/architectures/global_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/architectures/pyg_architectures.py` & `graphium-2.1.3/graphium/nn/architectures/pyg_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/base_graph_layer.py` & `graphium-2.1.3/graphium/nn/base_graph_layer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/base_layers.py` & `graphium-2.1.3/graphium/nn/base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/README.md` & `graphium-2.1.3/graphium/nn/encoders/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/base_encoder.py` & `graphium-2.1.3/graphium/nn/encoders/base_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/bessel_pos_encoder.py` & `graphium-2.1.3/graphium/nn/encoders/bessel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/gaussian_kernel_pos_encoder.py` & `graphium-2.1.3/graphium/nn/encoders/gaussian_kernel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/laplace_pos_encoder.py` & `graphium-2.1.3/graphium/nn/encoders/laplace_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/mlp_encoder.py` & `graphium-2.1.3/graphium/nn/encoders/mlp_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/encoders/signnet_pos_encoder.py` & `graphium-2.1.3/graphium/nn/encoders/signnet_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/README.md` & `graphium-2.1.3/graphium/nn/pyg_layers/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/dimenet_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/dimenet_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/gated_gcn_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/gated_gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/gcn_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/gin_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/gin_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/gps_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/gps_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/mpnn_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/mpnn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/pna_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/pna_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/pooling_pyg.py` & `graphium-2.1.3/graphium/nn/pyg_layers/pooling_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/pyg_layers/utils.py` & `graphium-2.1.3/graphium/nn/pyg_layers/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/residual_connections.py` & `graphium-2.1.3/graphium/nn/residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/nn/utils.py` & `graphium-2.1.3/graphium/nn/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/trainer/losses.py` & `graphium-2.1.3/graphium/trainer/losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/trainer/metrics.py` & `graphium-2.1.3/graphium/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/trainer/predictor.py` & `graphium-2.1.3/graphium/trainer/predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/trainer/predictor_options.py` & `graphium-2.1.3/graphium/trainer/predictor_options.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/trainer/predictor_summaries.py` & `graphium-2.1.3/graphium/trainer/predictor_summaries.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/arg_checker.py` & `graphium-2.1.3/graphium/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/command_line_utils.py` & `graphium-2.1.3/graphium/utils/command_line_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/custom_lr.py` & `graphium-2.1.3/graphium/utils/custom_lr.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/dict_tensor.py` & `graphium-2.1.3/graphium/utils/dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/fs.py` & `graphium-2.1.3/graphium/utils/fs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/mup.py` & `graphium-2.1.3/graphium/utils/mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/packing.py` & `graphium-2.1.3/graphium/utils/packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/read_file.py` & `graphium-2.1.3/graphium/utils/read_file.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/safe_run.py` & `graphium-2.1.3/graphium/utils/safe_run.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/spaces.py` & `graphium-2.1.3/graphium/utils/spaces.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/utils/tensor.py` & `graphium-2.1.3/graphium/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium/visualization/vis_utils.py` & `graphium-2.1.3/graphium/visualization/vis_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/graphium.egg-info/PKG-INFO` & `graphium-2.1.3/graphium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.1.2
+Version: 2.1.3
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `graphium-2.1.2/graphium.egg-info/SOURCES.txt` & `graphium-2.1.3/graphium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/mkdocs.yml` & `graphium-2.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/dev-datamodule-invalidate-cache.ipynb` & `graphium-2.1.3/notebooks/dev-datamodule-invalidate-cache.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/dev-datamodule-ogb.ipynb` & `graphium-2.1.3/notebooks/dev-datamodule-ogb.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/dev-datamodule.ipynb` & `graphium-2.1.3/notebooks/dev-datamodule.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/dev-pretrained.ipynb` & `graphium-2.1.3/notebooks/dev-pretrained.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/dev-training-loop.ipynb` & `graphium-2.1.3/notebooks/dev-training-loop.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/dev.ipynb` & `graphium-2.1.3/notebooks/dev.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/running-fingerprints-from-pretrained-model.ipynb` & `graphium-2.1.3/notebooks/running-fingerprints-from-pretrained-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/notebooks/running-model-from-config.ipynb` & `graphium-2.1.3/notebooks/running-model-from-config.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/profiling/configs_profiling.yaml` & `graphium-2.1.3/profiling/configs_profiling.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/profiling/profile_mol_to_graph.py` & `graphium-2.1.3/profiling/profile_mol_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/profiling/profile_predictor.py` & `graphium-2.1.3/profiling/profile_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/pyproject.toml` & `graphium-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/requirements_ipu.txt` & `graphium-2.1.3/requirements_ipu.txt`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/scripts/convert_yml.py` & `graphium-2.1.3/scripts/convert_yml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/scripts/ipu_venv.sh` & `graphium-2.1.3/scripts/ipu_venv.sh`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/config_test_ipu_dataloader.yaml` & `graphium-2.1.3/tests/config_test_ipu_dataloader.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/converted_fake_multilevel_data.parquet` & `graphium-2.1.3/tests/converted_fake_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/config_micro_ZINC.yaml` & `graphium-2.1.3/tests/data/config_micro_ZINC.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/micro_ZINC.csv` & `graphium-2.1.3/tests/data/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/micro_ZINC_corrupt.csv` & `graphium-2.1.3/tests/data/micro_ZINC_corrupt.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/micro_ZINC_shard_1.csv` & `graphium-2.1.3/tests/data/micro_ZINC_shard_1.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/micro_ZINC_shard_1.parquet` & `graphium-2.1.3/tests/data/micro_ZINC_shard_1.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/micro_ZINC_shard_2.csv` & `graphium-2.1.3/tests/data/micro_ZINC_shard_2.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/micro_ZINC_shard_2.parquet` & `graphium-2.1.3/tests/data/micro_ZINC_shard_2.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/data/pcqm4mv2-2k.csv` & `graphium-2.1.3/tests/data/pcqm4mv2-2k.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/fake_and_missing_multilevel_data.parquet` & `graphium-2.1.3/tests/fake_and_missing_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_architectures.py` & `graphium-2.1.3/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_attention.py` & `graphium-2.1.3/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_base_layers.py` & `graphium-2.1.3/tests/test_base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_collate.py` & `graphium-2.1.3/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_data_utils.py` & `graphium-2.1.3/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_datamodule.py` & `graphium-2.1.3/tests/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_dataset.py` & `graphium-2.1.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_dict_tensor.py` & `graphium-2.1.3/tests/test_dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_featurizer.py` & `graphium-2.1.3/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_ipu_dataloader.py` & `graphium-2.1.3/tests/test_ipu_dataloader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_ipu_losses.py` & `graphium-2.1.3/tests/test_ipu_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_ipu_metrics.py` & `graphium-2.1.3/tests/test_ipu_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_loaders.py` & `graphium-2.1.3/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_losses.py` & `graphium-2.1.3/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_metrics.py` & `graphium-2.1.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_mtl_architecture.py` & `graphium-2.1.3/tests/test_mtl_architecture.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_multitask_datamodule.py` & `graphium-2.1.3/tests/test_multitask_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_mup.py` & `graphium-2.1.3/tests/test_mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_packing.py` & `graphium-2.1.3/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_pe_nodepair.py` & `graphium-2.1.3/tests/test_pe_nodepair.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_pe_rw.py` & `graphium-2.1.3/tests/test_pe_rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_pe_spectral.py` & `graphium-2.1.3/tests/test_pe_spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_pos_transfer_funcs.py` & `graphium-2.1.3/tests/test_pos_transfer_funcs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_positional_encoders.py` & `graphium-2.1.3/tests/test_positional_encoders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_positional_encodings.py` & `graphium-2.1.3/tests/test_positional_encodings.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_predictor.py` & `graphium-2.1.3/tests/test_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_pyg_layers.py` & `graphium-2.1.3/tests/test_pyg_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_residual_connections.py` & `graphium-2.1.3/tests/test_residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.2/tests/test_utils.py` & `graphium-2.1.3/tests/test_utils.py`

 * *Files identical despite different names*

