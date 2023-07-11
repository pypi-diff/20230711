# Comparing `tmp/mct-nightly-1.9.0.20230709.post509.tar.gz` & `tmp/mct-nightly-1.9.0.20230710.post454.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.9.0.20230709.post509.tar", last modified: Sun Jul  9 00:05:10 2023, max compression
+gzip compressed data, was "mct-nightly-1.9.0.20230710.post454.tar", last modified: Mon Jul 10 00:04:55 2023, max compression
```

## Comparing `mct-nightly-1.9.0.20230709.post509.tar` & `mct-nightly-1.9.0.20230710.post454.tar`

### file list

```diff
@@ -1,526 +1,526 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.156835 mct-nightly-1.9.0.20230709.post509/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-09 00:05:10.156835 mct-nightly-1.9.0.20230709.post509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.052830 mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-09 00:05:09.000000 mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32637 2023-07-09 00:05:09.000000 mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 00:05:09.000000 mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-09 00:05:09.000000 mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-09 00:05:09.000000 mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.052830 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.052830 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.056830 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.056830 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.060830 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.060830 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.064831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.068831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.068831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.072831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.076831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.076831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.080831 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.084832 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.092832 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.092832 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.096832 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.100833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.100833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.104833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.104833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.104833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.108833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.108833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.108833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.108833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.108833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.108833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.112833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.112833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.112833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.112833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.116833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.116833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25782 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.120833 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.124834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.124834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.124834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.124834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.124834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.124834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.128834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.128834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.128834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.128834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.128834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.132834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.132834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.132834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.132834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.132834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/keras_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/pytorch_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.136834 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.140835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.140835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.140835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.140835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.140835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.144835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.148835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.152835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.156835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:05:10.156835 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-09 00:04:26.000000 mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-09 00:05:10.156835 mct-nightly-1.9.0.20230709.post509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-09 00:05:09.000000 mct-nightly-1.9.0.20230709.post509/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.556641 mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-10 00:04:55.000000 mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32637 2023-07-10 00:04:55.000000 mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 00:04:55.000000 mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 00:04:55.000000 mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 00:04:55.000000 mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.556641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.556641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.560641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.560641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.560641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.560641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.560641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.560641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.564641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.564641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.564641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.564641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.564641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.564641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.568641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.568641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.568641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.572641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.572641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.576641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.580641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.580641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.584641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27259 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.584641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.588641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.592641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.596641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.600641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.600641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.600641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.600641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/keras_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/pytorch_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.604641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.608641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.612641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:04:55.616641 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-10 00:04:12.000000 mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 00:04:55.620641 mct-nightly-1.9.0.20230710.post454/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-10 00:04:54.000000 mct-nightly-1.9.0.20230710.post454/setup.py
```

### Comparing `mct-nightly-1.9.0.20230709.post509/LICENSE.md` & `mct-nightly-1.9.0.20230710.post454/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/PKG-INFO` & `mct-nightly-1.9.0.20230710.post454/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230709.post509
+Version: 1.9.0.20230710.post454
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-1.9.0.20230709.post509/README.md` & `mct-nightly-1.9.0.20230710.post454/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230709.post509
+Version: 1.9.0.20230710.post454
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-1.9.0.20230709.post509/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.9.0.20230710.post454/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/constants.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,29 +521,28 @@
         Args:
             node: A graph node that wraps the operation for which the MAC count is computed.
             fw_info: FrameworkInfo object with information about the Keras model.
 
         Returns: The MAC count og the operation
         """
 
-        input_shape = node.input_shape
         output_shape = node.output_shape
         kernel_shape = node.get_weights_by_keys(fw_info.get_kernel_op_attributes(node.type)[0]).shape
         output_channel_axis, input_channel_axis = fw_info.kernel_channels_mapping.get(node.type)
 
         if node.type is Conv2D or node.type is Conv2DTranspose:
             # (C_out * W_out * H_out) * C_in * (W_kernel * H_kernel)
             return np.prod([x for x in output_shape if x is not None]) * \
-                   input_shape[input_channel_axis] * \
+                   kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
         elif node.type is DepthwiseConv2D:
             # Depth * (W_out * H_out) * C_in * (W_kernel * H_kernel)
             return node.framework_attr.get(DEPTH_MULTIPLIER) * \
                    np.prod([x for x in output_shape if x is not None]) / output_shape[output_channel_axis] * \
-                   input_shape[input_channel_axis] * \
+                   kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
         elif node.type is Dense:
             # IN * OUT
             return kernel_shape[0] * kernel_shape[1]
         else:
             return 0
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from model_compression_toolkit.core.common.mixed_precision.configurable_quant_id import \
     ConfigurableQuantizerIdentifier
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC,
                                      QuantizationMethod.UNIFORM, QuantizationMethod.LUT_POT_QUANTIZER],
-                quantizer_type=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
+                identifier=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
 class ConfigurableActivationQuantizer(BaseKerasInferableQuantizer):
     """
     Configurable activation quantizer for mixed precision search.
     It holds a set of activation quantizers for each of the given bit-width candidates, provided by the
     node's quantization config. This allows to use different quantized activations on-the-fly, according to the
     "active" quantization configuration index.
     """
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC,
                                      QuantizationMethod.UNIFORM, QuantizationMethod.LUT_POT_QUANTIZER,
                                      QuantizationMethod.LUT_SYM_QUANTIZER],
-                quantizer_type=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
+                identifier=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
 class ConfigurableWeightsQuantizer(BaseKerasInferableQuantizer):
     """
     Configurable weights quantizer for Keras mixed precision search.
     The quantizer holds a set of quantized layer's weights for each of the given bit-width candidates, provided by the
     node's quantization config. This allows to use different quantized weights on-the-fly.
 
     The general idea behind this kind of quantizer is that it gets the float tensor to quantize
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import torch.nn as nn
 from mct_quantizers.pytorch.quantizers import BasePyTorchInferableQuantizer
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC,
                                      QuantizationMethod.UNIFORM, QuantizationMethod.LUT_POT_QUANTIZER],
