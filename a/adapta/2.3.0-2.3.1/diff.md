# Comparing `tmp/adapta-2.3.0.tar.gz` & `tmp/adapta-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.3.0.tar", max compression
+gzip compressed data, was "adapta-2.3.1.tar", max compression
```

## Comparing `adapta-2.3.0.tar` & `adapta-2.3.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    10693 2023-07-05 09:27:26.020175 adapta-2.3.0/LICENSE
--rw-r--r--   0        0        0      666 2023-07-05 09:27:26.020175 adapta-2.3.0/README.md
--rw-r--r--   0        0        0      663 2023-07-05 09:27:26.020175 adapta-2.3.0/adapta/__init__.py
--rw-r--r--   0        0        0       22 2023-07-05 09:27:46.196101 adapta-2.3.0/adapta/_version.py
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.020175 adapta-2.3.0/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      694 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1914 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/README.md
--rw-r--r--   0        0        0      667 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/__init__.py
--rw-r--r--   0        0        0    12390 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/_base.py
--rw-r--r--   0        0        0     2950 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/_internal.py
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9167 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2211 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      741 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      794 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      963 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      672 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3215 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4466 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      653 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/_model.py
--rw-r--r--   0        0        0      699 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5319 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     3820 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      674 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3362 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      732 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/schema_management/README.md
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/schema_management/__init__.py
--rw-r--r--   0        0        0     1219 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/schema_management/schema_entity.py
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/__init__.py
--rw-r--r--   0        0        0     2140 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/README.md
--rw-r--r--   0        0        0     1450 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     8358 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2396 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1787 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2695 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2601 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3454 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0     1952 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/token_client.py
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      622 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0     9605 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     4791 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/base.py
--rw-r--r--   0        0        0      665 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3451 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3365 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2451 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/README.md
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4691 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      675 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1447 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7711 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     4523 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     2386 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      721 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11493 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2247 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     5302 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2063 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/base.py
--rw-r--r--   0        0        0     5711 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6630 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1519 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/local.py
--rw-r--r--   0        0        0     1953 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      666 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2216 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2358 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2887 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0     2761 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/utils/README.md
--rw-r--r--   0        0        0      668 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/utils/_common.py
--rw-r--r--   0        0        0     3930 2023-07-05 09:27:26.028175 adapta-2.3.0/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0     2211 2023-07-05 09:27:46.196101 adapta-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 adapta-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-07-11 12:10:10.396031 adapta-2.3.1/LICENSE
+-rw-r--r--   0        0        0      666 2023-07-11 12:10:10.396031 adapta-2.3.1/README.md
+-rw-r--r--   0        0        0      663 2023-07-11 12:10:10.396031 adapta-2.3.1/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 12:10:29.452716 adapta-2.3.1/adapta/_version.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.396031 adapta-2.3.1/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      694 2023-07-11 12:10:10.396031 adapta-2.3.1/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1914 2023-07-11 12:10:10.396031 adapta-2.3.1/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2023-07-11 12:10:10.396031 adapta-2.3.1/adapta/logs/README.md
+-rw-r--r--   0        0        0      667 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/__init__.py
+-rw-r--r--   0        0        0    12390 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/_base.py
+-rw-r--r--   0        0        0     2950 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/_internal.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9167 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2211 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      741 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      963 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      672 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3215 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      653 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/ml/_model.py
+-rw-r--r--   0        0        0      699 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5319 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     4012 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      674 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3362 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      732 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/schema_management/README.md
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/schema_management/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/schema_management/schema_entity.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/__init__.py
+-rw-r--r--   0        0        0     2140 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/README.md
+-rw-r--r--   0        0        0     1450 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     8358 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2396 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1787 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2695 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2601 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3454 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0     1952 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/security/clients/hashicorp_vault/token_client.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      622 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0     9605 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     4791 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0      665 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3451 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3365 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2451 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4691 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      675 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7711 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     4523 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     2386 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      721 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11493 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2247 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     5302 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2063 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/models/base.py
+-rw-r--r--   0        0        0     5711 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6630 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1519 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/models/local.py
+-rw-r--r--   0        0        0     1953 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      666 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2216 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2358 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2887 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0     2761 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/utils/README.md
+-rw-r--r--   0        0        0      668 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3930 2023-07-11 12:10:10.400032 adapta-2.3.1/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0     2211 2023-07-11 12:10:29.452716 adapta-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 adapta-2.3.1/PKG-INFO
```

### Comparing `adapta-2.3.0/LICENSE` & `adapta-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/README.md` & `adapta-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/__init__.py` & `adapta-2.3.1/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/connectors/__init__.py` & `adapta-2.3.1/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/connectors/service_bus/__init__.py` & `adapta-2.3.1/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/connectors/service_bus/_connector.py` & `adapta-2.3.1/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/README.md` & `adapta-2.3.1/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/__init__.py` & `adapta-2.3.1/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/_base.py` & `adapta-2.3.1/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/_internal.py` & `adapta-2.3.1/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/handlers/__init__.py` & `adapta-2.3.1/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.3.1/adapta/logs/handlers/datadog_api_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.3.1/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/models/__init__.py` & `adapta-2.3.1/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/models/_log_level.py` & `adapta-2.3.1/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/logs/models/_logs_metadata.py` & `adapta-2.3.1/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/metrics/__init__.py` & `adapta-2.3.1/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/metrics/_base.py` & `adapta-2.3.1/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/metrics/providers/README.md` & `adapta-2.3.1/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/metrics/providers/__init__.py` & `adapta-2.3.1/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/metrics/providers/datadog_provider.py` & `adapta-2.3.1/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/ml/__init__.py` & `adapta-2.3.1/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/ml/_model.py` & `adapta-2.3.1/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/ml/mlflow/__init__.py` & `adapta-2.3.1/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/ml/mlflow/_client.py` & `adapta-2.3.1/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/ml/mlflow/_functions.py` & `adapta-2.3.1/adapta/ml/mlflow/_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  limitations under the License.
 #
 
 import configparser
 import importlib
 import pathlib
 import tempfile
