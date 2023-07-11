# Comparing `tmp/evalml-0.77.0.tar.gz` & `tmp/evalml-0.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-b8ja8cfa/evalml-0.77.0.tar", last modified: Thu Jun  8 13:55:18 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-mu0morcw/evalml-0.78.0.tar", last modified: Tue Jul 11 15:58:17 2023, max compression
```

## Comparing `evalml-0.77.0.tar` & `evalml-0.78.0.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/
--rw-r--r--   0 root         (0) root         (0)     1513 2023-06-08 13:55:04.000000 evalml-0.77.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8233 2023-06-08 13:55:18.000000 evalml-0.77.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4824 2023-06-08 13:55:04.000000 evalml-0.77.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/
--rw-r--r--   0 root         (0) root         (0)      763 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/automl/
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/automl/automl_algorithm/
--rw-r--r--   0 root         (0) root         (0)      318 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12705 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    30444 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    21703 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    88380 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_search.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/automl/engine/
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/cf_engine.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/dask_engine.py
--rw-r--r--   0 root         (0) root         (0)    15405 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/engine_base.py
--rw-r--r--   0 root         (0) root         (0)     5060 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/sequential_engine.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/progress.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/data_checks/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_action.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_action_code.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     3156 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_message.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_message_code.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_message_type.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_checks.py
--rw-r--r--   0 root         (0) root         (0)    25088 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/default_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    11818 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    20762 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)    11843 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    17159 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9500 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7242 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8124 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/demos/
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/churn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/demos/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/diabetes.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/fraud.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/weather.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/wine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/exceptions/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/exceptions/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/model_family/
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_family/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_family/model_family.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_family/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/model_understanding/
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
--rw-r--r--   0 root         (0) root         (0)    18388 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/_partial_dependence_utils.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/force_plots.py
--rw-r--r--   0 root         (0) root         (0)    16822 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/metrics.py
--rw-r--r--   0 root         (0) root         (0)    27420 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/partial_dependence_functions.py
--rw-r--r--   0 root         (0) root         (0)    13556 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/permutation_importance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/_algorithms.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
--rw-r--r--   0 root         (0) root         (0)    36936 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15630 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/explainers.py
--rw-r--r--   0 root         (0) root         (0)    22293 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/objectives/
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     3392 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/fraud_cost.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/multiclass_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/objective_base.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/sensitivity_low_alert.py
--rw-r--r--   0 root         (0) root         (0)    33866 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/standard_metrics.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/time_series_regression_objective.py
--rw-r--r--   0 root         (0) root         (0)    15394 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/
--rw-r--r--   0 root         (0) root         (0)     1928 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/binary_classification_pipeline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     7845 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    40232 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/component_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/
--rw-r--r--   0 root         (0) root         (0)     1935 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10149 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/component_base.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/component_base_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/estimators/
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/
--rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8797 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4811 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8530 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13678 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7329 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5128 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/
--rw-r--r--   0 root         (0) root         (0)     1478 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6235 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/column_selectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
--rw-r--r--   0 root         (0) root         (0)    13779 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    12206 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/
--rw-r--r--   0 root         (0) root         (0)      599 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     5285 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
--rw-r--r--   0 root         (0) root         (0)     3116 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8253 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/imputer.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     6187 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    11389 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5899 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    15805 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)    17526 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
--rw-r--r--   0 root         (0) root         (0)     7283 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/oversampler.py
--rw-r--r--   0 root         (0) root         (0)     8265 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/undersampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/scalers/
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/scalers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/transformer.py
--rw-r--r--   0 root         (0) root         (0)    19130 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/utils.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/multiclass_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    33202 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/pipeline_meta.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    17176 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/time_series_classification_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    15747 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/time_series_pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/time_series_regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    53306 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/preprocessing/
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/no_split.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     5599 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/time_series_split.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/training_validation_split.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/problem_types/
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/problem_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/problem_types/problem_types.py
--rw-r--r--   0 root         (0) root         (0)     6085 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/problem_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/automl_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/dask_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9622 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
--rw-r--r--   0 root         (0) root         (0)    17604 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
--rw-r--r--   0 root         (0) root         (0)    14529 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
--rw-r--r--   0 root         (0) root         (0)   189671 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    39282 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38820 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification.py
--rw-r--r--   0 root         (0) root         (0)    15745 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
--rw-r--r--   0 root         (0) root         (0)     8716 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
--rw-r--r--   0 root         (0) root         (0)    12934 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_utils.py
--rw-r--r--   0 root         (0) root         (0)    33493 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_engine_base.py
--rw-r--r--   0 root         (0) root         (0)    37654 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_search_iterative.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_time_series_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/component_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27084 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    11644 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    16112 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6678 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8548 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_column_selector_transformers.py
--rw-r--r--   0 root         (0) root         (0)    64838 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_components.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     7573 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_en_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_en_regressor.py
--rw-r--r--   0 root         (0) root         (0)    15118 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_estimators.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_feature_selectors.py
--rw-r--r--   0 root         (0) root         (0)    14950 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_featuretools.py
--rw-r--r--   0 root         (0) root         (0)     9627 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
--rw-r--r--   0 root         (0) root         (0)    25736 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_imputer.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_knn_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     8017 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_label_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lda.py
--rw-r--r--   0 root         (0) root         (0)    13414 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     9754 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lsa.py
--rw-r--r--   0 root         (0) root         (0)    20457 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     9988 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_nullable_types_replacer.py
--rw-r--r--   0 root         (0) root         (0)    26816 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_one_hot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    25966 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)    19941 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_oversampler.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_pca.py
--rw-r--r--   0 root         (0) root         (0)    12025 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)    23430 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)    18269 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)    10542 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8928 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_target_encoder.py
--rw-r--r--   0 root         (0) root         (0)     9398 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    30311 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    24722 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_time_series_imputer.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     6246 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_undersampler.py
--rw-r--r--   0 root         (0) root         (0)     9766 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_xgboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)    80162 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     9729 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/tips.csv
--rw-r--r--   0 root         (0) root         (0)    61194 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/titanic.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/data_checks_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24199 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action.py
--rw-r--r--   0 root         (0) root         (0)    20667 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_message.py
--rw-r--r--   0 root         (0) root         (0)    29212 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)    13086 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    30182 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    26417 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8238 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5609 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)    18212 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4898 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/demo_tests/test_datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/dependency_update_check/
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
--rw-r--r--   0 root         (0) root         (0)      642 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/dependency_update_check/minimum_requirements.txt
--rw-r--r--   0 root         (0) root         (0)      778 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10709 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
--rw-r--r--   0 root         (0) root         (0)     5184 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/test_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/test_time_series_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/model_family_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_family_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_family_tests/test_model_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
--rw-r--r--   0 root         (0) root         (0)    67430 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
--rw-r--r--   0 root         (0) root         (0)     9790 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
--rw-r--r--   0 root         (0) root         (0)    19357 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)    14744 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)    27456 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    98520 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
--rw-r--r--   0 root         (0) root         (0)    29313 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
--rw-r--r--   0 root         (0) root         (0)    26181 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/objective_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_fraud_detection.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)    13953 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_objectives.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_sla.py
--rw-r--r--   0 root         (0) root         (0)    27155 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_standard_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
--rw-r--r--   0 root         (0) root         (0)     4688 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3652 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
--rw-r--r--   0 root         (0) root         (0)    94308 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_component_graph.py
--rw-r--r--   0 root         (0) root         (0)     8969 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_graphs.py
--rw-r--r--   0 root         (0) root         (0)    50312 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
--rw-r--r--   0 root         (0) root         (0)   101489 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     5621 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    70356 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_no_split.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_split_data.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/problem_type_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/problem_type_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/problem_type_tests/test_problem_types.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/test_all_test_dirs_included.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/tuner_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/test_random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     9170 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/test_skopt_tuner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/utils_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    30486 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)    12628 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tuners/
--rw-r--r--   0 root         (0) root         (0)      316 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     4675 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/skopt_tuner.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/tuner.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/tuner_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/utils/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/base_meta.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    26270 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     7066 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/update_checker.py
--rw-r--r--   0 root         (0) root         (0)     6346 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8233 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20684 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-08 13:55:04.000000 evalml-0.77.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 13:55:18.000000 evalml-0.77.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-07-11 15:58:03.000000 evalml-0.78.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-07-11 15:58:17.000000 evalml-0.78.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-07-11 15:58:03.000000 evalml-0.78.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/automl/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/automl/automl_algorithm/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/automl_algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12705 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/automl_algorithm/automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    31547 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/automl_algorithm/default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    21703 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/automl_algorithm/iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    88830 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/automl_search.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/automl/engine/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/engine/cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/engine/dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)    15405 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/engine/engine_base.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/engine/sequential_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/progress.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/automl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/data_checks/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check_action_code.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check_message_code.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_check_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    25088 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/default_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11862 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    20762 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    17159 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8124 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/data_checks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/demos/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/churn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/demos/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/diabetes.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/fraud.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/weather.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/demos/wine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/exceptions/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/model_family/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_family/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_family/model_family.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_family/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/model_understanding/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18388 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/_partial_dependence_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    16822 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    27420 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/partial_dependence_functions.py
+-rw-r--r--   0 root         (0) root         (0)    13556 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/permutation_importance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/model_understanding/prediction_explanations/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/prediction_explanations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/prediction_explanations/_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
+-rw-r--r--   0 root         (0) root         (0)    36936 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/prediction_explanations/_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15630 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/prediction_explanations/explainers.py
+-rw-r--r--   0 root         (0) root         (0)    22293 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/model_understanding/visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/objectives/
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/fraud_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/multiclass_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/objective_base.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/sensitivity_low_alert.py
+-rw-r--r--   0 root         (0) root         (0)    35534 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/standard_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/time_series_regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)    15394 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/objectives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/binary_classification_pipeline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    40232 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/component_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10149 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/component_base.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/component_base_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/estimators/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8797 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8530 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13678 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/column_selectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/dimensionality_reduction/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/encoders/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    13779 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12206 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/imputer.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5899 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    15805 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)    17526 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/samplers/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/samplers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/samplers/oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     8265 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/samplers/undersampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/pipelines/components/transformers/scalers/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/scalers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/transformers/transformer.py
+-rw-r--r--   0 root         (0) root         (0)    19130 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/components/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/multiclass_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    33202 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/pipeline_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    17176 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/time_series_classification_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    15747 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/time_series_pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/time_series_regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    53306 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/preprocessing/data_splitters/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/data_splitters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/data_splitters/no_split.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/data_splitters/sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/data_splitters/time_series_split.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/data_splitters/training_validation_split.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/preprocessing/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/problem_types/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/problem_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/problem_types/problem_types.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/problem_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/automl_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/dask_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9622 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
+-rw-r--r--   0 root         (0) root         (0)    17604 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)    14529 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)   189570 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    39282 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38797 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_classification.py
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_regression.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
+-rw-r--r--   0 root         (0) root         (0)    12934 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_automl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    34960 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_engine_base.py
+-rw-r--r--   0 root         (0) root         (0)    37347 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_search_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/automl_tests/test_time_series_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/component_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27084 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    11644 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    16112 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8548 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_column_selector_transformers.py
+-rw-r--r--   0 root         (0) root         (0)    64838 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_components.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_en_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_en_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    15118 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_estimators.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_feature_selectors.py
+-rw-r--r--   0 root         (0) root         (0)    14950 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     9627 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
+-rw-r--r--   0 root         (0) root         (0)    25736 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_knn_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     8017 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_lda.py
+-rw-r--r--   0 root         (0) root         (0)    13414 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_lgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     9754 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_lgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_lsa.py
+-rw-r--r--   0 root         (0) root         (0)    20457 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_nullable_types_replacer.py
+-rw-r--r--   0 root         (0) root         (0)    26816 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_one_hot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    25966 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    19941 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_pca.py
+-rw-r--r--   0 root         (0) root         (0)    12025 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    23430 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)    10542 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_target_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    30311 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    24722 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_time_series_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_undersampler.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/component_tests/test_xgboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    80732 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     9729 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data/tips.csv
+-rw-r--r--   0 root         (0) root         (0)    61194 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data/titanic.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/data_checks_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24199 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)    29212 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    19715 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    13203 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    30198 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    26417 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8238 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    18212 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/data_checks_tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/demo_tests/test_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/dependency_update_check/
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/dependency_update_check/minimum_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/integration_tests/test_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/integration_tests/test_time_series_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/model_family_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_family_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_family_tests/test_model_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)    67430 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    19357 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)    14744 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)    27456 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    98520 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
+-rw-r--r--   0 root         (0) root         (0)    26181 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/model_understanding_tests/test_visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/objective_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_fraud_detection.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)    13977 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_objectives.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_sla.py
+-rw-r--r--   0 root         (0) root         (0)    28528 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/objective_tests/test_standard_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
+-rw-r--r--   0 root         (0) root         (0)    94308 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/test_component_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8969 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/test_graphs.py
+-rw-r--r--   0 root         (0) root         (0)    50312 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
+-rw-r--r--   0 root         (0) root         (0)   101437 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     5621 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    70356 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/preprocessing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/preprocessing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/preprocessing_tests/test_no_split.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/preprocessing_tests/test_split_data.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/problem_type_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/problem_type_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/problem_type_tests/test_problem_types.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/test_all_test_dirs_included.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/tuner_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/tuner_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/tuner_tests/test_random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     9170 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/tuner_tests/test_skopt_tuner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tests/utils_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/utils_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/utils_tests/test_cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30486 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/utils_tests/test_gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4559 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/utils_tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/utils_tests/test_nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tests/utils_tests/test_woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/tuners/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tuners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tuners/grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tuners/random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tuners/skopt_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tuners/tuner.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/tuners/tuner_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml/utils/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/base_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26380 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/update_checker.py
+-rw-r--r--   0 root         (0) root         (0)     6346 2023-07-11 15:58:03.000000 evalml-0.78.0/evalml/utils/woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20684 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 15:58:17.000000 evalml-0.78.0/evalml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-07-11 15:58:03.000000 evalml-0.78.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:58:17.000000 evalml-0.78.0/setup.cfg
```

### Comparing `evalml-0.77.0/LICENSE` & `evalml-0.78.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/PKG-INFO` & `evalml-0.78.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.77.0
+Version: 0.78.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.77.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.78.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.77.0/README.md` & `evalml-0.78.0/README.md`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/__init__.py` & `evalml-0.78.0/evalml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", FutureWarning)
     warnings.simplefilter("ignore", DeprecationWarning)
     import skopt
 warnings.filterwarnings("ignore", category=FutureWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-__version__ = "0.77.0"
+__version__ = "0.78.0"
```