-                quantizer_type=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
+                identifier=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
 class ConfigurableActivationQuantizer(BasePyTorchInferableQuantizer):
     """
     Configurable activation quantizer for mixed precision search.
     It holds a set of activation quantizers for each of the given bit-width candidates, provided by the
     node's quantization config. This allows to use different quantized activations on-the-fly, according to the
     "active" quantization configuration index.
     """
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from mct_quantizers.pytorch.quantizers import BasePyTorchInferableQuantizer
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC,
                                      QuantizationMethod.UNIFORM, QuantizationMethod.LUT_POT_QUANTIZER,
                                      QuantizationMethod.LUT_SYM_QUANTIZER],
-                quantizer_type=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
+                identifier=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
 class ConfigurableWeightsQuantizer(BasePyTorchInferableQuantizer):
     """
     Configurable weights quantizer for Pytorch mixed precision search.
     The quantizer holds a set of quantized layer's weights for each of the given bit-width candidates, provided by the
     node's quantization config. This allows to use different quantized weights on-the-fly.
 
     The general idea behind this kind of quantizer is that it gets the float tensor to quantize
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,23 +477,22 @@
         Args:
             node: A graph node that wraps the operation for which the MAC count is computed.
             fw_info: FrameworkInfo object with information about the Pytorch model.
 
         Returns: The MAC count of the operation
         """
 
-        input_shape = node.input_shape[0]
         output_shape = node.output_shape[0]
         kernel_shape = node.get_weights_by_keys(fw_info.get_kernel_op_attributes(node.type)[0]).shape
         output_channel_axis, input_channel_axis = fw_info.kernel_channels_mapping.get(node.type)
 
         if node.type is Conv2d or node.type is ConvTranspose2d:
             # (C_out * W_out * H_out) * C_in * (W_kernel * H_kernel)
             return np.prod([x for x in output_shape if x is not None]) * \
