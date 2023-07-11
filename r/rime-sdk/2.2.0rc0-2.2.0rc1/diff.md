# Comparing `tmp/rime_sdk-2.2.0rc0.tar.gz` & `tmp/rime_sdk-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.2.0rc0.tar", last modified: Sat Jun 24 14:31:16 2023, max compression
+gzip compressed data, was "rime_sdk-2.2.0rc1.tar", last modified: Tue Jul 11 18:23:24 2023, max compression
```

## Comparing `rime_sdk-2.2.0rc0.tar` & `rime_sdk-2.2.0rc1.tar`

### file list

```diff
@@ -1,506 +1,502 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.922375 rime_sdk-2.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-24 14:31:16.922375 rime_sdk-2.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.878376 rime_sdk-2.2.0rc0/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63573 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.878376 rime_sdk-2.2.0rc0/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.878376 rime_sdk-2.2.0rc0/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    63758 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27235 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.878376 rime_sdk-2.2.0rc0/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.882376 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.882376 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21540 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64388 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64667 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.922375 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    46721 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/tags_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-06-24 14:31:13.000000 rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:31:16.878376 rime_sdk-2.2.0rc0/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-24 14:31:16.000000 rime_sdk-2.2.0rc0/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-06-24 14:31:16.000000 rime_sdk-2.2.0rc0/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:31:16.000000 rime_sdk-2.2.0rc0/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 14:31:16.000000 rime_sdk-2.2.0rc0/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 14:31:16.000000 rime_sdk-2.2.0rc0/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:31:16.000000 rime_sdk-2.2.0rc0/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:31:16.922375 rime_sdk-2.2.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-24 14:30:36.000000 rime_sdk-2.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.556411 rime_sdk-2.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 18:23:24.556411 rime_sdk-2.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.464409 rime_sdk-2.2.0rc1/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63997 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.464409 rime_sdk-2.2.0rc1/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.468409 rime_sdk-2.2.0rc1/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71842 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27058 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.468409 rime_sdk-2.2.0rc1/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.468409 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    48372 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.472409 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72384 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46002 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.556411 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    46231 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-11 18:23:19.000000 rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:24.464409 rime_sdk-2.2.0rc1/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 18:23:24.000000 rime_sdk-2.2.0rc1/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33348 2023-07-11 18:23:24.000000 rime_sdk-2.2.0rc1/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:23:24.000000 rime_sdk-2.2.0rc1/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 18:23:24.000000 rime_sdk-2.2.0rc1/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 18:23:24.000000 rime_sdk-2.2.0rc1/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 18:23:24.000000 rime_sdk-2.2.0rc1/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:23:24.556411 rime_sdk-2.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-11 18:22:31.000000 rime_sdk-2.2.0rc1/setup.py
```

### Comparing `rime_sdk-2.2.0rc0/LICENSE` & `rime_sdk-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/PKG-INFO` & `rime_sdk-2.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.2.0rc0
+Version: 2.2.0rc1
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc0/README.md` & `rime_sdk-2.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/__init__.py` & `rime_sdk-2.2.0rc1/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/client.py` & `rime_sdk-2.2.0rc1/rime_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     RimeLimitStatusStatus,
     RimeListImagesRequest,
     RimeManagedImage,
     RimeManagedImageStatus,
     RimeModelTask,
     RimeParentRoleSubjectRolePair,
     RimeStartFileScanRequest,
+    RimeUUID,
     RoleWorkspaceBody,
     RuntimeinfoCustomImage,
     RuntimeinfoCustomImageType,
     RuntimeinfoRunTimeInfo,
     StresstestsProjectIdUuidBody,
 )
 from rime_sdk.swagger.swagger_client.rest import ApiException
@@ -73,17 +74,15 @@
     HTTPStatus.SERVICE_UNAVAILABLE,
     HTTPStatus.TOO_MANY_REQUESTS,
     HTTPStatus.GATEWAY_TIMEOUT,
 ]
 
 
 class Client:
-    """A Client object provides an interface to RIME's \
-        services for creating Projects, starting Stress Test Jobs,\
-        and querying the backend for current Stress Test Jobs.
+    """A Client object provides an interface to RIME's services for creating Projects, starting Stress Test Jobs, and querying the backend for current Stress Test Jobs.
 
     To initialize the Client, provide the address of your RIME instance.
 
 
     Args:
         domain: str
             The base domain/address of the RIME service.
@@ -457,16 +456,15 @@
     def create_managed_image(
         self,
         name: str,
         requirements: List[ManagedImagePipRequirement],
         package_requirements: Optional[List[ManagedImagePackageRequirement]] = None,
         python_version: Optional[str] = None,
     ) -> ImageBuilder:
-        """Create a new managed Docker image with the desired\
-        custom requirements to run RIME on.
+        """Create a new managed Docker image with the desired custom requirements to run RIME on.
 
         These managed Docker images are managed by the RIME cluster and
         automatically upgrade when the installed version of RIME upgrades.
         Note: Images take a few minutes to be built.
 
         This method returns an object that can be used to track the progress of the
         image building job. The new custom image is only available for use in a stress
@@ -636,21 +634,19 @@
         version_specifier: Optional[str] = None,
     ) -> ManagedImagePipRequirement:
         """Construct a PipRequirement object for use in ``create_managed_image()``."""
         if not isinstance(name, str) or (
             version_specifier is not None and not isinstance(version_specifier, str)
         ):
             raise ValueError(
-                (
-                    "Proper specification of a pip requirement has the name"
-                    "of the library as the first argument and the version specifier"
-                    "string as the second argument"
-                    '(e.g. `pip_requirement("tensorflow", "==0.15.0")` or'
-                    '`pip_requirement("xgboost")`)'
-                )
+                "Proper specification of a pip requirement has the name"
+                "of the library as the first argument and the version specifier"
+                "string as the second argument"
+                '(e.g. `pip_requirement("tensorflow", "==0.15.0")` or'
+                '`pip_requirement("xgboost")`)'
             )
         res = ManagedImagePipRequirement(name=name)
         if version_specifier is not None:
             res.version_specifier = version_specifier
         return res
 
     @staticmethod
@@ -665,21 +661,19 @@
                 version_specifier is not None and not isinstance(version_specifier, str)
             )
             or (
                 version_specifier is not None and not re.match(r"\d", version_specifier)
             )
         ):
             raise ValueError(
-                (
-                    "Proper specification of a package requirement has the name"
-                    "of the library as the first argument and optionally the version"
-                    "specifier string as the second argument"
-                    '(e.g. `os_requirement("texlive", "20200406")` or'
-                    '`os_requirement("texlive")`)'
-                )
+                "Proper specification of a package requirement has the name"
+                "of the library as the first argument and optionally the version"
+                "specifier string as the second argument"
+                '(e.g. `os_requirement("texlive", "20200406")` or'
+                '`os_requirement("texlive")`)'
             )
         res = ManagedImagePackageRequirement(
             name=name, package_type=ManagedImagePackageType.ROCKYLINUX
         )
         if version_specifier is not None:
             res.version_specifier = version_specifier
         return res
