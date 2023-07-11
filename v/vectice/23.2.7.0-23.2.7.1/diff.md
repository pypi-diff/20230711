# Comparing `tmp/vectice-23.2.7.0.tar.gz` & `tmp/vectice-23.2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.7.0.tar", last modified: Mon Jul 10 08:19:24 2023, max compression
+gzip compressed data, was "vectice-23.2.7.1.tar", last modified: Tue Jul 11 11:53:58 2023, max compression
```

## Comparing `vectice-23.2.7.0.tar` & `vectice-23.2.7.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 08:19:16.000000 vectice-23.2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-10 08:19:24.550819 vectice-23.2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 08:19:16.000000 vectice-23.2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 08:19:16.000000 vectice-23.2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 08:19:24.550819 vectice-23.2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-10 08:19:16.000000 vectice-23.2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.538819 vectice-23.2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.538819 vectice-23.2.7.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.542819 vectice-23.2.7.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.546819 vectice-23.2.7.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.546819 vectice-23.2.7.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.546819 vectice-23.2.7.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.538819 vectice-23.2.7.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.647463 vectice-23.2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 11:53:45.000000 vectice-23.2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-11 11:53:58.647463 vectice-23.2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 11:53:45.000000 vectice-23.2.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 11:53:45.000000 vectice-23.2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 11:53:58.651463 vectice-23.2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-11 11:53:45.000000 vectice-23.2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.615463 vectice-23.2.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.619463 vectice-23.2.7.1/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.627463 vectice-23.2.7.1/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.635463 vectice-23.2.7.1/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.639463 vectice-23.2.7.1/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.639463 vectice-23.2.7.1/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.643463 vectice-23.2.7.1/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.647463 vectice-23.2.7.1/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.647463 vectice-23.2.7.1/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.619463 vectice-23.2.7.1/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.7.0/LICENSE` & `vectice-23.2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/PKG-INFO` & `vectice-23.2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.7.0
+Version: 23.2.7.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.7.0/setup.py` & `vectice-23.2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         "urllib3",
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
         "pandas",
         "typing-extensions==4.6.2",