-                   input_shape[input_channel_axis] * \
+                   kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
         elif node.type is Linear:
             # IN * OUT
             return kernel_shape[0] * kernel_shape[1]
         else:
             return 0
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/core/runner.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """
 
     weights_quantizers = {}
     if n.is_weights_quantization_enabled():
         quant_method = n.final_weights_quantization_cfg.weights_quantization_method
 
         quantizer_class = get_trainable_quantizer_class(quant_target=QuantizationTarget.Weights,
-                                                        quantizer_type=gptq_config.rounding_type,
+                                                        quantizer_id=gptq_config.rounding_type,
                                                         quant_method=quant_method,
                                                         quantizer_base_class=BaseKerasGPTQTrainableQuantizer)
         kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=n.type,
                                                               fw_info=DEFAULT_KERAS_INFO)
 
         weights_quantizers.update({kernel_attribute: quantizer_class(get_trainable_quantizer_weights_config(n),
                                                                      **gptq_config.gptq_quantizer_params_override)})
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     min_int = -int(signed) * (2 ** (num_bits - int(signed)))
     max_int = (2 ** (num_bits - int(signed))) - 1
     return delta * clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=RoundingType.SoftQuantizer)
+                identifier=RoundingType.SoftQuantizer)
 class SymmetricSoftRoundingGPTQ(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=0,
                                    max_val=2 ** num_bits - 1) + min_range
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
-                quantizer_type=RoundingType.SoftQuantizer)
+                identifier=RoundingType.SoftQuantizer)
 class UniformSoftRoundingGPTQ(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable uniform quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     min_int = -int(signed) * (2 ** (num_bits - int(signed)))
     max_int = (2 ** (num_bits - int(signed))) - 1
     return delta * qutils.ste_clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=RoundingType.STE)
+                identifier=RoundingType.STE)
 class STEWeightGPTQQuantizer(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to quantize a layer weights.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         to be compatible with the quantization infrastructure template.
     """
 
     weights_quantizers = {}
     if n.is_weights_quantization_enabled():
         quant_method = n.final_weights_quantization_cfg.weights_quantization_method
         quantizer_class = get_trainable_quantizer_class(quant_target=QuantizationTarget.Weights,
-                                                        quantizer_type=gptq_config.rounding_type,
+                                                        quantizer_id=gptq_config.rounding_type,
                                                         quant_method=quant_method,
                                                         quantizer_base_class=BasePytorchGPTQTrainableQuantizer)
         weights_quantizers.update({KERNEL: quantizer_class(get_trainable_quantizer_weights_config(n),
                                                            **gptq_config.gptq_quantizer_params_override)})
     activation_quantizers = []
     if n.is_activation_quantization_enabled():
         if n.final_activation_quantization_cfg is None:
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=-int(signed) * int_threshold,
                                    max_val=int_threshold - 1)
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=RoundingType.SoftQuantizer)
+                identifier=RoundingType.SoftQuantizer)
 class SymmetricSoftRoundingGPTQ(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=0,
                                    max_val=2 ** num_bits - 1) + min_range
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
-                quantizer_type=RoundingType.SoftQuantizer)
+                identifier=RoundingType.SoftQuantizer)
 class UniformSoftRoundingGPTQ(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable uniform quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     tensor_q = qutils.ste_round(qutils.ste_round(input_tensor_int + tensor_clipped))
 
     return delta * qutils.ste_clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=RoundingType.STE)