@@ -690,21 +684,19 @@
         fixed_version: Optional[str] = None,
     ) -> ListImagesRequestPipLibraryFilter:
         """Construct a PipLibraryFilter object for use in ``list_managed_images()``."""
         if not isinstance(name, str) or (
             fixed_version is not None and not isinstance(fixed_version, str)
         ):
             raise ValueError(
-                (
-                    "Proper specification of a pip library filter has the name"
-                    "of the library as the first argument and the semantic version"
-                    "string as the second argument"
-                    '(e.g. `pip_library_filter("tensorflow", "1.15.0")` or'
-                    '`pip_library_filter("xgboost")`)'
-                )
+                "Proper specification of a pip library filter has the name"
+                "of the library as the first argument and the semantic version"
+                "string as the second argument"
+                '(e.g. `pip_library_filter("tensorflow", "1.15.0")` or'
+                '`pip_library_filter("xgboost")`)'
             )
         res = ListImagesRequestPipLibraryFilter(name=name)
         if fixed_version is not None:
             res.version = fixed_version
         return res
 
     def list_managed_images(
@@ -875,15 +867,15 @@
     def _validate_config(self, test_run_config: Dict, project_id: str) -> None:
         """Validate the test run config."""
         # TODO(blaine): Add config validation service.
         if not isinstance(test_run_config, dict):
             raise ValueError("The configuration must be a dictionary")
         # TODO(VAL-316): do proper runtime validation of all of the types in the config
         if project_id and not self._project_exists(project_id):
-            raise ValueError("Project id {} does not exist".format(project_id))
+            raise ValueError(f"Project id {project_id} does not exist")
         if "model_id" in test_run_config:
             if isinstance(test_run_config["model_id"], str):
                 test_run_config["model_id"] = _get_uuid(test_run_config["model_id"])
         if "run_time_info" in test_run_config:
             if "agent_id" in test_run_config["run_time_info"]:
                 if isinstance(test_run_config["run_time_info"]["agent_id"], str):
                     test_run_config["run_time_info"]["agent_id"] = _get_uuid(
@@ -911,25 +903,32 @@
             test_run_config["test_suite_config"][
                 "individual_tests_config"
             ] = json.dumps(
                 test_run_config["test_suite_config"]["individual_tests_config"]
             )
 
     def start_stress_test(
-        self, test_run_config: dict, project_id: str, **exp_fields: Dict[str, object]
+        self,
+        test_run_config: dict,
+        project_id: str,
+        agent_id: Optional[str] = None,
+        **exp_fields: Dict[str, object],
     ) -> Job:
         """Start a Stress Testing run.
 
         Args:
             test_run_config: dict
                 Configuration for the test to be run, which specifies unique ids to
                 locate the model and datasets to be used for the test.
             project_id: str
                 Identifier for the Project where the resulting test run will be stored.
                 When not specified, stores the results in the default Project.
+            agent_id: Optional[str]
+                ID for the Agent where the Stress Test will be run.
+                Uses the default Agent for the workspace when not specified.
             exp_fields: Dict[str, object]
                 [BETA] Fields for experimental features.
 
         Returns:
             Job:
                 A Job that provides information about the model Stress Test job.
 
@@ -971,37 +970,44 @@
             )
             cv_api.config_validator_validate_test_config(
                 config_type="CONFIG_TYPE_TEST_RUN", body=validate_body
             )
             req = StresstestsProjectIdUuidBody(
                 test_run_config=test_run_config,
                 experimental_fields=exp_fields if exp_fields else None,
+                agent_id=RimeUUID(agent_id) if agent_id else None,
             )
             Client._throttler.throttle(
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_stress_test(
                 body=req,
                 project_id_uuid=project_id,
             ).job
         return Job(self._api_client, job.job_id)
 
     def _start_generative_stress_test(
-        self, test_run_config: dict, project_id: str
+        self,
+        test_run_config: dict,
+        project_id: str,
+        agent_id: Optional[str] = None,
     ) -> Job:
         """Start a Generative Stress Testing run.
 
         Args:
             test_run_config: dict
                 Configuration for the test to be run, which specifies unique ids to
                 locate the model and datasets to be used for the test.
             project_id: str
                 Identifier for the Project where the resulting test run will be stored.
                 When not specified, stores the results in the default Project.
+            agent_id: Optional[str]
+                ID for the Agent where the Generative Test will be run.
+                Uses the default Agent for the workspace when not specified.
 
         Returns:
             Job:
                 A Job that provides information about the model Stress Test job.
 
         Raises:
             ValueError
@@ -1041,14 +1047,15 @@
             #     config_json=json.dumps(test_run_config),
             # )
             # cv_api.config_validator_validate_test_config(
             #     config_type="CONFIG_TYPE_TEST_RUN", body=validate_body
             # )
             req = GenerativestresstestsProjectIdUuidBody(
                 test_run_config=test_run_config,
+                agent_id=RimeUUID(agent_id) if agent_id else None,
             )
             Client._throttler.throttle(
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_generative_stress_test(
                 body=req,
@@ -1496,14 +1503,15 @@
         if cpu_request_millicores is not None and cpu_request_millicores <= 0:
             raise ValueError(
                 "The requested number of millicores of CPU must be positive"
             )
         model_info = model_info_from_dict(model_file_info)
         req = RimeStartFileScanRequest(
             file_info=model_info,
+            agent_id=RimeUUID(agent_id) if agent_id else None,
         )
 
         req.run_time_info = RuntimeinfoRunTimeInfo()
         if cpu_request_millicores:
             req.run_time_info.resource_request.cpu_request_millicores = (
                 cpu_request_millicores
             )
@@ -1515,16 +1523,14 @@
             req.run_time_info.custom_image = RuntimeinfoCustomImageType(
                 custom_image=custom_image
             )
         if rime_managed_image:
             req.run_time_info.custom_image = RuntimeinfoCustomImageType(
                 managed_image_name=rime_managed_image
             )
-        if agent_id:
-            req.run_time_info.agent_id = agent_id
 
         Client._throttler.throttle(
             throttling_msg="Your request is throttled to limit # of file scans."
         )
         api = swagger_client.FileScanningApi(self._api_client)
         with RESTErrorHandler():
             response = api.file_scanning_start_file_scan(body=req)
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/data_collector.py` & `rime_sdk-2.2.0rc1/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.2.0rc1/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.2.0rc1/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.2.0rc1/rime_sdk/data_format_check/nlp_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,29 +133,15 @@
 
     if list_data is None or len(list_data) == 0:
         raise ValueError(
             f"No objects parsed from '{file_path}'. Please verify "
             "presence and format of input data and retry."
         )
 
-    # If schema is not provided, select or generate an appropriate one based
-    # on first data point and task/presence of predictions
-    if schema is None:
-        if input_type == PREDS:
-            schema = SCHEMA_BANK[task][PREDS]
-        elif input_type == INPUT_PREDS_SEPARATE:
-            schema = infer_schema_from_datapoint(
-                task, list_data[0], set(SCHEMA_BANK[task][PREDS].schema.keys())
-            )
-        elif input_type == INPUT_PREDS_INCLUDED:
-            schema = infer_schema_from_datapoint(task, list_data[0])
-        else:
-            raise ValueError(
-                ERROR_UNKNOWN_INPUT.format(input_type=input_type, accepted=INPUT_TYPES)
-            )
+    schema = get_schema(schema, task, input_type, list_data)
 
     print(f"\nInspecting '{file_path}':")
     for i in tqdm(range(0, len(list_data))):
         try:
             # TODO(RAT-1940): add manual non-null/non-empty check
             schema.validate(list_data[i])
         except SchemaError as e:
@@ -168,14 +154,40 @@
                 f"File '{file_path}', Index {i}:\n\n",
                 *e.args,
                 schema_msg,
             )
             raise
 
 
+def get_schema(
+    schema: Optional[Schema],
+    task: str,
+    input_type: Optional[str],
+    list_data: List[dict],
+) -> Schema:
+    """Infer the schema to use if schema is not provided."""
+    if schema is not None:
+        return schema
+
+    # If schema is not provided, select or generate an appropriate one based
+    # on first data point and task/presence of predictions
+    if input_type == PREDS:
+        return SCHEMA_BANK[task][PREDS]
+    elif input_type == INPUT_PREDS_SEPARATE:
+        return infer_schema_from_datapoint(
+            task, list_data[0], set(SCHEMA_BANK[task][PREDS].schema.keys())
+        )
+    elif input_type == INPUT_PREDS_INCLUDED:
+        return infer_schema_from_datapoint(task, list_data[0])
+    else:
+        raise ValueError(
+            ERROR_UNKNOWN_INPUT.format(input_type=input_type, accepted=INPUT_TYPES)
+        )
+
+
 def infer_schema_from_datapoint(
     task: str, datapoint: dict, excluded_keys: Optional[Iterable] = None
 ) -> Schema:
     """Generate a custom schema using the given task and datapoint.
 
     Start with the default schema (contains only required keys), and add keys as they
     are observed in the datapoint.
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.2.0rc1/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/detection_event.py` & `rime_sdk-2.2.0rc1/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/firewall.py` & `rime_sdk-2.2.0rc1/rime_sdk/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,16 +311,17 @@
     @property
     def project_id(self) -> str:
         """Return the ID of the parent project for this Firewall."""
         fw = self._get_firewall()
         return fw.project_id.uuid
 
     @prompt_confirmation("Are you sure you want to delete this Firewall? (y/n) ")
-    def delete_firewall(
-        self, force: Optional[bool] = False  # pylint: disable=unused-argument
+    def delete_firewall(  # pylint: disable=unused-argument
+        self,
+        force: Optional[bool] = False,  # noqa: ARG002 (unused-method-argument)
     ) -> None:
         """Delete Firewall.
 
         Args:
             force: Optional[bool] = False
                 When set to True, the Firewall will be deleted immediately. By default,
                 a confirmation is required.
@@ -483,14 +484,17 @@
                 Specifies whether to override existing bins.
             ram_request_megabytes: Optional[int]
                 Megabytes of RAM set as the Kubernetes pod limit for the Stress Test
                 Job. The default is 4000MB.
             cpu_request_millicores: Optional[int]
                 Millicores of CPU set as the Kubernetes pod limit for the Stress Test
                 Job. The default is 1500mi.
+            random_seed: Optional[int]
+                Random seed to use for the Job, so that Test Job result will be
+                deterministic.
             agent_id: Optional[str]
                 ID for the Agent where the Continuous Test will be run.
                 Uses the default Agent for the workspace when not specified.
             rime_managed_image: Optional[str]
                 Name of a Managed Image to use when running the model test.
                 The image must have all dependencies required by your model. To create
                 new Managed Images with your desired dependencies, use the client's
@@ -534,24 +538,24 @@
                 "The requested number of millicores of CPU must be positive"
             )
 
         req = ContinuoustestsFirewallIdUuidBody(
             test_run_incremental_config=TestrunTestRunIncrementalConfig(
                 eval_dataset_id=eval_data_id,
                 run_time_info=RuntimeinfoRunTimeInfo(
-                    agent_id=RimeUUID(agent_id) if agent_id else None,
                     resource_request=RuntimeinfoResourceRequest(
                         ram_request_megabytes=ram_request_megabytes,
                         cpu_request_millicores=cpu_request_millicores,
                     ),
                     random_seed=random_seed,
                 ),
             ),
             override_existing_bins=override_existing_bins,
             experimental_fields=exp_fields if exp_fields else None,
+            agent_id=RimeUUID(agent_id) if agent_id else None,
         )
         if custom_image:
             req.test_run_incremental_config.run_time_info.custom_image = (
                 RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
                     custom_image=custom_image
                 )
             )
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/image_builder.py` & `rime_sdk-2.2.0rc1/rime_sdk/image_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,30 +95,30 @@
         Returns:
             Dict:
                 A dictionary representing the Image's state.
         """
         # Create backend client stubs to use for the remainder of this session.
         image = RimeManagedImage(status=RimeManagedImageStatus.UNSPECIFIED)
         if verbose:
-            print("Querying for Managed Image '{}':".format(self._name))
+            print(f"Querying for Managed Image '{self._name}':")
         # Do not repeat if the job is finished or blocking is disabled.
         repeat = True
         poll_count = 0
         api = ImageRegistryApi(self._api_client)
-        while repeat and not image.status in (
+        while repeat and image.status not in (
             RimeManagedImageStatus.FAILED,
             RimeManagedImageStatus.OUTDATED,
             RimeManagedImageStatus.READY,
         ):
             with RESTErrorHandler():
                 image = api.image_registry_get_image(name=self._name).image
             if verbose:
                 status_name = image.status
                 print(
-                    "\rStatus: {}, Poll Count: {}".format(status_name, poll_count),
+                    f"\rStatus: {status_name}, Poll Count: {poll_count}",
                     end="",
                 )
             if wait_until_finish:
                 time.sleep(poll_rate_sec)
             else:
                 repeat = False
             poll_count += 1
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/config_parser.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/constants.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/decorators.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/file_upload.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/file_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Library providing a module for file services."""
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Iterator, List, Optional, Text
+from typing import Iterator, List, Optional
 
 import requests
 from requests.adapters import HTTPAdapter
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from rime_sdk.swagger.swagger_client import ApiClient, FileUploadApi
@@ -57,24 +57,24 @@
             str:
                 A reference to the uploaded file's location in the blob store. This
                 reference can be used to refer to that object when writing RIME configs.
 
         Raises:
             FileNotFoundError
                 When the path ``file_path`` does not exist.
-            IOError
+            OSError
                 When ``file_path`` is not a file.
             ValueError
                 When there was an error in obtaining a blobstore location from the
                 RIME backend or in uploading ``file_path`` to RIME's blob store.
         """
         if not file_path.exists():
             raise FileNotFoundError(f"path '{file_path}' does not exist")
         if not file_path.is_file():
-            raise IOError(f"path '{file_path}' is not a file")
+            raise OSError(f"path '{file_path}' is not a file")
 
         file_size = file_path.stat().st_size
 
         file_name = file_path.name
         if upload_path is not None:
             resp = self._file_upload_client.file_upload_get_dataset_file_upload_url(
                 file_name=file_name, upload_path=upload_path
@@ -115,33 +115,33 @@
             str:
                 A reference to the uploaded directory's location in the blob store. This
                 reference can be used to refer to that object when writing RIME configs.
 
         Raises:
             FileNotFoundError
                 When the directory ``dir_path`` does not exist.
-            IOError
+            OSError
                 When ``dir_path`` is not a directory or contains no files.
             ValueError
                 When there was an error in obtaining a blobstore location from the
                 RIME backend or in uploading ``dir_path`` to RIME's blob store.
         """
         if not dir_path.exists():
             raise FileNotFoundError(f"path '{dir_path}' does not exist")
         if not dir_path.is_dir():
-            raise IOError(f"path '{dir_path}' is not a directory")
+            raise OSError(f"path '{dir_path}' is not a directory")
         sub_paths = _get_files_to_upload(dir_path, upload_hidden)
-        rel_paths: List[Text] = []
+        rel_paths: List[str] = []
         total_size: int = 0
         for file_path in sub_paths:
             if file_path.is_file():
                 total_size += file_path.stat().st_size
                 rel_paths.append(str(file_path.relative_to(dir_path)))
         if len(rel_paths) == 0:
-            raise IOError(f"directory '{dir_path}' is empty")
+            raise OSError(f"directory '{dir_path}' is empty")
         if upload_path is not None:
             resp = self._file_upload_client.file_upload_get_model_directory_upload_urls(  # noqa: E501
                 directory_name=dir_path.name,
                 relative_file_paths=rel_paths,
                 upload_path=upload_path,
             )
         else:
@@ -184,15 +184,15 @@
                     # If the file is 0 bytes, using the TQDM io wrapper does not
                     # work, so we simply write an empty file directly.
                     http_response = session.put(url=upload_url, data="")
                     t.close()
                 else:
                     wrapped_file = CallbackIOWrapper(t.update, f, "read")
                     http_response = session.put(url=upload_url, data=wrapped_file)
-                if http_response.status_code != 200:
+                if http_response.status_code != requests.codes.ok:
                     raise ValueError(
                         f"upload of '{file_path}' failed with "
                         + f"{http_response.status_code}: {http_response.reason}"
                     )
 
     def _get_requests_session(self) -> requests.Session:
         """Create request session for submitting HTTPS requests with retries."""
@@ -209,12 +209,12 @@
                 + f"Input size given is {size / (10 ** 6)}MB"
             )
 
     def _upload_string(self, file_contents: str, upload_url: str) -> None:
         """Upload `file_contents` to the location at `upload_url` via a PUT request."""
         with self._get_requests_session() as session:
             http_response = session.put(url=upload_url, data=file_contents)
-            if http_response.status_code != 200:
+            if http_response.status_code != requests.codes.ok:
                 raise ValueError(
                     "upload of raw string file failed with "
                     + f"{http_response.status_code}: {http_response.reason}"
                 )
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Library for internal helpers on test objects."""
 from http import HTTPStatus
+from typing import Optional
 
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import ApiClient
 from rime_sdk.swagger.swagger_client.models import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.rest import ApiException
 
 
 def get_batch_result_response(
-    test_run_id: str, test_type: str, api_client: ApiClient = ApiClient()
+    test_run_id: str, test_type: str, api_client: Optional[ApiClient] = None
 ) -> TestrunresultGetBatchResultResponse:
     """Obtain the test batch summary response."""
     api = swagger_client.ResultsReaderApi(api_client)
     try:
         res: TestrunresultGetBatchResultResponse = api.results_reader_get_batch_result(
             test_run_id=test_run_id, test_type=test_type
         )
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/throttle_queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         # Compute the number of events in the current epoch above the desired number.
         events_in_epoch = sum(
             [now - x < self._epoch_duration_sec for x in self._timestamp_queue]
         )
         excess_events = events_in_epoch - self._desired_events_per_epoch
         throttled = excess_events >= 0
         if throttled:
-            logger.warning("Throttling: {}".format(throttling_msg))
+            logger.warning(f"Throttling: {throttling_msg}")
 
         # Add an exponential sleep penalty to throttle the events toward the desired
         # interval.
         # Note: small amounts of throttling occur while excess_events < 0. The total
         # contribution of this delay is
         #    T = DI * sum_{t=1}{N} 2^-t
         #      < DI * sum_{t=1}{inf} 2^-t
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/internal/utils.py` & `rime_sdk-2.2.0rc1/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/job.py` & `rime_sdk-2.2.0rc1/rime_sdk/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,21 +94,22 @@
 
     @staticmethod
     def _get_test_run_progress(test_run: RimeTestRunProgress) -> Optional[str]:
         test_batches = test_run.test_batches
         if len(test_batches) == 0:
             return None
         n = sum(batch.status == RimeTestTaskStatus.COMPLETED for batch in test_batches)
-        return "{:<2} / {:>2} tests completed".format(n, len(test_batches))
+        return f"{n:<2} / {len(test_batches):>2} tests completed"
 
     @abstractmethod
     def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
         """Pretty print the progress of the test run."""
 
-    def get_status(
+    # TODO(VAL-2282): refactor this function to have fewer branches and be more readable
+    def get_status(  # noqa: PLR0912 (too-many-branches)
         self,
         verbose: bool = True,
         wait_until_finish: bool = False,
         poll_rate_sec: float = 5.0,
     ) -> Dict:
         """Return the current status of the Job.
 
@@ -186,15 +187,15 @@
                 ):
                     print("Cancellation Requested")
                     # Only print "Cancellation Requested" once.
                     printed_cancellation_req = True
 
                 minute, second = divmod(job.running_time_secs, 60)
                 hour, minute = divmod(minute, 60)
-                progress_str = " ({})".format(progress) if progress else ""
+                progress_str = f" ({progress})" if progress else ""
                 print(
                     "\rStatus: {}, Running Time: {:02}:{:02}:{:05.2f}{}".format(
                         job.status, int(hour), int(minute), second, progress_str
                     ),
                     end="",
                 )
                 printed_poll_string = True
@@ -256,18 +257,16 @@
         """Request to cancel the Job.
 
         The RIME cluster will mark the Job with "Cancellation Requested" and then clean
         up the Job.
         """
         if self.job_type not in cancellable_job_types:
             raise ValueError(
-                (
-                    f"Cancelling jobs is only supported for "
-                    f"job types {cancellable_job_types}"
-                )
+                "Cancelling jobs is only supported for job types "
+                f"{cancellable_job_types}"
             )
         api = swagger_client.JobReaderApi(self._api_client)
         with RESTErrorHandler():
             api.job_reader_cancel_job(job_id=self.job_id)
 
     def get_agent_id(self) -> str:
         """Return the Agent ID running the Job."""
@@ -446,22 +445,26 @@
 
 
 class ImageBuilderJob(BaseJob):
     """This object provides an interface for monitoring a Image Builder Job in the RIME backend."""
 
     _job_type = RimeJobType.IMAGE_BUILDER
 
-    def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
+    def _get_progress(
+        self, job: RimeJobMetadata  # noqa: ARG002 (unused-method-argument)
+    ) -> Optional[str]:
         """Pretty print the progress of the test run."""
         # TODO: find a good way to pretty print the progress of a ImageBuilderJob
         return None
 
 
 class FileScanJob(BaseJob):
     """This object provides an interface for monitoring a File Scan Job in the RIME backend."""
 
     _job_type = RimeJobType.FILE_SCAN
 