-from typing import Optional, Dict
+from typing import Optional, Dict, Any
 
 import mlflow
 from mlflow.pyfunc import PythonModel
 
 from adapta.ml.mlflow._client import MlflowBasicClient
 from adapta.ml._model import MachineLearningModel
 
@@ -47,25 +47,27 @@
     model: MachineLearningModel,
     mlflow_client: MlflowBasicClient,
     model_name: str,
     experiment: str,
     run_name: str = None,
     transition_to_stage: str = None,
     metrics: Optional[Dict[str, float]] = None,
+    model_params: Optional[Dict[str, Any]] = None,
     artifacts_to_log: Dict[str, str] = None,
 ):
     """Registers mlflow model
 
     :param model: Machine learning model to register
     :param mlflow_client: Mlflow client
     :param model_name: Name of Mlflow model
     :param experiment: Name of Mlflow experiment
     :param run_name: Name of Mlflow run
     :param transition_to_stage: Whether to transition to stage
     :param metrics: Metrics to log
+    :param model_params: Model hyperparameters to log
     :param artifacts_to_log: Additional artifacts to log
     """
     assert transition_to_stage in [None, "Staging", "Production"]
 
     mlflow.set_experiment(experiment)
 
     path_model = pathlib.PurePath(tempfile.gettempdir(), "model")
@@ -98,13 +100,16 @@
             registered_model_name=model_name,
             artifacts=artifacts,
         )
 
         if metrics is not None:
             mlflow.log_metrics(metrics)
 
+        if model_params is not None:
+            mlflow.log_params(model_params)
+
         if transition_to_stage is not None:
             mlflow_client.set_model_stage(
                 model_name=model_name,
                 model_version=mlflow_client.get_latest_model_version(model_name).version,
                 stage=transition_to_stage,
             )
```

### Comparing `adapta-2.3.0/adapta/process_communication/__init__.py` & `adapta-2.3.1/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/process_communication/_models.py` & `adapta-2.3.1/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/schema_management/README.md` & `adapta-2.3.1/adapta/schema_management/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/schema_management/__init__.py` & `adapta-2.3.1/adapta/schema_management/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/schema_management/schema_entity.py` & `adapta-2.3.1/adapta/schema_management/schema_entity.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/__init__.py` & `adapta-2.3.1/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/README.md` & `adapta-2.3.1/adapta/security/clients/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/__init__.py` & `adapta-2.3.1/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/_azure_client.py` & `adapta-2.3.1/adapta/security/clients/_azure_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/_base.py` & `adapta-2.3.1/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/_local_client.py` & `adapta-2.3.1/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.3.1/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.3.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.3.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.3.1/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/security/clients/hashicorp_vault/token_client.py` & `adapta-2.3.1/adapta/security/clients/hashicorp_vault/token_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/__init__.py` & `adapta-2.3.1/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/blob/README.md` & `adapta-2.3.1/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/blob/__init__.py` & `adapta-2.3.1/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/blob/azure_storage_client.py` & `adapta-2.3.1/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/blob/base.py` & `adapta-2.3.1/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/cache/__init__.py` & `adapta-2.3.1/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/cache/_base.py` & `adapta-2.3.1/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/cache/redis_cache.py` & `adapta-2.3.1/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/README.md` & `adapta-2.3.1/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/__init__.py` & `adapta-2.3.1/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/azure_sql.py` & `adapta-2.3.1/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/models/__init__.py` & `adapta-2.3.1/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/models/_models.py` & `adapta-2.3.1/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/odbc.py` & `adapta-2.3.1/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/database/trino_sql.py` & `adapta-2.3.1/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/delta_lake/README.md` & `adapta-2.3.1/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/delta_lake/__init__.py` & `adapta-2.3.1/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/delta_lake/_functions.py` & `adapta-2.3.1/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/delta_lake/_models.py` & `adapta-2.3.1/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/models/__init__.py` & `adapta-2.3.1/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/models/azure.py` & `adapta-2.3.1/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/models/base.py` & `adapta-2.3.1/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/models/format.py` & `adapta-2.3.1/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/models/hive.py` & `adapta-2.3.1/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/models/local.py` & `adapta-2.3.1/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/secrets/README.md` & `adapta-2.3.1/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/secrets/__init__.py` & `adapta-2.3.1/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/secrets/_base.py` & `adapta-2.3.1/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.3.1/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.3.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/utils/README.md` & `adapta-2.3.1/adapta/utils/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/utils/__init__.py` & `adapta-2.3.1/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/utils/_common.py` & `adapta-2.3.1/adapta/utils/_common.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/adapta/utils/concurrent_task_runner.py` & `adapta-2.3.1/adapta/utils/concurrent_task_runner.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.0/pyproject.toml` & `adapta-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adapta"
-version = "2.3.0"
+version = "2.3.1"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
```

### Comparing `adapta-2.3.0/PKG-INFO` & `adapta-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.3.0
+Version: 2.3.1
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

