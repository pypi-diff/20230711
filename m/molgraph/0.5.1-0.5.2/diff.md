# Comparing `tmp/molgraph-0.5.1.tar.gz` & `tmp/molgraph-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.1.tar", last modified: Mon Jul 10 07:58:25 2023, max compression
+gzip compressed data, was "molgraph-0.5.2.tar", last modified: Tue Jul 11 18:19:52 2023, max compression
```

## Comparing `molgraph-0.5.1.tar` & `molgraph-0.5.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-10 07:58:25.397915 molgraph-0.5.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5888 2023-07-07 16:19:15.000000 molgraph-0.5.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.389916 molgraph-0.5.1/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.1/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.1/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6644 2023-07-04 20:05:31.000000 molgraph-0.5.1/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.1/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.1/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.1/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.1/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.1/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.1/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.1/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.1/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.1/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16271 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.1/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.1/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.1/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11134 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11954 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20608 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.1/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.1/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.1/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-07 12:52:08.000000 molgraph-0.5.1/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7775 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6953 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.1/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.1/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.1/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.1/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.1/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-10 07:58:25.397915 molgraph-0.5.1/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.1/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-11 18:19:52.431043 molgraph-0.5.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5949 2023-07-11 18:19:33.000000 molgraph-0.5.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.2/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-11 18:19:33.000000 molgraph-0.5.2/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.2/molgraph/applications/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.2/molgraph/applications/graph_transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.2/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.2/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.2/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.2/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.2/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.2/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.2/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.2/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.2/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16271 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.2/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.2/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.2/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11134 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11954 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20608 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.2/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.2/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.2/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.2/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6940 2023-07-11 18:19:33.000000 molgraph-0.5.2/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7054 2023-07-11 18:19:33.000000 molgraph-0.5.2/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.2/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.2/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.2/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.2/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.2/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-11 18:19:52.431043 molgraph-0.5.2/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.2/setup.py
```

### Comparing `molgraph-0.5.1/LICENSE` & `molgraph-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/PKG-INFO` & `molgraph-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.1
+Version: 0.5.2
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -26,23 +26,22 @@
 See [pre-print](https://arxiv.org/abs/2208.09944)
 
 ## Documentation
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
 
 ## Implementations
 
-- **Tensor**
-    - **GraphTensor**
-        - A composite tensor holding graph data.
-        - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
-        - Can conveniently go between both states (merge() and separate())
-        - Can propagate node information (features) based on edges (propagate())
-        - Can add, update and remove graph data (update(), remove())
-        - Has an associated GraphTensorSpec which it compatible with Keras and TensorFlow API.
-            - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
+- **Graph tensor** ([GraphTensor](http://github.com/akensert/molgraph/tree/main/molgraph/tensors/graph_tensor.py))
+    - A composite tensor holding graph data.
+    - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
+    - Can conveniently go between both states (merge() and separate())
+    - Can propagate node information (features) based on edges (propagate())
+    - Can add, update and remove graph data (update(), remove())
+    - Has an associated GraphTensorSpec which it makes it compatible with Keras and TensorFlow API.
+        - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
 - **Layers**
     
     - **Convolutional**
         - GCNConv ([GCNConv](http://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcn_conv.py))
         - GINConv ([GINConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gin_conv.py))
         - GCNIIConv ([GCNIIConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcnii_conv.py))
         - GraphSageConv ([GraphSageConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/graph_sage_conv.py))
```

### Comparing `molgraph-0.5.1/README.md` & `molgraph-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 See [pre-print](https://arxiv.org/abs/2208.09944)
 
 ## Documentation
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
 
 ## Implementations
 
-- **Tensor**
-    - **GraphTensor**
-        - A composite tensor holding graph data.
-        - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
-        - Can conveniently go between both states (merge() and separate())
-        - Can propagate node information (features) based on edges (propagate())
-        - Can add, update and remove graph data (update(), remove())
-        - Has an associated GraphTensorSpec which it compatible with Keras and TensorFlow API.
-            - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
+- **Graph tensor** ([GraphTensor](http://github.com/akensert/molgraph/tree/main/molgraph/tensors/graph_tensor.py))
+    - A composite tensor holding graph data.
+    - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
+    - Can conveniently go between both states (merge() and separate())
+    - Can propagate node information (features) based on edges (propagate())
+    - Can add, update and remove graph data (update(), remove())
+    - Has an associated GraphTensorSpec which it makes it compatible with Keras and TensorFlow API.
+        - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
 - **Layers**
     
     - **Convolutional**
         - GCNConv ([GCNConv](http://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcn_conv.py))
         - GINConv ([GINConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gin_conv.py))
         - GCNIIConv ([GCNIIConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcnii_conv.py))
         - GraphSageConv ([GraphSageConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/graph_sage_conv.py))
```

### Comparing `molgraph-0.5.1/molgraph/_filter_warnings.py` & `molgraph-0.5.2/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/applications/graph_transformer.py` & `molgraph-0.5.2/molgraph/applications/graph_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,80 @@
 from keras import constraints
 
 from typing import Optional
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
+from molgraph.tensors.graph_tensor import GraphTensorSpec
+
+from molgraph import chemistry
 
 from molgraph.layers.attentional.gt_conv import GTConv
 from molgraph.layers.positional_encoding.laplacian import (
     LaplacianPositionalEncoding)
 
 
+COMMON_KWARGS = {
+    'positional_encoding_dim': 16,
+    'merge_mode': 'concat',
+    'self_projection': True,
+    'normalization': True,
+    'residual': True,
+    'dropout': 0.15,
+    'activation': 'relu',  
+    'use_bias': True,
+    'kernel_initializer': None,
+    'bias_initializer': None,
+    'kernel_regularizer': None,
+    'bias_regularizer': None,
+    'activity_regularizer': None,
+    'kernel_constraint': None,
+    'bias_constraint': None,
+}
+
+CONDITIONAL_KWARGS = {
+    'LARGE': {
+        'steps': 8,
+        'units': 1024,
+        'heads': 16,
+    },
+    'MEDIUM': {
+        'steps': 6,
+        'units': 256,
+        'heads': 8,
+    },
+    'SMALL': {
+        'steps': 4,
+        'units': 64,
+        'heads': 4,    
+    }
+}
+
+
+molecule_encoder = chemistry.MolecularGraphEncoder(
+    atom_encoder=chemistry.Tokenizer([
+
+    ]),
+    bond_encoder=chemistry.Tokenizer([
+
+    ]),
+    positional_encoding_dim=16,
+)
+
+# molecule_encoder.to_spec()
+
+def GraphTransformer(
+    mode: str,
+):
+    pass
+
+
+
+
 class GraphTransformer(keras.Model):
 
     '''Graph transformer model.
 
     Implementation is based on Dwivedi et al. (2021) [#]_.
 
     Args:
```

### Comparing `molgraph-0.5.1/molgraph/chemistry/__init__.py` & `molgraph-0.5.2/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.2/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.2/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.2/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.2/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.2/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.2/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/encoders.py` & `molgraph-0.5.2/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/features.py` & `molgraph-0.5.2/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.2/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/ops.py` & `molgraph-0.5.2/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/chemistry/vis.py` & `molgraph-0.5.2/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/__init__.py` & `molgraph-0.5.2/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.2/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.2/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.2/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.2/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.2/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.2/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.2/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.2/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.2/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.2/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.2/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.2/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.2/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/gnn_layer.py` & `molgraph-0.5.2/molgraph/layers/gnn_layer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/gnn_ops.py` & `molgraph-0.5.2/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.2/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.2/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.2/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.2/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.2/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.2/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.2/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.2/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.2/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.2/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.2/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.2/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/losses/link_losses.py` & `molgraph-0.5.2/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/losses/masked_losses.py` & `molgraph-0.5.2/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.2/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.2/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/models/__init__.py` & `molgraph-0.5.2/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/models/dgin.py` & `molgraph-0.5.2/molgraph/models/dmpnn.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 from tensorflow import keras
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
-from molgraph.layers.gnn_ops import propagate_node_features
-from molgraph.layers.message_passing.edge_conv import edge_message_step
+from molgraph.layers.message_passing.edge_conv import EdgeConv
+from molgraph.layers.message_passing.mpnn_conv import MPNNConv
+from molgraph.layers.readout.node_readout import NodeReadout
 
 
 @keras.saving.register_keras_serializable(package='molgraph')
-class DGIN(keras.models.Model):
+class DMPNN(keras.layers.Layer):
 
-    '''Directed graph isomorphism network (DGIN).
+    '''Directed message passing neural network (DMPNN).
+
+    Implementation based on Wieder et al. (2021) [#]_, though adding several
+    `MPNNConv` layers for the node message passing (similar to how DGIN adds 
+    several `GINConv` layers for the node message passsing).
 
-    Implementation is based on Wieder et al. (2021) [#]_. 
-    
     **Important:**
 
-    As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
-    of molecules with a single atom, please add self loops: 
+    As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. 
+    If your dataset consists of molecules with a single atom, please add self loops: 
     ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
-    
+
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
@@ -34,20 +37,20 @@
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build Functional model
     >>> inputs = tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec)
-    >>> x = molgraph.models.DGIN(units=32, name='dgin')(inputs)
-    >>> x = molgraph.layers.SetGatherReadout(name='readout')(x)
+    >>> x = molgraph.models.DMPNN(units=32, name='dmpnn')(inputs)
+    >>> x = molgraph.layers.Readout(name='readout')(x)
     >>> outputs = tf.keras.layers.Dense(10, activation='sigmoid')(x)
-    >>> dgin_classifier = tf.keras.Model(inputs, outputs)
+    >>> dmpnn_classifier = tf.keras.Model(inputs, outputs)
     >>> # Make predictions
-    >>> preds = dgin_classifier.predict(graph_tensor, verbose=0)
+    >>> preds = dmpnn_classifier.predict(graph_tensor, verbose=0)
     >>> preds.shape
     (2, 10)
  
     Args:
         units (int, None):
             Number of hiden units of the message passing. These include the
             dense layers associated with the message functions, and GRU cells
@@ -55,63 +58,86 @@
             set to the input dimension. Default to None.
         activation (tf.keras.activations.Activation, callable, str, None):
             Activation function applied to the projections. Default to 'relu'.
         edge_message_steps (int):
             Number of edge message passing steps. Default to 4.
         node_message_steps (int):
             Number of node message passing steps. Default to 4.
-        dropout: (float, None):
-            Dropout applied to the output of step. Default to None.
-        parallel_iterations (int, None):
-            Number of ``parallel_iterations`` to be set for ``tf.map_fn`` to find
-            the reverse edge features to be subtracted from the aggregated edge features.
-        dense_kwargs (dict, None):
+        edge_message_kwargs (dict, None):
             An optional dictionary of parameters which can be passed to the
-            dense layers of this model. Note: as ``units`` and ``activation``
+            `EdgeConv` layers of this model. Note: as ``units`` and ``activation``
+            are already specified, it will be dropped from the dict (if it exists 
+            there). If None, an empty dict will be passed. Default to None.
+        node_message_kwargs (dict, None):
+            An optional dictionary of parameters which can be passed to the
+            `GINConv` layers of this model. Note: as ``units`` and ``activation``
             are already specified, it will be dropped from the dict (if it exists 
             there). If None, an empty dict will be passed. Default to None.
 
     References:
         .. [#] https://www.mdpi.com/1420-3049/26/20/6185
     '''
     
     def __init__(
         self,
         units: Optional[int] = None,
         activation: Union[
             None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
         edge_message_steps: int = 4,
         node_message_steps: int = 4,
-        dropout: Optional[float] = None,
-        parallel_iterations: Optional[int] = None,
-        dense_kwargs: Optional[dict] = None,
+        edge_message_kwargs: Optional[dict] = None,
+        node_message_kwargs: Optional[dict] = None,
         **kwargs
     ):
         super().__init__(**kwargs)
+
         self.units = units
         self.activation = keras.activations.get(activation)
+
+        if edge_message_kwargs is None:
+            edge_message_kwargs = {}
+        else:
+            edge_message_kwargs.pop('units', None)
+            edge_message_kwargs.pop('activation', None)
+
+        self.edge_message_kwargs = edge_message_kwargs
+
+        if node_message_kwargs is None:
+            node_message_kwargs = {}
+        else:
+            node_message_kwargs.pop('units', None)
+            node_message_kwargs.pop('activation', None)
+
+        self.node_message_kwargs = node_message_kwargs
+
         self.edge_message_steps = edge_message_steps
         self.node_message_steps = node_message_steps
-        self.dropout = (
-            None if dropout is None else keras.layers.Dropout(dropout))
-        self.parallel_iterations = parallel_iterations
-        self.dense_kwargs = {} if dense_kwargs is None else dense_kwargs
-        self.dense_kwargs.pop('units', None)
-        self.dense_kwargs.pop('activaton', None)
 
-    def build(self, input_shape: Optional[Tuple[int, ...]] = None) -> None:
+
+    def build(self, input_shape: tf.TensorShape) -> None:
+        
         if not self.units:
             self.units = input_shape[-1]
-        self.initial_projection = keras.layers.Dense(
-            self.units, self.activation, **self.dense_kwargs)
-        self.update_projection = keras.layers.Dense(
-            self.units, **self.dense_kwargs)
-        self.node_projection = keras.layers.Dense(
-            self.units + input_shape[-1], **self.dense_kwargs)
-        self.epsilon = tf.Variable(0.)
+
+        self.edge_message_functions = [
+            EdgeConv(
+                units=self.units, 
+                activation=self.activation, 
+                **self.edge_message_kwargs
+            ) for _ in range(self.edge_message_steps)
+        ]
+        self.node_message_functions = [
+            MPNNConv(
+                units=self.units, 
+                activation=self.activation, 
+                **self.node_message_kwargs
+            ) for _ in range(self.node_message_steps)
+        ]
+        self.node_readout = NodeReadout()
+
         self.built = True
     
     def call(self, tensor: GraphTensor) -> GraphTensor:
 
         '''Defines the computation from inputs to outputs.
         
         This method should not be called directly, but indirectly
@@ -127,69 +153,39 @@
                 A ``GraphTensor`` with updated node features.
         '''
         
         tensor_orig = tensor
         if isinstance(tensor.node_feature, tf.RaggedTensor):
             tensor = tensor.merge()
         
-        # MPNN requires edge features, if edge features do not exist,
-        # we initialize a ones vector.
-        if tensor.edge_feature is None:
-            tensor = tensor.update({
-                'edge_feature': tf.ones(
-                    shape=[tf.shape(tensor.edge_dst)[0], 1],
-                    dtype=tensor.node_feature.dtype)})
-            
-        edge_feature = tf.gather(tensor.node_feature, tensor.edge_src)
-        edge_feature = tf.concat([edge_feature, tensor.edge_feature], axis=-1)
-        edge_feature = self.initial_projection(edge_feature)
-        
-        tensor = tensor.update({'edge_feature': edge_feature})
-        
-        for _ in range(self.edge_message_steps):
-            
-            message = edge_message_step(
-                edge_feature=tensor.edge_feature,
-                edge_src=tensor.edge_src,
-                edge_dst=tensor.edge_dst)
-
-            edge_feature = self.activation(
-                self.update_projection(message) + edge_feature)
-            
-            if self.dropout is not None:
-                edge_feature = self.dropout(edge_feature)
-
-            # TODO: should skip connection be applied? 
-            tensor = tensor.update({'edge_feature': edge_feature})
-
-        message = tf.math.unsorted_segment_sum(
-            tensor.edge_feature, tensor.edge_dst, tf.shape(tensor.node_feature)[0]) 
-        
-        node_feature = tf.concat([tensor.node_feature, message], axis=-1)
-        
-        node_feature_initial = self.node_projection(
-            node_feature * (1 + self.epsilon))
-        
-        for _ in range(self.node_message_steps):
-            node_feature = propagate_node_features(
-                node_feature=node_feature, 
-                edge_src=tensor.edge_src,
-                edge_dst=tensor.edge_dst)
-            node_feature = node_feature + node_feature_initial
-            
-        return tensor_orig.update({'node_feature': node_feature})
+        x = tensor
+        for edge_message_step in self.edge_message_functions:
+            x = edge_message_step(x)
+
+        # Pool messages (n_edges, dim) -> (n_nodes, dim)
+        x = self.node_readout(x)
+        
+        # Concatenate initial node features and aggregated node features
+        node_feature = tf.concat([
+            tensor.node_feature, x.node_feature], axis=-1)
+        
+        x = x.update(node_feature=node_feature)
+        for node_message_step in self.node_message_functions:
+            x = node_message_step(x)
+
+        return tensor_orig.update(
+            node_feature=x.node_feature,
+            edge_state=x.edge_state)
+
 
     def get_config(self) -> dict:
         base_config = super().get_config()
         config = {
             'units': self.units,
             'activation': keras.activations.serialize(self.activation),
             'edge_message_steps': self.edge_message_steps,
             'node_message_steps': self.node_message_steps,
-            'dropout': self.dropout,
-            'parallel_iterations': self.parallel_iterations,
-            'dense_kwargs': self.dense_kwargs,
+            'edge_message_kwargs': self.edge_message_kwargs,
+            'node_message_kwargs': self.node_message_kwargs,
         }
         base_config.update(config)
-        return base_config
-    
-    
+        return base_config
```

### Comparing `molgraph-0.5.1/molgraph/models/dmpnn.py` & `molgraph-0.5.2/molgraph/models/dgin.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 from tensorflow import keras
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
-from molgraph.layers.message_passing.edge_conv import edge_message_step
+from molgraph.layers.message_passing.edge_conv import EdgeConv
+from molgraph.layers.convolutional.gin_conv import GINConv
+from molgraph.layers.readout.node_readout import NodeReadout
 
 
 @keras.saving.register_keras_serializable(package='molgraph')
-class DMPNN(keras.models.Model):
+class DGIN(keras.layers.Layer):
 
-    '''Directed message passing neural network (DMPNN).
-
-    Implementation is based on Yang et al. (2019) [#]_.
+    '''Directed graph isomorphism network (DGIN).
 
+    Implementation based on Wieder et al. (2021) [#]_. 
+    
     **Important:**
 
-    As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
-    of molecules with a single atom, please add self loops: 
+    As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. 
+    If your dataset consists of molecules with a single atom, please add self loops: 
     ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
-
+    
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
@@ -33,79 +35,107 @@
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build Functional model
     >>> inputs = tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec)
-    >>> x = molgraph.models.DMPNN(units=32, name='dmpnn')(inputs)
-    >>> x = molgraph.layers.SetGatherReadout(name='readout')(x)
+    >>> x = molgraph.models.DGIN(units=32, name='dgin')(inputs)
+    >>> x = molgraph.layers.Readout(name='readout')(x)
     >>> outputs = tf.keras.layers.Dense(10, activation='sigmoid')(x)
-    >>> dmpnn_classifier = tf.keras.Model(inputs, outputs)
+    >>> dgin_classifier = tf.keras.Model(inputs, outputs)
     >>> # Make predictions
-    >>> preds = dmpnn_classifier.predict(graph_tensor, verbose=0)
+    >>> preds = dgin_classifier.predict(graph_tensor, verbose=0)
     >>> preds.shape
     (2, 10)
  
     Args:
         units (int, None):
             Number of hiden units of the message passing. These include the
             dense layers associated with the message functions, and GRU cells
             associated with the update functions. If None, hidden units are
             set to the input dimension. Default to None.
         activation (tf.keras.activations.Activation, callable, str, None):
             Activation function applied to the projections. Default to 'relu'.
-        steps (int):
-            Number of message passing steps. Default to 4.
-        dropout: (float, None):
-            Dropout applied to the output of step. Default to None.
-        parallel_iterations (int, None):
-            Number of ``parallel_iterations`` to be set for ``tf.map_fn`` to find
-            the reverse edge features to be subtracted from the aggregated edge features.
-        dense_kwargs (dict, None):
+        edge_message_steps (int):
+            Number of edge message passing steps. Default to 4.
+        node_message_steps (int):
+            Number of node message passing steps. Default to 4.
+        edge_message_kwargs (dict, None):
+            An optional dictionary of parameters which can be passed to the
+            `EdgeConv` layers of this model. Note: as ``units`` and ``activation``
+            are already specified, it will be dropped from the dict (if it exists 
+            there). If None, an empty dict will be passed. Default to None.
+        node_message_kwargs (dict, None):
             An optional dictionary of parameters which can be passed to the
-            dense layers of this model. Note: as ``units`` and ``activation``
+            `GINConv` layers of this model. Note: as ``units`` and ``activation``
             are already specified, it will be dropped from the dict (if it exists 
             there). If None, an empty dict will be passed. Default to None.
 
     References:
-        .. [#] https://arxiv.org/pdf/1904.01561.pdf
+        .. [#] https://www.mdpi.com/1420-3049/26/20/6185
     '''
     
     def __init__(
         self,
         units: Optional[int] = None,
         activation: Union[
             None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
-        steps: int = 4,
-        dropout: Optional[float] = None,
-        parallel_iterations: Optional[int] = None,
-        dense_kwargs: Optional[dict] = None,
+        edge_message_steps: int = 4,
+        node_message_steps: int = 4,
+        edge_message_kwargs: Optional[dict] = None,
+        node_message_kwargs: Optional[dict] = None,
         **kwargs
     ):
         super().__init__(**kwargs)
+
         self.units = units
         self.activation = keras.activations.get(activation)
-        self.steps = steps
-        self.dropout = (
-            None if dropout is None else keras.layers.Dropout(dropout))
-        self.parallel_iterations = parallel_iterations
-        self.dense_kwargs = {} if dense_kwargs is None else dense_kwargs
-        self.dense_kwargs.pop('units', None)
-        self.dense_kwargs.pop('activaton', None)
 
-    def build(self, input_shape: Optional[Tuple[int, ...]] = None) -> None:
+        if edge_message_kwargs is None:
+            edge_message_kwargs = {}
+        else:
+            edge_message_kwargs.pop('units', None)
+            edge_message_kwargs.pop('activation', None)
+
+        self.edge_message_kwargs = edge_message_kwargs
+
+        if node_message_kwargs is None:
+            node_message_kwargs = {}
+        else:
+            node_message_kwargs.pop('units', None)
+            node_message_kwargs.pop('activation', None)
+            
+        self.node_message_kwargs = node_message_kwargs
+
+        self.edge_message_steps = edge_message_steps
+        self.node_message_steps = node_message_steps
+
+    def build(self, input_shape: tf.TensorShape) -> None:
+
         if not self.units:
             self.units = input_shape[-1]
-        self.initial_projection = keras.layers.Dense(
-            self.units, self.activation, **self.dense_kwargs)
-        self.update_projection = keras.layers.Dense(
-            self.units, **self.dense_kwargs)
-        self.final_projection = keras.layers.Dense(
-            self.units, self.activation, **self.dense_kwargs)
+
+        self.edge_message_functions = [
+            EdgeConv(
+                units=self.units, 
+                activation=self.activation, 
+                **self.edge_message_kwargs
+            ) for _ in range(self.edge_message_steps)
+        ]
+        self.node_message_functions = [
+            GINConv(
+                units=self.units, 
+                activation=self.activation, 
+                use_edge_features=False,
+                **self.node_message_kwargs
+            ) for _ in range(self.node_message_steps)
+        ]
+        self.node_readout = NodeReadout()
+
         self.built = True
     
     def call(self, tensor: GraphTensor) -> GraphTensor:
 
         '''Defines the computation from inputs to outputs.
         
         This method should not be called directly, but indirectly
@@ -121,58 +151,41 @@
                 A ``GraphTensor`` with updated node features.
         '''
         
         tensor_orig = tensor
         if isinstance(tensor.node_feature, tf.RaggedTensor):
             tensor = tensor.merge()
         
-        # MPNN requires edge features, if edge features do not exist,
-        # we initialize a ones vector.
-        if tensor.edge_feature is None:
-            tensor = tensor.update({
-                'edge_feature': tf.ones(
-                    shape=[tf.shape(tensor.edge_dst)[0], 1],
-                    dtype=tensor.node_feature.dtype)})
-            
-        edge_feature = tf.gather(tensor.node_feature, tensor.edge_src)
-        edge_feature = tf.concat([edge_feature, tensor.edge_feature], axis=-1)
-        edge_feature = self.initial_projection(edge_feature)
-        
-        tensor = tensor.update({'edge_feature': edge_feature})
-        
-        for _ in range(self.steps):
-            
-            message = edge_message_step(
-                edge_feature=tensor.edge_feature,
-                edge_src=tensor.edge_src,
-                edge_dst=tensor.edge_dst)
-    
-            edge_feature = self.activation(
-                self.update_projection(message) + edge_feature)
-            
-            if self.dropout is not None:
-                edge_feature = self.dropout(edge_feature)
-
-            # TODO: should skip connection be applied? 
-            tensor = tensor.update({'edge_feature': edge_feature})
+        x = tensor
+        for edge_message_step in self.edge_message_functions:
+            x = edge_message_step(x)
+
+        # Pool messages (n_edges, dim) -> (n_nodes, dim)
+        x = self.node_readout(x)
+        
+        # Concatenate initial node features and aggregated node features
+        node_feature = tf.concat([
+            tensor.node_feature, x.node_feature], axis=-1)
+        
+        x = x.update(node_feature=node_feature)
+        for node_message_step in self.node_message_functions:
+            x = node_message_step(x)
+
+        return tensor_orig.update(
+            node_feature=x.node_feature,
+            edge_state=x.edge_state)
 
-        message = tf.math.unsorted_segment_sum(
-            tensor.edge_feature, tensor.edge_dst, tf.shape(tensor.node_feature)[0]) 
-            
-        node_feature = self.final_projection(
-            tf.concat([tensor.node_feature, message], axis=-1))
-        
-        return tensor_orig.update({'node_feature': node_feature})
 
     def get_config(self) -> dict:
         base_config = super().get_config()
         config = {
             'units': self.units,
             'activation': keras.activations.serialize(self.activation),
-            'steps': self.steps,
-            'dropout': self.dropout,
-            'parallel_iterations': self.parallel_iterations,
-            'dense_kwargs': self.dense_kwargs,
+            'edge_message_steps': self.edge_message_steps,
+            'node_message_steps': self.node_message_steps,
+            'edge_message_kwargs': self.edge_message_kwargs,
+            'node_message_kwargs': self.node_message_kwargs,
         }
         base_config.update(config)
         return base_config
+
```

### Comparing `molgraph-0.5.1/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.2/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.2/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/models/mpnn.py` & `molgraph-0.5.2/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.2/molgraph/models/pretraining/autoencoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.2/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.2/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.2/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.2/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.2/molgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.1
+Version: 0.5.2
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -26,23 +26,22 @@
 See [pre-print](https://arxiv.org/abs/2208.09944)
 
 ## Documentation
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
 
 ## Implementations
 
-- **Tensor**
-    - **GraphTensor**
-        - A composite tensor holding graph data.
-        - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
-        - Can conveniently go between both states (merge() and separate())
-        - Can propagate node information (features) based on edges (propagate())
-        - Can add, update and remove graph data (update(), remove())
-        - Has an associated GraphTensorSpec which it compatible with Keras and TensorFlow API.
-            - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
+- **Graph tensor** ([GraphTensor](http://github.com/akensert/molgraph/tree/main/molgraph/tensors/graph_tensor.py))
+    - A composite tensor holding graph data.
+    - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
+    - Can conveniently go between both states (merge() and separate())
+    - Can propagate node information (features) based on edges (propagate())
+    - Can add, update and remove graph data (update(), remove())
+    - Has an associated GraphTensorSpec which it makes it compatible with Keras and TensorFlow API.
+        - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
 - **Layers**
     
     - **Convolutional**
         - GCNConv ([GCNConv](http://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcn_conv.py))
         - GINConv ([GINConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gin_conv.py))
         - GCNIIConv ([GCNIIConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcnii_conv.py))
         - GraphSageConv ([GraphSageConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/graph_sage_conv.py))
```

### Comparing `molgraph-0.5.1/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.2/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.1/setup.py` & `molgraph-0.5.2/setup.py`

 * *Files identical despite different names*