+                identifier=RoundingType.STE)
 class STEWeightGPTQQuantizer(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to quantize a layer weights.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/keras_quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/keras_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/legacy/pytorch_quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/legacy/pytorch_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/logger.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from mct_quantizers.keras.quantizers import WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, \
     ActivationPOTInferableQuantizer, ActivationSymmetricInferableQuantizer
 from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEWeightQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer inputs.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerWeightsConfig):
         """
@@ -168,15 +168,15 @@
                                                       per_channel=self.per_channel,
                                                       channel_axis=self.channel_axis,
                                                       input_rank=len(self.threshold_shape))
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEActivationQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer outputs.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerActivationConfig):
         """
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEUniformWeightQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer inputs.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerWeightsConfig):
         """
@@ -145,15 +145,15 @@
                                                 per_channel=self.per_channel,
                                                 channel_axis=self.channel_axis,
                                                 input_rank=len(self.min_max_shape))
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.UNIFORM],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEUniformActivationQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer outputs.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerActivationConfig):
         """
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
 from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEWeightQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer weights.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerWeightsConfig):
         """
@@ -128,15 +128,15 @@
                                                       per_channel=self.quantization_config.weights_per_channel_threshold,
                                                       channel_axis=self.quantization_config.weights_channels_axis)
 
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEActivationQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer activations.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerActivationConfig):
         """
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
 from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEUniformWeightQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer inputs.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerWeightsConfig):
         """
@@ -116,15 +116,15 @@
                                                 min_range=_min, max_range=_max,
                                                 per_channel=self.quantization_config.weights_per_channel_threshold,
                                                 channel_axis=self.quantization_config.weights_channels_axis)
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.UNIFORM],
-                quantizer_type=TrainingMethod.STE)
+                identifier=TrainingMethod.STE)
 class STEUniformActivationQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer activations.
     """
 
     def __init__(self, quantization_config: TrainableQuantizerActivationConfig):
         """
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,32 +14,31 @@
 # ==============================================================================
 from typing import Union, Any
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from mct_quantizers import QuantizationTarget
 from mct_quantizers.common.constants \
-    import QUANTIZATION_TARGET, QUANTIZATION_METHOD, QUANTIZER_TYPE
+    import QUANTIZATION_TARGET, QUANTIZATION_METHOD, QUANTIZER_ID
 from mct_quantizers.common.get_all_subclasses \
     import get_all_subclasses
 
 
 def get_trainable_quantizer_class(quant_target: QuantizationTarget,
-                                  quantizer_type: Union[Any, Any],
+                                  quantizer_id: Any,
                                   quant_method: QuantizationMethod,
                                   quantizer_base_class: type) -> type:
     """
     Searches for a trainable quantizer class that matches the requested QuantizationTarget and QuantizationMethod and
     a task dedicated quantizer type. Exactly one class should be found.
 
     Args:
         quant_target: QuantizationTarget value which indicates what is the target for quantization to
             use the quantizer for.
-        quantizer_type: The type of the quantizer (quantization technique).
-            This can differ, depending on the purpose the quantizer is for.
+        quantizer_id: A unique identifier for the quantizer class.
         quant_method: A list of QuantizationMethod values to indicate all type of quantization methods that the
             quantizer supports.
         quantizer_base_class: A type of quantizer that the requested quantizer should inherit from.
 
     Returns: A class of a quantizer that inherits from BaseKerasQATTrainableQuantizer.
 
     """
@@ -47,17 +46,17 @@
     if len(qat_quantizer_classes) == 0:
         Logger.error(f"No quantizers were found that inherit from {quantizer_base_class}.")  # pragma: no cover
 
     filtered_quantizers = list(filter(lambda q_class: getattr(q_class, QUANTIZATION_TARGET, None) is not None and
                                                       getattr(q_class, QUANTIZATION_TARGET) == quant_target and
                                                       getattr(q_class, QUANTIZATION_METHOD, None) is not None and
                                                        quant_method in getattr(q_class, QUANTIZATION_METHOD, []) and
-                                                      getattr(q_class, QUANTIZER_TYPE, None) == quantizer_type,
+                                                      getattr(q_class, QUANTIZER_ID, None) == quantizer_id,
                                       qat_quantizer_classes))
 
     if len(filtered_quantizers) != 1:
         Logger.error(f"Found {len(filtered_quantizers)} quantizer for target {quant_target.value} "  # pragma: no cover
                      f"that matches the requested quantization method {quant_method.name} and "
-                     f"quantizer type {quantizer_type.value} but there should be exactly one."
+                     f"quantizer type {quantizer_id.value} but there should be exactly one."
                      f"The possible quantizers that were found are {filtered_quantizers}.")
 
     return filtered_quantizers[0]
```

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-1.9.0.20230710.post454/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230709.post509/setup.py` & `mct-nightly-1.9.0.20230710.post454/setup.py`

 * *Files identical despite different names*