-        "pyspark",
         "dataclasses-json==0.5.8",
     ],
     extras_require={
         "dev": [
             "black",
             "gitpython",
             "mypy",
@@ -77,14 +76,15 @@
             "pytest-randomly",
             "coverage",
             "pytest-cov",
             "scikit-learn<=0.24.2",
             "testcontainers",
             "testbook",
             "db-dtypes>=1.1.1",
+            "pyspark",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `vectice-23.2.7.0/src/vectice/__init__.py` & `vectice-23.2.7.1/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/__init__.py` & `vectice-23.2.7.1/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/_auth.py` & `vectice-23.2.7.1/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/attachment.py` & `vectice-23.2.7.1/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/client.py` & `vectice-23.2.7.1/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_api.py` & `vectice-23.2.7.1/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_code.py` & `vectice-23.2.7.1/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_code_version.py` & `vectice-23.2.7.1/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_dataset.py` & `vectice-23.2.7.1/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_entity_file.py` & `vectice-23.2.7.1/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.7.1/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_model.py` & `vectice-23.2.7.1/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_organization.py` & `vectice-23.2.7.1/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.7.1/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/http_error.py` & `vectice-23.2.7.1/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/http_error_handlers.py` & `vectice-23.2.7.1/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/iteration.py` & `vectice-23.2.7.1/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/__init__.py` & `vectice-23.2.7.1/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/artifact_version.py` & `vectice-23.2.7.1/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/code.py` & `vectice-23.2.7.1/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/code_version.py` & `vectice-23.2.7.1/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/dataset_register.py` & `vectice-23.2.7.1/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/dataset_representation.py` & `vectice-23.2.7.1/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/dataset_version.py` & `vectice-23.2.7.1/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-23.2.7.1/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/files_metadata.py` & `vectice-23.2.7.1/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/iteration.py` & `vectice-23.2.7.1/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/last_assets.py` & `vectice-23.2.7.1/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/metric.py` & `vectice-23.2.7.1/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/model.py` & `vectice-23.2.7.1/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/model_register.py` & `vectice-23.2.7.1/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/model_representation.py` & `vectice-23.2.7.1/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/model_version.py` & `vectice-23.2.7.1/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/model_version_representation.py` & `vectice-23.2.7.1/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/paged_response.py` & `vectice-23.2.7.1/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/phase.py` & `vectice-23.2.7.1/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/project.py` & `vectice-23.2.7.1/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/property.py` & `vectice-23.2.7.1/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/public_config.py` & `vectice-23.2.7.1/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/step.py` & `vectice-23.2.7.1/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/json/workspace.py` & `vectice-23.2.7.1/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/last_assets.py` & `vectice-23.2.7.1/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/phase.py` & `vectice-23.2.7.1/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/project.py` & `vectice-23.2.7.1/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/rest_api.py` & `vectice-23.2.7.1/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/step.py` & `vectice-23.2.7.1/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/version.py` & `vectice-23.2.7.1/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/api/workspace.py` & `vectice-23.2.7.1/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/connection.py` & `vectice-23.2.7.1/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/__init__.py` & `vectice-23.2.7.1/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/attachment_container.py` & `vectice-23.2.7.1/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/dataset.py` & `vectice-23.2.7.1/src/vectice/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 from typing import Union
 
-from pyspark.sql.dataframe import DataFrame as SparkDF
 from typing_extensions import get_args
 
 from vectice.models.property import Property
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
@@ -70,29 +69,35 @@
             (self._resource is not None and self._resource._dataframes is not None)
             or (self._training_resource is not None and self._training_resource._dataframes is not None)
             or (self._testing_resource is not None and self._testing_resource._dataframes is not None)
             or (self._validation_resource is not None and self._validation_resource._dataframes is not None)
         )
 
         if self._has_dataframe:
+            try:
+                from pyspark.sql.dataframe import DataFrame as SparkDF
 
-            def has_spark(resource: Resource | None) -> bool:
-                if resource is None or resource._dataframes is None:
+                def has_spark(resource: Resource | None) -> bool:
+                    if resource is None or resource._dataframes is None:
+                        return False
+                    for df in resource._dataframes:
+                        if isinstance(df, SparkDF):
+                            return True
                     return False
-                for df in resource._dataframes:
-                    if isinstance(df, SparkDF):
-                        return True
-                return False
-
-            self._has_spark_df = (
-                has_spark(self._resource)
-                or has_spark(self._training_resource)
-                or has_spark(self._testing_resource)
-                or has_spark(self._validation_resource)
-            )
+
+                self._has_spark_df = (
+                    has_spark(self._resource)
+                    or has_spark(self._training_resource)
+                    or has_spark(self._testing_resource)
+                    or has_spark(self._validation_resource)
+                )
+
+            except ImportError:
+                self._has_spark_df = False
+                pass
         else:
             self._has_spark_df = False
 
     @staticmethod
     def origin(
         resource: Resource,
         name: str | None = None,
```

### Comparing `vectice-23.2.7.0/src/vectice/models/git_version.py` & `vectice-23.2.7.1/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/iteration.py` & `vectice-23.2.7.1/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/metric.py` & `vectice-23.2.7.1/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/model.py` & `vectice-23.2.7.1/src/vectice/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,16 @@
     @metrics.setter
     def metrics(self, metrics: dict[str, int] | list[Metric] | Metric | None):
         """Set the model's metrics.
 
         Parameters:
             metrics: The metrics of the model.
         """
-        self._format_metrics(metrics)
+        _logger.warning("To save your updated model metrics, you must reassign your dataset to a step.")
+        self._metrics = self._format_metrics(metrics)
 
     @property
     def properties(self) -> list[Property] | None:
         """The model's properties.
 
         Returns:
             The model's properties.
@@ -167,15 +168,16 @@
     @properties.setter
     def properties(self, properties: dict[str, str] | list[Property] | Property | None):
         """Set the model's properties.
 
         Parameters:
             properties: The properties of the model.
         """
-        self._format_properties(properties)
+        _logger.warning("To save your updated dataset properties, you must reassign your dataset to a step.")
+        self._properties = self._format_properties(properties)
 
     @property
     def attachments(self) -> list[str] | None:
         """The attachments associated with the model.
 
         Returns:
             The attachments associated with the model.
```

### Comparing `vectice-23.2.7.0/src/vectice/models/phase.py` & `vectice-23.2.7.1/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/project.py` & `vectice-23.2.7.1/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/property.py` & `vectice-23.2.7.1/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/representation/dataset_representation.py` & `vectice-23.2.7.1/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/__init__.py` & `vectice-23.2.7.1/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/base.py` & `vectice-23.2.7.1/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.7.1/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-23.2.7.1/src/vectice/models/resource/databricks_table_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from __future__ import annotations
 
 import datetime
 import re
 from typing import Optional
 
 from dateutil import parser
-from pyspark.sql import DataFrame, SparkSession
+
+try:
+    from pyspark.sql import SparkSession
+
+    spark_imported = True
+except ImportError:
+    spark_imported = False
+    pass
 
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata.column_metadata import DBColumn
+from vectice.models.resource.metadata.dataframe_config import DataFrameType
 from vectice.models.resource.metadata.db_metadata import DBMetadata, MetadataDB
 from vectice.models.resource.metadata.extra_metadata import ExtraMetadata
 
 
 class DatabricksTableResource(Resource):
     """Databricks tables resource reference wrapper.
 
@@ -32,39 +40,43 @@
     """
 
     _origin = "DatabricksTable"
 
     def __init__(
         self,
         paths: str | list[str],
-        dataframes: DataFrame | list[DataFrame] | None = None,
+        dataframes: DataFrameType | list[DataFrameType] | None = None,
         spark_client: SparkSession | None = None,
         capture_schema_only: bool = False,
     ):
         """Initialize a DatabricksTableResource resource.
 
         Parameters:
             paths: The paths to retrieve the tables. Should be either the table name or the location of the table.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats.
             spark_client (Optional): The spark session allowing vectice to capture the table metadata.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
         """
+        if spark_imported is False:
+            raise ImportError("Pyspark is not installed.")
         super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
         self._spark_client = spark_client
 
     def _fetch_data(self):
-        tables: dict[str, tuple[dict | None, DataFrame | None]] = {}
+        tables: dict[str, tuple[dict | None, DataFrameType | None]] = {}
         df_index = 0
         for path in self._paths:
             path_tables, new_df_index = self._fetch_table_data(index=df_index, path=path)
             tables.update(path_tables)
             df_index += new_df_index
         return tables
 
-    def _fetch_table_data(self, index: int, path: str) -> tuple[dict[str, tuple[dict | None, DataFrame | None]], int]:
+    def _fetch_table_data(
+        self, index: int, path: str
+    ) -> tuple[dict[str, tuple[dict | None, DataFrameType | None]], int]:
         table_display_name = path
         has_at = re.search("@", path)
         has_version = re.search("@v", path)
         table_path = path.split("@")[0] if has_at else path
 
         dataframe = self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
 
@@ -192,15 +204,15 @@
         date_time = history_row["timestamp"]
         return [
             ExtraMetadata(key="version", value=f"v{version}", display_name="Version"),
             ExtraMetadata(key="timestamp", value=str(date_time.isoformat()), display_name="Timestamp"),
         ]
 
     def _build_metadata(self) -> DBMetadata:
-        tables_metadata: dict[str, tuple[dict | None, DataFrame | None]] = self.data
+        tables_metadata: dict[str, tuple[dict | None, DataFrameType | None]] = self.data
         dbs: list[MetadataDB] = []
         for table_name, [table_metadata, dataframe] in tables_metadata.items():
             columns: list[DBColumn] | None = None
             size = None
             updated_date = None
             created_date = None
             rows_number = None
```

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/description.py` & `vectice-23.2.7.1/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/file_resource.py` & `vectice-23.2.7.1/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.7.1/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from typing import Union
 
 from pandas.core.frame import DataFrame as PandasDF
-from pyspark.pandas.frame import DataFrame as PysparkPandasDF
-from pyspark.sql.dataframe import DataFrame as SparkDF
 
 from vectice.models.resource.metadata.df_wrapper_resource import DataFrameWrapper
 
-DataFramePandasType = Union[PysparkPandasDF, PandasDF]
-DataFrameTypeWithoutWrapper = Union[DataFramePandasType, SparkDF]
-DataFrameType = Union[DataFrameTypeWithoutWrapper, DataFrameWrapper]
+try:
+    from pyspark.pandas.frame import DataFrame as PysparkPandasDF
+    from pyspark.sql.dataframe import DataFrame as SparkDF
+
+    DataFramePandasType = Union[PysparkPandasDF, PandasDF]
+    DataFrameTypeWithoutWrapper = Union[DataFramePandasType, SparkDF]
+    DataFrameType = Union[DataFrameTypeWithoutWrapper, DataFrameWrapper]
+
+except ImportError:
+    DataFramePandasType = PandasDF  # type: ignore
+    DataFrameType = Union[DataFramePandasType, DataFrameWrapper]  # type: ignore
+
 
 MIN_ROWS_CAPTURE_STATS = 100
 MAX_COLUMNS_CAPTURE_STATS = 100
```

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
-from typing import Dict, Tuple
+from typing import TYPE_CHECKING, Dict, Tuple
 
-from pyspark.sql import DataFrame as SparkDF
-from pyspark.sql import SparkSession
-from pyspark.sql import functions as f
+if TYPE_CHECKING:
+    from pyspark.sql import DataFrame as SparkDF
 
 from vectice.models.resource.metadata.column_metadata import (
     BooleanStat,
     Column,
     ColumnCategoryType,
     DateStat,
     NumericalStat,
@@ -19,17 +18,28 @@
     TextStat,
 )
 from vectice.models.resource.metadata.dataframe_config import MAX_COLUMNS_CAPTURE_STATS
 from vectice.models.resource.metadata.df_wrapper_resource import DataFrameWrapper
 
 _logger = logging.getLogger(__name__)
 
+try:
+    from pyspark.sql import SparkSession
+    from pyspark.sql import functions as f
 
-class SparkDFWrapper(DataFrameWrapper[SparkDF]):
+    spark_imported = True
+except ImportError:
+    spark_imported = False
+    pass
+
+
+class SparkDFWrapper(DataFrameWrapper):
     def __init__(self, dataframe: SparkDF):
+        if spark_imported is False:
+            raise ImportError("Pyspark is not installed.")
         super().__init__(dataframe)
         self.spark = SparkSession.builder.getOrCreate()
 
     def get_size(self) -> Size:
         self.rows: int = self.dataframe.count()
         self.columns_numbers: int = len(self.dataframe.columns)
```

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from datetime import datetime
+from typing import TYPE_CHECKING
 
-from pyspark import pandas as ps
-from pyspark.pandas.frame import DataFrame as PysparkPandasDF
+if TYPE_CHECKING:
+    from pyspark import pandas as ps
+    from pyspark.pandas.frame import DataFrame as PysparkPandasDF
 
 
 class TimeSeries:
     def __init__(self):
         pass
 
     def __len__(self) -> int:
```

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.7.1/src/vectice/models/resource/metadata/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 import logging
 from typing import Dict
 
 from pandas.core.frame import DataFrame as PandasDF
-from pyspark.pandas.frame import DataFrame as PysparkPandasDF
-from pyspark.sql.dataframe import DataFrame as SparkDF
 
 from vectice.models.resource.metadata.base import MetadataSettings
 from vectice.models.resource.metadata.column_metadata import Column
 from vectice.models.resource.metadata.dataframe_config import DataFrameType
 from vectice.models.resource.metadata.df_wrapper_pandas import PandasDFWrapper
 from vectice.models.resource.metadata.df_wrapper_pyspark_pandas import PysparkPandasDFWrapper
 from vectice.models.resource.metadata.df_wrapper_resource import DataFrameWrapper
@@ -55,24 +53,31 @@
         self._dataframe = dataframe
         self._wrapper: PandasDFWrapper | PysparkPandasDFWrapper | SparkDFWrapper | None = None
         self._settings = MetadataSettings()
         self.capture_schema_only = capture_schema_only
 
         if isinstance(self._dataframe, PandasDF):
             self._wrapper = PandasDFWrapper(self._dataframe)
-        elif isinstance(self._dataframe, SparkDF):
-            self._wrapper = SparkDFWrapper(self._dataframe)
-        elif isinstance(self._dataframe, PysparkPandasDF):
-            _logger.warning(
-                "WARNING: Pandas on spark is not supported yet, pass a Pandas or a Spark DataFrame to get statistics."
-            )
         elif isinstance(self._dataframe, DataFrameWrapper):
             _logger.warning(
                 "WARNING: Custom wrappers are not supported yet, pass a Pandas or a Spark DataFrame to get statistics."
             )
+        else:
+            try:
+                from pyspark.pandas.frame import DataFrame as PysparkPandasDF
+                from pyspark.sql.dataframe import DataFrame as SparkDF
+
+                if isinstance(self._dataframe, SparkDF):
+                    self._wrapper = SparkDFWrapper(self._dataframe)
+                elif isinstance(self._dataframe, PysparkPandasDF):
+                    _logger.warning(
+                        "WARNING: Pandas on spark is not supported yet, pass a Pandas or a Spark DataFrame to get statistics."
+                    )
+            except ImportError:
+                pass
 
     def set_settings(self, settings: MetadataSettings):
         self._settings = settings
 
     def asdict(self) -> dict:
         size_info: Dict[str, int | float | None] = {}
         skipped_statistics = False
```

### Comparing `vectice-23.2.7.0/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.7.1/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/step.py` & `vectice-23.2.7.1/src/vectice/models/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/step_dataset.py` & `vectice-23.2.7.1/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/step_image.py` & `vectice-23.2.7.1/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/step_model.py` & `vectice-23.2.7.1/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/step_number.py` & `vectice-23.2.7.1/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/step_string.py` & `vectice-23.2.7.1/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/models/workspace.py` & `vectice-23.2.7.1/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.7.1/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/utils/common_utils.py` & `vectice-23.2.7.1/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/utils/configuration.py` & `vectice-23.2.7.1/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/utils/deprecation.py` & `vectice-23.2.7.1/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/utils/last_assets.py` & `vectice-23.2.7.1/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice/utils/logging_utils.py` & `vectice-23.2.7.1/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.7.1/src/vectice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.7.0
+Version: 23.2.7.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.7.0/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.7.1/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.0/src/vectice.egg-info/requires.txt` & `vectice-23.2.7.1/src/vectice.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 urllib3
 gql[requests]
 GitPython
 packaging
 Pillow
 pandas
 typing-extensions==4.6.2
-pyspark
 dataclasses-json==0.5.8
 
 [dev]
 black
 gitpython
 mypy
 ruff
@@ -48,7 +47,8 @@
 pytest-randomly
 coverage
 pytest-cov
 scikit-learn<=0.24.2
 testcontainers
 testbook
 db-dtypes>=1.1.1
+pyspark
```