### Comparing `evalml-0.77.0/evalml/automl/automl_algorithm/automl_algorithm.py` & `evalml-0.78.0/evalml/automl/automl_algorithm/automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/automl_algorithm/default_algorithm.py` & `evalml-0.78.0/evalml/automl/automl_algorithm/default_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         text_in_ensembling (boolean): If True and ensembling is True, then n_jobs will be set to 1 to avoid downstream sklearn stacking issues related to nltk. Defaults to False.
         top_n (int): top n number of pipelines to use for long mode.
         num_long_explore_pipelines (int): number of pipelines to explore for each top n pipeline at the start of long mode.
         num_long_pipelines_per_batch (int): number of pipelines per batch for each top n pipeline through long mode.
         allow_long_running_models (bool): Whether or not to allow longer-running models for large multiclass problems. If False and no pipelines, component graphs, or model families are provided,
             AutoMLSearch will not use Elastic Net or XGBoost when there are more than 75 multiclass targets and will not use CatBoost when there are more than 150 multiclass targets. Defaults to False.
         features (list)[FeatureBase]: List of features to run DFS on in AutoML pipelines. Defaults to None. Features will only be computed if the columns used by the feature exist in the input and if the feature has not been computed yet.
+        run_feature_selection (bool): If True, will run a separate feature selection pipeline and only use selected features in subsequent batches.
+            If False, will use all of the features for every pipeline. Only used for default algorithm.
         verbose (boolean): Whether or not to display logging information regarding pipeline building. Defaults to False.
         exclude_featurizers (list[str]): A list of featurizer components to exclude from the pipelines built by DefaultAlgorithm.
             Valid options are "DatetimeFeaturizer", "EmailFeaturizer", "URLFeaturizer", "NaturalLanguageFeaturizer", "TimeSeriesFeaturizer"
         allowed_model_families (list(str, ModelFamily)): The model families to search. The default of None searches over all
             model families. Run evalml.pipelines.components.utils.allowed_model_families("binary") to see options. Change `binary`
             to `multiclass` or `regression` depending on the problem type.
         excluded_model_families (list[ModelFamily]): A list of model families to exclude from the estimators used when building pipelines. For default algorithm, this only excludes estimators in the non-naive batches.
@@ -96,14 +98,15 @@
         text_in_ensembling=False,
         top_n=3,
         ensembling=False,
         num_long_explore_pipelines=50,
         num_long_pipelines_per_batch=10,
         allow_long_running_models=False,
         features=None,
