# Comparing `tmp/graphium-2.1.1.tar.gz` & `tmp/graphium-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphium-2.1.1.tar", last modified: Thu Jul  6 18:49:58 2023, max compression
+gzip compressed data, was "graphium-2.1.2.tar", last modified: Tue Jul 11 19:29:34 2023, max compression
```

## Comparing `graphium-2.1.1.tar` & `graphium-2.1.2.tar`

### file list

```diff
@@ -1,327 +1,330 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.693771 graphium-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.569769 graphium-2.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.573769 graphium-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-06 18:45:04.000000 graphium-2.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-06 18:45:04.000000 graphium-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-06 18:45:04.000000 graphium-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-06 18:49:58.689770 graphium-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-06 18:45:04.000000 graphium-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 18:45:04.000000 graphium-2.1.1/cleanup_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.577769 graphium-2.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.557769 graphium-2.1.1/docs/_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.577769 graphium-2.1.1/docs/_assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/_assets/css/custom-graphium.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/_assets/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.585769 graphium-2.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.config.md
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.data.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.features.md
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.ipu.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.585769 graphium-2.1.1/docs/api/graphium.nn/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.nn/architectures.md
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.nn/encoders.md
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.nn/graphium.nn.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.nn/pyg_layers.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.trainer.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/api/graphium.visualization.md
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/baseline.md
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/cli_references.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/datasets.md
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/design.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.593769 graphium-2.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/images/datamodule.png
--rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/images/full_graph_network.png
--rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/pretrained_models.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.557769 graphium-2.1.1/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.597770 graphium-2.1.1/docs/tutorials/feature_processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/feature_processing/choosing_parallelization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/feature_processing/csv_to_parquet.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/feature_processing/timing_parallel.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.597770 graphium-2.1.1/docs/tutorials/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/gnn/add_new_gnn_layers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/gnn/making_gnn_networks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/gnn/using_gnn_layers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.601770 graphium-2.1.1/docs/tutorials/model_training/
--rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/model_training/running-multitask-ipu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-06 18:45:04.000000 graphium-2.1.1/docs/tutorials/model_training/simple-molecular-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-06 18:45:04.000000 graphium-2.1.1/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.605769 graphium-2.1.1/expts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.613770 graphium-2.1.1/expts/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/configs/config_gps_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/configs/config_gps_10M_pcqm4m_mod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/configs/config_gpspp_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/configs/config_mpnn_10M_b3lyp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/configs/config_mpnn_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/configs/config_mpnn_pcqm4m.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.613770 graphium-2.1.1/expts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/data/micro_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/data/tiny_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/dataset_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/main_run_get_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/main_run_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/main_run_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/main_run_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.625770 graphium-2.1.1/expts/neurips2023_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.625770 graphium-2.1.1/expts/neurips2023_configs/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_classifigression_l1000.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_large_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_large_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_large_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_large_mpnn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_luis_jama.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_small_gated_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_small_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_small_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_small_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/config_small_mpnn.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.629770 graphium-2.1.1/expts/neurips2023_configs/debug/
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/debug/config_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.633770 graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.637770 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.645770 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/run_validation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-06 18:45:04.000000 graphium-2.1.1/expts/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.645770 graphium-2.1.1/graphium/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.645770 graphium-2.1.1/graphium/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.649770 graphium-2.1.1/graphium/config/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/config_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/fake_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-06 18:45:04.000000 graphium-2.1.1/graphium/config/zinc_default_multitask_pyg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.649770 graphium-2.1.1/graphium/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.649770 graphium-2.1.1/graphium/data/L1000/
--rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.653770 graphium-2.1.1/graphium/data/QM9/
--rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/QM9/micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/QM9/micro_qm9.parquet
--rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/QM9/norm_micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)   108384 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.653770 graphium-2.1.1/graphium/data/make_data_splits/
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.653770 graphium-2.1.1/graphium/data/micro_ZINC/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/micro_ZINC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/micro_ZINC/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/multilevel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.653770 graphium-2.1.1/graphium/data/multitask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/multitask/tiny_ZINC_SA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/multitask/tiny_ZINC_logp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/multitask/tiny_ZINC_score.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/sdf2csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.653770 graphium-2.1.1/graphium/data/single_atom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/single_atom_dataset/single_atom_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/smiles_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.653770 graphium-2.1.1/graphium/expts/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/expts/pyg_batching_sparse.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.657770 graphium-2.1.1/graphium/features/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/commute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/electrostatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/nmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/periodic_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/test_new_pes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/features/transfer_pos_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.657770 graphium-2.1.1/graphium/ipu/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/ipu_simple_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/ipu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/ipu_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/ipu/to_dense_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.661770 graphium-2.1.1/graphium/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.661770 graphium-2.1.1/graphium/nn/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/architectures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/architectures/encoder_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    73133 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/architectures/global_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/architectures/pyg_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/base_graph_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/base_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.661770 graphium-2.1.1/graphium/nn/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/bessel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/laplace_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/mlp_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/encoders/signnet_pos_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.665770 graphium-2.1.1/graphium/nn/pyg_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/dimenet_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/gated_gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/gin_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/gps_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/mpnn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/pna_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/pooling_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/pyg_layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.665770 graphium-2.1.1/graphium/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/predictor_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/trainer/predictor_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.669770 graphium-2.1.1/graphium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/custom_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/moving_average_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/mup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/safe_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/utils/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.669770 graphium-2.1.1/graphium/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/visualization/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 18:45:05.000000 graphium-2.1.1/graphium/visualization/vis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.645770 graphium-2.1.1/graphium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-06 18:49:58.000000 graphium-2.1.1/graphium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-06 18:49:58.000000 graphium-2.1.1/graphium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:49:58.000000 graphium-2.1.1/graphium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 18:49:58.000000 graphium-2.1.1/graphium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 18:49:58.000000 graphium-2.1.1/graphium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 18:49:58.000000 graphium-2.1.1/graphium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-06 18:45:05.000000 graphium-2.1.1/lightning.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-06 18:45:05.000000 graphium-2.1.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.669770 graphium-2.1.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/dev-datamodule-invalidate-cache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/dev-datamodule-ogb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/dev-datamodule.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/dev-pretrained.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/dev-training-loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/running-fingerprints-from-pretrained-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-06 18:45:05.000000 graphium-2.1.1/notebooks/running-model-from-config.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.669770 graphium-2.1.1/profiling/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-06 18:45:05.000000 graphium-2.1.1/profiling/configs_profiling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-06 18:45:05.000000 graphium-2.1.1/profiling/profile_mol_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 18:45:05.000000 graphium-2.1.1/profiling/profile_one_of_k_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-06 18:45:05.000000 graphium-2.1.1/profiling/profile_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-06 18:45:05.000000 graphium-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-06 18:45:05.000000 graphium-2.1.1/requirements_ipu.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.673770 graphium-2.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-06 18:45:05.000000 graphium-2.1.1/scripts/convert_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 18:45:05.000000 graphium-2.1.1/scripts/ipu_start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-06 18:45:05.000000 graphium-2.1.1/scripts/ipu_venv.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:49:58.693771 graphium-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.685770 graphium-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/config_test_ipu_dataloader.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/converted_fake_multilevel_data.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:58.685770 graphium-2.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/config_micro_ZINC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/micro_ZINC_corrupt.csv
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/micro_ZINC_shard_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/micro_ZINC_shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/micro_ZINC_shard_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/micro_ZINC_shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/data/pcqm4mv2-2k.csv
--rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/fake_and_missing_multilevel_data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_base_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_mtl_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_multitask_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_mup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_pe_nodepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_pe_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_pe_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_pos_transfer_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_positional_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_positional_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_pyg_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-06 18:45:05.000000 graphium-2.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.172443 graphium-2.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.120440 graphium-2.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.120440 graphium-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 19:24:38.000000 graphium-2.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-11 19:24:38.000000 graphium-2.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-11 19:24:38.000000 graphium-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:29:34.172443 graphium-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-11 19:24:38.000000 graphium-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:24:38.000000 graphium-2.1.2/cleanup_files.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 19:24:38.000000 graphium-2.1.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.108440 graphium-2.1.2/docs/_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/_assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/_assets/css/custom-graphium.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/_assets/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/_assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/_assets/js/google-analytics.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.config.md
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.ipu.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.124440 graphium-2.1.2/docs/api/graphium.nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/architectures.md
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/graphium.nn.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.nn/pyg_layers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.trainer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/api/graphium.visualization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/baseline.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/cli_references.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/design.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/datamodule.png
+-rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/full_graph_network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/pretrained_models.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.112440 graphium-2.1.2/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/tutorials/feature_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/choosing_parallelization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/csv_to_parquet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/feature_processing/timing_parallel.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/tutorials/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/gnn/add_new_gnn_layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/gnn/making_gnn_networks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/gnn/using_gnn_layers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/docs/tutorials/model_training/
+-rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/model_training/running-multitask-ipu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-11 19:24:38.000000 graphium-2.1.2/docs/tutorials/model_training/simple-molecular-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 19:24:38.000000 graphium-2.1.2/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/expts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.128440 graphium-2.1.2/expts/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m_mod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_gpspp_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_mpnn_10M_b3lyp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_mpnn_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/configs/config_mpnn_pcqm4m.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.132441 graphium-2.1.2/expts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/data/micro_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/data/tiny_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/dataset_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_get_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/main_run_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.132441 graphium-2.1.2/expts/neurips2023_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.132441 graphium-2.1.2/expts/neurips2023_configs/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_classifigression_l1000.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_large_mpnn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_luis_jama.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gated_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/config_small_mpnn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/debug/config_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/run_validation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-11 19:24:38.000000 graphium-2.1.2/expts/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/graphium/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/config_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/fake_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/config/zinc_default_multitask_pyg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.140441 graphium-2.1.2/graphium/data/L1000/
+-rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/QM9/
+-rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/QM9/micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/QM9/micro_qm9.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/QM9/norm_micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108384 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/make_data_splits/
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/micro_ZINC/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/micro_ZINC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/micro_ZINC/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multilevel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/multitask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/tiny_ZINC_SA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/tiny_ZINC_logp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/multitask/tiny_ZINC_score.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/sdf2csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/data/single_atom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/single_atom_dataset/single_atom_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/smiles_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.144441 graphium-2.1.2/graphium/expts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/expts/pyg_batching_sparse.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.148441 graphium-2.1.2/graphium/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/commute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/electrostatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/nmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/periodic_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/test_new_pes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/features/transfer_pos_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.148441 graphium-2.1.2/graphium/ipu/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_simple_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/ipu_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/ipu/to_dense_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.148441 graphium-2.1.2/graphium/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.152442 graphium-2.1.2/graphium/nn/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/encoder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73133 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/global_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/architectures/pyg_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/base_graph_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/base_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.152442 graphium-2.1.2/graphium/nn/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/bessel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/laplace_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/mlp_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/encoders/signnet_pos_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.156442 graphium-2.1.2/graphium/nn/pyg_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/dimenet_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gated_gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gin_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/gps_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/mpnn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/pna_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/pooling_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/pyg_layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.156442 graphium-2.1.2/graphium/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/predictor_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/trainer/predictor_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.156442 graphium-2.1.2/graphium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/custom_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/moving_average_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/safe_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/utils/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/graphium/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/visualization/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 19:24:38.000000 graphium-2.1.2/graphium/visualization/vis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.136441 graphium-2.1.2/graphium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-11 19:29:34.000000 graphium-2.1.2/graphium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:29:33.000000 graphium-2.1.2/graphium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 19:24:38.000000 graphium-2.1.2/lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-11 19:24:38.000000 graphium-2.1.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-datamodule-invalidate-cache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-datamodule-ogb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-datamodule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-pretrained.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev-training-loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/running-fingerprints-from-pretrained-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-11 19:24:38.000000 graphium-2.1.2/notebooks/running-model-from-config.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/configs_profiling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/profile_mol_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/profile_one_of_k_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 19:24:38.000000 graphium-2.1.2/profiling/profile_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-11 19:24:38.000000 graphium-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 19:24:38.000000 graphium-2.1.2/requirements_ipu.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.160442 graphium-2.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-11 19:24:38.000000 graphium-2.1.2/scripts/convert_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:24:38.000000 graphium-2.1.2/scripts/ipu_start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 19:24:38.000000 graphium-2.1.2/scripts/ipu_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:29:34.172443 graphium-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.168443 graphium-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/config_test_ipu_dataloader.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/converted_fake_multilevel_data.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:34.168443 graphium-2.1.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/config_micro_ZINC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_corrupt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/micro_ZINC_shard_2.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/data/pcqm4mv2-2k.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/fake_and_missing_multilevel_data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_base_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_mtl_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_multitask_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pe_nodepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pe_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pe_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pos_transfer_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_positional_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_positional_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_pyg_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-11 19:24:38.000000 graphium-2.1.2/tests/test_utils.py
```

### Comparing `graphium-2.1.1/.github/CODE_OF_CONDUCT.md` & `graphium-2.1.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `graphium-2.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/.github/workflows/code-check.yml` & `graphium-2.1.2/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/.github/workflows/doc.yml` & `graphium-2.1.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/.github/workflows/release.yml` & `graphium-2.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/.github/workflows/test.yml` & `graphium-2.1.2/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -42,17 +42,27 @@
           cache-environment: true
           cache-downloads: true
           create-args: >-
             python=${{ matrix.python-version }}
             pytorch=${{ matrix.pytorch-version }}
 
       - name: Install library
-        run: python -m pip install --no-deps .
+        run: python -m pip install --no-deps -e . # `-e` required for correct `coverage` run.
 
       - name: Run tests
         run: pytest
 
+      - name: Codecov Upload
+        uses: codecov/codecov-action@v3
+        with:
+          files: ./coverage.xml
+          flags: unittests
+          name: codecov-umbrella
+          fail_ci_if_error: false
+          verbose: false
+          env_vars: ${{ matrix.python-version }},${{ matrix.pytorch-version }}
+
       - name: Test CLI
         run: graphium --help
 
       - name: Test building the doc
         run: mkdocs build
```