-    def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
+    def _get_progress(
+        self, job: RimeJobMetadata  # noqa: ARG002 (unused-method-argument)
+    ) -> Optional[str]:
         """Pretty print the progress of the test run."""
         # TODO: find a good way to pretty print the progress of a FileScanJob
         return None
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/monitor.py` & `rime_sdk-2.2.0rc1/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/project.py` & `rime_sdk-2.2.0rc1/rime_sdk/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Library defining the interface to a Project."""
 import json
+import os
 from datetime import timedelta
 from http import HTTPStatus
-from typing import Any, Dict, Iterator, List, NamedTuple, Optional
+from pathlib import Path
+from typing import Any, Dict, Iterator, List, NamedTuple, Optional, Union
 
 from google.protobuf.field_mask_pb2 import FieldMask
 from google.protobuf.json_format import MessageToDict
 
 from rime_sdk.data_collector import DataCollector
 from rime_sdk.firewall import Firewall
 from rime_sdk.internal.config_parser import (
     _get_individual_tests_config_swagger,
     convert_single_data_info_to_swagger,
     convert_single_pred_info_to_swagger,
 )
 from rime_sdk.internal.decorators import prompt_confirmation
+from rime_sdk.internal.file_upload import FileUploadModule
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.swagger_utils import parse_str_to_uuid, timedelta_to_rest
 from rime_sdk.internal.utils import (
     convert_dict_to_html,
     get_swagger_field_mask,
     make_link,
 )
@@ -762,16 +765,16 @@
             raise ValueError("Webhook must be a non empty string")
         webhook_config = NotificationWebhookConfig(webhook=webhook)
         return self._remove_notif_entry(
             notif_type_str=notif_type_str, email=None, webhook_config=webhook_config
         )
 
     @prompt_confirmation("Are you sure you want to delete this Project? (y/n) ")
-    def delete(
-        self, force: Optional[bool] = False  # pylint: disable=unused-argument
+    def delete(  # pylint: disable=unused-argument
+        self, force: Optional[bool] = False  # noqa: ARG002 (unused-method-argument)
     ) -> None:
         """Delete this Project.
 
         Args:
             force: Optional[bool] = False
                 When set to True, the Project will be deleted immediately. By default,
                 a confirmation is required.
@@ -881,19 +884,26 @@
         """Register and validate a new dataset in this Project.
 
         Args:
             name: str
                 The chosen name of the dataset.
             remote_path: str
                 The path to the dataset artifact.
-
+            data_params: dict
+                A dictionary that contains the data parameters.
+                The data parameters must match the API specification
+                of the `data_info.data_params` field in the `RegisterDataset` request.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
+            ct_info: Optional[dict] = None,
+                An optional dictionary that contains the CT info.
+                The CT info must match the API specification of the `ct_info`
+                field in the `RegisterDataset` request.
             skip_validation: Optional[bool] = False,
                 An optional boolean that indicates whether to skip validation.
                 Validation ensures that the dataset is valid for Robust
                 Intelligence's systems.
             agent_id: Optional[str] = None,
                 Agent for running validation. If omitted the workspace's default
                 agent will be used.
@@ -921,14 +931,90 @@
             tags=tags,
             metadata=metadata,
             ct_info=ct_info,
             skip_validation=skip_validation,
             agent_id=agent_id,
         )
 
+    def upload_and_register_dataset_from_file(
+        self,
+        name: str,
+        file_path: Union[Path, str],
+        upload_path: Optional[str] = None,
+        data_params: Optional[dict] = None,
+        tags: Optional[List[str]] = None,
+        metadata: Optional[dict] = None,
+        ct_info: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
+        agent_id: Optional[str] = None,
+    ) -> str:
+        """Upload, register and validate a new dataset in this Project.
+
+        The uploaded file is stored in the Robust Intelligence cluster in a blob store
+        using its file name.
+
+        Args:
+            name: str
+                The chosen name of the dataset.
+            file_path: Union[Path, str]
+                The local path to the dataset artifact, to be uploaded to Robust
+                Intelligence's blob store.
+            upload_path: Optional[str] = None,
+                Name of the directory in the blob store file system. If omitted,
+                a unique random string will be the directory.
+            data_params: dict
+                A dictionary that contains the data parameters.
+                The data parameters must match the API specification
+                of the `data_info.data_params` field in the `RegisterDataset` request.
+            tags: Optional[List[str]] = None,
+                An optional list of tags to associate with the dataset.
+            metadata: Optional[dict] = None,
+                An optional dictionary of metadata to associate with the dataset.
+            ct_info: Optional[dict] = None,
+                An optional dictionary that contains the CT info.
+                The CT info must match the API specification of the `ct_info`
+                field in the `RegisterDataset` request.
+            skip_validation: Optional[bool] = False,
+                An optional boolean that indicates whether to skip validation.
+                Validation ensures that the dataset is valid for Robust
+                Intelligence's systems.
+            agent_id: Optional[str] = None,
+                Agent for running validation. If omitted the workspace's default
+                agent will be used.
+
+        Returns:
+            str:
+                The ID of the newly registered dataset.
+
+        Raises:
+            ValueError
+                This error is generated when the request to the Registry
+                service fails.
+            DatasetValidationError
+                This error is generated when the dataset is invalid.
+        """
+
+        if upload_path is not None and upload_path == "":
+            raise ValueError("specified upload_path must not be an empty string")
+        if isinstance(file_path, str):
+            file_path = Path(file_path)
+        with RESTErrorHandler():
+            fum = FileUploadModule(self._api_client)
+            remote_path = fum.upload_dataset_file(file_path, upload_path)
+        return self.register_dataset_from_file(
+            name,
+            remote_path,
+            data_params=data_params,
+            tags=tags,
+            metadata=metadata,
+            ct_info=ct_info,
+            skip_validation=skip_validation,
+            agent_id=agent_id,
+        )
+
     def register_model(
         self,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
@@ -1052,15 +1138,15 @@
                 service fails.
             ModelValidationError
                 This error is generated when the model is invalid.
 
         Example:
             .. code-block:: python
 
-                model_id = project.register_model_path(
+                model_id = project.register_model_from_path(
                     name=MODEL_NAME,
                     remote_path=MODEL_PATH,
                 )
         """
         model_config = {"model_path": {"path": remote_path}}
         return self._registry.register_model(
             self.project_id,
@@ -1069,14 +1155,112 @@
             tags=tags,
             metadata=metadata,
             external_id=external_id,
             integration_id=integration_id,
             skip_validation=skip_validation,
             agent_id=agent_id,
         )