+        run_feature_selection=True,
         verbose=False,
         exclude_featurizers=None,
     ):
         super().__init__(
             allowed_pipelines=[],
             allowed_model_families=allowed_model_families,
             excluded_model_families=excluded_model_families,
@@ -128,14 +131,15 @@
         self.verbose = verbose
         self._selected_cat_cols = []
         self._split = False
         self.allow_long_running_models = allow_long_running_models
         self._X_with_cat_cols = None
         self._X_without_cat_cols = None
         self.features = features
+        self.run_feature_selection = run_feature_selection
         self.ensembling = ensembling
         self.exclude_featurizers = exclude_featurizers or []
 
         if allowed_model_families is not None and excluded_model_families is not None:
             raise ValueError(
                 "Both `allowed_model_families` and `excluded_model_families` cannot be set.",
             )
@@ -380,25 +384,26 @@
     def _create_n_pipelines(self, pipelines, n, create_starting_parameters=False):
         next_batch = []
         for _ in range(n):
             for pipeline in pipelines:
                 if pipeline.name not in self._tuners:
                     self._create_tuner(pipeline)
 
-                select_parameters = self._create_select_parameters()
                 parameters = (
                     self._tuners[pipeline.name].get_starting_parameters(
                         self._hyperparameters,
                         self.random_seed,
                     )
                     if create_starting_parameters
                     else self._tuners[pipeline.name].propose()
                 )
                 parameters = self._transform_parameters(pipeline, parameters)
-                parameters.update(select_parameters)
+                if self.run_feature_selection:
+                    select_parameters = self._create_select_parameters()
+                    parameters.update(select_parameters)
                 next_batch.append(
                     pipeline.new(parameters=parameters, random_seed=self.random_seed),
                 )
         return next_batch
 
     def _create_long_exploration(self, n):
         estimators = [
@@ -445,15 +450,17 @@
         Returns:
             list(PipelineBase): a list of instances of PipelineBase subclasses, ready to be trained and evaluated.
         """
         if self.ensembling:
             if self._batch_number == 0:
                 next_batch = self._create_naive_pipelines()
             elif self._batch_number == 1:
-                next_batch = self._create_naive_pipelines(use_features=True)
+                next_batch = self._create_naive_pipelines(
+                    use_features=self.run_feature_selection,
+                )
             elif self._batch_number == 2:
                 next_batch = self._create_fast_final()
             elif self.batch_number == 3:
                 next_batch = self._create_ensemble(
                     self._pipeline_parameters.get("Label Encoder", {}),
                 )
             elif self.batch_number == 4:
@@ -480,15 +487,17 @@
                     self._top_n_pipelines,
                     self.num_long_pipelines_per_batch,
                 )
         else:
             if self._batch_number == 0:
                 next_batch = self._create_naive_pipelines()
             elif self._batch_number == 1:
-                next_batch = self._create_naive_pipelines(use_features=True)
+                next_batch = self._create_naive_pipelines(
+                    use_features=self.run_feature_selection,
+                )
             elif self._batch_number == 2:
                 next_batch = self._create_fast_final()
             elif self.batch_number == 3:
                 next_batch = self._create_long_exploration(n=self.top_n)
             else:
                 next_batch = self._create_n_pipelines(
                     self._top_n_pipelines,
@@ -618,22 +627,30 @@
                 },
             )
 
     def _make_split_pipeline(self, estimator, pipeline_name=None):
         # Should be category, not categorical so that we make sure to exclude
         # all logical types with the "category" tag
         numeric_exclude_types = ["category", "EmailAddress", "URL"]
-        if self._X_with_cat_cols is None or self._X_without_cat_cols is None:
+        if (
+            self.run_feature_selection
+            and self._X_with_cat_cols is None
+            or self._X_without_cat_cols is None
+        ):
             self._X_without_cat_cols = self.X.ww.select(
                 exclude=numeric_exclude_types,
             )
 
             self._X_with_cat_cols = self.X.ww[self._selected_cat_cols]
 
-        if self._selected_cat_cols and self._selected_cols:
+        if (
+            self.run_feature_selection
+            and self._selected_cat_cols
+            and self._selected_cols
+        ):
             self._split = True
 
             categorical_pipeline_parameters = {
                 "Select Columns Transformer": {"columns": self._selected_cat_cols},
             }
             numeric_pipeline_parameters = {
                 "Select Columns Transformer": {"columns": self._selected_cols},
@@ -695,15 +712,19 @@
                 self.problem_type,
                 pipeline_name=pipeline_name,
                 random_seed=self.random_seed,
                 sub_pipeline_names=sub_pipeline_names,
                 pre_pipeline_components=pre_pipeline_components,
                 post_pipelines_components=post_pipelines_components,
             )
-        elif self._selected_cat_cols and not self._selected_cols:
+        elif (
+            self.run_feature_selection
+            and self._selected_cat_cols
+            and not self._selected_cols
+        ):
             categorical_pipeline_parameters = {
                 "Select Columns Transformer": {"columns": self._selected_cat_cols},
             }
             categorical_pipeline = make_pipeline(
                 self._X_with_cat_cols,
                 self.y,
                 estimator,
@@ -711,15 +732,15 @@
                 sampler_name=self.sampler_name,
                 parameters=categorical_pipeline_parameters,
                 extra_components_before=[SelectColumns],
                 features=self.features,
                 exclude_featurizers=self.exclude_featurizers,
             )
             return categorical_pipeline
-        else:
+        elif self.run_feature_selection:
             numeric_pipeline_parameters = {
                 "Select Columns Transformer": {"columns": self._selected_cols},
             }
             numeric_pipeline = make_pipeline(
                 self.X,
                 self.y,
                 estimator,
@@ -727,7 +748,18 @@
                 sampler_name=self.sampler_name,
                 parameters=numeric_pipeline_parameters,
                 extra_components_after=[SelectColumns],
                 features=self.features,
                 exclude_featurizers=self.exclude_featurizers,
             )
             return numeric_pipeline
+
+        else:
+            pipeline = make_pipeline(
+                self.X,
+                self.y,
+                estimator,
+                self.problem_type,
+                sampler_name=self.sampler_name,
+                exclude_featurizers=self.exclude_featurizers,
+            )
+            return pipeline
```

### Comparing `evalml-0.77.0/evalml/automl/automl_algorithm/iterative_algorithm.py` & `evalml-0.78.0/evalml/automl/automl_algorithm/iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/automl_search.py` & `evalml-0.78.0/evalml/automl/automl_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,17 @@
             to `multiclass` or `regression` depending on the problem type. Note that if allowed_pipelines is provided,
             this parameter will be ignored.
 
         features (list)[FeatureBase]: List of features to run DFS on AutoML pipelines. Defaults to None.
             Features will only be computed if the columns used by the feature exist in the search input
             and if the feature itself is not in search input. If features is an empty list, the DFS Transformer will not be included in pipelines.
 
+        run_feature_selection (bool): If True, will run a separate feature selection pipeline and only use selected features in subsequent batches.
+            If False, will use all of the features for every pipeline. Only used for default algorithm, setting is no-op for iterative algorithm.
+
         data_splitter (sklearn.model_selection.BaseCrossValidator): Data splitting method to use. Defaults to StratifiedKFold.
 
         tuner_class: The tuner class to use. Defaults to SKOptTuner.
 
         optimize_thresholds (bool): Whether or not to optimize the binary pipeline threshold. Defaults to True.
 
         start_iteration_callback (callable): Function called before each pipeline training iteration.
@@ -466,14 +469,15 @@
         patience=None,
         tolerance=None,
         data_splitter=None,
         allowed_component_graphs=None,
         allowed_model_families=None,
         excluded_model_families=None,
         features=None,
+        run_feature_selection=True,
         start_iteration_callback=None,
         add_result_callback=None,
         error_callback=None,
         additional_objectives=None,
         alternate_thresholding_objective="F1",
         random_seed=0,
         n_jobs=-1,
@@ -807,15 +811,14 @@
             internal_search_parameters.update({"pipeline": self.problem_configuration})
 
         self.features = features
         if self.features is not None:
             internal_search_parameters.update(
                 {"DFS Transformer": {"features": self.features}},
             )
-
         self.sampler_method = sampler_method
         self.sampler_balanced_ratio = sampler_balanced_ratio
         self._sampler_name = None
 
         featurizer_names = [
             "DatetimeFeaturizer",
             "EmailFeaturizer",
@@ -840,14 +843,15 @@
                 "TimeSeriesFeaturizer" in exclude_featurizers
                 and "DatetimeFeaturizer" not in exclude_featurizers
             ):
                 raise ValueError(
                     "For time series problems, if TimeSeriesFeaturizer is excluded, must also exclude DatetimeFeaturizer",
                 )
         self.exclude_featurizers = exclude_featurizers or []
+        self.run_feature_selection = run_feature_selection
 
         if excluded_model_families:
             if not isinstance(excluded_model_families, list):
                 raise ValueError(
                     "`excluded_model_families` must be passed in the form of a list.",
                 )
             if not all(isinstance(x, ModelFamily) for x in excluded_model_families):
@@ -940,14 +944,15 @@
                 excluded_model_families=self.excluded_model_families,
                 tuner_class=self.tuner_class,
                 random_seed=self.random_seed,
                 search_parameters=internal_search_parameters,
                 text_in_ensembling=text_in_ensembling,
                 allow_long_running_models=allow_long_running_models,
                 features=features,
+                run_feature_selection=run_feature_selection,
                 ensembling=self.ensembling,
                 verbose=self.verbose,
                 n_jobs=self.n_jobs,
                 exclude_featurizers=self.exclude_featurizers,
             )
         else:
             raise ValueError("Please specify a valid automl algorithm.")
```

### Comparing `evalml-0.77.0/evalml/automl/callbacks.py` & `evalml-0.78.0/evalml/automl/callbacks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/engine/cf_engine.py` & `evalml-0.78.0/evalml/automl/engine/cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/engine/dask_engine.py` & `evalml-0.78.0/evalml/automl/engine/dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/engine/engine_base.py` & `evalml-0.78.0/evalml/automl/engine/engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/engine/sequential_engine.py` & `evalml-0.78.0/evalml/automl/engine/sequential_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/pipeline_search_plots.py` & `evalml-0.78.0/evalml/automl/pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/progress.py` & `evalml-0.78.0/evalml/automl/progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/automl/utils.py` & `evalml-0.78.0/evalml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/__init__.py` & `evalml-0.78.0/evalml/data_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/class_imbalance_data_check.py` & `evalml-0.78.0/evalml/data_checks/class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_check.py` & `evalml-0.78.0/evalml/data_checks/data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_check_action.py` & `evalml-0.78.0/evalml/data_checks/data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_check_action_code.py` & `evalml-0.78.0/evalml/data_checks/data_check_action_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_check_action_option.py` & `evalml-0.78.0/evalml/data_checks/data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_check_message.py` & `evalml-0.78.0/evalml/data_checks/data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_check_message_code.py` & `evalml-0.78.0/evalml/data_checks/data_check_message_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/data_checks.py` & `evalml-0.78.0/evalml/data_checks/data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/datetime_format_data_check.py` & `evalml-0.78.0/evalml/data_checks/datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/default_data_checks.py` & `evalml-0.78.0/evalml/data_checks/default_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/id_columns_data_check.py` & `evalml-0.78.0/evalml/data_checks/id_columns_data_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Data check that checks if any of the features are likely to be ID columns."""
+
 from evalml.data_checks import (
     DataCheck,
     DataCheckActionCode,
     DataCheckActionOption,
     DataCheckMessageCode,
     DataCheckWarning,
 )
@@ -176,24 +177,27 @@
 
         col_names = [col for col in X.columns]
         cols_named_id = [
             col for col in col_names if (str(col).lower() == "id")
         ]  # columns whose name is "id"
         id_cols = {col: 0.95 for col in cols_named_id}
 
-        for dtypes in [["Double"], ["Integer", "IntegerNullable", "Categorical"]]:
-            X_temp = X.ww.select(include=dtypes)
+        for types in [
+            ["Double"],
+            ["Integer", "IntegerNullable", "Categorical", "Unknown"],
+        ]:
+            X_temp = X.ww.select(include=types)
             check_all_unique = X_temp.nunique() == len(X_temp)
             cols_with_all_unique = check_all_unique[
                 check_all_unique
             ].index.tolist()  # columns whose values are all unique
 
             # Temporary solution for downstream instances of integers being mapped to doubles.
             # Will be removed when resolved.
-            if dtypes == ["Double"]:
+            if types == ["Double"]:
                 cols_with_all_unique = [
                     col
                     for col in cols_with_all_unique
                     if all(
                         X_temp[col].mod(1).eq(0),
                     )  # Parse out columns that contain all `integer` values
                 ]
```

### Comparing `evalml-0.77.0/evalml/data_checks/invalid_target_data_check.py` & `evalml-0.78.0/evalml/data_checks/invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/multicollinearity_data_check.py` & `evalml-0.78.0/evalml/data_checks/multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/no_variance_data_check.py` & `evalml-0.78.0/evalml/data_checks/no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/null_data_check.py` & `evalml-0.78.0/evalml/data_checks/null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/outliers_data_check.py` & `evalml-0.78.0/evalml/data_checks/outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/sparsity_data_check.py` & `evalml-0.78.0/evalml/data_checks/sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/target_distribution_data_check.py` & `evalml-0.78.0/evalml/data_checks/target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/target_leakage_data_check.py` & `evalml-0.78.0/evalml/data_checks/target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/ts_parameters_data_check.py` & `evalml-0.78.0/evalml/data_checks/ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/ts_splitting_data_check.py` & `evalml-0.78.0/evalml/data_checks/ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/uniqueness_data_check.py` & `evalml-0.78.0/evalml/data_checks/uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/data_checks/utils.py` & `evalml-0.78.0/evalml/data_checks/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/breast_cancer.py` & `evalml-0.78.0/evalml/demos/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/churn.py` & `evalml-0.78.0/evalml/demos/churn.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/data/churn.csv` & `evalml-0.78.0/evalml/demos/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/data/daily-min-temperatures.csv` & `evalml-0.78.0/evalml/demos/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/data/fraud_transactions.csv.gz` & `evalml-0.78.0/evalml/demos/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/diabetes.py` & `evalml-0.78.0/evalml/demos/diabetes.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/fraud.py` & `evalml-0.78.0/evalml/demos/fraud.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/weather.py` & `evalml-0.78.0/evalml/demos/weather.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/demos/wine.py` & `evalml-0.78.0/evalml/demos/wine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/exceptions/__init__.py` & `evalml-0.78.0/evalml/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/exceptions/exceptions.py` & `evalml-0.78.0/evalml/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_family/model_family.py` & `evalml-0.78.0/evalml/model_family/model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_family/utils.py` & `evalml-0.78.0/evalml/model_family/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/__init__.py` & `evalml-0.78.0/evalml/model_understanding/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py` & `evalml-0.78.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/_partial_dependence_utils.py` & `evalml-0.78.0/evalml/model_understanding/_partial_dependence_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/decision_boundary.py` & `evalml-0.78.0/evalml/model_understanding/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/feature_explanations.py` & `evalml-0.78.0/evalml/model_understanding/feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/force_plots.py` & `evalml-0.78.0/evalml/model_understanding/force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/metrics.py` & `evalml-0.78.0/evalml/model_understanding/metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/partial_dependence_functions.py` & `evalml-0.78.0/evalml/model_understanding/partial_dependence_functions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/permutation_importance.py` & `evalml-0.78.0/evalml/model_understanding/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/prediction_explanations/_algorithms.py` & `evalml-0.78.0/evalml/model_understanding/prediction_explanations/_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py` & `evalml-0.78.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/prediction_explanations/_user_interface.py` & `evalml-0.78.0/evalml/model_understanding/prediction_explanations/_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/prediction_explanations/explainers.py` & `evalml-0.78.0/evalml/model_understanding/prediction_explanations/explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/model_understanding/visualizations.py` & `evalml-0.78.0/evalml/model_understanding/visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/objectives/__init__.py` & `evalml-0.78.0/evalml/objectives/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from evalml.objectives.objective_base import ObjectiveBase
 from evalml.objectives.regression_objective import RegressionObjective
 from evalml.objectives.standard_metrics import (
     AUC,
     F1,
     MAE,
     MAPE,
+    SMAPE,
     MSE,
     MeanSquaredLogError,
     R2,
     RootMeanSquaredError,
     RootMeanSquaredLogError,
     AccuracyBinary,
     AccuracyMulticlass,
```

### Comparing `evalml-0.77.0/evalml/objectives/binary_classification_objective.py` & `evalml-0.78.0/evalml/objectives/binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/objectives/cost_benefit_matrix.py` & `evalml-0.78.0/evalml/objectives/cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/objectives/fraud_cost.py` & `evalml-0.78.0/evalml/objectives/fraud_cost.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/objectives/lead_scoring.py` & `evalml-0.78.0/evalml/objectives/lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/objectives/objective_base.py` & `evalml-0.78.0/evalml/objectives/objective_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/objectives/sensitivity_low_alert.py` & `evalml-0.78.0/evalml/objectives/sensitivity_low_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     BinaryClassificationObjective,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class SensitivityLowAlert(BinaryClassificationObjective):
-    """Create instance of SensitivityLowAlert.
+    """Sensitivity at Low Alert Rates.
 
     Args:
         alert_rate (float): percentage of top scores to classify as high risk.
     """
 
     name = "Sensitivity at Low Alert Rates"
     greater_is_better = True
```

### Comparing `evalml-0.77.0/evalml/objectives/standard_metrics.py` & `evalml-0.78.0/evalml/objectives/standard_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Standard machine learning objective functions."""
 import warnings
 
 import numpy as np
 import pandas as pd
 from sklearn import metrics
 from sklearn.preprocessing import label_binarize
+from sktime.performance_metrics.forecasting import MeanAbsolutePercentageError
 
 from evalml.objectives.binary_classification_objective import (
     BinaryClassificationObjective,
 )
 from evalml.objectives.multiclass_classification_objective import (
     MulticlassClassificationObjective,
 )
@@ -846,14 +847,53 @@
 
     @classproperty
     def positive_only(self):
         """If True, this objective is only valid for positive data."""
         return True
 
 
+class SMAPE(TimeSeriesRegressionObjective):
+    """Mean absolute percentage error for time series regression. Scaled by 100 to return a percentage.
+
+    Only valid for nonzero inputs. Otherwise, will throw a ValueError.
+
+    Example:
+        >>> y_true = pd.Series([1.5, 2, 3, 1, 0.5, 1, 2.5, 2.5, 1, 0.5, 2])
+        >>> y_pred = pd.Series([1.5, 2.5, 2, 1, 0.5, 1, 3, 2.25, 0.75, 0.25, 1.75])
+        >>> np.testing.assert_almost_equal(SMAPE().objective_function(y_true, y_pred), 18.13652589)
+    """
+
+    name = "Symmetric Mean Absolute Percentage Error"
+    greater_is_better = False
+    score_needs_proba = False
+    perfect_score = 0.0
+    is_bounded_like_percentage = True  # Range [0, 200]
+    expected_range = [0, 200]
+
+    def objective_function(self, y_true, y_predicted, X=None, sample_weight=None):
+        """Objective function for mean absolute percentage error for time series regression."""
+        if ((abs(y_true) + abs(y_predicted)) == 0).any():
+            raise ValueError(
+                "Symmetric Mean Absolute Percentage Error cannot be used when "
+                "true and predicted targets both contain the value 0.",
+            )
+        if isinstance(y_true, pd.Series):
+            y_true = y_true.to_numpy()
+        if isinstance(y_predicted, pd.Series):
+            y_predicted = y_predicted.to_numpy()
+
+        smape = MeanAbsolutePercentageError(symmetric=True)
+        return smape(y_true, y_predicted) * 100
+
+    @classproperty
+    def positive_only(self):
+        """If True, this objective is only valid for positive data."""
+        return True
+
+
 class MSE(RegressionObjective):
     """Mean squared error for regression.
 
     Example:
         >>> y_true = pd.Series([1.5, 2, 3, 1, 0.5, 1, 2.5, 2.5, 1, 0.5, 2])
         >>> y_pred = pd.Series([1.5, 2.5, 2, 1, 0.5, 1, 3, 2.25, 0.75, 0.25, 1.75])
         >>> np.testing.assert_almost_equal(MSE().objective_function(y_true, y_pred), 0.1590909)
```

### Comparing `evalml-0.77.0/evalml/objectives/utils.py` & `evalml-0.78.0/evalml/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/__init__.py` & `evalml-0.78.0/evalml/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/binary_classification_pipeline.py` & `evalml-0.78.0/evalml/pipelines/binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/binary_classification_pipeline_mixin.py` & `evalml-0.78.0/evalml/pipelines/binary_classification_pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/classification_pipeline.py` & `evalml-0.78.0/evalml/pipelines/classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/component_graph.py` & `evalml-0.78.0/evalml/pipelines/component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/component_base.py` & `evalml-0.78.0/evalml/pipelines/components/component_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/component_base_meta.py` & `evalml-0.78.0/evalml/pipelines/components/component_base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py` & `evalml-0.78.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/estimator.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/et_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py` & `evalml-0.78.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/column_selectors.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/column_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/label_encoder.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/encoders/label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/target_encoder.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/imputer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/target_imputer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/__init__.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/lsa.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/samplers/base_sampler.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/samplers/oversampler.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/samplers/oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/samplers/undersampler.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/samplers/undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/transformers/transformer.py` & `evalml-0.78.0/evalml/pipelines/components/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/components/utils.py` & `evalml-0.78.0/evalml/pipelines/components/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/multiclass_classification_pipeline.py` & `evalml-0.78.0/evalml/pipelines/multiclass_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/pipeline_base.py` & `evalml-0.78.0/evalml/pipelines/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/pipeline_meta.py` & `evalml-0.78.0/evalml/pipelines/pipeline_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/regression_pipeline.py` & `evalml-0.78.0/evalml/pipelines/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/time_series_classification_pipelines.py` & `evalml-0.78.0/evalml/pipelines/time_series_classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/time_series_pipeline_base.py` & `evalml-0.78.0/evalml/pipelines/time_series_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/time_series_regression_pipeline.py` & `evalml-0.78.0/evalml/pipelines/time_series_regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/pipelines/utils.py` & `evalml-0.78.0/evalml/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/preprocessing/data_splitters/no_split.py` & `evalml-0.78.0/evalml/preprocessing/data_splitters/no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/preprocessing/data_splitters/sk_splitters.py` & `evalml-0.78.0/evalml/preprocessing/data_splitters/sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/preprocessing/data_splitters/time_series_split.py` & `evalml-0.78.0/evalml/preprocessing/data_splitters/time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/preprocessing/data_splitters/training_validation_split.py` & `evalml-0.78.0/evalml/preprocessing/data_splitters/training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/preprocessing/utils.py` & `evalml-0.78.0/evalml/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/problem_types/problem_types.py` & `evalml-0.78.0/evalml/problem_types/problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/problem_types/utils.py` & `evalml-0.78.0/evalml/problem_types/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/dask_test_utils.py` & `evalml-0.78.0/evalml/tests/automl_tests/dask_test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py` & `evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py` & `evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py` & `evalml-0.78.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     PipelineBase,
     RegressionPipeline,
     StackedEnsembleClassifier,
 )
 from evalml.pipelines.components import (
     ARIMARegressor,
     DateTimeFeaturizer,
-    DecisionTreeClassifier,
     EmailFeaturizer,
     NaturalLanguageFeaturizer,
     RandomForestClassifier,
     SelectColumns,
     TimeSeriesFeaturizer,
     URLFeaturizer,
 )
@@ -264,15 +263,15 @@
     assert isinstance(batch_times[1]["Total time of batch"], float)
     assert isinstance(batch_times[2]["Total time of batch"], float)
     assert isinstance(batch_times[3]["Total time of batch"], float)
 
     assert len(batch_times) == 3
     assert len(batch_times[1]) == 2
     assert len(batch_times[2]) == 2
-    assert len(batch_times[3]) == 8
+    assert len(batch_times[3]) == 6
 
     assert "Batch Time Stats" in out
     assert "Batch 1 time stats" in out
     assert "Batch 2 time stats" in out
     assert "Batch 3 time stats" in out
 
 
@@ -3270,41 +3269,39 @@
             ] == Categorical((0.01, 0.02, 0.03)).rvs(random_state=automl.random_seed)
 
 
 def test_automl_pipeline_params_kwargs(AutoMLTestEnv, X_y_multi):
     X, y = X_y_multi
     hyperparams = {
         "Imputer": {"numeric_impute_strategy": Categorical(["most_frequent"])},
-        "Decision Tree Classifier": {
+        "XGBoost Classifier": {
             "max_depth": Integer(1, 2),
-            "ccp_alpha": Real(0.1, 0.5),
+            "eta": Real(0.01, 0.5),
         },
     }
     automl = AutoMLSearch(
         X_train=X,
         y_train=y,
         problem_type="multiclass",
         search_parameters=hyperparams,
-        allowed_model_families=[ModelFamily.DECISION_TREE],
+        allowed_model_families=[ModelFamily.XGBOOST],
         n_jobs=1,
     )
     env = AutoMLTestEnv("multiclass")
     with env.test_context(score_return_value={automl.objective.name: 1.0}):
         automl.search()
     for i, row in automl.rankings.iterrows():
         if "Imputer" in row["parameters"]:
             assert (
                 row["parameters"]["Imputer"]["numeric_impute_strategy"]
                 == "most_frequent"
             )
-        if "Decision Tree Classifier" in row["parameters"]:
-            assert (
-                0.1 < row["parameters"]["Decision Tree Classifier"]["ccp_alpha"] < 0.5
-            )
-            assert row["parameters"]["Decision Tree Classifier"]["max_depth"] == 1
+        if "XGBoost Classifier" in row["parameters"]:
+            assert 0.1 < row["parameters"]["XGBoost Classifier"]["eta"] < 0.5
+            assert row["parameters"]["XGBoost Classifier"]["max_depth"] == 1
 
 
 @pytest.mark.parametrize("random_seed", [0, 1, 9])
 def test_automl_pipeline_random_seed(AutoMLTestEnv, random_seed, X_y_multi):
     X, y = X_y_multi
     automl = AutoMLSearch(
         X_train=X,
@@ -4692,16 +4689,16 @@
     if problem_type == "binary":
         X, y = X_y_binary
         problem_configuration = None
         allowed_component_graphs = {
             "cg": {
                 "Imputer": ["Imputer", "X", "y"],
                 "Label Encoder": ["Label Encoder", "Imputer.x", "y"],
-                "Decision Tree Classifier": [
-                    "Decision Tree Classifier",
+                "Random Forest Classifier": [
+                    "Random Forest Classifier",
                     "Label Encoder.x",
                     "Label Encoder.y",
                 ],
             },
         }
     else:
         X, _, y = ts_data(problem_type="time series binary")
@@ -4716,16 +4713,16 @@
                 "Imputer": ["Imputer", "X", "y"],
                 "Label Encoder": ["Label Encoder", "Imputer.x", "y"],
                 "DateTime Featurizer": [
                     "DateTime Featurizer",
                     "Label Encoder.x",
                     "Label Encoder.y",
                 ],
-                "Decision Tree Classifier": [
-                    "Decision Tree Classifier",
+                "Random Forest Classifier": [
+                    "Random Forest Classifier",
                     "DateTime Featurizer.x",
                     "Label Encoder.y",
                 ],
             },
         }
         batches = 2 if algorithm == "default" else batches
 
@@ -4741,28 +4738,28 @@
         problem_configuration=problem_configuration,
         allowed_component_graphs=allowed_component_graphs,
         search_parameters=search_parameters,
         automl_algorithm=algorithm,
         max_batches=batches,
     )
     aml.search()
-    estimator_args = inspect.getargspec(DecisionTreeClassifier)
+    estimator_args = inspect.getargspec(RandomForestClassifier)
     # estimator_args[0] gives the parameter names, while [3] gives the associated values
     # estimator_args[0][i + 1] to skip 'self' in the estimator
     # we do len - 1 in order to skip the random seed, which isn't present in the row['parameters']
     expected_params = {
         estimator_args[0][i + 1]: estimator_args[3][i]
         for i in range(len(estimator_args[3]) - 1)
     }
     sorted_full_rank = aml.full_rankings.sort_values(by="id")
     found_dtc = False
     for _, row in sorted_full_rank.iterrows():
         # we check the initial decision tree classifier parameters.
-        if "Decision Tree Classifier" in row["parameters"]:
-            assert expected_params == row["parameters"]["Decision Tree Classifier"]
+        if "Random Forest Classifier" in row["parameters"]:
+            assert expected_params == row["parameters"]["Random Forest Classifier"]
             found_dtc = True
             break
     assert found_dtc
     for tuners in aml.automl_algorithm._tuners.values():
         assert (
             tuners._pipeline_hyperparameter_ranges["Imputer"]["numeric_impute_strategy"]
             == expected
```

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_algorithm.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1263,15 +1263,15 @@
     if algo == "default":
         env = AutoMLTestEnv("multiclass")
         with env.test_context(score_return_value={"Log Loss Multiclass": 1.0}):
             automl.search()
     if allow_long_running_models or unique == 10:
         assert "Dropping estimators" not in caplog.text
         return
-    estimators = ["Elastic Net Classifier", "CatBoost Classifier", "XGBoost Classifier"]
+    estimators = ["Elastic Net Classifier", "XGBoost Classifier"]
 
     assert "Dropping estimators {}".format(", ".join(sorted(estimators))) in caplog.text
 
 
 def test_automl_threshold_score(fraud_100):
     X, y = fraud_100
     X_train, X_valid, y_train, y_valid = split_data(X, y, "binary")
```

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_automl_utils.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_automl_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_default_algorithm.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_default_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1057,7 +1057,47 @@
             X=X,
             y=y,
             problem_type="binary",
             allowed_model_families=[ModelFamily.RANDOM_FOREST],
             excluded_model_families=[ModelFamily.XGBOOST],
             sampler_name=None,
         )
+
+
+@pytest.mark.parametrize("run_feature_selection", [True, False])
+def test_default_algorithm_run_feature_selection(run_feature_selection, X_y_binary):
+    X, y = X_y_binary
+    algo_selection = DefaultAlgorithm(
+        X=X,
+        y=y,
+        problem_type="binary",
+        allowed_model_families=[
+            ModelFamily.RANDOM_FOREST,
+            ModelFamily.XGBOOST,
+            ModelFamily.LINEAR_MODEL,
+        ],
+        run_feature_selection=run_feature_selection,
+        sampler_name=None,
+    )
+
+    batches = [algo_selection.next_batch() for _ in range(0, 3)]
+
+    assert algo_selection.run_feature_selection is run_feature_selection
+
+    for i, batch in enumerate(batches):
+        for pipeline in batch:
+            if run_feature_selection and i > 0:
+                if i == 1:
+                    assert "RF Classifier Select From Model" in list(
+                        pipeline.component_graph.component_dict.keys(),
+                    )
+                else:
+                    assert "Select Columns Transformer" in list(
+                        pipeline.component_graph.component_dict.keys(),
+                    )
+            else:
+                assert "RF Classifier Select From Model" not in list(
+                    pipeline.component_graph.component_dict.keys(),
+                )
+                assert "Select Columns Transformer" not in list(
+                    pipeline.component_graph.component_dict.keys(),
+                )
```

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_engine_base.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_iterative_algorithm.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_iterative_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -726,31 +726,27 @@
     estimators_in_first_batch = [p.estimator.name for p in next_batch]
 
     if problem_type == ProblemTypes.REGRESSION:
         linear_models = ["Elastic Net Regressor"]
         extra_dep_estimators = [
             "XGBoost Regressor",
             "LightGBM Regressor",
-            "CatBoost Regressor",
         ]
         core_estimators = [
             "Random Forest Regressor",
-            "Decision Tree Regressor",
             "Extra Trees Regressor",
         ]
     else:
         linear_models = ["Elastic Net Classifier", "Logistic Regression Classifier"]
         extra_dep_estimators = [
             "XGBoost Classifier",
             "LightGBM Classifier",
-            "CatBoost Classifier",
         ]
         core_estimators = [
             "Random Forest Classifier",
-            "Decision Tree Classifier",
             "Extra Trees Classifier",
         ]
     assert (
         estimators_in_first_batch
         == linear_models + extra_dep_estimators + core_estimators
     )
 
@@ -758,41 +754,37 @@
 def test_iterative_algorithm_first_batch_order_param(X_y_binary):
     X, y = X_y_binary
 
     # put random forest first
     estimator_family_order = [
         ModelFamily.RANDOM_FOREST,
         ModelFamily.LINEAR_MODEL,
-        ModelFamily.DECISION_TREE,
         ModelFamily.EXTRA_TREES,
         ModelFamily.XGBOOST,
         ModelFamily.LIGHTGBM,
-        ModelFamily.CATBOOST,
     ]
     algo = IterativeAlgorithm(
         X=X,
         y=y,
         problem_type="binary",
         _estimator_family_order=estimator_family_order,
     )
     next_batch = algo.next_batch()
     estimators_in_first_batch = [p.estimator.name for p in next_batch]
 
     final_estimators = [
         "XGBoost Classifier",
         "LightGBM Classifier",
-        "CatBoost Classifier",
     ]
     assert (
         estimators_in_first_batch
         == [
             "Random Forest Classifier",
             "Elastic Net Classifier",
             "Logistic Regression Classifier",
-            "Decision Tree Classifier",
             "Extra Trees Classifier",
         ]
         + final_estimators
     )
 
 
 @pytest.mark.parametrize(
@@ -840,15 +832,15 @@
 @pytest.mark.parametrize("allow_long_running_models", [True, False])
 @pytest.mark.parametrize(
     "length,models_missing",
     [
         (10, []),
         (75, []),
         (100, ["Elastic Net Classifier", "XGBoost Classifier"]),
-        (160, ["Elastic Net Classifier", "XGBoost Classifier", "CatBoost Classifier"]),
+        (160, ["Elastic Net Classifier", "XGBoost Classifier"]),
     ],
 )
 def test_iterative_algorithm_allow_long_running_models(
     length,
     models_missing,
     allow_long_running_models,
     allowed_component_graphs,
@@ -887,15 +879,15 @@
             assert all([s not in p.name for s in models_missing])
 
 
 @pytest.mark.parametrize("problem", ["binary", "multiclass", "regression"])
 @pytest.mark.parametrize("allow_long_running_models", [True, False])
 @pytest.mark.parametrize(
     "length,models_missing",
-    [(10, 0), (75, 0), (100, 2), (160, 3)],
+    [(10, 0), (75, 0), (100, 2), (160, 2)],
 )
 def test_iterative_algorithm_allow_long_running_models_problem(
     length,
     models_missing,
     allow_long_running_models,
     problem,
 ):
```

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_pipeline_search_plots.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_progress.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_search.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_search_iterative.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_search_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/automl_tests/test_time_series_split.py` & `evalml-0.78.0/evalml/tests/automl_tests/test_time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py` & `evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py` & `evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py` & `evalml-0.78.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_arima_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_arima_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_baseline_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_baseline_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_catboost_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_catboost_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_column_selector_transformers.py` & `evalml-0.78.0/evalml/tests/component_tests/test_column_selector_transformers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_components.py` & `evalml-0.78.0/evalml/tests/component_tests/test_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_datetime_featurizer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_drop_rows_transformer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_en_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_en_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_en_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_en_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_estimators.py` & `evalml-0.78.0/evalml/tests/component_tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_et_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_et_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_feature_selectors.py` & `evalml-0.78.0/evalml/tests/component_tests/test_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_featuretools.py` & `evalml-0.78.0/evalml/tests/component_tests/test_featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py` & `evalml-0.78.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_imputer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_knn_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_knn_imputer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_label_encoder.py` & `evalml-0.78.0/evalml/tests/component_tests/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_lda.py` & `evalml-0.78.0/evalml/tests/component_tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_lgbm_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_lgbm_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_log_transformer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_lsa.py` & `evalml-0.78.0/evalml/tests/component_tests/test_lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_natural_language_featurizer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_nullable_types_replacer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_nullable_types_replacer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_one_hot_encoder.py` & `evalml-0.78.0/evalml/tests/component_tests/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_ordinal_encoder.py` & `evalml-0.78.0/evalml/tests/component_tests/test_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_oversampler.py` & `evalml-0.78.0/evalml/tests/component_tests/test_oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_pca.py` & `evalml-0.78.0/evalml/tests/component_tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_per_column_imputer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_prophet_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_simple_imputer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_standard_scaler.py` & `evalml-0.78.0/evalml/tests/component_tests/test_standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_svm_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_svm_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_target_encoder.py` & `evalml-0.78.0/evalml/tests/component_tests/test_target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_target_imputer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_time_series_featurizer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_time_series_imputer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_time_series_regularizer.py` & `evalml-0.78.0/evalml/tests/component_tests/test_time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_undersampler.py` & `evalml-0.78.0/evalml/tests/component_tests/test_undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_utils.py` & `evalml-0.78.0/evalml/tests/component_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_xgboost_classifier.py` & `evalml-0.78.0/evalml/tests/component_tests/test_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/component_tests/test_xgboost_regressor.py` & `evalml-0.78.0/evalml/tests/component_tests/test_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/conftest.py` & `evalml-0.78.0/evalml/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,48 +102,64 @@
     return graphviz
 
 
 @pytest.fixture
 def get_test_data_with_or_without_primary_key():
     def _get_test_data_with_primary_key(input_type, has_primary_key):
         X = None
-        if input_type == "integer":
+        if input_type == "Integer":
             X_dict = {
                 "col_1_id": [0, 1, 2, 3],
                 "col_2": [2, 3, 4, 5],
                 "col_3_id": [1, 1, 2, 3],
                 "col_5": [0, 0, 1, 2],
             }
             if not has_primary_key:
                 X_dict["col_1_id"] = [1, 1, 2, 3]
             X = pd.DataFrame.from_dict(X_dict)
 
-        elif input_type == "integer_nullable":
+        elif input_type == "IntegerNullable":
             X_dict = {
                 "col_1_id": pd.Series([0, 1, 2, 3], dtype="Int64"),
                 "col_2": pd.Series([2, 3, 4, 5], dtype="Int64"),
                 "col_3_id": pd.Series([1, 1, 2, 3], dtype="Int64"),
                 "col_5": pd.Series([0, 0, 1, 2], dtype="Int64"),
             }
             if not has_primary_key:
                 X_dict["col_1_id"] = pd.Series([1, 1, 2, 3], dtype="Int64")
             X = pd.DataFrame.from_dict(X_dict)
 
-        elif input_type == "double":
+        elif input_type == "Double":
             X_dict = {
                 "col_1_id": [0.0, 1.0, 2.0, 3.0],
                 "col_2": [2, 3, 4, 5],
                 "col_3_id": [1, 1, 2, 3],
                 "col_5": [0, 0, 1, 2],
             }
             if not has_primary_key:
                 X_dict["col_1_id"] = [1.0, 1.0, 2.0, 3.0]
             X = pd.DataFrame.from_dict(X_dict)
 
-        elif input_type == "string":
+        elif input_type == "Unknown":
+            X_dict = {
+                "col_1_id": ["a", "b", "c", "d"],
+                "col_2": ["w", "x", "y", "z"],
+                "col_3_id": [
+                    "123456789012345",
+                    "234567890123456",
+                    "3456789012345678",
+                    "45678901234567",
+                ],
+                "col_5": ["0", "0", "1", "2"],
+            }
+            if not has_primary_key:
+                X_dict["col_1_id"] = ["b", "b", "c", "d"]
+            X = pd.DataFrame.from_dict(X_dict)
+
+        elif input_type == "Categorical":
             X_dict = {
                 "col_1_id": ["a", "b", "c", "d"],
                 "col_2": ["w", "x", "y", "z"],
                 "col_3_id": [
                     "123456789012345",
                     "234567890123456",
                     "3456789012345678",
```

### Comparing `evalml-0.77.0/evalml/tests/data/churn.csv` & `evalml-0.78.0/evalml/tests/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data/daily-min-temperatures.csv` & `evalml-0.78.0/evalml/tests/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data/fraud_transactions.csv.gz` & `evalml-0.78.0/evalml/tests/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data/tips.csv` & `evalml-0.78.0/evalml/tests/data/tips.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data/titanic.csv` & `evalml-0.78.0/evalml/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action_option.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_message.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_checks.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             ],
         ).to_dict(),
     ]
 
 
 @pytest.mark.parametrize(
     "input_type",
-    ["integer", "integer_nullable", "string", "double"],
+    ["Integer", "IntegerNullable", "Unknown", "Double", "Categorical"],
 )
 def test_identified_first_col_primary_key(
     input_type,
     get_test_data_with_or_without_primary_key,
 ):
     X = get_test_data_with_or_without_primary_key(
         input_type=input_type,
@@ -296,27 +296,27 @@
             ],
         ).to_dict(),
     ]
 
 
 @pytest.mark.parametrize(
     "input_type",
-    ["integer", "integer_nullable", "string", "double"],
+    ["Integer", "IntegerNullable", "Unknown", "Double", "Categorical"],
 )
 def test_unidentified_first_col_primary_key(
     input_type,
     get_test_data_with_or_without_primary_key,
 ):
     X = get_test_data_with_or_without_primary_key(
         input_type=input_type,
         has_primary_key=False,
     )
 
     id_cols_check = IDColumnsDataCheck(id_threshold=0.95)
-    if input_type == "string":
+    if input_type in ["Unknown", "Categorical"]:
         order = ["col_2", "col_3_id", "col_1_id"]
     else:
         order = ["col_2", "col_1_id", "col_3_id"]
     order_msg = f"Columns '{order[0]}', '{order[1]}', '{order[2]}' are 95.0% or more likely to be an ID column"
 
     assert id_cols_check.validate(X) == [
         DataCheckWarning(
@@ -331,21 +331,23 @@
                     metadata={"columns": order},
                 ),
             ],
         ).to_dict(),
     ]
 
     X = X.rename(columns={"col_1_id": "col_1"})
-    if input_type == "integer":
+    if input_type == "Integer":
         X.at[0, "col_1"] = 0
-    elif input_type == "integer_nullable":
+    elif input_type == "IntegerNullable":
         X.at[0, "col_1"] = 0
-    elif input_type == "double":
+    elif input_type == "Double":
         X.at[0, "col_1"] = 0.0
-    elif input_type == "string":
+    elif input_type == "Unknown":
+        X.at[0, "col_1"] = "a"
+    elif input_type == "Categorical":
         X["col_1"] = X["col_1"].cat.add_categories("a")
         X.at[0, "col_1"] = "a"
 
     assert id_cols_check.validate(X) == [
         DataCheckWarning(
             message="Columns 'col_1', 'col_2', 'col_3_id' are 95.0% or more likely to be an ID column",
             data_check_name=id_data_check_name,
```

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     DataCheckMessageCode,
     DataChecks,
     DataCheckWarning,
     DCAOParameterType,
     InvalidTargetDataCheck,
 )
 from evalml.exceptions import DataCheckInitError
-from evalml.objectives import MAPE, MeanSquaredLogError, RootMeanSquaredLogError
+from evalml.objectives import MAPE, SMAPE, MeanSquaredLogError, RootMeanSquaredLogError
 from evalml.problem_types import ProblemTypes, is_binary, is_multiclass, is_regression
 from evalml.utils.woodwork_utils import numeric_and_boolean_ww
 
 invalid_targets_data_check_name = InvalidTargetDataCheck.name
 
 
 def test_invalid_target_data_check_invalid_n_unique():
@@ -393,15 +393,15 @@
             },
         ).to_dict(),
     ]
 
 
 @pytest.mark.parametrize(
     "objective",
-    [RootMeanSquaredLogError(), MeanSquaredLogError(), MAPE()],
+    [RootMeanSquaredLogError(), MeanSquaredLogError(), MAPE(), SMAPE()],
 )
 def test_invalid_target_data_check_invalid_labels_for_nonnegative_objective_instances(
     objective,
 ):
     X = pd.DataFrame({"column_one": [100, 200, 100, 200, 200, 100, 200, 100] * 25})
     y = pd.Series([2, 2, 3, 3, -1, -1, 1, 1] * 25)
```

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_null_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_outliers_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/data_checks_tests/test_utils.py` & `evalml-0.78.0/evalml/tests/data_checks_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/demo_tests/test_datasets.py` & `evalml-0.78.0/evalml/tests/demo_tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt` & `evalml-0.78.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 black==23.3.0
 catboost==1.2
 category-encoders==2.5.1.post0
-click==8.1.3
+click==8.1.4
 cloudpickle==2.2.1
 colorama==0.4.6
 dask==2023.3.2
 distributed==2023.3.2.1
 featuretools==1.26.0
 graphviz==0.20.1
 holidays==0.20
 imbalanced-learn==0.10.1
 ipywidgets==8.0.4
 kaleido==0.2.1
 lightgbm==3.3.5
 lime==0.2.0.1
-matplotlib==3.7.1
+matplotlib==3.7.2
 matplotlib-inline==0.1.6
 networkx==3.1
 nlp-primitives==2.11.0
-numpy==1.23.5
+numpy==1.24.4
 packaging==23.1
 pandas==1.5.3
-plotly==5.14.1
+plotly==5.15.0
 pmdarima==2.0.3
 pyzmq==25.1.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.10.1
 seaborn==0.12.2
-shap==0.41.0
+shap==0.42.0
 sktime==0.17.0
 statsmodels==0.14.0
 texttable==1.6.7
 tomli==2.0.1
 vowpalwabbit==9.8.0
 woodwork==0.24.0
-xgboost==1.7.5
+xgboost==1.7.6
```

### Comparing `evalml-0.77.0/evalml/tests/dependency_update_check/minimum_requirements.txt` & `evalml-0.78.0/evalml/tests/dependency_update_check/minimum_requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 plotly==5.0.0
 pmdarima==1.8.5
 pyzmq==20.0.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.5.0
 seaborn==0.11.1
-shap==0.40.0
+shap==0.42.0
 sktime==0.17.0
 statsmodels==0.12.2
 texttable==1.6.2
 tomli==2.0.1
 vowpalwabbit==8.11.0
 woodwork[dask]==0.22.0
 xgboost==1.7.0
```

### Comparing `evalml-0.77.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt` & `evalml-0.78.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 pytest-xdist==2.1.0
 pytest==7.1.2
 pyzmq==20.0.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.5.0
 seaborn==0.11.1
-shap==0.40.0
+shap==0.42.0
 sktime==0.17.0
 statsmodels==0.12.2
 texttable==1.6.2
 tomli==2.0.1
 vowpalwabbit==8.11.0
 woodwork[dask]==0.22.0
 xgboost==1.7.0
```

### Comparing `evalml-0.77.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py` & `evalml-0.78.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/integration_tests/test_nullable_types.py` & `evalml-0.78.0/evalml/tests/integration_tests/test_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/integration_tests/test_time_series_integration.py` & `evalml-0.78.0/evalml/tests/integration_tests/test_time_series_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_family_tests/test_model_family.py` & `evalml-0.78.0/evalml/tests/model_family_tests/test_model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/test_decision_boundary.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/test_decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/test_feature_explanations.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/test_feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/test_metrics.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/test_partial_dependence.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/test_permutation_importance.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/model_understanding_tests/test_visualizations.py` & `evalml-0.78.0/evalml/tests/model_understanding_tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_binary_classification_objective.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_fraud_detection.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_fraud_detection.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_lead_scoring.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_objectives.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_objectives.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     normalize_objectives,
     organize_objectives,
     ranking_only_objectives,
     recommendation_score,
 )
 from evalml.objectives.fraud_cost import FraudCost
 from evalml.objectives.objective_base import ObjectiveBase
-from evalml.objectives.standard_metrics import MAPE
+from evalml.objectives.standard_metrics import MAPE, SMAPE
 from evalml.objectives.utils import _all_objectives_dict
 from evalml.problem_types import ProblemTypes
 
 
 def test_create_custom_objective():
     class MockEmptyObjective(ObjectiveBase):
         def objective_function(self, y_true, y_predicted, X=None):
@@ -107,39 +107,39 @@
     }
 
 
 def test_get_core_objectives_types():
     assert len(get_core_objectives(ProblemTypes.MULTICLASS)) == 13
     assert len(get_core_objectives(ProblemTypes.BINARY)) == 8
     assert len(get_core_objectives(ProblemTypes.REGRESSION)) == 7
-    assert len(get_core_objectives(ProblemTypes.TIME_SERIES_REGRESSION)) == 7
+    assert len(get_core_objectives(ProblemTypes.TIME_SERIES_REGRESSION)) == 8
 
 
 def test_get_optimization_objectives_types():
     assert len(get_optimization_objectives(ProblemTypes.MULTICLASS)) == 13
     assert len(get_optimization_objectives(ProblemTypes.BINARY)) == 8
     assert len(get_optimization_objectives(ProblemTypes.REGRESSION)) == 7
-    assert len(get_optimization_objectives(ProblemTypes.TIME_SERIES_REGRESSION)) == 7
+    assert len(get_optimization_objectives(ProblemTypes.TIME_SERIES_REGRESSION)) == 8
 
 
 def test_get_ranking_objectives_types():
     assert len(get_ranking_objectives(ProblemTypes.MULTICLASS)) == 16
     assert len(get_ranking_objectives(ProblemTypes.BINARY)) == 9
     assert len(get_ranking_objectives(ProblemTypes.REGRESSION)) == 9
-    assert len(get_ranking_objectives(ProblemTypes.TIME_SERIES_REGRESSION)) == 10
+    assert len(get_ranking_objectives(ProblemTypes.TIME_SERIES_REGRESSION)) == 11
 
 
 def test_optimization_excludes_ranking():
     objs = get_optimization_objectives(ProblemTypes.BINARY)
     for obj in objs:
         assert obj.__class__ not in ranking_only_objectives()
 
 
 def test_get_time_series_objectives_types(time_series_objectives):
-    assert len(time_series_objectives) == 10
+    assert len(time_series_objectives) == 11
 
 
 def test_objective_outputs(
     X_y_binary,
     X_y_multi,
 ):
     _, y_binary = X_y_binary
@@ -225,17 +225,17 @@
     else:
         obj = obj()
 
     # Make any changes to data needed for objective
     if isinstance(obj, FraudCost):
         # FraudCost needs an "amount" column
         X = pd.DataFrame({"amount": [100, 5, 250, 89] * 5})
-    elif isinstance(obj, MAPE):
+    elif isinstance(obj, (MAPE, SMAPE)):
         if isinstance(y_true.ww.logical_type, BooleanNullable):
-            pytest.skip("MAPE doesn't support inputs containing 0")
+            pytest.skip("MAPE and SMAPE don't support inputs containing 0")
         # Replace numeric inputs containing 0
         y_true = y_true.ww.replace({0: 10})
         y_pred = y_pred.replace({0: 10})
 
     score = obj.score(y_true=y_true, y_predicted=y_pred, X=X)
     assert not pd.isna(score)
```

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_sla.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_sla.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/objective_tests/test_standard_metrics.py` & `evalml-0.78.0/evalml/tests/objective_tests/test_standard_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas as pd
 import pytest
 
 from evalml.objectives import (
     F1,
     MAPE,
     MSE,
+    SMAPE,
     AccuracyBinary,
     AccuracyMulticlass,
     BalancedAccuracyBinary,
     BalancedAccuracyMulticlass,
     BinaryClassificationObjective,
     CostBenefitMatrix,
     ExpVariance,
@@ -707,14 +708,52 @@
     ) == pytest.approx(4 / 6 * 100)
     assert obj.score(
         pd.Series(s2_actual, index=range(10, 14)),
         pd.Series(s2_predicted, index=range(20, 24)),
     ) == pytest.approx(8 / 4 * 100)
 
 
+def test_smape_time_series_model():
+    obj = SMAPE()
+
+    s1_actual = np.array([0, 0, 1, 1, 1, 1, 2, 0, 2])
+    s1_predicted = np.array([0, 1, 0, 1, 1, 2, 1, 2, 0])
+
+    s2_actual = np.array([-1, -2, 1, 3])
+    s2_predicted = np.array([1, 2, -1, -3])
+
+    s3_actual = np.array([1, 2, 4, 2, 1, 2])
+    s3_predicted = np.array([0, 2, 2, 0, 3, 2])
+
+    s4_actual = np.array([0, 2, 0, 2, 1, 2])
+    s4_predicted = np.array([1, 2, 2, 1, 3, 2])
+
+    with pytest.raises(
+        ValueError,
+        match="Symmetric Mean Absolute Percentage Error cannot be used when "
+        "true and predicted targets both contain the value 0.",
+    ):
+        obj.score(s1_actual, s1_predicted)
+    assert obj.score(s2_actual, s2_predicted) == pytest.approx(8 / 4 * 100)
+    assert obj.score(s3_actual, s3_predicted) == pytest.approx((17 / 6) / 3 * 100)
+    assert obj.score(s4_actual, s4_predicted) == pytest.approx((17 / 6) / 3 * 100)
+    assert obj.score(
+        pd.Series(s3_actual, index=range(-12, -6)),
+        s3_predicted,
+    ) == pytest.approx((17 / 6) / 3 * 100)
+    assert obj.score(
+        pd.Series(s2_actual, index=range(10, 14)),
+        pd.Series(s2_predicted, index=range(20, 24)),
+    ) == pytest.approx(8 / 4 * 100)
+    assert obj.score(
+        pd.Series(s4_actual, index=range(-12, -6)),
+        s4_predicted,
+    ) == pytest.approx((17 / 6) / 3 * 100)
+
+
 @pytest.mark.parametrize("objective_class", _all_objectives_dict().values())
 def test_calculate_percent_difference(objective_class):
     score = 5
     reference_score = 10
     denominator = 1 if objective_class.is_bounded_like_percentage else reference_score
 
     change = (
```

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/test_component_graph.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/test_component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/test_graphs.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/test_pipeline_utils.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/test_pipeline_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,26 +591,26 @@
             else:
                 assert not any(
                     "sampler" in comp.name for comp in pipeline.component_graph
                 )
 
 
 def test_get_estimators():
-    assert len(get_estimators(problem_type=ProblemTypes.BINARY)) == 8
+    assert len(get_estimators(problem_type=ProblemTypes.BINARY)) == 6
     assert (
         len(
             get_estimators(
                 problem_type=ProblemTypes.BINARY,
                 model_families=[ModelFamily.LINEAR_MODEL],
             ),
         )
         == 2
     )
-    assert len(get_estimators(problem_type=ProblemTypes.MULTICLASS)) == 8
-    assert len(get_estimators(problem_type=ProblemTypes.REGRESSION)) == 7
+    assert len(get_estimators(problem_type=ProblemTypes.MULTICLASS)) == 6
+    assert len(get_estimators(problem_type=ProblemTypes.REGRESSION)) == 5
 
     assert len(get_estimators(problem_type=ProblemTypes.BINARY, model_families=[])) == 0
     assert (
         len(get_estimators(problem_type=ProblemTypes.MULTICLASS, model_families=[]))
         == 0
     )
     assert (
```

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/test_pipelines.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/test_pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,14 @@
 
 
 def test_allowed_model_families():
     families = [
         ModelFamily.RANDOM_FOREST,
         ModelFamily.LINEAR_MODEL,
         ModelFamily.EXTRA_TREES,
-        ModelFamily.DECISION_TREE,
-        ModelFamily.CATBOOST,
         ModelFamily.XGBOOST,
         ModelFamily.LIGHTGBM,
     ]
     expected_model_families_binary = set(families)
     expected_model_families_regression = set(families)
     assert (
         set(allowed_model_families(ProblemTypes.BINARY))
@@ -111,31 +109,34 @@
     )
 
 
 def test_all_estimators(
     is_using_conda,
 ):
     if is_using_conda:
-        n_estimators = 17
+        n_estimators = 13
     else:
-        n_estimators = 18
+        n_estimators = 14
     assert len(_all_estimators_used_in_search()) == n_estimators
 
 
 def test_required_fields():
     class TestPipelineWithoutComponentGraph(PipelineBase):
         pass
 
     with pytest.raises(TypeError):
         TestPipelineWithoutComponentGraph(parameters={})
 
 
 @pytest.mark.parametrize("filetype", ["str", "BytesIO"])
 def test_serialization(
-    X_y_binary, tmpdir, logistic_regression_binary_pipeline, filetype
+    X_y_binary,
+    tmpdir,
+    logistic_regression_binary_pipeline,
+    filetype,
 ):
     X, y = X_y_binary
     path = os.path.join(str(tmpdir), "pipe.pkl")
     pipeline = logistic_regression_binary_pipeline
     pipeline.fit(X, y)
 
     pipeline.save(path)
```

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py` & `evalml-0.78.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/preprocessing_tests/test_no_split.py` & `evalml-0.78.0/evalml/tests/preprocessing_tests/test_no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/preprocessing_tests/test_sk_splitters.py` & `evalml-0.78.0/evalml/tests/preprocessing_tests/test_sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/preprocessing_tests/test_split_data.py` & `evalml-0.78.0/evalml/tests/preprocessing_tests/test_split_data.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/preprocessing_tests/test_training_validation_split.py` & `evalml-0.78.0/evalml/tests/preprocessing_tests/test_training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/problem_type_tests/test_problem_types.py` & `evalml-0.78.0/evalml/tests/problem_type_tests/test_problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/test_all_test_dirs_included.py` & `evalml-0.78.0/evalml/tests/test_all_test_dirs_included.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/tuner_tests/test_grid_search_tuner.py` & `evalml-0.78.0/evalml/tests/tuner_tests/test_grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/tuner_tests/test_random_search_tuner.py` & `evalml-0.78.0/evalml/tests/tuner_tests/test_random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/tuner_tests/test_skopt_tuner.py` & `evalml-0.78.0/evalml/tests/tuner_tests/test_skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/utils_tests/test_cli_utils.py` & `evalml-0.78.0/evalml/tests/utils_tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/utils_tests/test_gen_utils.py` & `evalml-0.78.0/evalml/tests/utils_tests/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/utils_tests/test_logger.py` & `evalml-0.78.0/evalml/tests/utils_tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     mock_time.return_value = time_passed
     time = time_elapsed(start_time=0)
     assert time == answer
 
 
 @pytest.mark.parametrize(
     "type_, allowed_families, number_, number_min_dep",
-    [("binary", None, 8, 5), ("multiclass", 2, 2, 2), ("regression", 3, 3, 3)],
+    [("binary", None, 6, 5), ("multiclass", 1, 1, 2), ("regression", 2, 2, 3)],
 )
 @pytest.mark.parametrize("verbose", [True, False])
 def test_pipeline_count(
     type_,
     allowed_families,
     number_,
     number_min_dep,
@@ -123,30 +123,29 @@
             X_train=X,
             y_train=y,
             problem_type=type_,
             verbose=verbose,
             automl_algorithm="iterative",
         )
     else:
-        if allowed_families == 2:
+        if allowed_families == 1:
             _ = AutoMLSearch(
                 X_train=X,
                 y_train=y,
                 problem_type=type_,
-                allowed_model_families=["random_forest", "decision_tree"],
+                allowed_model_families=["random_forest"],
                 verbose=verbose,
                 automl_algorithm="iterative",
             )
-        elif allowed_families == 3:
+        elif allowed_families == 2:
             _ = AutoMLSearch(
                 X_train=X,
                 y_train=y,
                 problem_type=type_,
                 allowed_model_families=[
                     "random_forest",
-                    "decision_tree",
                     "extra_trees",
                 ],
                 verbose=verbose,
                 automl_algorithm="iterative",
             )
     assert (f"{number_} pipelines ready for search" in caplog.text) == verbose
```

### Comparing `evalml-0.77.0/evalml/tests/utils_tests/test_nullable_type_utils.py` & `evalml-0.78.0/evalml/tests/utils_tests/test_nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tests/utils_tests/test_woodwork_utils.py` & `evalml-0.78.0/evalml/tests/utils_tests/test_woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tuners/grid_search_tuner.py` & `evalml-0.78.0/evalml/tuners/grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tuners/random_search_tuner.py` & `evalml-0.78.0/evalml/tuners/random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tuners/skopt_tuner.py` & `evalml-0.78.0/evalml/tuners/skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/tuners/tuner.py` & `evalml-0.78.0/evalml/tuners/tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/utils/__init__.py` & `evalml-0.78.0/evalml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/utils/base_meta.py` & `evalml-0.78.0/evalml/utils/base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/utils/cli_utils.py` & `evalml-0.78.0/evalml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/utils/gen_utils.py` & `evalml-0.78.0/evalml/utils/gen_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,18 @@
     "KNeighborsClassifier",
     "SVMClassifier",
     "SVMRegressor",
     "LinearRegressor",
     "VowpalWabbitBinaryClassifier",
     "VowpalWabbitMulticlassClassifier",
     "VowpalWabbitRegressor",
+    "DecisionTreeClassifier",
+    "DecisionTreeRegressor",
+    "CatBoostRegressor",
+    "CatBoostClassifier",
 }
 
 
 def get_importable_subclasses(base_class, used_in_automl=True):
     """Get importable subclasses of a base class. Used to list all of our estimators, transformers, components and pipelines dynamically.
 
     Args:
```

### Comparing `evalml-0.77.0/evalml/utils/logger.py` & `evalml-0.78.0/evalml/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/utils/nullable_type_utils.py` & `evalml-0.78.0/evalml/utils/nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml/utils/woodwork_utils.py` & `evalml-0.78.0/evalml/utils/woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml.egg-info/PKG-INFO` & `evalml-0.78.0/evalml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.77.0
+Version: 0.78.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.77.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.78.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.77.0/evalml.egg-info/SOURCES.txt` & `evalml-0.78.0/evalml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.77.0/evalml.egg-info/requires.txt` & `evalml-0.78.0/evalml.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-numpy<=1.23.5,>=1.21.0
+numpy>=1.21.0
 pandas>=1.5.0
 scipy>=1.5.0
 scikit-learn>=1.2.2
 scikit-optimize>=0.9.0
 pyzmq>=20.0.0
 colorama>=0.4.4
 cloudpickle>=1.5.0
 click>=8.0.0
-shap>=0.40.0
+shap>=0.42.0
 statsmodels>=0.12.2
 texttable>=1.6.2
 woodwork[dask]>=0.22.0
 dask!=2022.10.1,>=2022.2.0
 distributed!=2022.10.1,>=2022.2.0
 featuretools[dask]>=1.16.0
 nlp-primitives>=2.9.0
@@ -21,15 +21,15 @@
 ipywidgets<8.0.5,>=7.5
 xgboost>=1.7.0
 catboost>=1.1.1
 lightgbm>=2.3.1
 matplotlib>=3.3.3
 seaborn>=0.11.1
 category-encoders<=2.5.1.post0,>=2.2.2
-imbalanced-learn>=0.9.1
+imbalanced-learn<0.11.0,>=0.9.1
 pmdarima>=1.8.5
 sktime==0.17.0
 lime>=0.2.0.1
 vowpalwabbit>=8.11.0
 tomli>=2.0.1
 packaging>=23.0
 black[jupyter]>=22.3.0
```

### Comparing `evalml-0.77.0/pyproject.toml` & `evalml-0.78.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 maintainers = [
     {name="Alteryx, Inc.", email="open_source_support@alteryx.com"}
 ]
 keywords = ["data science", "machine learning", "optimization", "automl"]
 license = {file = "LICENSE"}
 requires-python = ">=3.8,<4"
 dependencies = [
-    "numpy >= 1.21.0, <=1.23.5",
+    "numpy >= 1.21.0",
     "pandas >= 1.5.0",
     "scipy >= 1.5.0",
     "scikit-learn >= 1.2.2",
     "scikit-optimize >= 0.9.0",
     "pyzmq >= 20.0.0",
     "colorama >= 0.4.4",
     "cloudpickle >= 1.5.0",
     "click >= 8.0.0",
-    "shap >= 0.40.0",
+    "shap >= 0.42.0",
     "statsmodels >= 0.12.2",
     "texttable >= 1.6.2",
     "woodwork[dask] >= 0.22.0",
     "dask >= 2022.2.0, != 2022.10.1",
     "distributed >= 2022.2.0, != 2022.10.1",
     "featuretools[dask] >= 1.16.0",
     "nlp-primitives >= 2.9.0",
@@ -53,15 +53,15 @@
     "xgboost >= 1.7.0",
     "catboost >= 1.1.1",
     "lightgbm >= 2.3.1",
     "matplotlib >= 3.3.3",
     "graphviz >= 0.13; platform_system!='Windows'",
     "seaborn >= 0.11.1",
     "category-encoders >= 2.2.2, <= 2.5.1.post0",
-    "imbalanced-learn >= 0.9.1",
+    "imbalanced-learn >= 0.9.1, <0.11.0",
     "pmdarima >= 1.8.5",
     "sktime == 0.17.0",
     "lime >= 0.2.0.1",
     "vowpalwabbit >= 8.11.0",
     "tomli >= 2.0.1",
     "packaging >= 23.0",
     "black[jupyter] >= 22.3.0",
```