### Comparing `graphium-2.1.1/.gitignore` & `graphium-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/LICENSE` & `graphium-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/PKG-INFO` & `graphium-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.1.1
+Version: 2.1.2
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,15 @@
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/graphium/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/graphium)](https://github.com/datamol-io/graphium/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/graphium)](https://github.com/datamol-io/graphium/network/members)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
+[![codecov](https://codecov.io/gh/datamol-io/graphium/branch/main/graph/badge.svg?token=bHOkKY5Fze)](https://codecov.io/gh/datamol-io/graphium)
 
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
```

### Comparing `graphium-2.1.1/README.md` & `graphium-2.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/graphium/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/graphium)](https://github.com/datamol-io/graphium/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/graphium)](https://github.com/datamol-io/graphium/network/members)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
+[![codecov](https://codecov.io/gh/datamol-io/graphium/branch/main/graph/badge.svg?token=bHOkKY5Fze)](https://codecov.io/gh/datamol-io/graphium)
 
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
```

### Comparing `graphium-2.1.1/docs/_assets/css/custom-graphium.css` & `graphium-2.1.2/docs/_assets/css/custom-graphium.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 :root {
-  --graphium-primary: #70ad47ff;
+  --graphium-primary: #70ad47;
   --graphium-secondary: #343a40;
 
   /* Primary color shades */
   --md-primary-fg-color: var(--graphium-primary);
   --md-primary-fg-color--light: var(--graphium-primary);
   --md-primary-fg-color--dark: var(--graphium-primary);
   --md-primary-bg-color: var(--graphium-secondary);
@@ -13,67 +13,66 @@
   /* Accent color shades */
   --md-accent-fg-color: var(--graphium-secondary);
   --md-accent-fg-color--transparent: var(--graphium-secondary);
   --md-accent-bg-color: var(--graphium-secondary);
   --md-accent-bg-color--light: var(--graphium-secondary);
 }
 
-:root>* {
+:root > * {
   /* Code block color shades */
   --md-code-bg-color: hsla(0, 0%, 96%, 1);
   --md-code-fg-color: hsla(200, 18%, 26%, 1);
 
   /* Footer */
-  --md-footer-bg-color: var(--datamol-primary);
+  --md-footer-bg-color: var(--graphium-primary);
   /* --md-footer-bg-color--dark: hsla(0, 0%, 0%, 0.32); */
   --md-footer-fg-color: var(--graphium-secondary);
   --md-footer-fg-color--light: var(--graphium-secondary);
   --md-footer-fg-color--lighter: var(--graphium-secondary);
-
 }
 
 .md-header {
-  background-image: linear-gradient(to right, #70ad47ff, #70ad47ff);
+  background-color: #70ad47;
 }
 
 .md-footer {
-  background-image: linear-gradient(to right, #70ad47ff, #70ad47ff);
+  background-color: #70ad47;
 }
 
 .md-tabs {
-  background-image: linear-gradient(to right, #F4F6F9, #E2CEC3);
+  background-image: linear-gradient(to right, #f4f6f9, #e2cec3);
 }
 
 .md-header__topic {
-  color: rgb(255, 255, 255);
+  color: #fff;
 }
 
 .md-source__repository,
 .md-source__icon,
 .md-search__input,
 .md-search__input::placeholder,
-.md-search__input~.md-search__icon,
+.md-search__input ~ .md-search__icon,
 .md-footer__inner.md-grid,
 .md-copyright__highlight,
 .md-copyright,
 .md-footer-meta.md-typeset a,
 .md-version {
-  color: rgb(255, 255, 255) !important;
+  color: #fff !important;
 }
 
 .md-search__form {
   background-color: rgba(255, 255, 255, 0.2);
 }
 
 .md-search__input {
-  color: #222222 !important;
+  color: #222 !important;
 }
 
 .md-header__topic {
-  color: rgb(255, 255, 255);
+  color: #fff;
   font-size: 1.4em;
 }
 
 /* Increase the size of the logo */
 .md-header__button.md-logo img,
 .md-header__button.md-logo svg {
   height: 2rem !important;
```

### Comparing `graphium-2.1.1/docs/_assets/css/custom.css` & `graphium-2.1.2/docs/_assets/css/custom.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /* Indentation. */
 div.doc-contents:not(.first) {
   padding-left: 25px;
-  border-left: 4px solid rgba(230, 230, 230);
+  border-left: 4px solid #e6e6e6;
   margin-bottom: 80px;
 }
 
 /* Don't capitalize names. */
 h5.doc-heading {
   text-transform: none !important;
 }
```

### Comparing `graphium-2.1.1/docs/api/graphium.features.md` & `graphium-2.1.2/docs/api/graphium.features.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/api/graphium.ipu.md` & `graphium-2.1.2/docs/api/graphium.ipu.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/api/graphium.nn/encoders.md` & `graphium-2.1.2/docs/api/graphium.nn/encoders.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/api/graphium.nn/pyg_layers.md` & `graphium-2.1.2/docs/api/graphium.nn/pyg_layers.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/api/graphium.utils.md` & `graphium-2.1.2/docs/api/graphium.utils.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/baseline.md` & `graphium-2.1.2/docs/baseline.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/datasets.md` & `graphium-2.1.2/docs/datasets.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/design.md` & `graphium-2.1.2/docs/design.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/images/datamodule.png` & `graphium-2.1.2/docs/images/datamodule.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/images/full_graph_network.png` & `graphium-2.1.2/docs/images/full_graph_network.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/images/logo.png` & `graphium-2.1.2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/images/logo.svg` & `graphium-2.1.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/index.md` & `graphium-2.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/pretrained_models.md` & `graphium-2.1.2/docs/pretrained_models.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb` & `graphium-2.1.2/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/feature_processing/choosing_parallelization.ipynb` & `graphium-2.1.2/docs/tutorials/feature_processing/choosing_parallelization.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/feature_processing/csv_to_parquet.ipynb` & `graphium-2.1.2/docs/tutorials/feature_processing/csv_to_parquet.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/feature_processing/timing_parallel.ipynb` & `graphium-2.1.2/docs/tutorials/feature_processing/timing_parallel.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/gnn/add_new_gnn_layers.ipynb` & `graphium-2.1.2/docs/tutorials/gnn/add_new_gnn_layers.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/gnn/making_gnn_networks.ipynb` & `graphium-2.1.2/docs/tutorials/gnn/making_gnn_networks.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/gnn/using_gnn_layers.ipynb` & `graphium-2.1.2/docs/tutorials/gnn/using_gnn_layers.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/model_training/running-multitask-ipu.ipynb` & `graphium-2.1.2/docs/tutorials/model_training/running-multitask-ipu.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/docs/tutorials/model_training/simple-molecular-model.ipynb` & `graphium-2.1.2/docs/tutorials/model_training/simple-molecular-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/env.yml` & `graphium-2.1.2/env.yml`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
   # Optional deps
   - sympy
   - tensorboard
 
   # Dev
   - pytest >=6.0
   - pytest-xdist
+  - pytest-cov
   - nbconvert
   - black >=23
   - jupyterlab
   - ipywidgets
 
   # Doc
   - mkdocs
```

### Comparing `graphium-2.1.1/expts/configs/config_gps_10M_pcqm4m.yaml` & `graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/configs/config_gps_10M_pcqm4m_mod.yaml` & `graphium-2.1.2/expts/configs/config_gps_10M_pcqm4m_mod.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/configs/config_gpspp_10M_pcqm4m.yaml` & `graphium-2.1.2/expts/configs/config_gpspp_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/configs/config_mpnn_10M_b3lyp.yaml` & `graphium-2.1.2/expts/configs/config_mpnn_10M_b3lyp.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/configs/config_mpnn_10M_pcqm4m.yaml` & `graphium-2.1.2/expts/configs/config_mpnn_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/configs/config_mpnn_pcqm4m.yaml` & `graphium-2.1.2/expts/configs/config_mpnn_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/data/micro_zinc_splits.csv` & `graphium-2.1.2/expts/data/micro_zinc_splits.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/dataset_benchmark.py` & `graphium-2.1.2/expts/dataset_benchmark.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/main_run_get_fingerprints.py` & `graphium-2.1.2/expts/main_run_get_fingerprints.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/main_run_multitask.py` & `graphium-2.1.2/expts/main_run_multitask.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/main_run_predict.py` & `graphium-2.1.2/expts/main_run_predict.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/main_run_test.py` & `graphium-2.1.2/expts/main_run_test.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml` & `graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml` & `graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml` & `graphium-2.1.2/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_classifigression_l1000.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_classifigression_l1000.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_large_gcn.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_large_gcn.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     - deviceIterations(10) # IPU would require large batches to be ready for the model.
     - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
     - _Popart.set("defaultBufferingDepth", 128)
     - Precision.enableStochasticRounding(True)
+    # - Precision.enableFloatingPointExceptions(True)
 
 # accelerator:
 #   type: cpu  # cpu or ipu or gpu
 #   config_override:
 #     datamodule:
 #       batch_size_training: 64
 #       batch_size_inference: 256
@@ -116,15 +117,15 @@
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
-    processed_graph_data_path: "/net/group/software-apps/datacache/neurips2023-large/"
+    processed_graph_data_path: "../datacache/neurips2023-large/"
     featurization:
     # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
     # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
     # 'num_chiral_centers (not included yet)']
       atom_property_list_onehot: [atomic-number, group, period, total-valence]
       atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
       # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
@@ -163,15 +164,15 @@
   mup_base_path: null
   pre_nn:   # Set as null to avoid a pre-nn network
     out_dim: 64
     hidden_dims: 256
     depth: 2
     activation: relu
     last_activation: none
-    dropout: &dropout 0.18
+    dropout: &dropout 0.1
     normalization: &normalization layer_norm
     last_normalization: *normalization
     residual_type: none
 
   pre_nn_edges: null
 
   pe_encoders:
@@ -326,15 +327,15 @@
     pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
     lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 20
+    max_num_epochs: &max_epochs 100
     warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
@@ -370,15 +371,15 @@
       task: binary
       multitask_handling: mean-per-label
       threshold_kwargs: null
   pcqm4m_g25: &pcqm_metrics
     - name: mae
       metric: mae_ipu
       target_nan_mask: null
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
     - name: r2
@@ -400,8 +401,8 @@
     # monitor: *monitor
     # mode: *mode
     # save_top_k: 1
     save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
-    check_val_every_n_epoch: 20
+    check_val_every_n_epoch: 10
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_large_gin.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_large_gin.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_large_gine.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_large_mpnn.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-# Testing the gine model with the PCQMv2 dataset on IPU.
+# Testing the mpnn only model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_large_data_gine
+  name: &name neurips2023_large_data_mpnn
   config_override: "expts/neurips2023_configs/config_large_gcn.yaml"
 
 architecture:
+  model_type: FullGraphMultiTaskNetwork
+  mup_base_path: null
+
   pre_nn_edges:   # Set as null to avoid a pre-nn network
     out_dim: 32
     hidden_dims: 128
     depth: 2
     activation: relu
     last_activation: none
-    dropout: *dropout
-    normalization: *normalization
-    last_normalization: *normalization
+    dropout: 0.18
+    normalization: layer_norm
+    last_normalization: layer_norm
     residual_type: none
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: &gnn_dim 704
+    out_dim: &gnn_dim 64
     hidden_dims: *gnn_dim
-    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:mpnnplus' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_kwargs:  # Parameters for the model itself. You could define dropout_attn: 0.1
+      node_residual: false
+      mpnn_type: 'pyg:mpnnplus'
+      in_dim_edges: 32
+      out_dim_edges: 32
 
   graph_output_nn:
     graph:
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
     node:
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
 
-predictor:
-  optim_kwargs:
-    lr: 8.e-5 # warmup can be scheduled using torch_scheduler_kwargs
-
 trainer:
   logger:
     name: *name
     project: *name
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-large-gine/
+    dirpath: models_checkpoints/neurips2023-large-mpnn/
     filename: *name
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_large_mpnn.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_large_gine.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-# Testing the mpnn only model with the PCQMv2 dataset on IPU.
+# Testing the gine model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_large_data_mpnn
+  name: &name neurips2023_large_data_gine
   config_override: "expts/neurips2023_configs/config_large_gcn.yaml"
 
 architecture:
-  model_type: FullGraphMultiTaskNetwork
-  mup_base_path: null
-
   pre_nn_edges:   # Set as null to avoid a pre-nn network
     out_dim: 32
     hidden_dims: 128
     depth: 2
     activation: relu
     last_activation: none
-    dropout: 0.18
-    normalization: layer_norm
-    last_normalization: layer_norm
+    dropout: 0.1
+    normalization: &normalization layer_norm
+    last_normalization: *normalization
     residual_type: none
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: &gnn_dim 64
+    out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
-    layer_type: 'pyg:mpnnplus' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
-    layer_kwargs:  # Parameters for the model itself. You could define dropout_attn: 0.1
-      node_residual: false
-      mpnn_type: 'pyg:mpnnplus'
-      in_dim_edges: 32
-      out_dim_edges: 32
+    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
   graph_output_nn:
     graph:
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
     node:
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
 
 trainer:
   logger:
     name: *name
     project: *name
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-large-mpnn/
+    dirpath: models_checkpoints/neurips2023-large-gine/
     filename: *name
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_luis_jama.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_luis_jama.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_small_gated_gcn.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_small_gated_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_small_gcn.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_small_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_small_gine.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_small_gine.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/config_small_mpnn.yaml` & `graphium-2.1.2/expts/neurips2023_configs/config_small_mpnn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/debug/config_debug.yaml` & `graphium-2.1.2/expts/neurips2023_configs/debug/config_debug.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml` & `graphium-2.1.2/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -56,26 +56,26 @@
       l1000_vcap:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
-        sample_size: 2000 # use sample_size for test
+        # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_vcap_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_vcap_random_splits.pt`
 
       l1000_mcf7:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
-        sample_size: 2000 # use sample_size for test
+        # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_mcf7_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_mcf7_random_splits.pt`
 
       pcba_1328:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCBA_1328_1564k.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCBA_1328_1564k.parquet
@@ -314,23 +314,25 @@
     pcba_1328: []
     pcqm4m_g25: []
     pcqm4m_n4: [] 
   loss_fun:
     l1000_vcap:
       name: hybrid_ce_ipu
       n_brackets: 5
+      alpha: 0.5
     l1000_mcf7:
       name: hybrid_ce_ipu
       n_brackets: 5
+      alpha: 0.5
     pcba_1328: bce_ipu
     pcqm4m_g25: mae_ipu
     pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 5.e-4 # warmup can be scheduled using torch_scheduler_kwargs
+    lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
     max_num_epochs: &max_epochs 10
     warmup_epochs: 5
     verbose: False
   scheduler_kwargs:
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml` & `graphium-2.1.2/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -158,26 +158,25 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
-    in_dim: 64 # or otherwise the correct value
     out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gin' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -158,26 +158,25 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
-    in_dim: 64 # or otherwise the correct value
     out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gin' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Testing the gine model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_large_data_gine_mcf7
+  name: &name neurips2023_large_data_gine_vcap
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
@@ -12,15 +12,15 @@
         ipu_dataloader_training_opts:
           mode: async
           max_num_nodes_per_graph: 60 # train max nodes: 20, max_edges: 54
           max_num_edges_per_graph: 100
         ipu_dataloader_inference_opts:
           mode: async
           max_num_nodes_per_graph: 60 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 100
+          max_num_edges_per_graph: 150
         # Data handling-related
         batch_size_training: 10
         batch_size_inference: 2
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
@@ -49,31 +49,31 @@
 #         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
-      l1000_mcf7:
+      l1000_vcap:
         df: null
-        df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
+        df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
+        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
-        splits_path: graphium/data/neurips2023/large-dataset/l1000_mcf7_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_mcf7_random_splits.pt`
+        splits_path: graphium/data/neurips2023/large-dataset/l1000_vcap_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_vcap_random_splits.pt`
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
-    processed_graph_data_path: "../datacache/neurips2023-large/mcf7/"
+    processed_graph_data_path: "../datacache/neurips2023-large/vcap/"
     featurization:
     # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
     # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
     # 'num_chiral_centers (not included yet)']
       atom_property_list_onehot: [atomic-number, group, period, total-valence]
       atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
       # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
@@ -117,24 +117,15 @@
     activation: relu
     last_activation: none
     dropout: &dropout 0.18
     normalization: &normalization layer_norm
     last_normalization: *normalization
     residual_type: none
 
-  pre_nn_edges:   # Set as null to avoid a pre-nn network
-    out_dim: 32
-    hidden_dims: 128
-    depth: 2
-    activation: relu
-    last_activation: none
-    dropout: *dropout
-    normalization: *normalization
-    last_normalization: *normalization
-    residual_type: none
+  pre_nn_edges: null
 
   pe_encoders:
     out_dim: 32
     pool: "sum" #"mean" "max"
     last_norm: None #"batch_norm", "layer_norm"
     encoders: #la_pos |  rw_pos
       la_pos:  # Set as null to avoid a pre-nn network
@@ -158,25 +149,26 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
+    in_dim: 64 # or otherwise the correct value
     out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gin' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
@@ -184,37 +176,35 @@
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
-
   task_heads:
-    l1000_mcf7:
+    l1000_vcap:
       task_level: graph
       out_dim: 4890
       hidden_dims: 128
       depth: 2
       activation: none
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
-
 #Task-specific
 predictor:
   metrics_on_progress_bar:
-    l1000_mcf7: []
+    l1000_vcap: []
   metrics_on_training_set:
-    l1000_mcf7: []
+    l1000_vcap: []
   loss_fun:
-    l1000_mcf7:
+    l1000_vcap:
       name: hybrid_ce_ipu
       n_brackets: 5
   random_seed: *seed
   optim_kwargs:
     lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
@@ -227,15 +217,15 @@
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
-  l1000_mcf7: &classif_metrics
+  l1000_vcap: &classif_metrics
     - name: auroc
       metric: auroc_ipu
       num_classes: 5
       task: multiclass
       multitask_handling: mean-per-label
       threshold_kwargs: null
     - name: avpr
@@ -256,15 +246,15 @@
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-large-gine/mcf7/
+    dirpath: models_checkpoints/neurips2023-large-gine/vcap/
     filename: *name
     # monitor: *monitor
     # mode: *mode
     # save_top_k: 1
     save_last: True
   trainer:
     max_epochs: *max_epochs
```

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml` & `graphium-2.1.2/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Testing the gine model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_large_data_gine_vcap
+  name: &name neurips2023_large_data_gine_mcf7
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
@@ -12,15 +12,15 @@
         ipu_dataloader_training_opts:
           mode: async
           max_num_nodes_per_graph: 60 # train max nodes: 20, max_edges: 54
           max_num_edges_per_graph: 100
         ipu_dataloader_inference_opts:
           mode: async
           max_num_nodes_per_graph: 60 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 150
+          max_num_edges_per_graph: 100
         # Data handling-related
         batch_size_training: 10
         batch_size_inference: 2
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
@@ -49,31 +49,31 @@
 #         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
-      l1000_vcap:
+      l1000_mcf7:
         df: null
-        df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
+        df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
+        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
-        splits_path: graphium/data/neurips2023/large-dataset/l1000_vcap_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_vcap_random_splits.pt`
+        splits_path: graphium/data/neurips2023/large-dataset/l1000_mcf7_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_mcf7_random_splits.pt`
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
-    processed_graph_data_path: "../datacache/neurips2023-large/vcap/"
+    processed_graph_data_path: "../datacache/neurips2023-large/mcf7/"
     featurization:
     # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
     # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
     # 'num_chiral_centers (not included yet)']
       atom_property_list_onehot: [atomic-number, group, period, total-valence]
       atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
       # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
@@ -117,24 +117,15 @@
     activation: relu
     last_activation: none
     dropout: &dropout 0.18
     normalization: &normalization layer_norm
     last_normalization: *normalization
     residual_type: none
 
-  pre_nn_edges:   # Set as null to avoid a pre-nn network
-    out_dim: 32
-    hidden_dims: 128
-    depth: 2
-    activation: relu
-    last_activation: none
-    dropout: *dropout
-    normalization: *normalization
-    last_normalization: *normalization
-    residual_type: none
+  pre_nn_edges: null
 
   pe_encoders:
     out_dim: 32
     pool: "sum" #"mean" "max"
     last_norm: None #"batch_norm", "layer_norm"
     encoders: #la_pos |  rw_pos
       la_pos:  # Set as null to avoid a pre-nn network
@@ -158,25 +149,26 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
+    in_dim: 64 # or otherwise the correct value
     out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gin' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
@@ -184,35 +176,37 @@
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
+
   task_heads:
-    l1000_vcap:
+    l1000_mcf7:
       task_level: graph
       out_dim: 4890
       hidden_dims: 128
       depth: 2
       activation: none
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
+
 #Task-specific
 predictor:
   metrics_on_progress_bar:
-    l1000_vcap: []
+    l1000_mcf7: []
   metrics_on_training_set:
-    l1000_vcap: []
+    l1000_mcf7: []
   loss_fun:
-    l1000_vcap:
+    l1000_mcf7:
       name: hybrid_ce_ipu
       n_brackets: 5
   random_seed: *seed
   optim_kwargs:
     lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
@@ -225,15 +219,15 @@
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
-  l1000_vcap: &classif_metrics
+  l1000_mcf7: &classif_metrics
     - name: auroc
       metric: auroc_ipu
       num_classes: 5
       task: multiclass
       multitask_handling: mean-per-label
       threshold_kwargs: null
     - name: avpr
@@ -254,15 +248,15 @@
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-large-gine/vcap/
+    dirpath: models_checkpoints/neurips2023-large-gine/mcf7/
     filename: *name
     # monitor: *monitor
     # mode: *mode
     # save_top_k: 1
     save_last: True
   trainer:
     max_epochs: *max_epochs
```

### Comparing `graphium-2.1.1/expts/run_validation_test.py` & `graphium-2.1.2/expts/run_validation_test.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/expts/test_yaml.py` & `graphium-2.1.2/expts/test_yaml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/cli/data.py` & `graphium-2.1.2/graphium/cli/data.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/config/_loader.py` & `graphium-2.1.2/graphium/config/_loader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/config/config_convert.py` & `graphium-2.1.2/graphium/config/config_convert.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml` & `graphium-2.1.2/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/config/fake_multilevel_multitask_pyg.yaml` & `graphium-2.1.2/graphium/config/fake_multilevel_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/config/zinc_default_multitask_pyg.yaml` & `graphium-2.1.2/graphium/config/zinc_default_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb` & `graphium-2.1.2/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/QM9/micro_qm9.csv` & `graphium-2.1.2/graphium/data/QM9/micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/QM9/micro_qm9.parquet` & `graphium-2.1.2/graphium/data/QM9/micro_qm9.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/QM9/norm_micro_qm9.csv` & `graphium-2.1.2/graphium/data/QM9/norm_micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/README.md` & `graphium-2.1.2/graphium/data/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/collate.py` & `graphium-2.1.2/graphium/data/collate.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/datamodule.py` & `graphium-2.1.2/graphium/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/dataset.py` & `graphium-2.1.2/graphium/data/dataset.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb` & `graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb` & `graphium-2.1.2/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/micro_ZINC/micro_ZINC.csv` & `graphium-2.1.2/graphium/data/micro_ZINC/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/multilevel_utils.py` & `graphium-2.1.2/graphium/data/multilevel_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/multitask/tiny_ZINC_SA.csv` & `graphium-2.1.2/graphium/data/multitask/tiny_ZINC_SA.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/multitask/tiny_ZINC_logp.csv` & `graphium-2.1.2/graphium/data/multitask/tiny_ZINC_logp.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/multitask/tiny_ZINC_score.csv` & `graphium-2.1.2/graphium/data/multitask/tiny_ZINC_score.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/normalization.py` & `graphium-2.1.2/graphium/data/normalization.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/sdf2csv.py` & `graphium-2.1.2/graphium/data/sdf2csv.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/smiles_transform.py` & `graphium-2.1.2/graphium/data/smiles_transform.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/data/utils.py` & `graphium-2.1.2/graphium/data/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/expts/pyg_batching_sparse.ipynb` & `graphium-2.1.2/graphium/expts/pyg_batching_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/README.md` & `graphium-2.1.2/graphium/features/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/commute.py` & `graphium-2.1.2/graphium/features/commute.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/electrostatic.py` & `graphium-2.1.2/graphium/features/electrostatic.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/featurizer.py` & `graphium-2.1.2/graphium/features/featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/graphormer.py` & `graphium-2.1.2/graphium/features/graphormer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/nmp.py` & `graphium-2.1.2/graphium/features/nmp.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/periodic_table.csv` & `graphium-2.1.2/graphium/features/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/positional_encoding.py` & `graphium-2.1.2/graphium/features/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/properties.py` & `graphium-2.1.2/graphium/features/properties.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/rw.py` & `graphium-2.1.2/graphium/features/rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/spectral.py` & `graphium-2.1.2/graphium/features/spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/test_new_pes.ipynb` & `graphium-2.1.2/graphium/features/test_new_pes.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/features/transfer_pos_level.py` & `graphium-2.1.2/graphium/features/transfer_pos_level.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/ipu/ipu_dataloader.py` & `graphium-2.1.2/graphium/ipu/ipu_dataloader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/ipu/ipu_losses.py` & `graphium-2.1.2/graphium/ipu/ipu_losses.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,21 +106,22 @@
         return loss
 
 
 class HybridCELossIPU(HybridCELoss):
     def __init__(
         self,
         n_brackets,
+        alpha: float = 0.5,
     ) -> None:
         """
         Parameters:
             n_brackets: the number of brackets that will be used to group the regression targets.
                 Expected to have the same size as the number of classes in the transformed regression task.
         """
-        super().__init__(n_brackets=n_brackets)
+        super().__init__(n_brackets=n_brackets, alpha=alpha)
 
     def forward(self, input: Tensor, target: Tensor) -> Tensor:
         """
         Parameters:
             input: (batch_size x n_classes) tensor of logits predicted for each bracket.
             target: (batch_size) or (batch_size, 1) tensor of target brackets in {0, 1, ..., self.n_brackets}.
         """
```

### Comparing `graphium-2.1.1/graphium/ipu/ipu_metrics.py` & `graphium-2.1.2/graphium/ipu/ipu_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/ipu/ipu_simple_lightning.py` & `graphium-2.1.2/graphium/ipu/ipu_simple_lightning.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/ipu/ipu_utils.py` & `graphium-2.1.2/graphium/ipu/ipu_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/ipu/ipu_wrapper.py` & `graphium-2.1.2/graphium/ipu/ipu_wrapper.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/ipu/to_dense_batch.py` & `graphium-2.1.2/graphium/ipu/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/README.md` & `graphium-2.1.2/graphium/nn/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/architectures/encoder_manager.py` & `graphium-2.1.2/graphium/nn/architectures/encoder_manager.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/architectures/global_architectures.py` & `graphium-2.1.2/graphium/nn/architectures/global_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/architectures/pyg_architectures.py` & `graphium-2.1.2/graphium/nn/architectures/pyg_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/base_graph_layer.py` & `graphium-2.1.2/graphium/nn/base_graph_layer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/base_layers.py` & `graphium-2.1.2/graphium/nn/base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/README.md` & `graphium-2.1.2/graphium/nn/encoders/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/base_encoder.py` & `graphium-2.1.2/graphium/nn/encoders/base_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/bessel_pos_encoder.py` & `graphium-2.1.2/graphium/nn/encoders/bessel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/gaussian_kernel_pos_encoder.py` & `graphium-2.1.2/graphium/nn/encoders/gaussian_kernel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/laplace_pos_encoder.py` & `graphium-2.1.2/graphium/nn/encoders/laplace_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/mlp_encoder.py` & `graphium-2.1.2/graphium/nn/encoders/mlp_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/encoders/signnet_pos_encoder.py` & `graphium-2.1.2/graphium/nn/encoders/signnet_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/README.md` & `graphium-2.1.2/graphium/nn/pyg_layers/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/dimenet_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/dimenet_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/gated_gcn_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/gated_gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/gcn_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/gin_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/gin_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/gps_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/gps_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/mpnn_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/mpnn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/pna_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/pna_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/pooling_pyg.py` & `graphium-2.1.2/graphium/nn/pyg_layers/pooling_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/pyg_layers/utils.py` & `graphium-2.1.2/graphium/nn/pyg_layers/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/residual_connections.py` & `graphium-2.1.2/graphium/nn/residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/nn/utils.py` & `graphium-2.1.2/graphium/nn/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/trainer/losses.py` & `graphium-2.1.2/graphium/trainer/losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/trainer/metrics.py` & `graphium-2.1.2/graphium/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/trainer/predictor.py` & `graphium-2.1.2/graphium/trainer/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,25 +456,27 @@
             n_epochs=self.current_epoch,
         )
         metrics_logs = self.task_epoch_summary.get_metrics_logs()  # Dict[task, metric_logs]
         metrics_logs["_global"]["grad_norm"] = self.get_gradient_norm()
         outputs.update(metrics_logs)  # Dict[task, metric_logs]. Concatenate them?
 
         concatenated_metrics_logs = {}  # self.task_epoch_summary.concatenate_metrics_logs(metrics_logs)
-        concatenated_metrics_logs["loss"] = outputs["loss"]
+        concatenated_metrics_logs["train/loss"] = outputs["loss"]
         outputs["grad_norm"] = self.get_gradient_norm()
         concatenated_metrics_logs["train/grad_norm"] = outputs["grad_norm"]
         concatenated_metrics_logs["train/batch_time"] = train_batch_time
         concatenated_metrics_logs["train/batch_tput"] = tput
-
+        # report the training loss for each individual tasks
+        for task in self.tasks:
+            concatenated_metrics_logs[f"train/loss/{task}"] = outputs["task_losses"][task]
+        # get the mean loss value for individual tasks as they are a tensor of size --> gradient accumulation * replication * device_iter
         for key in concatenated_metrics_logs:
             if isinstance(concatenated_metrics_logs[key], torch.Tensor):
                 if concatenated_metrics_logs[key].numel() > 1:
                     concatenated_metrics_logs[key] = concatenated_metrics_logs[key].mean()
-
         if self.logger is not None:
             self.logger.log_metrics(
                 concatenated_metrics_logs, step=self.global_step
             )  # This is a pytorch lightning function call
 
     def training_step(self, batch: Dict[str, Tensor], to_cpu: bool = True) -> Dict[str, Any]:
         step_dict = None
```

### Comparing `graphium-2.1.1/graphium/trainer/predictor_options.py` & `graphium-2.1.2/graphium/trainer/predictor_options.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/trainer/predictor_summaries.py` & `graphium-2.1.2/graphium/trainer/predictor_summaries.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/arg_checker.py` & `graphium-2.1.2/graphium/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/command_line_utils.py` & `graphium-2.1.2/graphium/utils/command_line_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/custom_lr.py` & `graphium-2.1.2/graphium/utils/custom_lr.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/dict_tensor.py` & `graphium-2.1.2/graphium/utils/dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/fs.py` & `graphium-2.1.2/graphium/utils/fs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/mup.py` & `graphium-2.1.2/graphium/utils/mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/packing.py` & `graphium-2.1.2/graphium/utils/packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/read_file.py` & `graphium-2.1.2/graphium/utils/read_file.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/safe_run.py` & `graphium-2.1.2/graphium/utils/safe_run.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/spaces.py` & `graphium-2.1.2/graphium/utils/spaces.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/utils/tensor.py` & `graphium-2.1.2/graphium/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium/visualization/vis_utils.py` & `graphium-2.1.2/graphium/visualization/vis_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/graphium.egg-info/PKG-INFO` & `graphium-2.1.2/graphium.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.1.1
+Version: 2.1.2
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,15 @@
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/graphium/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/graphium)](https://github.com/datamol-io/graphium/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/graphium)](https://github.com/datamol-io/graphium/network/members)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
+[![codecov](https://codecov.io/gh/datamol-io/graphium/branch/main/graph/badge.svg?token=bHOkKY5Fze)](https://codecov.io/gh/datamol-io/graphium)
 
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
```

### Comparing `graphium-2.1.1/graphium.egg-info/SOURCES.txt` & `graphium-2.1.2/graphium.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 README.md
 cleanup_files.sh
+codecov.yml
 env.yml
 lightning.txt
 mkdocs.yml
 pyproject.toml
 requirements_ipu.txt
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
@@ -20,14 +21,15 @@
 docs/datasets.md
 docs/design.md
 docs/index.md
 docs/license.md
 docs/pretrained_models.md
 docs/_assets/css/custom-graphium.css
 docs/_assets/css/custom.css
+docs/_assets/js/google-analytics.js
 docs/api/graphium.config.md
 docs/api/graphium.data.md
 docs/api/graphium.features.md
 docs/api/graphium.ipu.md
 docs/api/graphium.trainer.md
 docs/api/graphium.utils.md
 docs/api/graphium.visualization.md
```

### Comparing `graphium-2.1.1/mkdocs.yml` & `graphium-2.1.2/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -44,29 +44,29 @@
   - Contribute: contribute.md
   - License: license.md
   - CLI: cli_references.md
 
 theme:
   name: material
   # NOTE(hadim): to customize the material primary and secondary
-  # color check `docs/assets/css/datamol-custom.css`.
+  # color check `docs/_assets/css/custom-graphium.css`.
   features:
     - navigation.tabs
     - navigation.expand
   favicon: images/logo.png
   logo: images/logo.svg
 
 extra_css:
   - _assets/css/custom.css
   - _assets/css/custom-graphium.css
 
 extra_javascript:
-  - javascripts/config.js
   - https://polyfill.io/v3/polyfill.min.js?features=es6
   - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
+  - _assets/js/google-analytics.js
 
 markdown_extensions:
   - admonition
   - markdown_include.include
   - pymdownx.emoji
   - pymdownx.magiclink
   - pymdownx.superfences
```

### Comparing `graphium-2.1.1/notebooks/dev-datamodule-invalidate-cache.ipynb` & `graphium-2.1.2/notebooks/dev-datamodule-invalidate-cache.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/dev-datamodule-ogb.ipynb` & `graphium-2.1.2/notebooks/dev-datamodule-ogb.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/dev-datamodule.ipynb` & `graphium-2.1.2/notebooks/dev-datamodule.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/dev-pretrained.ipynb` & `graphium-2.1.2/notebooks/dev-pretrained.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/dev-training-loop.ipynb` & `graphium-2.1.2/notebooks/dev-training-loop.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/dev.ipynb` & `graphium-2.1.2/notebooks/dev.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/running-fingerprints-from-pretrained-model.ipynb` & `graphium-2.1.2/notebooks/running-fingerprints-from-pretrained-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/notebooks/running-model-from-config.ipynb` & `graphium-2.1.2/notebooks/running-model-from-config.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/profiling/configs_profiling.yaml` & `graphium-2.1.2/profiling/configs_profiling.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/profiling/profile_mol_to_graph.py` & `graphium-2.1.2/profiling/profile_mol_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/profiling/profile_predictor.py` & `graphium-2.1.2/profiling/profile_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/pyproject.toml` & `graphium-2.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -89,16 +89,27 @@
 [tool.black]
 line-length = 110
 target-version = ['py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--verbose --durations=10 -n auto"
+addopts = "--verbose --durations=10 -n auto --cov=graphium --cov-fail-under=60 --cov-report xml --cov-report term"
 testpaths = ["tests"]
 filterwarnings = [
     "ignore::DeprecationWarning:ray.*:",
     "ignore::DeprecationWarning:numba.*:",
     "ignore::DeprecationWarning:lightning_fabric.*:",
     "ignore::DeprecationWarning:pytorch_lightning.*:",
     "ignore::DeprecationWarning:pkg_resources.*:",
 ]
+
+[tool.coverage.run]
+source = ["graphium/"]
+disable_warnings = ["no-data-collected"]
+data_file = ".coverage/coverage"
+
+[tool.coverage.report]
+omit = ["graphium/__init__.py", "graphium/_version.py"]
+
+[tool.coverage.xml]
+output = "coverage.xml"
```

### Comparing `graphium-2.1.1/requirements_ipu.txt` & `graphium-2.1.2/requirements_ipu.txt`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/scripts/convert_yml.py` & `graphium-2.1.2/scripts/convert_yml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/scripts/ipu_venv.sh` & `graphium-2.1.2/scripts/ipu_venv.sh`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/config_test_ipu_dataloader.yaml` & `graphium-2.1.2/tests/config_test_ipu_dataloader.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/converted_fake_multilevel_data.parquet` & `graphium-2.1.2/tests/converted_fake_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/config_micro_ZINC.yaml` & `graphium-2.1.2/tests/data/config_micro_ZINC.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/micro_ZINC.csv` & `graphium-2.1.2/tests/data/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/micro_ZINC_corrupt.csv` & `graphium-2.1.2/tests/data/micro_ZINC_corrupt.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/micro_ZINC_shard_1.csv` & `graphium-2.1.2/tests/data/micro_ZINC_shard_1.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/micro_ZINC_shard_1.parquet` & `graphium-2.1.2/tests/data/micro_ZINC_shard_1.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/micro_ZINC_shard_2.csv` & `graphium-2.1.2/tests/data/micro_ZINC_shard_2.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/micro_ZINC_shard_2.parquet` & `graphium-2.1.2/tests/data/micro_ZINC_shard_2.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/data/pcqm4mv2-2k.csv` & `graphium-2.1.2/tests/data/pcqm4mv2-2k.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/fake_and_missing_multilevel_data.parquet` & `graphium-2.1.2/tests/fake_and_missing_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_architectures.py` & `graphium-2.1.2/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_attention.py` & `graphium-2.1.2/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_base_layers.py` & `graphium-2.1.2/tests/test_base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_collate.py` & `graphium-2.1.2/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_data_utils.py` & `graphium-2.1.2/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_datamodule.py` & `graphium-2.1.2/tests/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_dataset.py` & `graphium-2.1.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_dict_tensor.py` & `graphium-2.1.2/tests/test_dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_featurizer.py` & `graphium-2.1.2/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_ipu_dataloader.py` & `graphium-2.1.2/tests/test_ipu_dataloader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_ipu_losses.py` & `graphium-2.1.2/tests/test_ipu_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_ipu_metrics.py` & `graphium-2.1.2/tests/test_ipu_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_loaders.py` & `graphium-2.1.2/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_losses.py` & `graphium-2.1.2/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_metrics.py` & `graphium-2.1.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_mtl_architecture.py` & `graphium-2.1.2/tests/test_mtl_architecture.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_multitask_datamodule.py` & `graphium-2.1.2/tests/test_multitask_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_mup.py` & `graphium-2.1.2/tests/test_mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_packing.py` & `graphium-2.1.2/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_pe_nodepair.py` & `graphium-2.1.2/tests/test_pe_nodepair.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_pe_rw.py` & `graphium-2.1.2/tests/test_pe_rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_pe_spectral.py` & `graphium-2.1.2/tests/test_pe_spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_pos_transfer_funcs.py` & `graphium-2.1.2/tests/test_pos_transfer_funcs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_positional_encoders.py` & `graphium-2.1.2/tests/test_positional_encoders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_positional_encodings.py` & `graphium-2.1.2/tests/test_positional_encodings.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_predictor.py` & `graphium-2.1.2/tests/test_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_pyg_layers.py` & `graphium-2.1.2/tests/test_pyg_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_residual_connections.py` & `graphium-2.1.2/tests/test_residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.1/tests/test_utils.py` & `graphium-2.1.2/tests/test_utils.py`

 * *Files identical despite different names*