+
+    def upload_and_register_model_from_path(
+        self,
+        name: str,
+        file_path: Union[Path, str],
+        upload_model_dir: bool = False,
+        upload_hidden: bool = False,
+        upload_path: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        metadata: Optional[dict] = None,
+        external_id: Optional[str] = None,
+        integration_id: Optional[str] = None,
+        skip_validation: Optional[bool] = False,
+        agent_id: Optional[str] = None,
+    ) -> str:
+        """Upload, register and validate a new model in this Project.
+
+        The uploaded file is stored in the Robust Intelligence cluster in a blob store
+        using its file name.
+
+        Args:
+            name: str
+                The chosen name of the model.
+            file_path: Union[Path, str]
+                The local path to the model artifact, to be uploaded to Robust
+                Intelligence's blob store.
+            upload_model_dir: bool = False
+                Whether to upload the directory containing the model artifact, in
+                addition to the model artifact itself. Note that if set to True, this
+                method will upload *everything* in the model's containing directory, so
+                only place files required to run the model in the directory.
+            upload_hidden: bool = False
+                Whether or not to upload hidden files or subdirectories
+                (ie. those beginning with a '.') in dir_path.
+            upload_path: Optional[str] = None,
+                Name of the directory in the blob store file system. If omitted,
+                a unique random string will be the directory.
+            tags: Optional[List[str]] = None,
+                An optional list of tags to associate with the model.
+            metadata: Optional[dict] = None,
+                An optional dictionary of metadata to associate with the model.
+            external_id: Optional[str] = None,
+                An optional external ID that can be used to identify the model.
+            integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration for access.
+            skip_validation: Optional[bool] = False,
+                An optional boolean that indicates whether to skip validation.
+                Validation ensures that the model is valid for Robust
+                Intelligence's systems.
+            agent_id: Optional[str] = None,
+                Agent for running validation. If omitted the workspace's default
+                agent will be used.
+
+        Returns:
+            str:
+                The ID of the newly registered model.
+
+        Raises:
+            ValueError
+                This error is generated when the request to the Registry
+                service fails.
+            ModelValidationError
+                This error is generated when the model is invalid.
+
+        Example:
+            .. code-block:: python
+
+                model_id = project.upload_and_register_model_from_path(
+                    name=MODEL_NAME,
+                    file_path=MODEL_PATH,
+                )
+        """
+        if upload_path is not None and upload_path == "":
+            raise ValueError("specified upload_path must not be an empty string")
+        if isinstance(file_path, str):
+            file_path = Path(file_path)
+        with RESTErrorHandler():
+            fum = FileUploadModule(self._api_client)
+            if upload_model_dir:
+                remote_dir_path = fum.upload_model_directory(
+                    file_path.parent,
+                    upload_hidden=upload_hidden,
+                    upload_path=upload_path,
+                )
+                remote_path = os.path.join(remote_dir_path, file_path.name)
+            else:
+                remote_path = fum.upload_dataset_file(file_path, upload_path)
+        return self.register_model_from_path(
+            name,
+            remote_path,
+            tags=tags,
+            metadata=metadata,
+            external_id=external_id,
+            integration_id=integration_id,
+            skip_validation=skip_validation,
+            agent_id=agent_id,
+        )
 
     def register_predictions(
         self,
         dataset_id: str,
         model_id: str,
         pred_config: dict,
         integration_id: Optional[str] = None,
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/registry.py` & `rime_sdk-2.2.0rc1/rime_sdk/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         """
         data_info_swagger = convert_single_data_info_to_swagger(data_config)
         req = ProjectIdUuidDatasetBody(
             project_id=RimeUUID(uuid=project_id),
             name=name,
             data_info=data_info_swagger,
             skip_validation=skip_validation,
-            agent_id=get_agent_id_uuid(agent_id),
+            agent_id=RimeUUID(agent_id) if agent_id else None,
         )
 
         metadata_str: Optional[str] = None
         if metadata is not None:
             metadata_str = json.dumps(metadata)
         if tags is not None or metadata_str is not None:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
@@ -219,15 +219,15 @@
                     agent_id=AGENT_ID,
                 )
         """
         req = ProjectIdUuidModelBody(
             project_id=RimeUUID(uuid=project_id),
             name=name,
             skip_validation=skip_validation,
-            agent_id=get_agent_id_uuid(agent_id),
+            agent_id=RimeUUID(agent_id) if agent_id else None,
         )
 
         if model_config is not None:
             # When the `model_path` key is provided to the dictionary, the value
             # must be a dictionary whose `path` value points to a python
             # file that holds a `predict_dict` or `predict_df` function.
             # When the `model_loading` key is provided to the dictionary, the value
@@ -337,15 +337,15 @@
         pred_info_swagger = convert_single_pred_info_to_swagger(pred_config)
 
         req = DatasetIdPredictionBody(
             project_id=RimeUUID(uuid=project_id),
             model_id=RimeUUID(uuid=model_id),
             pred_info=pred_info_swagger,
             skip_validation=skip_validation,
-            agent_id=get_agent_id_uuid(agent_id),
+            agent_id=RimeUUID(agent_id) if agent_id else None,
         )
 
         metadata_str: Optional[str] = None
         if metadata is not None:
             metadata_str = json.dumps(metadata)
         if tags is not None or metadata_str is not None:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
@@ -697,14 +697,7 @@
                 service fails.
         """
         api = swagger_client.RegistryServiceApi(self._api_client)
         with RESTErrorHandler():
             api.registry_service_delete_prediction_set(
                 dataset_id=dataset_id, model_id_uuid=model_id
             )
-
-
-def get_agent_id_uuid(agent_id: Optional[str]) -> Optional[RimeUUID]:
-    """Create UUID from agent ID parameter."""
-    if agent_id is None or len(agent_id) == 0:
-        return None
-    return RimeUUID(agent_id)
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 from rime_sdk.swagger.swagger_client.models.notification_job_action_config import NotificationJobActionConfig
 from rime_sdk.swagger.swagger_client.models.notification_monitoring_config import NotificationMonitoringConfig
 from rime_sdk.swagger.swagger_client.models.notification_notification import NotificationNotification
 from rime_sdk.swagger.swagger_client.models.notification_notification_type import NotificationNotificationType
 from rime_sdk.swagger.swagger_client.models.notification_object_type import NotificationObjectType
 from rime_sdk.swagger.swagger_client.models.notification_webhook_config import NotificationWebhookConfig
 from rime_sdk.swagger.swagger_client.models.notifsettings_notification_id_uuid_body import NotifsettingsNotificationIdUuidBody
-from rime_sdk.swagger.swagger_client.models.object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_ import ObjectContainingTheUpdatesOnlyTheFieldsSpecifiedInTheMaskWillBeUsedByTheBackendNoteTheIDFieldIsNecessaryToFindTheGivenNotificationSetting_
 from rime_sdk.swagger.swagger_client.models.predictions_model_id_uuid_body import PredictionsModelIdUuidBody
 from rime_sdk.swagger.swagger_client.models.project_add_users_to_project_response import ProjectAddUsersToProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_create_project_request import ProjectCreateProjectRequest
 from rime_sdk.swagger.swagger_client.models.project_create_project_response import ProjectCreateProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_delete_project_response import ProjectDeleteProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_get_project_response import ProjectGetProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_get_project_url_response import ProjectGetProjectURLResponse
@@ -223,27 +222,25 @@
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_response import RimeCreateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_request import RimeCreateNotificationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_response import RimeCreateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_user_request import RimeCreateUserRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_user_response import RimeCreateUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_request import RimeCreateWorkspaceRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_response import RimeCreateWorkspaceResponse
-from rime_sdk.swagger.swagger_client.models.rime_create_workspace_tag_response import RimeCreateWorkspaceTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_deactivate_agent_response import RimeDeactivateAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_agent_response import RimeDeleteAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_custom_monitor_response import RimeDeleteCustomMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_dataset_response import RimeDeleteDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_firewall_response import RimeDeleteFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_image_response import RimeDeleteImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_integration_response import RimeDeleteIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_model_card_response import RimeDeleteModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_model_response import RimeDeleteModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_prediction_set_response import RimeDeletePredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_uploaded_file_url_response import RimeDeleteUploadedFileURLResponse
-from rime_sdk.swagger.swagger_client.models.rime_delete_workspace_tag_response import RimeDeleteWorkspaceTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_ensure_image_existence_response import RimeEnsureImageExistenceResponse
 from rime_sdk.swagger.swagger_client.models.rime_failing_row import RimeFailingRow
 from rime_sdk.swagger.swagger_client.models.rime_failing_rows_result import RimeFailingRowsResult
 from rime_sdk.swagger.swagger_client.models.rime_feature_flags import RimeFeatureFlags
 from rime_sdk.swagger.swagger_client.models.rime_feature_type import RimeFeatureType
 from rime_sdk.swagger.swagger_client.models.rime_float_list import RimeFloatList
 from rime_sdk.swagger.swagger_client.models.rime_get_agent_response import RimeGetAgentResponse
@@ -309,15 +306,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_prediction_sets_response import RimeListPredictionSetsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_project_tags_in_workspace_response import RimeListProjectTagsInWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_uploaded_file_urls_response import RimeListUploadedFileURLsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_of_workspace_response import RimeListUsersOfWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_request_query import RimeListUsersRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_users_response import RimeListUsersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspace_integrations_response import RimeListWorkspaceIntegrationsResponse
-from rime_sdk.swagger.swagger_client.models.rime_list_workspace_tags_response import RimeListWorkspaceTagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspaces_request_query import RimeListWorkspacesRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_workspaces_response import RimeListWorkspacesResponse
 from rime_sdk.swagger.swagger_client.models.rime_long_description_tab import RimeLongDescriptionTab
 from rime_sdk.swagger.swagger_client.models.rime_managed_image import RimeManagedImage
 from rime_sdk.swagger.swagger_client.models.rime_managed_image_status import RimeManagedImageStatus
 from rime_sdk.swagger.swagger_client.models.rime_model_card import RimeModelCard
 from rime_sdk.swagger.swagger_client.models.rime_model_task import RimeModelTask
@@ -359,15 +355,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_str_list import RimeStrList
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
 from rime_sdk.swagger.swagger_client.models.rime_suggestion import RimeSuggestion
 from rime_sdk.swagger.swagger_client.models.rime_sync_image_tag_response import RimeSyncImageTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_table_column import RimeTableColumn
 from rime_sdk.swagger.swagger_client.models.rime_table_column_type import RimeTableColumnType
-from rime_sdk.swagger.swagger_client.models.rime_tag import RimeTag
 from rime_sdk.swagger.swagger_client.models.rime_test_case_monitor_info import RimeTestCaseMonitorInfo
 from rime_sdk.swagger.swagger_client.models.rime_test_case_status import RimeTestCaseStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_metric import RimeTestMetric
 from rime_sdk.swagger.swagger_client.models.rime_test_metric_category import RimeTestMetricCategory
 from rime_sdk.swagger.swagger_client.models.rime_test_run_progress import RimeTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_test_task_status import RimeTestTaskStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_type import RimeTestType
@@ -380,15 +375,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_update_integration_response import RimeUpdateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_model_card_response import RimeUpdateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_monitor_response import RimeUpdateMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_notification_response import RimeUpdateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_user_of_workspace_response import RimeUpdateUserOfWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_user_response import RimeUpdateUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_workspace_response import RimeUpdateWorkspaceResponse
-from rime_sdk.swagger.swagger_client.models.rime_update_workspace_tag_response import RimeUpdateWorkspaceTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_upsert_feature_flags_response import RimeUpsertFeatureFlagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_user_detail_with_role import RimeUserDetailWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_role import RimeUserRole
 from rime_sdk.swagger.swagger_client.models.rime_user_with_role import RimeUserWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_write_mask import RimeUserWriteMask
 from rime_sdk.swagger.swagger_client.models.rime_validate_test_config_response import RimeValidateTestConfigResponse
 from rime_sdk.swagger.swagger_client.models.rime_workspace import RimeWorkspace
@@ -410,15 +404,14 @@
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.stresstests_project_id_uuid_body import StresstestsProjectIdUuidBody
-from rime_sdk.swagger.swagger_client.models.tags_name_body import TagsNameBody
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_category_summary_metric import TestRunMetricsCategorySummaryMetric
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_model_perf_metric import TestRunMetricsModelPerfMetric
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
 from rime_sdk.swagger.swagger_client.models.testrun_data_profiling import TestrunDataProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_generative_test_run_config import TestrunGenerativeTestRunConfig
@@ -428,44 +421,47 @@
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
+from rime_sdk.swagger.swagger_client.models.testrunresult_get_monitor_categories_response import TestrunresultGetMonitorCategoriesResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_test_config_response import TestrunresultGetTestConfigResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_test_run_response import TestrunresultGetTestRunResponse
+from rime_sdk.swagger.swagger_client.models.testrunresult_get_validation_categories_response import TestrunresultGetValidationCategoriesResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_batch_results_response import TestrunresultListBatchResultsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_feature_results_response import TestrunresultListFeatureResultsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_summary_tests_response import TestrunresultListSummaryTestsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_test_cases_response import TestrunresultListTestCasesResponse
+from rime_sdk.swagger.swagger_client.models.testrunresult_list_test_runs_request_query import TestrunresultListTestRunsRequestQuery
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_test_runs_response import TestrunresultListTestRunsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_rename_test_run_response import TestrunresultRenameTestRunResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_result_summary_counts import TestrunresultResultSummaryCounts
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_batch_result import TestrunresultTestBatchResult
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_batch_result_display import TestrunresultTestBatchResultDisplay
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_case import TestrunresultTestCase
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_case_display import TestrunresultTestCaseDisplay
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_feature_result import TestrunresultTestFeatureResult
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_feature_result_display import TestrunresultTestFeatureResultDisplay
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_run_detail import TestrunresultTestRunDetail
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_run_metrics import TestrunresultTestRunMetrics
-from rime_sdk.swagger.swagger_client.models.the_updates_to_the_monitor_ import TheUpdatesToTheMonitor_
 from rime_sdk.swagger.swagger_client.models.user_favorite_projects import UserFavoriteProjects
 from rime_sdk.swagger.swagger_client.models.user_private_info import UserPrivateInfo
 from rime_sdk.swagger.swagger_client.models.user_role import UserRole
 from rime_sdk.swagger.swagger_client.models.user_user_detail import UserUserDetail
 from rime_sdk.swagger.swagger_client.models.users_user_id_uuid_body import UsersUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body import UsersUserUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body1 import UsersUserUserIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.v1betaintegrationsintegration_id_uuid_integration import V1betaintegrationsintegrationIdUuidIntegration
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
+from rime_sdk.swagger.swagger_client.models.v1betamonitorsmonitor_id_uuid_monitor import V1betamonitorsmonitorIdUuidMonitor
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
+from rime_sdk.swagger.swagger_client.models.v1notifsettingsnotification_id_uuid_notification import V1notifsettingsnotificationIdUuidNotification
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
-from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_tags_body import WorkspaceIdUuidTagsBody
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def firewall_service_create_firewall(self, body, **kwargs):  # noqa: E501
         """CreateFirewall  # noqa: E501
 
-        Creates a firewall with the required fields.  # noqa: E501
+        Creates a firewall with the required fields. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_create_firewall(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RimeCreateFirewallRequest body: (required)
@@ -53,15 +53,15 @@
         else:
             (data) = self.firewall_service_create_firewall_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
     def firewall_service_create_firewall_with_http_info(self, body, **kwargs):  # noqa: E501
         """CreateFirewall  # noqa: E501
 
-        Creates a firewall with the required fields.  # noqa: E501
+        Creates a firewall with the required fields. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_create_firewall_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RimeCreateFirewallRequest body: (required)
@@ -130,15 +130,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def firewall_service_delete_firewall(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """DeleteFirewall  # noqa: E501
 
-        Deletes the firewall with the specified ID.  # noqa: E501
+        Deletes the firewall with the specified ID. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_delete_firewall(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -152,15 +152,15 @@
         else:
             (data) = self.firewall_service_delete_firewall_with_http_info(firewall_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def firewall_service_delete_firewall_with_http_info(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """DeleteFirewall  # noqa: E501
 
-        Deletes the firewall with the specified ID.  # noqa: E501
+        Deletes the firewall with the specified ID. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_delete_firewall_with_http_info(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -225,15 +225,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def firewall_service_get_firewall(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """GetFirewall  # noqa: E501
 
-        Gets the firewall that matches the specified ID.  # noqa: E501
+        Gets the firewall that matches the specified ID. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_get_firewall(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -247,15 +247,15 @@
         else:
             (data) = self.firewall_service_get_firewall_with_http_info(firewall_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def firewall_service_get_firewall_with_http_info(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """GetFirewall  # noqa: E501
 
-        Gets the firewall that matches the specified ID.  # noqa: E501
+        Gets the firewall that matches the specified ID. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_get_firewall_with_http_info(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -320,15 +320,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def firewall_service_get_url(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """GetURL  # noqa: E501
 
-        Returns the URL for the specified Firewall in the Robust Intelligence web application.  # noqa: E501
+        Returns the URL for the specified Firewall in the Robust Intelligence web application. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_get_url(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -342,15 +342,15 @@
         else:
             (data) = self.firewall_service_get_url_with_http_info(firewall_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def firewall_service_get_url_with_http_info(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """GetURL  # noqa: E501
 
-        Returns the URL for the specified Firewall in the Robust Intelligence web application.  # noqa: E501
+        Returns the URL for the specified Firewall in the Robust Intelligence web application. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_get_url_with_http_info(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -415,15 +415,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def firewall_service_update_firewall(self, body, firewall_firewall_id_uuid, **kwargs):  # noqa: E501
         """UpdateFirewall  # noqa: E501
 
-        Updates a firewall's editable fields.  # noqa: E501
+        Updates a firewall's editable fields. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_update_firewall(body, firewall_firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param FirewallFirewallFirewallIdUuidBody body: (required)
@@ -438,15 +438,15 @@
         else:
             (data) = self.firewall_service_update_firewall_with_http_info(body, firewall_firewall_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def firewall_service_update_firewall_with_http_info(self, body, firewall_firewall_id_uuid, **kwargs):  # noqa: E501
         """UpdateFirewall  # noqa: E501
 
-        Updates a firewall's editable fields.  # noqa: E501
+        Updates a firewall's editable fields. This service is deprecated in Robust Intelligence v2.2 and will not be supported from v2.4.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_update_firewall_with_http_info(body, firewall_firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param FirewallFirewallFirewallIdUuidBody body: (required)
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,14 +337,101 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def results_reader_get_monitor_categories(self, **kwargs):  # noqa: E501
+        """GetMonitorCategories  # noqa: E501
+
+        Returns test categories belongs to monitor.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.results_reader_get_monitor_categories(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :return: TestrunresultGetMonitorCategoriesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.results_reader_get_monitor_categories_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.results_reader_get_monitor_categories_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def results_reader_get_monitor_categories_with_http_info(self, **kwargs):  # noqa: E501
+        """GetMonitorCategories  # noqa: E501
+
+        Returns test categories belongs to monitor.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.results_reader_get_monitor_categories_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :return: TestrunresultGetMonitorCategoriesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method results_reader_get_monitor_categories" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1-beta/test-runs/test-category/monitor', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TestrunresultGetMonitorCategoriesResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def results_reader_get_test_config(self, test_run_id, config_name, **kwargs):  # noqa: E501
         """GetTestConfig  # noqa: E501
 
         Returns the test configuration of the specified test run as bytes.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_get_test_config(test_run_id, config_name, async_req=True)
@@ -425,15 +512,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/test-runs/{testRunId}/test-config/{configName}', 'GET',
+            '/v1-beta/test-runs/{testRunId}/test-config/{configName}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='TestrunresultGetTestConfigResponse',  # noqa: E501
@@ -535,14 +622,101 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def results_reader_get_validation_categories(self, **kwargs):  # noqa: E501
+        """GetValidationCategories  # noqa: E501
+
+        Returns test categories belongs to validation.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.results_reader_get_validation_categories(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :return: TestrunresultGetValidationCategoriesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.results_reader_get_validation_categories_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.results_reader_get_validation_categories_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def results_reader_get_validation_categories_with_http_info(self, **kwargs):  # noqa: E501
+        """GetValidationCategories  # noqa: E501
+
+        Returns test categories belongs to validation.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.results_reader_get_validation_categories_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :return: TestrunresultGetValidationCategoriesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method results_reader_get_validation_categories" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1-beta/test-runs/test-category/validation', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TestrunresultGetValidationCategoriesResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def results_reader_list_batch_results(self, **kwargs):  # noqa: E501
         """ListBatchResults  # noqa: E501
 
         Returns a paginated list of batch results from a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_batch_results(async_req=True)
@@ -963,16 +1137,18 @@
         Lists all test runs belonging to a project.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_test_runs(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str project_id: The ID of the project containing the requested test runs. Specify exactly one of the page_token field or this field.
+        :param str project_id: The field is deprecated in v2.2. Use first_page_query.project_id instead. The field will be removed after v2.3. The ID of the project containing the requested test runs. Specify exactly one of the page_token field or this field.
         :param str page_token: A token representing one page from the list returned by a ListTestRuns query. The ListTestRuns query returns a page_token when there is more than one page of results. Specify exactly one of the projectId field or this field.
+        :param str first_page_query_project_id_uuid: Unique object ID.
+        :param str first_page_query_testing_type: The test type of Test Runs to request. Defaults to Stress Testing.   - TEST_TYPE_STRESS_TESTING_UNSPECIFIED: Default type as stress testing
         :param str page_size: The maximum number of Test Run objects to return in a single page.
         :return: TestrunresultListTestRunsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -987,23 +1163,25 @@
         Lists all test runs belonging to a project.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_test_runs_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str project_id: The ID of the project containing the requested test runs. Specify exactly one of the page_token field or this field.
+        :param str project_id: The field is deprecated in v2.2. Use first_page_query.project_id instead. The field will be removed after v2.3. The ID of the project containing the requested test runs. Specify exactly one of the page_token field or this field.
         :param str page_token: A token representing one page from the list returned by a ListTestRuns query. The ListTestRuns query returns a page_token when there is more than one page of results. Specify exactly one of the projectId field or this field.
+        :param str first_page_query_project_id_uuid: Unique object ID.
+        :param str first_page_query_testing_type: The test type of Test Runs to request. Defaults to Stress Testing.   - TEST_TYPE_STRESS_TESTING_UNSPECIFIED: Default type as stress testing
         :param str page_size: The maximum number of Test Run objects to return in a single page.
         :return: TestrunresultListTestRunsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['project_id', 'page_token', 'page_size']  # noqa: E501
+        all_params = ['project_id', 'page_token', 'first_page_query_project_id_uuid', 'first_page_query_testing_type', 'page_size']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1020,14 +1198,18 @@
         path_params = {}
 
         query_params = []
         if 'project_id' in params:
             query_params.append(('projectId', params['project_id']))  # noqa: E501
         if 'page_token' in params:
             query_params.append(('pageToken', params['page_token']))  # noqa: E501
+        if 'first_page_query_project_id_uuid' in params:
+            query_params.append(('firstPageQuery.projectId.uuid', params['first_page_query_project_id_uuid']))  # noqa: E501
+        if 'first_page_query_testing_type' in params:
+            query_params.append(('firstPageQuery.testingType', params['first_page_query_testing_type']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('pageSize', params['page_size']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -234,121 +234,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def workspace_service_create_workspace_tag(self, body, workspace_id_uuid, **kwargs):  # noqa: E501
-        """CreateWorkspaceTag  # noqa: E501
-
-        Creates a new tag within a Workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_create_workspace_tag(body, workspace_id_uuid, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param WorkspaceIdUuidTagsBody body: (required)
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :return: RimeCreateWorkspaceTagResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.workspace_service_create_workspace_tag_with_http_info(body, workspace_id_uuid, **kwargs)  # noqa: E501
-        else:
-            (data) = self.workspace_service_create_workspace_tag_with_http_info(body, workspace_id_uuid, **kwargs)  # noqa: E501
-            return data
-
-    def workspace_service_create_workspace_tag_with_http_info(self, body, workspace_id_uuid, **kwargs):  # noqa: E501
-        """CreateWorkspaceTag  # noqa: E501
-
-        Creates a new tag within a Workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_create_workspace_tag_with_http_info(body, workspace_id_uuid, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param WorkspaceIdUuidTagsBody body: (required)
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :return: RimeCreateWorkspaceTagResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['body', 'workspace_id_uuid']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method workspace_service_create_workspace_tag" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'body' is set
-        if ('body' not in params or
-                params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `workspace_service_create_workspace_tag`")  # noqa: E501
-        # verify the required parameter 'workspace_id_uuid' is set
-        if ('workspace_id_uuid' not in params or
-                params['workspace_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_create_workspace_tag`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'workspace_id_uuid' in params:
-            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'body' in params:
-            body_params = params['body']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1/workspace/{workspaceId.uuid}/tags', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='RimeCreateWorkspaceTagResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def workspace_service_delete_workspace(self, workspace_id_uuid, **kwargs):  # noqa: E501
         """DeleteWorkspace  # noqa: E501
 
         Deletes an existing Workspace by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_delete_workspace(workspace_id_uuid, async_req=True)
@@ -436,117 +329,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def workspace_service_delete_workspace_tag(self, workspace_id_uuid, name, **kwargs):  # noqa: E501
-        """DeleteWorkspaceTag  # noqa: E501
-
-        Deletes an existing tag within a Workspace by tag name.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_delete_workspace_tag(workspace_id_uuid, name, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :param str name: Name of the tag. (required)
-        :return: RimeDeleteWorkspaceTagResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.workspace_service_delete_workspace_tag_with_http_info(workspace_id_uuid, name, **kwargs)  # noqa: E501
-        else:
-            (data) = self.workspace_service_delete_workspace_tag_with_http_info(workspace_id_uuid, name, **kwargs)  # noqa: E501
-            return data
-
-    def workspace_service_delete_workspace_tag_with_http_info(self, workspace_id_uuid, name, **kwargs):  # noqa: E501
-        """DeleteWorkspaceTag  # noqa: E501
-
-        Deletes an existing tag within a Workspace by tag name.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_delete_workspace_tag_with_http_info(workspace_id_uuid, name, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :param str name: Name of the tag. (required)
-        :return: RimeDeleteWorkspaceTagResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['workspace_id_uuid', 'name']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method workspace_service_delete_workspace_tag" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'workspace_id_uuid' is set
-        if ('workspace_id_uuid' not in params or
-                params['workspace_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_delete_workspace_tag`")  # noqa: E501
-        # verify the required parameter 'name' is set
-        if ('name' not in params or
-                params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `workspace_service_delete_workspace_tag`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'workspace_id_uuid' in params:
-            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
-        if 'name' in params:
-            path_params['name'] = params['name']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1/workspace/{workspaceId.uuid}/tags/{name}', 'DELETE',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='RimeDeleteWorkspaceTagResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def workspace_service_get_workspace(self, workspace_id_uuid, **kwargs):  # noqa: E501
         """GetWorkspace  # noqa: E501
 
         Return a Workspace by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_get_workspace(workspace_id_uuid, async_req=True)
@@ -832,109 +622,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def workspace_service_list_workspace_tags(self, workspace_id_uuid, **kwargs):  # noqa: E501
-        """ListWorkspaceTags  # noqa: E501
-
-        Lists all tags created within a Workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_list_workspace_tags(workspace_id_uuid, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :return: RimeListWorkspaceTagsResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.workspace_service_list_workspace_tags_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
-        else:
-            (data) = self.workspace_service_list_workspace_tags_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
-            return data
-
-    def workspace_service_list_workspace_tags_with_http_info(self, workspace_id_uuid, **kwargs):  # noqa: E501
-        """ListWorkspaceTags  # noqa: E501
-
-        Lists all tags created within a Workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_list_workspace_tags_with_http_info(workspace_id_uuid, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :return: RimeListWorkspaceTagsResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['workspace_id_uuid']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method workspace_service_list_workspace_tags" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'workspace_id_uuid' is set
-        if ('workspace_id_uuid' not in params or
-                params['workspace_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_list_workspace_tags`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'workspace_id_uuid' in params:
-            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1/workspace/{workspaceId.uuid}/tags', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='RimeListWorkspaceTagsResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def workspace_service_list_workspaces(self, **kwargs):  # noqa: E501
         """ListWorkspaces  # noqa: E501
 
         List Workspaces with optional filter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_list_workspaces(async_req=True)
@@ -1346,122 +1041,7 @@
             response_type='RimeUpdateWorkspaceResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
-
-    def workspace_service_update_workspace_tag(self, body, workspace_id_uuid, name, **kwargs):  # noqa: E501
-        """UpdateWorkspaceTag  # noqa: E501
-
-        Updates an existing tag within a Workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_update_workspace_tag(body, workspace_id_uuid, name, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param TagsNameBody body: (required)
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :param str name: Name of the tag. (required)
-        :return: RimeUpdateWorkspaceTagResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.workspace_service_update_workspace_tag_with_http_info(body, workspace_id_uuid, name, **kwargs)  # noqa: E501
-        else:
-            (data) = self.workspace_service_update_workspace_tag_with_http_info(body, workspace_id_uuid, name, **kwargs)  # noqa: E501
-            return data
-
-    def workspace_service_update_workspace_tag_with_http_info(self, body, workspace_id_uuid, name, **kwargs):  # noqa: E501
-        """UpdateWorkspaceTag  # noqa: E501
-
-        Updates an existing tag within a Workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.workspace_service_update_workspace_tag_with_http_info(body, workspace_id_uuid, name, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param TagsNameBody body: (required)
-        :param str workspace_id_uuid: Unique object ID. (required)
-        :param str name: Name of the tag. (required)
-        :return: RimeUpdateWorkspaceTagResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['body', 'workspace_id_uuid', 'name']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method workspace_service_update_workspace_tag" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'body' is set
-        if ('body' not in params or
-                params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `workspace_service_update_workspace_tag`")  # noqa: E501
-        # verify the required parameter 'workspace_id_uuid' is set
-        if ('workspace_id_uuid' not in params or
-                params['workspace_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_update_workspace_tag`")  # noqa: E501
-        # verify the required parameter 'name' is set
-        if ('name' not in params or
-                params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `workspace_service_update_workspace_tag`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'workspace_id_uuid' in params:
-            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
-        if 'name' in params:
-            path_params['name'] = params['name']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'body' in params:
-            body_params = params['body']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1/workspace/{workspaceId.uuid}/tags/{name}', 'PUT',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='RimeUpdateWorkspaceTagResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 from rime_sdk.swagger.swagger_client.models.notification_job_action_config import NotificationJobActionConfig
 from rime_sdk.swagger.swagger_client.models.notification_monitoring_config import NotificationMonitoringConfig
 from rime_sdk.swagger.swagger_client.models.notification_notification import NotificationNotification
 from rime_sdk.swagger.swagger_client.models.notification_notification_type import NotificationNotificationType
 from rime_sdk.swagger.swagger_client.models.notification_object_type import NotificationObjectType
 from rime_sdk.swagger.swagger_client.models.notification_webhook_config import NotificationWebhookConfig
 from rime_sdk.swagger.swagger_client.models.notifsettings_notification_id_uuid_body import NotifsettingsNotificationIdUuidBody
-from rime_sdk.swagger.swagger_client.models.object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_ import ObjectContainingTheUpdatesOnlyTheFieldsSpecifiedInTheMaskWillBeUsedByTheBackendNoteTheIDFieldIsNecessaryToFindTheGivenNotificationSetting_
 from rime_sdk.swagger.swagger_client.models.predictions_model_id_uuid_body import PredictionsModelIdUuidBody
 from rime_sdk.swagger.swagger_client.models.project_add_users_to_project_response import ProjectAddUsersToProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_create_project_request import ProjectCreateProjectRequest
 from rime_sdk.swagger.swagger_client.models.project_create_project_response import ProjectCreateProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_delete_project_response import ProjectDeleteProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_get_project_response import ProjectGetProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_get_project_url_response import ProjectGetProjectURLResponse
@@ -195,27 +194,25 @@
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_response import RimeCreateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_request import RimeCreateNotificationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_response import RimeCreateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_user_request import RimeCreateUserRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_user_response import RimeCreateUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_request import RimeCreateWorkspaceRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_response import RimeCreateWorkspaceResponse
-from rime_sdk.swagger.swagger_client.models.rime_create_workspace_tag_response import RimeCreateWorkspaceTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_deactivate_agent_response import RimeDeactivateAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_agent_response import RimeDeleteAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_custom_monitor_response import RimeDeleteCustomMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_dataset_response import RimeDeleteDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_firewall_response import RimeDeleteFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_image_response import RimeDeleteImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_integration_response import RimeDeleteIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_model_card_response import RimeDeleteModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_model_response import RimeDeleteModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_prediction_set_response import RimeDeletePredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_delete_uploaded_file_url_response import RimeDeleteUploadedFileURLResponse
-from rime_sdk.swagger.swagger_client.models.rime_delete_workspace_tag_response import RimeDeleteWorkspaceTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_ensure_image_existence_response import RimeEnsureImageExistenceResponse
 from rime_sdk.swagger.swagger_client.models.rime_failing_row import RimeFailingRow
 from rime_sdk.swagger.swagger_client.models.rime_failing_rows_result import RimeFailingRowsResult
 from rime_sdk.swagger.swagger_client.models.rime_feature_flags import RimeFeatureFlags
 from rime_sdk.swagger.swagger_client.models.rime_feature_type import RimeFeatureType
 from rime_sdk.swagger.swagger_client.models.rime_float_list import RimeFloatList
 from rime_sdk.swagger.swagger_client.models.rime_get_agent_response import RimeGetAgentResponse
@@ -281,15 +278,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_prediction_sets_response import RimeListPredictionSetsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_project_tags_in_workspace_response import RimeListProjectTagsInWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_uploaded_file_urls_response import RimeListUploadedFileURLsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_of_workspace_response import RimeListUsersOfWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_request_query import RimeListUsersRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_users_response import RimeListUsersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspace_integrations_response import RimeListWorkspaceIntegrationsResponse
-from rime_sdk.swagger.swagger_client.models.rime_list_workspace_tags_response import RimeListWorkspaceTagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspaces_request_query import RimeListWorkspacesRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_workspaces_response import RimeListWorkspacesResponse
 from rime_sdk.swagger.swagger_client.models.rime_long_description_tab import RimeLongDescriptionTab
 from rime_sdk.swagger.swagger_client.models.rime_managed_image import RimeManagedImage
 from rime_sdk.swagger.swagger_client.models.rime_managed_image_status import RimeManagedImageStatus
 from rime_sdk.swagger.swagger_client.models.rime_model_card import RimeModelCard
 from rime_sdk.swagger.swagger_client.models.rime_model_task import RimeModelTask
@@ -331,15 +327,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_str_list import RimeStrList
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
 from rime_sdk.swagger.swagger_client.models.rime_suggestion import RimeSuggestion
 from rime_sdk.swagger.swagger_client.models.rime_sync_image_tag_response import RimeSyncImageTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_table_column import RimeTableColumn
 from rime_sdk.swagger.swagger_client.models.rime_table_column_type import RimeTableColumnType
-from rime_sdk.swagger.swagger_client.models.rime_tag import RimeTag
 from rime_sdk.swagger.swagger_client.models.rime_test_case_monitor_info import RimeTestCaseMonitorInfo
 from rime_sdk.swagger.swagger_client.models.rime_test_case_status import RimeTestCaseStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_metric import RimeTestMetric
 from rime_sdk.swagger.swagger_client.models.rime_test_metric_category import RimeTestMetricCategory
 from rime_sdk.swagger.swagger_client.models.rime_test_run_progress import RimeTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_test_task_status import RimeTestTaskStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_type import RimeTestType
@@ -352,15 +347,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_update_integration_response import RimeUpdateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_model_card_response import RimeUpdateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_monitor_response import RimeUpdateMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_notification_response import RimeUpdateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_user_of_workspace_response import RimeUpdateUserOfWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_user_response import RimeUpdateUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_workspace_response import RimeUpdateWorkspaceResponse
-from rime_sdk.swagger.swagger_client.models.rime_update_workspace_tag_response import RimeUpdateWorkspaceTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_upsert_feature_flags_response import RimeUpsertFeatureFlagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_user_detail_with_role import RimeUserDetailWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_role import RimeUserRole
 from rime_sdk.swagger.swagger_client.models.rime_user_with_role import RimeUserWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_write_mask import RimeUserWriteMask
 from rime_sdk.swagger.swagger_client.models.rime_validate_test_config_response import RimeValidateTestConfigResponse
 from rime_sdk.swagger.swagger_client.models.rime_workspace import RimeWorkspace
@@ -382,15 +376,14 @@
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.stresstests_project_id_uuid_body import StresstestsProjectIdUuidBody
-from rime_sdk.swagger.swagger_client.models.tags_name_body import TagsNameBody
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_category_summary_metric import TestRunMetricsCategorySummaryMetric
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_model_perf_metric import TestRunMetricsModelPerfMetric
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
 from rime_sdk.swagger.swagger_client.models.testrun_data_profiling import TestrunDataProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_generative_test_run_config import TestrunGenerativeTestRunConfig
@@ -400,44 +393,47 @@
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
+from rime_sdk.swagger.swagger_client.models.testrunresult_get_monitor_categories_response import TestrunresultGetMonitorCategoriesResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_test_config_response import TestrunresultGetTestConfigResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_test_run_response import TestrunresultGetTestRunResponse
+from rime_sdk.swagger.swagger_client.models.testrunresult_get_validation_categories_response import TestrunresultGetValidationCategoriesResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_batch_results_response import TestrunresultListBatchResultsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_feature_results_response import TestrunresultListFeatureResultsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_summary_tests_response import TestrunresultListSummaryTestsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_test_cases_response import TestrunresultListTestCasesResponse
+from rime_sdk.swagger.swagger_client.models.testrunresult_list_test_runs_request_query import TestrunresultListTestRunsRequestQuery
 from rime_sdk.swagger.swagger_client.models.testrunresult_list_test_runs_response import TestrunresultListTestRunsResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_rename_test_run_response import TestrunresultRenameTestRunResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_result_summary_counts import TestrunresultResultSummaryCounts
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_batch_result import TestrunresultTestBatchResult
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_batch_result_display import TestrunresultTestBatchResultDisplay
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_case import TestrunresultTestCase
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_case_display import TestrunresultTestCaseDisplay
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_feature_result import TestrunresultTestFeatureResult
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_feature_result_display import TestrunresultTestFeatureResultDisplay
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_run_detail import TestrunresultTestRunDetail
 from rime_sdk.swagger.swagger_client.models.testrunresult_test_run_metrics import TestrunresultTestRunMetrics
-from rime_sdk.swagger.swagger_client.models.the_updates_to_the_monitor_ import TheUpdatesToTheMonitor_
 from rime_sdk.swagger.swagger_client.models.user_favorite_projects import UserFavoriteProjects
 from rime_sdk.swagger.swagger_client.models.user_private_info import UserPrivateInfo
 from rime_sdk.swagger.swagger_client.models.user_role import UserRole
 from rime_sdk.swagger.swagger_client.models.user_user_detail import UserUserDetail
 from rime_sdk.swagger.swagger_client.models.users_user_id_uuid_body import UsersUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body import UsersUserUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body1 import UsersUserUserIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.v1betaintegrationsintegration_id_uuid_integration import V1betaintegrationsintegrationIdUuidIntegration
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
+from rime_sdk.swagger.swagger_client.models.v1betamonitorsmonitor_id_uuid_monitor import V1betamonitorsmonitorIdUuidMonitor
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
+from rime_sdk.swagger.swagger_client.models.v1notifsettingsnotification_id_uuid_notification import V1notifsettingsnotificationIdUuidNotification
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
-from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_tags_body import WorkspaceIdUuidTagsBody
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,37 +27,42 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'firewall_id': 'object',
         'test_run_incremental_config': 'TestrunTestRunIncrementalConfig',
         'override_existing_bins': 'bool',
+        'agent_id': 'RimeUUID',
         'experimental_fields': 'dict(str, object)'
     }
 
     attribute_map = {
         'firewall_id': 'firewallId',
         'test_run_incremental_config': 'testRunIncrementalConfig',
         'override_existing_bins': 'overrideExistingBins',
+        'agent_id': 'agentId',
         'experimental_fields': 'experimentalFields'
     }
 
-    def __init__(self, firewall_id=None, test_run_incremental_config=None, override_existing_bins=None, experimental_fields=None):  # noqa: E501
+    def __init__(self, firewall_id=None, test_run_incremental_config=None, override_existing_bins=None, agent_id=None, experimental_fields=None):  # noqa: E501
         """ContinuoustestsFirewallIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._firewall_id = None
         self._test_run_incremental_config = None
         self._override_existing_bins = None
+        self._agent_id = None
         self._experimental_fields = None
         self.discriminator = None
         if firewall_id is not None:
             self.firewall_id = firewall_id
         if test_run_incremental_config is not None:
             self.test_run_incremental_config = test_run_incremental_config
         if override_existing_bins is not None:
             self.override_existing_bins = override_existing_bins
+        if agent_id is not None:
+            self.agent_id = agent_id
         if experimental_fields is not None:
             self.experimental_fields = experimental_fields
 
     @property
     def firewall_id(self):
         """Gets the firewall_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
 
@@ -119,14 +124,35 @@
         :param override_existing_bins: The override_existing_bins of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :type: bool
         """
 
         self._override_existing_bins = override_existing_bins
 
     @property
+    def agent_id(self):
+        """Gets the agent_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
+
+
+        :return: The agent_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this ContinuoustestsFirewallIdUuidBody.
+
+
+        :param agent_id: The agent_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
+    @property
     def experimental_fields(self):
         """Gets the experimental_fields of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
 
         Fields that enable experimental functionality.  WARNING: these fields are experimental; ie, their functionality may not be reliable or backwards-compatible. Do not use these fields in production.  # noqa: E501
 
         :return: The experimental_fields of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :rtype: dict(str, object)
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,31 +25,36 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
-        'test_run_config': 'TestrunGenerativeTestRunConfig'
+        'test_run_config': 'TestrunGenerativeTestRunConfig',
+        'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
         'project_id': 'projectId',
-        'test_run_config': 'testRunConfig'
+        'test_run_config': 'testRunConfig',
+        'agent_id': 'agentId'
     }
 
-    def __init__(self, project_id=None, test_run_config=None):  # noqa: E501
+    def __init__(self, project_id=None, test_run_config=None, agent_id=None):  # noqa: E501
         """GenerativestresstestsProjectIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._test_run_config = None
+        self._agent_id = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         if test_run_config is not None:
             self.test_run_config = test_run_config
+        if agent_id is not None:
+            self.agent_id = agent_id
 
     @property
     def project_id(self):
         """Gets the project_id of this GenerativestresstestsProjectIdUuidBody.  # noqa: E501
 
         Uniquely specifies a Project.  # noqa: E501
 
@@ -87,14 +92,35 @@
 
         :param test_run_config: The test_run_config of this GenerativestresstestsProjectIdUuidBody.  # noqa: E501
         :type: TestrunGenerativeTestRunConfig
         """
 
         self._test_run_config = test_run_config
 
+    @property
+    def agent_id(self):
+        """Gets the agent_id of this GenerativestresstestsProjectIdUuidBody.  # noqa: E501
+
+
+        :return: The agent_id of this GenerativestresstestsProjectIdUuidBody.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this GenerativestresstestsProjectIdUuidBody.
+
+
+        :param agent_id: The agent_id of this GenerativestresstestsProjectIdUuidBody.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'monitor': 'TheUpdatesToTheMonitor_',
+        'monitor': 'V1betamonitorsmonitorIdUuidMonitor',
         'mask': 'str'
     }
 
     attribute_map = {
         'monitor': 'monitor',
         'mask': 'mask'
     }
@@ -49,25 +49,25 @@
 
     @property
     def monitor(self):
         """Gets the monitor of this MonitorsMonitorIdUuidBody.  # noqa: E501
 
 
         :return: The monitor of this MonitorsMonitorIdUuidBody.  # noqa: E501
-        :rtype: TheUpdatesToTheMonitor_
+        :rtype: V1betamonitorsmonitorIdUuidMonitor
         """
         return self._monitor
 
     @monitor.setter
     def monitor(self, monitor):
         """Sets the monitor of this MonitorsMonitorIdUuidBody.
 
 
         :param monitor: The monitor of this MonitorsMonitorIdUuidBody.  # noqa: E501
-        :type: TheUpdatesToTheMonitor_
+        :type: V1betamonitorsmonitorIdUuidMonitor
         """
 
         self._monitor = monitor
 
     @property
     def mask(self):
         """Gets the mask of this MonitorsMonitorIdUuidBody.  # noqa: E501
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'notification': 'ObjectContainingTheUpdatesOnlyTheFieldsSpecifiedInTheMaskWillBeUsedByTheBackendNoteTheIDFieldIsNecessaryToFindTheGivenNotificationSetting_',
+        'notification': 'V1notifsettingsnotificationIdUuidNotification',
         'mask': 'str'
     }
 
     attribute_map = {
         'notification': 'notification',
         'mask': 'mask'
     }
@@ -49,25 +49,25 @@
 
     @property
     def notification(self):
         """Gets the notification of this NotifsettingsNotificationIdUuidBody.  # noqa: E501
 
 
         :return: The notification of this NotifsettingsNotificationIdUuidBody.  # noqa: E501
-        :rtype: ObjectContainingTheUpdatesOnlyTheFieldsSpecifiedInTheMaskWillBeUsedByTheBackendNoteTheIDFieldIsNecessaryToFindTheGivenNotificationSetting_
+        :rtype: V1notifsettingsnotificationIdUuidNotification
         """
         return self._notification
 
     @notification.setter
     def notification(self, notification):
         """Sets the notification of this NotifsettingsNotificationIdUuidBody.
 
 
         :param notification: The notification of this NotifsettingsNotificationIdUuidBody.  # noqa: E501
-        :type: ObjectContainingTheUpdatesOnlyTheFieldsSpecifiedInTheMaskWillBeUsedByTheBackendNoteTheIDFieldIsNecessaryToFindTheGivenNotificationSetting_
+        :type: V1notifsettingsnotificationIdUuidNotification
         """
 
         self._notification = notification
 
     @property
     def mask(self):
         """Gets the mask of this NotifsettingsNotificationIdUuidBody.  # noqa: E501
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCreateWorkspaceTagResponse(object):
+class RimeGetJobResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'tag': 'RimeTag'
+        'job': 'RimeJobMetadata'
     }
 
     attribute_map = {
-        'tag': 'tag'
+        'job': 'job'
     }
 
-    def __init__(self, tag=None):  # noqa: E501
-        """RimeCreateWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
-        self._tag = None
+    def __init__(self, job=None):  # noqa: E501
+        """RimeGetJobResponse - a model defined in Swagger"""  # noqa: E501
+        self._job = None
         self.discriminator = None
-        if tag is not None:
-            self.tag = tag
+        if job is not None:
+            self.job = job
 
     @property
-    def tag(self):
-        """Gets the tag of this RimeCreateWorkspaceTagResponse.  # noqa: E501
+    def job(self):
+        """Gets the job of this RimeGetJobResponse.  # noqa: E501
 
 
-        :return: The tag of this RimeCreateWorkspaceTagResponse.  # noqa: E501
-        :rtype: RimeTag
+        :return: The job of this RimeGetJobResponse.  # noqa: E501
+        :rtype: RimeJobMetadata
         """
-        return self._tag
+        return self._job
 
-    @tag.setter
-    def tag(self, tag):
-        """Sets the tag of this RimeCreateWorkspaceTagResponse.
+    @job.setter
+    def job(self, job):
+        """Sets the job of this RimeGetJobResponse.
 
 
-        :param tag: The tag of this RimeCreateWorkspaceTagResponse.  # noqa: E501
-        :type: RimeTag
+        :param job: The job of this RimeGetJobResponse.  # noqa: E501
+        :type: RimeJobMetadata
         """
 
-        self._tag = tag
+        self._job = job
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCreateWorkspaceTagResponse, dict):
+        if issubclass(RimeGetJobResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCreateWorkspaceTagResponse):
+        if not isinstance(other, RimeGetJobResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteWorkspaceTagResponse(object):
+class RimeValidateTestConfigResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeValidateTestConfigResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteWorkspaceTagResponse, dict):
+        if issubclass(RimeValidateTestConfigResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteWorkspaceTagResponse):
+        if not isinstance(other, RimeValidateTestConfigResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,61 +11,35 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeGetJobResponse(object):
+class RimeRegisterPredictionSetResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'job': 'RimeJobMetadata'
     }
 
     attribute_map = {
-        'job': 'job'
     }
 
-    def __init__(self, job=None):  # noqa: E501
-        """RimeGetJobResponse - a model defined in Swagger"""  # noqa: E501
-        self._job = None
+    def __init__(self):  # noqa: E501
+        """RimeRegisterPredictionSetResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if job is not None:
-            self.job = job
-
-    @property
-    def job(self):
-        """Gets the job of this RimeGetJobResponse.  # noqa: E501
-
-
-        :return: The job of this RimeGetJobResponse.  # noqa: E501
-        :rtype: RimeJobMetadata
-        """
-        return self._job
-
-    @job.setter
-    def job(self, job):
-        """Sets the job of this RimeGetJobResponse.
-
-
-        :param job: The job of this RimeGetJobResponse.  # noqa: E501
-        :type: RimeJobMetadata
-        """
-
-        self._job = job
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeGetJobResponse, dict):
+        if issubclass(RimeRegisterPredictionSetResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeGetJobResponse):
+        if not isinstance(other, RimeRegisterPredictionSetResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListWorkspaceTagsResponse(object):
+class UsersUserUserIdUuidBody1(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'RimeUUID',
-        'tags': 'list[RimeTag]'
+        'workspace_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'tags': 'tags'
+        'user': 'user'
     }
 
-    def __init__(self, workspace_id=None, tags=None):  # noqa: E501
-        """RimeListWorkspaceTagsResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
-        self._tags = None
+        self._user = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
-        if tags is not None:
-            self.tags = tags
+        if user is not None:
+            self.user = user
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this RimeListWorkspaceTagsResponse.  # noqa: E501
+        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this RimeListWorkspaceTagsResponse.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: object
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this RimeListWorkspaceTagsResponse.
+        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this RimeListWorkspaceTagsResponse.  # noqa: E501
-        :type: RimeUUID
+        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: object
         """
 
         self._workspace_id = workspace_id
 
     @property
-    def tags(self):
-        """Gets the tags of this RimeListWorkspaceTagsResponse.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
 
 
-        :return: The tags of this RimeListWorkspaceTagsResponse.  # noqa: E501
-        :rtype: list[RimeTag]
+        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._tags
+        return self._user
 
-    @tags.setter
-    def tags(self, tags):
-        """Sets the tags of this RimeListWorkspaceTagsResponse.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody1.
 
 
-        :param tags: The tags of this RimeListWorkspaceTagsResponse.  # noqa: E501
-        :type: list[RimeTag]
+        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._tags = tags
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListWorkspaceTagsResponse, dict):
+        if issubclass(UsersUserUserIdUuidBody1, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListWorkspaceTagsResponse):
+        if not isinstance(other, UsersUserUserIdUuidBody1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeRegisterPredictionSetResponse(object):
+class RimeResolveDetectionEventResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeRegisterPredictionSetResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeResolveDetectionEventResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeRegisterPredictionSetResponse, dict):
+        if issubclass(RimeResolveDetectionEventResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeRegisterPredictionSetResponse):
+        if not isinstance(other, RimeResolveDetectionEventResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,34 +11,40 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeResolveDetectionEventResponse(object):
+class RimeTestType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
+    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeResolveDetectionEventResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeTestType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeResolveDetectionEventResponse, dict):
+        if issubclass(RimeTestType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeResolveDetectionEventResponse):
+        if not isinstance(other, RimeTestType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,35 +26,40 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'file_info': 'FilescanningModelFileInfo',
         'run_time_info': 'RuntimeinfoRunTimeInfo',
-        'workspace_id': 'RimeUUID'
+        'workspace_id': 'RimeUUID',
+        'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
         'file_info': 'fileInfo',
         'run_time_info': 'runTimeInfo',
-        'workspace_id': 'workspaceId'
+        'workspace_id': 'workspaceId',
+        'agent_id': 'agentId'
     }
 
-    def __init__(self, file_info=None, run_time_info=None, workspace_id=None):  # noqa: E501
+    def __init__(self, file_info=None, run_time_info=None, workspace_id=None, agent_id=None):  # noqa: E501
         """RimeStartFileScanRequest - a model defined in Swagger"""  # noqa: E501
         self._file_info = None
         self._run_time_info = None
         self._workspace_id = None
+        self._agent_id = None
         self.discriminator = None
         if file_info is not None:
             self.file_info = file_info
         if run_time_info is not None:
             self.run_time_info = run_time_info
         if workspace_id is not None:
             self.workspace_id = workspace_id
+        if agent_id is not None:
+            self.agent_id = agent_id
 
     @property
     def file_info(self):
         """Gets the file_info of this RimeStartFileScanRequest.  # noqa: E501
 
 
         :return: The file_info of this RimeStartFileScanRequest.  # noqa: E501
@@ -111,14 +116,35 @@
 
         :param workspace_id: The workspace_id of this RimeStartFileScanRequest.  # noqa: E501
         :type: RimeUUID
         """
 
         self._workspace_id = workspace_id
 
+    @property
+    def agent_id(self):
+        """Gets the agent_id of this RimeStartFileScanRequest.  # noqa: E501
+
+
+        :return: The agent_id of this RimeStartFileScanRequest.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this RimeStartFileScanRequest.
+
+
+        :param agent_id: The agent_id of this RimeStartFileScanRequest.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,120 +11,115 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTag(object):
+class RiskscoreRiskScore(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'name': 'str',
-        'creation_time': 'datetime',
-        'num_projects': 'str'
+        'type': 'RiskscoreRiskCategoryType',
+        'severity': 'RimeSeverity',
+        'score': 'float'
     }
 
     attribute_map = {
-        'name': 'name',
-        'creation_time': 'creationTime',
-        'num_projects': 'numProjects'
+        'type': 'type',
+        'severity': 'severity',
+        'score': 'score'
     }
 
-    def __init__(self, name=None, creation_time=None, num_projects=None):  # noqa: E501
-        """RimeTag - a model defined in Swagger"""  # noqa: E501
-        self._name = None
-        self._creation_time = None
-        self._num_projects = None
+    def __init__(self, type=None, severity=None, score=None):  # noqa: E501
+        """RiskscoreRiskScore - a model defined in Swagger"""  # noqa: E501
+        self._type = None
+        self._severity = None
+        self._score = None
         self.discriminator = None
-        self.name = name
-        if creation_time is not None:
-            self.creation_time = creation_time
-        if num_projects is not None:
-            self.num_projects = num_projects
+        if type is not None:
+            self.type = type
+        if severity is not None:
+            self.severity = severity
+        if score is not None:
+            self.score = score
 
     @property
-    def name(self):
-        """Gets the name of this RimeTag.  # noqa: E501
+    def type(self):
+        """Gets the type of this RiskscoreRiskScore.  # noqa: E501
 
-        Name of the Tag.  # noqa: E501
 
-        :return: The name of this RimeTag.  # noqa: E501
-        :rtype: str
+        :return: The type of this RiskscoreRiskScore.  # noqa: E501
+        :rtype: RiskscoreRiskCategoryType
         """
-        return self._name
+        return self._type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this RimeTag.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this RiskscoreRiskScore.
 
-        Name of the Tag.  # noqa: E501
 
-        :param name: The name of this RimeTag.  # noqa: E501
-        :type: str
+        :param type: The type of this RiskscoreRiskScore.  # noqa: E501
+        :type: RiskscoreRiskCategoryType
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._type = type
 
     @property
-    def creation_time(self):
-        """Gets the creation_time of this RimeTag.  # noqa: E501
+    def severity(self):
+        """Gets the severity of this RiskscoreRiskScore.  # noqa: E501
 
-        Creation time of the Workspace.  # noqa: E501
 
-        :return: The creation_time of this RimeTag.  # noqa: E501
-        :rtype: datetime
+        :return: The severity of this RiskscoreRiskScore.  # noqa: E501
+        :rtype: RimeSeverity
         """
-        return self._creation_time
+        return self._severity
 
-    @creation_time.setter
-    def creation_time(self, creation_time):
-        """Sets the creation_time of this RimeTag.
+    @severity.setter
+    def severity(self, severity):
+        """Sets the severity of this RiskscoreRiskScore.
 
-        Creation time of the Workspace.  # noqa: E501
 
-        :param creation_time: The creation_time of this RimeTag.  # noqa: E501
-        :type: datetime
+        :param severity: The severity of this RiskscoreRiskScore.  # noqa: E501
+        :type: RimeSeverity
         """
 
-        self._creation_time = creation_time
+        self._severity = severity
 
     @property
-    def num_projects(self):
-        """Gets the num_projects of this RimeTag.  # noqa: E501
+    def score(self):
+        """Gets the score of this RiskscoreRiskScore.  # noqa: E501
 
-        Number of Projects associated with the Workspace.  # noqa: E501
+        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
 
-        :return: The num_projects of this RimeTag.  # noqa: E501
-        :rtype: str
+        :return: The score of this RiskscoreRiskScore.  # noqa: E501
+        :rtype: float
         """
-        return self._num_projects
+        return self._score
 
-    @num_projects.setter
-    def num_projects(self, num_projects):
-        """Sets the num_projects of this RimeTag.
+    @score.setter
+    def score(self, score):
+        """Sets the score of this RiskscoreRiskScore.
 
-        Number of Projects associated with the Workspace.  # noqa: E501
+        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
 
-        :param num_projects: The num_projects of this RimeTag.  # noqa: E501
-        :type: str
+        :param score: The score of this RiskscoreRiskScore.  # noqa: E501
+        :type: float
         """
 
-        self._num_projects = num_projects
+        self._score = score
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -139,15 +134,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTag, dict):
+        if issubclass(RiskscoreRiskScore, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -155,15 +150,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTag):
+        if not isinstance(other, RiskscoreRiskScore):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestType(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
-    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestType - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestType, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestType):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,34 +11,45 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateWorkspaceTagResponse(object):
+class StatedbJobStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "JOB_STATUS_UNSPECIFIED"
+    PENDING = "JOB_STATUS_PENDING"
+    RUNNING = "JOB_STATUS_RUNNING"
+    FAILED = "JOB_STATUS_FAILED"
+    SUCCEEDED = "JOB_STATUS_SUCCEEDED"
+    REQUESTED = "JOB_STATUS_REQUESTED"
+    CANCELLED = "JOB_STATUS_CANCELLED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
+        """StatedbJobStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +65,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateWorkspaceTagResponse, dict):
+        if issubclass(StatedbJobStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +81,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateWorkspaceTagResponse):
+        if not isinstance(other, StatedbJobStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,34 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeValidateTestConfigResponse(object):
+class TestrunTestSensitivity(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
+    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
+    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
+    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeValidateTestConfigResponse - a model defined in Swagger"""  # noqa: E501
+        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeValidateTestConfigResponse, dict):
+        if issubclass(TestrunTestSensitivity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeValidateTestConfigResponse):
+        if not isinstance(other, TestrunTestSensitivity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,115 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RiskscoreRiskScore(object):
+class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'type': 'RiskscoreRiskCategoryType',
-        'severity': 'RimeSeverity',
-        'score': 'float'
+        'user_id': 'object',
+        'user_role': 'RimeActorRole'
     }
 
     attribute_map = {
-        'type': 'type',
-        'severity': 'severity',
-        'score': 'score'
+        'user_id': 'userId',
+        'user_role': 'userRole'
     }
 
-    def __init__(self, type=None, severity=None, score=None):  # noqa: E501
-        """RiskscoreRiskScore - a model defined in Swagger"""  # noqa: E501
-        self._type = None
-        self._severity = None
-        self._score = None
+    def __init__(self, user_id=None, user_role=None):  # noqa: E501
+        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
+        self._user_id = None
+        self._user_role = None
         self.discriminator = None
-        if type is not None:
-            self.type = type
-        if severity is not None:
-            self.severity = severity
-        if score is not None:
-            self.score = score
+        if user_id is not None:
+            self.user_id = user_id
+        if user_role is not None:
+            self.user_role = user_role
 
     @property
-    def type(self):
-        """Gets the type of this RiskscoreRiskScore.  # noqa: E501
+    def user_id(self):
+        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The type of this RiskscoreRiskScore.  # noqa: E501
-        :rtype: RiskscoreRiskCategoryType
+        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: object
         """
-        return self._type
+        return self._user_id
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this RiskscoreRiskScore.
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param type: The type of this RiskscoreRiskScore.  # noqa: E501
-        :type: RiskscoreRiskCategoryType
+        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: object
         """
 
-        self._type = type
+        self._user_id = user_id
 
     @property
-    def severity(self):
-        """Gets the severity of this RiskscoreRiskScore.  # noqa: E501
+    def user_role(self):
+        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
 
-        :return: The severity of this RiskscoreRiskScore.  # noqa: E501
-        :rtype: RimeSeverity
+        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._severity
+        return self._user_role
 
-    @severity.setter
-    def severity(self, severity):
-        """Sets the severity of this RiskscoreRiskScore.
+    @user_role.setter
+    def user_role(self, user_role):
+        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
 
-        :param severity: The severity of this RiskscoreRiskScore.  # noqa: E501
-        :type: RimeSeverity
+        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._severity = severity
-
-    @property
-    def score(self):
-        """Gets the score of this RiskscoreRiskScore.  # noqa: E501
-
-        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
-
-        :return: The score of this RiskscoreRiskScore.  # noqa: E501
-        :rtype: float
-        """
-        return self._score
-
-    @score.setter
-    def score(self, score):
-        """Sets the score of this RiskscoreRiskScore.
-
-        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
-
-        :param score: The score of this RiskscoreRiskScore.  # noqa: E501
-        :type: float
-        """
-
-        self._score = score
+        self._user_role = user_role
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -134,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RiskscoreRiskScore, dict):
+        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -150,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RiskscoreRiskScore):
+        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,46 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class StatedbJobStatus(object):
+class TestrunresultGetTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "JOB_STATUS_UNSPECIFIED"
-    PENDING = "JOB_STATUS_PENDING"
-    RUNNING = "JOB_STATUS_RUNNING"
-    FAILED = "JOB_STATUS_FAILED"
-    SUCCEEDED = "JOB_STATUS_SUCCEEDED"
-    REQUESTED = "JOB_STATUS_REQUESTED"
-    CANCELLED = "JOB_STATUS_CANCELLED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'test_run': 'TestrunresultTestRunDetail'
     }
 
     attribute_map = {
+        'test_run': 'testRun'
     }
 
-    def __init__(self):  # noqa: E501
-        """StatedbJobStatus - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, test_run=None):  # noqa: E501
+        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_run = None
         self.discriminator = None
+        if test_run is not None:
+            self.test_run = test_run
+
+    @property
+    def test_run(self):
+        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+
+
+        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :rtype: TestrunresultTestRunDetail
+        """
+        return self._test_run
+
+    @test_run.setter
+    def test_run(self, test_run):
+        """Sets the test_run of this TestrunresultGetTestRunResponse.
+
+
+        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :type: TestrunresultTestRunDetail
+        """
+
+        self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -65,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StatedbJobStatus, dict):
+        if issubclass(TestrunresultGetTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -81,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StatedbJobStatus):
+        if not isinstance(other, TestrunresultGetTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,33 +26,38 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'test_run_config': 'TestrunTestRunConfig',
+        'agent_id': 'RimeUUID',
         'experimental_fields': 'dict(str, object)'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'test_run_config': 'testRunConfig',
+        'agent_id': 'agentId',
         'experimental_fields': 'experimentalFields'
     }
 
-    def __init__(self, project_id=None, test_run_config=None, experimental_fields=None):  # noqa: E501
+    def __init__(self, project_id=None, test_run_config=None, agent_id=None, experimental_fields=None):  # noqa: E501
         """StresstestsProjectIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._test_run_config = None
+        self._agent_id = None
         self._experimental_fields = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         if test_run_config is not None:
             self.test_run_config = test_run_config
+        if agent_id is not None:
+            self.agent_id = agent_id
         if experimental_fields is not None:
             self.experimental_fields = experimental_fields
 
     @property
     def project_id(self):
         """Gets the project_id of this StresstestsProjectIdUuidBody.  # noqa: E501
 
@@ -93,14 +98,35 @@
         :param test_run_config: The test_run_config of this StresstestsProjectIdUuidBody.  # noqa: E501
         :type: TestrunTestRunConfig
         """
 
         self._test_run_config = test_run_config
 
     @property
+    def agent_id(self):
+        """Gets the agent_id of this StresstestsProjectIdUuidBody.  # noqa: E501
+
+
+        :return: The agent_id of this StresstestsProjectIdUuidBody.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this StresstestsProjectIdUuidBody.
+
+
+        :param agent_id: The agent_id of this StresstestsProjectIdUuidBody.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
+    @property
     def experimental_fields(self):
         """Gets the experimental_fields of this StresstestsProjectIdUuidBody.  # noqa: E501
 
         Fields that enable experimental functionality.  WARNING: these fields are experimental; ie, their functionality may not be reliable or backwards-compatible. Do not use these fields in production.  # noqa: E501
 
         :return: The experimental_fields of this StresstestsProjectIdUuidBody.  # noqa: E501
         :rtype: dict(str, object)
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,43 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestSensitivity(object):
+class TestrunresultRenameTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
-    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
-    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
-    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'test_run': 'TestrunresultTestRunDetail'
     }
 
     attribute_map = {
+        'test_run': 'testRun'
     }
 
-    def __init__(self):  # noqa: E501
-        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, test_run=None):  # noqa: E501
+        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_run = None
         self.discriminator = None
+        if test_run is not None:
+            self.test_run = test_run
+
+    @property
+    def test_run(self):
+        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+
+
+        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+        :rtype: TestrunresultTestRunDetail
+        """
+        return self._test_run
+
+    @test_run.setter
+    def test_run(self, test_run):
+        """Sets the test_run of this TestrunresultRenameTestRunResponse.
+
+
+        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+        :type: TestrunresultTestRunDetail
+        """
+
+        self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -62,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestSensitivity, dict):
+        if issubclass(TestrunresultRenameTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestSensitivity):
+        if not isinstance(other, TestrunresultRenameTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultGetTestRunResponse(object):
+class UserPrivateInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_run': 'TestrunresultTestRunDetail'
+        'favorite_projects': 'list[UserFavoriteProjects]'
     }
 
     attribute_map = {
-        'test_run': 'testRun'
+        'favorite_projects': 'favoriteProjects'
     }
 
-    def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_run = None
+    def __init__(self, favorite_projects=None):  # noqa: E501
+        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
+        self._favorite_projects = None
         self.discriminator = None
-        if test_run is not None:
-            self.test_run = test_run
+        if favorite_projects is not None:
+            self.favorite_projects = favorite_projects
 
     @property
-    def test_run(self):
-        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+    def favorite_projects(self):
+        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
-        :rtype: TestrunresultTestRunDetail
+        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :rtype: list[UserFavoriteProjects]
         """
-        return self._test_run
+        return self._favorite_projects
 
-    @test_run.setter
-    def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultGetTestRunResponse.
+    @favorite_projects.setter
+    def favorite_projects(self, favorite_projects):
+        """Sets the favorite_projects of this UserPrivateInfo.
 
 
-        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
-        :type: TestrunresultTestRunDetail
+        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :type: list[UserFavoriteProjects]
         """
 
-        self._test_run = test_run
+        self._favorite_projects = favorite_projects
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultGetTestRunResponse, dict):
+        if issubclass(UserPrivateInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultGetTestRunResponse):
+        if not isinstance(other, UserPrivateInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_validation_categories_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultRenameTestRunResponse(object):
+class TestrunresultGetValidationCategoriesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_run': 'TestrunresultTestRunDetail'
+        'categories': 'list[TestrunTestCategoryType]'
     }
 
     attribute_map = {
-        'test_run': 'testRun'
+        'categories': 'categories'
     }
 
-    def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_run = None
+    def __init__(self, categories=None):  # noqa: E501
+        """TestrunresultGetValidationCategoriesResponse - a model defined in Swagger"""  # noqa: E501
+        self._categories = None
         self.discriminator = None
-        if test_run is not None:
-            self.test_run = test_run
+        if categories is not None:
+            self.categories = categories
 
     @property
-    def test_run(self):
-        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+    def categories(self):
+        """Gets the categories of this TestrunresultGetValidationCategoriesResponse.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :rtype: TestrunresultTestRunDetail
+        :return: The categories of this TestrunresultGetValidationCategoriesResponse.  # noqa: E501
+        :rtype: list[TestrunTestCategoryType]
         """
-        return self._test_run
+        return self._categories
 
-    @test_run.setter
-    def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultRenameTestRunResponse.
+    @categories.setter
+    def categories(self, categories):
+        """Sets the categories of this TestrunresultGetValidationCategoriesResponse.
 
 
-        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :type: TestrunresultTestRunDetail
+        :param categories: The categories of this TestrunresultGetValidationCategoriesResponse.  # noqa: E501
+        :type: list[TestrunTestCategoryType]
         """
 
-        self._test_run = test_run
+        self._categories = categories
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultRenameTestRunResponse, dict):
+        if issubclass(TestrunresultGetValidationCategoriesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultRenameTestRunResponse):
+        if not isinstance(other, TestrunresultGetValidationCategoriesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_get_monitor_categories_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserPrivateInfo(object):
+class TestrunresultGetMonitorCategoriesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'favorite_projects': 'list[UserFavoriteProjects]'
+        'categories': 'list[TestrunTestCategoryType]'
     }
 
     attribute_map = {
-        'favorite_projects': 'favoriteProjects'
+        'categories': 'categories'
     }
 
-    def __init__(self, favorite_projects=None):  # noqa: E501
-        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
-        self._favorite_projects = None
+    def __init__(self, categories=None):  # noqa: E501
+        """TestrunresultGetMonitorCategoriesResponse - a model defined in Swagger"""  # noqa: E501
+        self._categories = None
         self.discriminator = None
-        if favorite_projects is not None:
-            self.favorite_projects = favorite_projects
+        if categories is not None:
+            self.categories = categories
 
     @property
-    def favorite_projects(self):
-        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
+    def categories(self):
+        """Gets the categories of this TestrunresultGetMonitorCategoriesResponse.  # noqa: E501
 
 
-        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
-        :rtype: list[UserFavoriteProjects]
+        :return: The categories of this TestrunresultGetMonitorCategoriesResponse.  # noqa: E501
+        :rtype: list[TestrunTestCategoryType]
         """
-        return self._favorite_projects
+        return self._categories
 
-    @favorite_projects.setter
-    def favorite_projects(self, favorite_projects):
-        """Sets the favorite_projects of this UserPrivateInfo.
+    @categories.setter
+    def categories(self, categories):
+        """Sets the categories of this TestrunresultGetMonitorCategoriesResponse.
 
 
-        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
-        :type: list[UserFavoriteProjects]
+        :param categories: The categories of this TestrunresultGetMonitorCategoriesResponse.  # noqa: E501
+        :type: list[TestrunTestCategoryType]
         """
 
-        self._favorite_projects = favorite_projects
+        self._categories = categories
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserPrivateInfo, dict):
+        if issubclass(TestrunresultGetMonitorCategoriesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserPrivateInfo):
+        if not isinstance(other, TestrunresultGetMonitorCategoriesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,43 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class UsersUserIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'user': 'V1usersuserIdUuidUser',
+        'mask': 'RimeUserWriteMask'
     }
 
     attribute_map = {
+        'user': 'user',
+        'mask': 'mask'
     }
 
-    def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, user=None, mask=None):  # noqa: E501
+        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._user = None
+        self._mask = None
         self.discriminator = None
+        if user is not None:
+            self.user = user
+        if mask is not None:
+            self.mask = mask
+
+    @property
+    def user(self):
+        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+
+
+        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: V1usersuserIdUuidUser
+        """
+        return self._user
+
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserIdUuidBody.
+
+
+        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :type: V1usersuserIdUuidUser
+        """
+
+        self._user = user
+
+    @property
+    def mask(self):
+        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+
+
+        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: RimeUserWriteMask
+        """
+        return self._mask
+
+    @mask.setter
+    def mask(self, mask):
+        """Sets the mask of this UsersUserIdUuidBody.
+
+
+        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :type: RimeUserWriteMask
+        """
+
+        self._mask = mask
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -62,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(UsersUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, UsersUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,89 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody1(object):
+class ValidationValidatePredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'is_valid': 'bool',
+        'error_message': 'str'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'user': 'user'
+        'is_valid': 'isValid',
+        'error_message': 'errorMessage'
     }
 
-    def __init__(self, workspace_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._user = None
+    def __init__(self, is_valid=None, error_message=None):  # noqa: E501
+        """ValidationValidatePredictionsResponse - a model defined in Swagger"""  # noqa: E501
+        self._is_valid = None
+        self._error_message = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if user is not None:
-            self.user = user
+        if is_valid is not None:
+            self.is_valid = is_valid
+        if error_message is not None:
+            self.error_message = error_message
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def is_valid(self):
+        """Gets the is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
 
-        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :rtype: object
+        :return: The is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._workspace_id
+        return self._is_valid
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
+    @is_valid.setter
+    def is_valid(self, is_valid):
+        """Sets the is_valid of this ValidationValidatePredictionsResponse.
 
-        Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :type: object
+        :param is_valid: The is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :type: bool
         """
 
-        self._workspace_id = workspace_id
+        self._is_valid = is_valid
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def error_message(self):
+        """Gets the error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
 
 
-        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._user
+        return self._error_message
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody1.
+    @error_message.setter
+    def error_message(self, error_message):
+        """Sets the error_message of this ValidationValidatePredictionsResponse.
 
 
-        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param error_message: The error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :type: str
         """
 
-        self._user = user
+        self._error_message = error_message
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserUserIdUuidBody1, dict):
+        if issubclass(ValidationValidatePredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserUserIdUuidBody1):
+        if not isinstance(other, ValidationValidatePredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,92 +11,91 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WorkspaceIdUuidTagsBody(object):
+class WorkspaceIdUuidUsersBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'workspace_id': 'object',
-        'name': 'str'
+        'users': 'list[RimeUserWithRole]'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'name': 'name'
+        'users': 'users'
     }
 
-    def __init__(self, workspace_id=None, name=None):  # noqa: E501
-        """WorkspaceIdUuidTagsBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, users=None):  # noqa: E501
+        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
-        self._name = None
+        self._users = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
-        self.name = name
+        if users is not None:
+            self.users = users
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :rtype: object
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this WorkspaceIdUuidTagsBody.
+        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :type: object
         """
 
         self._workspace_id = workspace_id
 
     @property
-    def name(self):
-        """Gets the name of this WorkspaceIdUuidTagsBody.  # noqa: E501
+    def users(self):
+        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
-        Name of the tag.  # noqa: E501
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :return: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
-        :rtype: str
+        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :rtype: list[RimeUserWithRole]
         """
-        return self._name
+        return self._users
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this WorkspaceIdUuidTagsBody.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this WorkspaceIdUuidUsersBody.
 
-        Name of the tag.  # noqa: E501
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :param name: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
-        :type: str
+        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :type: list[RimeUserWithRole]
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._users = users
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -111,15 +110,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkspaceIdUuidTagsBody, dict):
+        if issubclass(WorkspaceIdUuidUsersBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -127,15 +126,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkspaceIdUuidTagsBody):
+        if not isinstance(other, WorkspaceIdUuidUsersBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,91 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WorkspaceIdUuidUsersBody(object):
+class TestrunresultListTestRunsRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'object',
-        'users': 'list[RimeUserWithRole]'
+        'project_id': 'RimeUUID',
+        'testing_type': 'RimeTestType'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'users': 'users'
+        'project_id': 'projectId',
+        'testing_type': 'testingType'
     }
 
-    def __init__(self, workspace_id=None, users=None):  # noqa: E501
-        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._users = None
+    def __init__(self, project_id=None, testing_type=None):  # noqa: E501
+        """TestrunresultListTestRunsRequestQuery - a model defined in Swagger"""  # noqa: E501
+        self._project_id = None
+        self._testing_type = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if users is not None:
-            self.users = users
+        if project_id is not None:
+            self.project_id = project_id
+        if testing_type is not None:
+            self.testing_type = testing_type
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
+    def project_id(self):
+        """Gets the project_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
 
-        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :rtype: object
+        :return: The project_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._workspace_id
+        return self._project_id
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
+    @project_id.setter
+    def project_id(self, project_id):
+        """Sets the project_id of this TestrunresultListTestRunsRequestQuery.
 
-        Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :type: object
+        :param project_id: The project_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._workspace_id = workspace_id
+        self._project_id = project_id
 
     @property
-    def users(self):
-        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+    def testing_type(self):
+        """Gets the testing_type of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
 
-        List of Users to add to the Workspace.  # noqa: E501
 
-        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :rtype: list[RimeUserWithRole]
+        :return: The testing_type of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :rtype: RimeTestType
         """
-        return self._users
+        return self._testing_type
 
-    @users.setter
-    def users(self, users):
-        """Sets the users of this WorkspaceIdUuidUsersBody.
+    @testing_type.setter
+    def testing_type(self, testing_type):
+        """Sets the testing_type of this TestrunresultListTestRunsRequestQuery.
 
-        List of Users to add to the Workspace.  # noqa: E501
 
-        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :type: list[RimeUserWithRole]
+        :param testing_type: The testing_type of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :type: RimeTestType
         """
 
-        self._users = users
+        self._testing_type = testing_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkspaceIdUuidUsersBody, dict):
+        if issubclass(TestrunresultListTestRunsRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkspaceIdUuidUsersBody):
+        if not isinstance(other, TestrunresultListTestRunsRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.2.0rc1/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/test_batch.py` & `rime_sdk-2.2.0rc1/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc0/rime_sdk/test_run.py` & `rime_sdk-2.2.0rc1/rime_sdk/test_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,15 @@
             api = swagger_client.ResultsReaderApi(self._api_client)
             res: TestrunresultGetTestRunResponse = api.results_reader_get_test_run(
                 test_run_id=self.test_run_id
             )
         return res.test_run.web_app_url.url
 
     def get_result_df(self) -> pd.DataFrame:
-        """Return high level summary information for a complete stress Test Run in a\
-        single-row dataframe.
+        """Return high level summary information for a complete stress Test Run in a single-row dataframe.
 
         This dataframe includes information such as model metrics on the reference and\
         evaluation datasets, overall RIME results such as severity across tests,\
         and high level metadata such as the project ID and model task.
 
         Place these rows together to build a table of test to build a table of test
         run results for comparison. This only works for stress test jobs that
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.2.0rc1/rime_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.2.0rc0
+Version: 2.2.0rc1
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc0/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.2.0rc1/rime_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
 rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
 rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
 rime_sdk/swagger/swagger_client/models/notification_notification.py
 rime_sdk/swagger/swagger_client/models/notification_notification_type.py
 rime_sdk/swagger/swagger_client/models/notification_object_type.py
 rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
 rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
-rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
 rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
 rime_sdk/swagger/swagger_client/models/project_create_project_request.py
 rime_sdk/swagger/swagger_client/models/project_create_project_response.py
 rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
 rime_sdk/swagger/swagger_client/models/project_get_project_response.py
 rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
@@ -247,27 +246,25 @@
 rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
-rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
 rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
 rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
-rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
 rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
 rime_sdk/swagger/swagger_client/models/rime_failing_row.py
 rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
 rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
 rime_sdk/swagger/swagger_client/models/rime_feature_type.py
 rime_sdk/swagger/swagger_client/models/rime_float_list.py
 rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
@@ -333,15 +330,14 @@
 rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
-rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
 rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
 rime_sdk/swagger/swagger_client/models/rime_managed_image.py
 rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
 rime_sdk/swagger/swagger_client/models/rime_model_card.py
 rime_sdk/swagger/swagger_client/models/rime_model_task.py
@@ -383,15 +379,14 @@
 rime_sdk/swagger/swagger_client/models/rime_str_list.py
 rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
 rime_sdk/swagger/swagger_client/models/rime_subject_type.py
 rime_sdk/swagger/swagger_client/models/rime_suggestion.py
 rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
 rime_sdk/swagger/swagger_client/models/rime_table_column.py
 rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
-rime_sdk/swagger/swagger_client/models/rime_tag.py
 rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
 rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
 rime_sdk/swagger/swagger_client/models/rime_test_metric.py
 rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
 rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
 rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
 rime_sdk/swagger/swagger_client/models/rime_test_type.py
@@ -403,15 +398,14 @@
 rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
-rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
 rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
 rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
 rime_sdk/swagger/swagger_client/models/rime_user_role.py
 rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
 rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
 rime_sdk/swagger/swagger_client/models/rime_uuid.py
 rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
@@ -434,15 +428,14 @@
 rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
 rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
 rime_sdk/swagger/swagger_client/models/statedb_job_status.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
 rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
-rime_sdk/swagger/swagger_client/models/tags_name_body.py
 rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
 rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
 rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
 rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
 rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
 rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
 rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
@@ -452,44 +445,47 @@
 rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
 rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+rime_sdk/swagger/swagger_client/models/testrunresult_get_monitor_categories_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+rime_sdk/swagger/swagger_client/models/testrunresult_get_validation_categories_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
 rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
 rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
-rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
 rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
 rime_sdk/swagger/swagger_client/models/user_private_info.py
 rime_sdk/swagger/swagger_client/models/user_role.py
 rime_sdk/swagger/swagger_client/models/user_user_detail.py
 rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
 rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
 rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
 rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
 rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
 rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
 rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
 rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
-rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
 rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
 rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
```

### Comparing `rime_sdk-2.2.0rc0/setup.py` & `rime_sdk-2.2.0rc1/setup.py`

 * *Files identical despite different names*

