# Comparing `tmp/frequenz-sdk-0.22.0.tar.gz` & `tmp/frequenz-sdk-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-sdk-0.22.0.tar", last modified: Tue Jul  4 12:08:17 2023, max compression
+gzip compressed data, was "frequenz-sdk-0.22.1.tar", last modified: Tue Jul 11 15:43:51 2023, max compression
```

## Comparing `frequenz-sdk-0.22.0.tar` & `frequenz-sdk-0.22.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3897 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)     6208 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.010006 frequenz-sdk-0.22.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/src/frequenz/sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/src/frequenz/sdk/_api_client/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_math.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_channel_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_config_managing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.014006 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_data_sourcing/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_data_sourcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
--rw-r--r--   0 runner    (1001) docker     (122)    15805 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6947 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7745 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    17218 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    28316 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/config/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12014 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23526 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/_component.py
--rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/_component_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/_component_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     5480 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/power/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18962 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/power/_distribution_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_base_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.018005 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    32060 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3885 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     5242 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     9501 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13082 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_moving_window.py
--rw-r--r--   0 runner    (1001) docker     (122)    16175 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)    21519 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_quantities.py
--rw-r--r--   0 runner    (1001) docker     (122)    28782 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_ringbuffer/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18830 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8411 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    16979 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    18773 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
--rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/logical_meter/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/logical_meter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15511 2023-07-04 12:08:06.000000 frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:08:17.022006 frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-04 12:08:16.000000 frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4904 2023-07-04 12:08:17.000000 frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 12:08:16.000000 frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-04 12:08:16.000000 frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-04 12:08:16.000000 frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3897 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6208 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.275658 frequenz-sdk-0.22.1/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_channel_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_config_managing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15805 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6947 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7745 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17218 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28316 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/power_distributing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12014 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23526 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5480 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/power/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18962 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/power/_distribution_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_base_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32060 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3885 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5242 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9501 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13082 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_moving_window.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16175 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21539 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28782 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18830 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8411 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16979 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18773 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15511 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4904 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/top_level.txt
```

### Comparing `frequenz-sdk-0.22.0/CONTRIBUTING.md` & `frequenz-sdk-0.22.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/LICENSE` & `frequenz-sdk-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/PKG-INFO` & `frequenz-sdk-0.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.22.0
+Version: 0.22.1
 Summary: Frequenz Python SDK
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
```

### Comparing `frequenz-sdk-0.22.0/README.md` & `frequenz-sdk-0.22.1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/docs/css/mkdocstrings.css` & `frequenz-sdk-0.22.1/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/docs/css/style.css` & `frequenz-sdk-0.22.1/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/docs/logo.png` & `frequenz-sdk-0.22.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/docs/mkdocstrings_autoapi.py` & `frequenz-sdk-0.22.1/docs/mkdocstrings_autoapi.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/mkdocs.yml` & `frequenz-sdk-0.22.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/pyproject.toml` & `frequenz-sdk-0.22.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/conftest.py` & `frequenz-sdk-0.22.1/src/conftest.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/_api_client/api_client.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_asyncio.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_asyncio.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_constants.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_math.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_math.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/_internal/_singleton_meta.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/__init__.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_channel_registry.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_channel_registry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_config_managing.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_config_managing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_decorator.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_decorator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_resampling.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/_run_utils.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_run_utils.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/__init__.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/power_distributing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/request.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/request.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/actor/power_distributing/result.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/result.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/config/_config.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/__init__.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/_data_pipeline.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/_graph.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_graph.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/_client.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_client.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/_connection.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_connection.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/client/_retry.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_retry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/__init__.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/_component.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/_component_data.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_data.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/component/_component_states.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_states.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/microgrid/connection_manager.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/connection_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/power/_distribution_algorithm.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/power/_distribution_algorithm.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/__init__.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_base_types.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_base_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_moving_window.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_moving_window.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_quantities.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_quantities.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             precision = int(fspec_parts[1])
         else:
             precision = 3
         if not self._exponent_unit_map:
             return f"{self._base_value:.{precision}f}"
 
         abs_value = abs(self._base_value)
-        exponent = math.floor(math.log10(abs_value))
+        exponent = math.floor(math.log10(abs_value)) if abs_value else 0
         unit_place = exponent - exponent % 3
         if unit_place < min(self._exponent_unit_map):
             unit = self._exponent_unit_map[min(self._exponent_unit_map.keys())]
             unit_place = min(self._exponent_unit_map)
         elif unit_place > max(self._exponent_unit_map):
             unit = self._exponent_unit_map[max(self._exponent_unit_map.keys())]
             unit_place = max(self._exponent_unit_map)
```

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_resampling.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_methods.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py` & `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/PKG-INFO` & `frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.22.0
+Version: 0.22.1
 Summary: Frequenz Python SDK
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
```

### Comparing `frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/SOURCES.txt` & `frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.0/src/frequenz_sdk.egg-info/requires.txt` & `frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

