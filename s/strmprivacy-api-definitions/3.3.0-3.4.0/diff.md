# Comparing `tmp/strmprivacy-api-definitions-3.3.0.tar.gz` & `tmp/strmprivacy-api-definitions-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strmprivacy-api-definitions-3.3.0.tar", last modified: Thu Jun 29 07:57:55 2023, max compression
+gzip compressed data, was "strmprivacy-api-definitions-3.4.0.tar", last modified: Tue Jul 11 07:56:12 2023, max compression
```

## Comparing `strmprivacy-api-definitions-3.3.0.tar` & `strmprivacy-api-definitions-3.4.0.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.408593 strmprivacy-api-definitions-3.3.0/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-29 07:57:55.407593 strmprivacy-api-definitions-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:57:55.408593 strmprivacy-api-definitions-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-29 07:57:30.000000 strmprivacy-api-definitions-3.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.373589 strmprivacy-api-definitions-3.3.0/strmprivacy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.373589 strmprivacy-api-definitions-3.3.0/strmprivacy/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.374590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.374590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12198 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16789 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.375589 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.377590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3261 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.377590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.377590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5030 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.378590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.378590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5338 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.379590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.379590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7665 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10858 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.379590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.380590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.380590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.381590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3987 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6740 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.381590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.382590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8979 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.382590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.383590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7497 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.383590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.384590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5978 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.384590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.384590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22863 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28488 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.385590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.385590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9865 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.386591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.386591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81835 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.387591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12632 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.387591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.388591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15658 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20098 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.388591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.389591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.389591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.391591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7909 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6958 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10345 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.391591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.392591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6199 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9342 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.392591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.392591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.393591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.393591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5369 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8964 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.394591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.394591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.394591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.395591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.395591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.396592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10605 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13648 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.396592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.397592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.397592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.398592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9075 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.398592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.399592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.399592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.399592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.400592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.400592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4521 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7409 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.401592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.401592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7458 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14509 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.402592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.402592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.402592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.403592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    17973 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.403592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.404592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5254 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.404592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.405592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.405592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.406592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4644 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4831 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.407593 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7436 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.884743 strmprivacy-api-definitions-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 07:56:12.884743 strmprivacy-api-definitions-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 07:56:12.884743 strmprivacy-api-definitions-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-07-11 07:55:54.000000 strmprivacy-api-definitions-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.852741 strmprivacy-api-definitions-3.4.0/strmprivacy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.852741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.852741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.853741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12198 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.853741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.855741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.855741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.855741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.856741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.856741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.856741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.857741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10858 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.857741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.858741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.858741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.859741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.859741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.859741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8979 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.860741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.860741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.860741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.861741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.861741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.862742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22863 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.862742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.863741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9865 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.863741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.864742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.864742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12632 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.865742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.865742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15658 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20098 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.866742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.866742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.866742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.868742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6958 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10345 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.868742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.869742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6199 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.869742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.870742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.870742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.870742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8964 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.871742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.871742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.871742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.872742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.872742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.873742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10605 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13648 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.873742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.873742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.874742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.874742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.874742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.875742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.875742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.876742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.876742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.877742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.877742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.877742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.878743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.878743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.878743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.879742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17973 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.879742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.880743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.881743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.881743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.881743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.882743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.883743 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/top_level.txt
```

### Comparing `strmprivacy-api-definitions-3.3.0/PKG-INFO` & `strmprivacy-api-definitions-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.3.0
+Version: 3.4.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.3.0/setup.py` & `strmprivacy-api-definitions-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 _sym_db = _symbol_database.Default()
 
 
 from strmprivacy.api.entities.v1 import entities_v1_pb2 as strmprivacy_dot_api_dot_entities_dot_v1_dot_entities__v1__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'strmprivacy/api/audit/v1/audit_v1.proto\x12\x18strmprivacy.api.audit.v1\x1a-strmprivacy/api/entities/v1/entities_v1.proto\x1a\x17validate/validate.proto\"\xa4\x01\n\x14GetAuditTrailRequest\x12P\n\nentity_ref\x18\x01 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12\x1b\n\tpage_size\x18\x02 \x01(\x05R\x08pageSize\x12\x1d\n\npage_token\x18\x03 \x01(\tR\tpageToken\"\x87\x01\n\x15GetAuditTrailResponse\x12\x46\n\x07\x65ntries\x18\x01 \x03(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryR\x07\x65ntries\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"\x82\x01\n\x1c\x43reateAuditTrailEntryRequest\x12\x62\n\x11\x61udit_trail_entry\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0f\x61uditTrailEntry\"y\n\x1d\x43reateAuditTrailEntryResponse\x12X\n\x11\x61udit_trail_entry\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryR\x0f\x61uditTrailEntry2\x8b\x02\n\x0c\x41uditService\x12p\n\rGetAuditTrail\x12..strmprivacy.api.audit.v1.GetAuditTrailRequest\x1a/.strmprivacy.api.audit.v1.GetAuditTrailResponse\x12\x88\x01\n\x15\x43reateAuditTrailEntry\x12\x36.strmprivacy.api.audit.v1.CreateAuditTrailEntryRequest\x1a\x37.strmprivacy.api.audit.v1.CreateAuditTrailEntryResponseB`\n\x1bio.strmprivacy.api.audit.v1P\x01Z?github.com/strmprivacy/api-definitions-go/v2/api/audit/v1;auditb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'strmprivacy/api/audit/v1/audit_v1.proto\x12\x18strmprivacy.api.audit.v1\x1a-strmprivacy/api/entities/v1/entities_v1.proto\x1a\x17validate/validate.proto\"\xc6\x01\n\x14GetAuditTrailRequest\x12\x46\n\nentity_ref\x18\x01 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefR\tentityRef\x12\x1b\n\tpage_size\x18\x02 \x01(\x05R\x08pageSize\x12\x1d\n\npage_token\x18\x03 \x01(\tR\tpageToken\x12*\n\nproject_id\x18\x04 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\x87\x01\n\x15GetAuditTrailResponse\x12\x46\n\x07\x65ntries\x18\x01 \x03(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryR\x07\x65ntries\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"\x82\x01\n\x1c\x43reateAuditTrailEntryRequest\x12\x62\n\x11\x61udit_trail_entry\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0f\x61uditTrailEntry\"y\n\x1d\x43reateAuditTrailEntryResponse\x12X\n\x11\x61udit_trail_entry\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryR\x0f\x61uditTrailEntry2\x8b\x02\n\x0c\x41uditService\x12p\n\rGetAuditTrail\x12..strmprivacy.api.audit.v1.GetAuditTrailRequest\x1a/.strmprivacy.api.audit.v1.GetAuditTrailResponse\x12\x88\x01\n\x15\x43reateAuditTrailEntry\x12\x36.strmprivacy.api.audit.v1.CreateAuditTrailEntryRequest\x1a\x37.strmprivacy.api.audit.v1.CreateAuditTrailEntryResponseB`\n\x1bio.strmprivacy.api.audit.v1P\x01Z?github.com/strmprivacy/api-definitions-go/v2/api/audit/v1;auditb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'strmprivacy.api.audit.v1.audit_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033io.strmprivacy.api.audit.v1P\001Z?github.com/strmprivacy/api-definitions-go/v2/api/audit/v1;audit'
-  _GETAUDITTRAILREQUEST.fields_by_name['entity_ref']._options = None
-  _GETAUDITTRAILREQUEST.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _GETAUDITTRAILREQUEST.fields_by_name['project_id']._options = None
+  _GETAUDITTRAILREQUEST.fields_by_name['project_id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
   _CREATEAUDITTRAILENTRYREQUEST.fields_by_name['audit_trail_entry']._options = None
   _CREATEAUDITTRAILENTRYREQUEST.fields_by_name['audit_trail_entry']._serialized_options = b'\372B\005\212\001\002\020\001'
   _GETAUDITTRAILREQUEST._serialized_start=142
-  _GETAUDITTRAILREQUEST._serialized_end=306
-  _GETAUDITTRAILRESPONSE._serialized_start=309
-  _GETAUDITTRAILRESPONSE._serialized_end=444
-  _CREATEAUDITTRAILENTRYREQUEST._serialized_start=447
-  _CREATEAUDITTRAILENTRYREQUEST._serialized_end=577
-  _CREATEAUDITTRAILENTRYRESPONSE._serialized_start=579
-  _CREATEAUDITTRAILENTRYRESPONSE._serialized_end=700
-  _AUDITSERVICE._serialized_start=703
-  _AUDITSERVICE._serialized_end=970
+  _GETAUDITTRAILREQUEST._serialized_end=340
+  _GETAUDITTRAILRESPONSE._serialized_start=343
+  _GETAUDITTRAILRESPONSE._serialized_end=478
+  _CREATEAUDITTRAILENTRYREQUEST._serialized_start=481
+  _CREATEAUDITTRAILENTRYREQUEST._serialized_end=611
+  _CREATEAUDITTRAILENTRYRESPONSE._serialized_start=613
+  _CREATEAUDITTRAILENTRYRESPONSE._serialized_end=734
+  _AUDITSERVICE._serialized_start=737
+  _AUDITSERVICE._serialized_end=1004
 # @@protoc_insertion_point(module_scope)
```

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/entities_v1_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.type import datetime_pb2 as google_dot_type_dot_datetime__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-strmprivacy/api/entities/v1/entities_v1.proto\x12\x1bstrmprivacy.api.entities.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1agoogle/type/datetime.proto\x1a\x17validate/validate.proto\"\xab\x05\n\x06Stream\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x0b\xe0\x41\x02\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12-\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x0b\xfa\x42\x08r\x06\x18\xe8\x07\xd0\x01\x01R\x0b\x64\x65scription\x12/\n\x0e\x63onsent_levels\x18\x03 \x03(\x05\x42\x08\xfa\x42\x05\x92\x01\x02\x10\x32R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x04 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12\x1d\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x03\xe0\x41\x03R\x07\x65nabled\x12@\n\x06limits\x18\x06 \x01(\x0b\x32#.strmprivacy.api.entities.v1.LimitsB\x03\xe0\x41\x03R\x06limits\x12#\n\rlinked_stream\x18\x07 \x01(\tR\x0clinkedStream\x12$\n\x04tags\x18\x08 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x10\x14\x18\x01\"\x04r\x02\x18\x64R\x04tags\x12O\n\x0b\x63redentials\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.CredentialsB\x03\xe0\x41\x03R\x0b\x63redentials\x12N\n\rmasked_fields\x18\n \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\x12&\n\x0bkafka_topic\x18\x0b \x01(\tB\x05\x18\x01\xe0\x41\x03R\nkafkaTopic\x12(\n\tpolicy_id\x18\x0c \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xaa\x01\n\x0e\x45xtendedStream\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x03R\x06stream\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12\x17\n\x04uuid\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\"\n\nkey_stream\x18\x04 \x01(\x08\x42\x03\xe0\x41\x03R\tkeyStream\"\xc2\x01\n\x13\x45xtendedStreamGroup\x12U\n\rsource_stream\x18\x01 \x01(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamB\x03\xe0\x41\x03R\x0csourceStream\x12T\n\x0f\x64\x65rived_streams\x18\x02 \x03(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamR\x0e\x64\x65rivedStreams\"\x91\x03\n\x0cMaskedFields\x12\x1b\n\thash_type\x18\x01 \x01(\tR\x08hashType\x12\x37\n\x04seed\x18\x02 \x01(\tB#\xfa\x42 r\x1e\x18\xe8\x07\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04seed\x12\x63\n\x0e\x66ield_patterns\x18\x03 \x03(\x0b\x32<.strmprivacy.api.entities.v1.MaskedFields.FieldPatternsEntryR\rfieldPatterns\x1aw\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12K\n\x05value\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MaskedFields.PatternListR\x05value:\x02\x38\x01\x1aM\n\x0bPatternList\x12>\n\x0e\x66ield_patterns\x18\x01 \x03(\tB\x17\xfa\x42\x14\x92\x01\x11\x18\x01\"\rr\x0b\xba\x01\x08strmMetaR\rfieldPatterns\"R\n\x06Limits\x12\"\n\nevent_rate\x18\x01 \x01(\x03\x42\x03\xe0\x41\x03R\teventRate\x12$\n\x0b\x65vent_count\x18\x02 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\x92\x01\n\tKeyStream\x12@\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefB\x03\xe0\x41\x03R\x03ref\x12\x1d\n\x06status\x18\x02 \x01(\tB\x05\x18\x01\xe0\x41\x03R\x06status\x12$\n\x0bkafka_topic\x18\x03 \x01(\tB\x03\xe0\x41\x03R\nkafkaTopic\"\x9c\x01\n\tStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x9f\x01\n\x0cKeyStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xa1\x01\n\x0b\x43redentials\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\tbillingId\x12 \n\tclient_id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12\"\n\nproject_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"\xdf\x01\n\x04Sink\x12;\n\x03ref\x18\x01 \x01(\x0b\x32$.strmprivacy.api.entities.v1.SinkRefB\x03\xe0\x41\x02R\x03ref\x12G\n\tsink_type\x18\x02 \x01(\x0e\x32%.strmprivacy.api.entities.v1.SinkTypeB\x03\xe0\x41\x02R\x08sinkType\x12\x43\n\x06\x62ucket\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.BucketConfigH\x00R\x06\x62ucket:\x02\x18\x01\x42\x08\n\x06\x63onfig\"J\n\x07SinkRef\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name:\x02\x18\x01\"\x83\x01\n\x0c\x42ucketConfig\x12$\n\x0b\x62ucket_name\x18\x04 \x01(\tB\x03\xe0\x41\x02R\nbucketName\x12%\n\x0b\x63redentials\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x0b\x63redentials\x12&\n\x0f\x61ssume_role_arn\x18\x06 \x01(\tR\rassumeRoleArn\"\x9f\x05\n\rDataConnector\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\ts3_bucket\x18\x02 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.AwsS3BucketLocationH\x00R\x08s3Bucket\x12~\n\x1bgoogle_cloud_storage_bucket\x18\x03 \x01(\x0b\x32=.strmprivacy.api.entities.v1.GoogleCloudStorageBucketLocationH\x00R\x18googleCloudStorageBucket\x12\x81\x01\n\x1c\x61zure_blob_storage_container\x18\x04 \x01(\x0b\x32>.strmprivacy.api.entities.v1.AzureBlobStorageContainerLocationH\x00R\x19\x61zureBlobStorageContainer\x12P\n\rjdbc_location\x18\x07 \x01(\x0b\x32).strmprivacy.api.entities.v1.JdbcLocationH\x00R\x0cjdbcLocation\x12\x1f\n\x04uuid\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x04uuid\x12j\n\x12\x64\x65pendent_entities\x18\x06 \x01(\x0b\x32;.strmprivacy.api.entities.v1.DataConnectorDependentEntitiesR\x11\x64\x65pendentEntitiesB\x0f\n\x08location\x12\x03\xf8\x42\x01\"\xa0\x01\n\x10\x44\x61taConnectorRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb3\x02\n\x1e\x44\x61taConnectorDependentEntities\x12S\n\x0f\x62\x61tch_exporters\x18\x01 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12\x44\n\nbatch_jobs\x18\x02 \x03(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobR\tbatchJobs\x12v\n\x1cmicro_aggregation_batch_jobs\x18\x03 \x03(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobR\x19microAggregationBatchJobs\"\x9e\x01\n\x13\x41wsS3BucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\x12\x32\n\x0f\x61ssume_role_arn\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\rassumeRoleArn\"w\n GoogleCloudStorageBucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\"\x8a\x02\n!AzureBlobStorageContainerLocation\x12\x37\n\x13storage_account_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x11storageAccountUri\x12.\n\x0e\x63ontainer_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\rcontainerName\x12|\n\x18\x63lient_secret_credential\x18\x03 \x01(\x0b\x32\x38.strmprivacy.api.entities.v1.AzureClientSecretCredentialB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x16\x63lientSecretCredential\"\x97\x01\n\x1b\x41zureClientSecretCredential\x12$\n\ttenant_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08tenantId\x12$\n\tclient_id\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x63lientId\x12,\n\rclient_secret\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0c\x63lientSecret\"\xad\x01\n\x0cJdbcLocation\x12\"\n\x08jdbc_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07jdbcUri\x12)\n\x0bprivate_key\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xd0\x01\x01R\nprivateKey\x12N\n\rdatabase_type\x18\x03 \x01(\x0e\x32).strmprivacy.api.entities.v1.DatabaseTypeR\x0c\x64\x61tabaseType\"\xa3\x01\n\x08\x44\x61taType\x12:\n\x03\x63sv\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.CsvConfigH\x00R\x03\x63sv\x12I\n\x08\x64\x61tabase\x18\x02 \x01(\x0b\x32+.strmprivacy.api.entities.v1.DatabaseConfigH\x00R\x08\x64\x61tabaseB\x10\n\tdata_type\x12\x03\xf8\x42\x01\"%\n\tCsvConfig\x12\x18\n\x07\x63harset\x18\x01 \x01(\tR\x07\x63harset\"\x8a\x05\n\rBatchExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.BatchExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefH\x00R\tstreamRef\x12Q\n\x0ekey_stream_ref\x18\x03 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefH\x00R\x0ckeyStreamRef\x12I\n\x08interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x12\xe0\x41\x02\xfa\x42\x0c\xaa\x01\t\"\x03\x08\x90\x1c\x32\x02\x08\x1eR\x08interval\x12*\n\tsink_name\x18\x05 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\x08sinkName\x12[\n\x0bpath_prefix\x18\x06 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x36\n\x17include_existing_events\x18\x07 \x01(\x08R\x15includeExistingEvents\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x08 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRefB\x1f\n\x18stream_or_key_stream_ref\x12\x03\xf8\x42\x01\"\x98\x01\n\x15\x45xtendedBatchExporter\x12\x17\n\x04uuid\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12K\n\x08\x65xporter\x18\x03 \x01(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterB\x03\xe0\x41\x03R\x08\x65xporter\"\xa3\x01\n\x10\x42\x61tchExporterRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xfa\x01\n\x0cKafkaCluster\x12\x43\n\x03ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x02R\x03ref\x12\x30\n\x11\x62ootstrap_servers\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x10\x62ootstrapServers\x12V\n\x0e\x61uth_mechanism\x18\x03 \x01(\x0e\x32*.strmprivacy.api.entities.v1.AuthMechanismB\x03\xe0\x41\x02R\rauthMechanism\x12\x1b\n\ttoken_uri\x18\x04 \x01(\tR\x08tokenUri\"\x93\x01\n\x0fKafkaClusterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\xb3\x02\n\rKafkaExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.KafkaExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tstreamRef\x12H\n\x06target\x18\x03 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.KafkaExporterTargetR\x06target\x12<\n\x05users\x18\x04 \x03(\x0b\x32&.strmprivacy.api.entities.v1.KafkaUserR\x05users\"v\n\x10KafkaExporterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\x87\x02\n\x13KafkaExporterTarget\x12W\n\x0b\x63luster_ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nclusterRef\x12\x34\n\x05topic\x18\x02 \x01(\tB\x1e\xfa\x42\x1br\x19\x18\xf9\x01\x32\x11^[a-zA-Z0-9._-]+$\xd0\x01\x01R\x05topic\x12(\n\tclient_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08\x63lientId\x12\x37\n\rclient_secret\x18\x04 \x01(\tB\x12\xfa\x42\x0fr\r2\x08^[ -~]+$\xd0\x01\x01R\x0c\x63lientSecret\"\xc2\x02\n\tKafkaUser\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KafkaUserRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x33\n\x13kafka_exporter_name\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x11kafkaExporterName\x12\x19\n\x05topic\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12 \n\tclient_id\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x06 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12R\n\x0b\x63luster_ref\x18\x07 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x03R\nclusterRef\"n\n\x0cKafkaUserRef\x12!\n\nbilling_id\x18\x01 \x01(\tB\x02\x18\x01R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12\"\n\nproject_id\x18\x03 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"6\n\rConsentLevels\x12%\n\x0e\x63onsent_levels\x18\x01 \x03(\x05R\rconsentLevels\"\x9d\x01\n\x13\x43onsentLevelMapping\x12O\n\x03ref\x18\x01 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.ConsentLevelMappingRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\"\x8d\x01\n\x16\x43onsentLevelMappingRef\x12+\n\nbilling_id\x18\x01 \x01(\tB\x0c\x18\x01\xfa\x42\x07r\x05\x18\x00\xd0\x01\x01R\tbillingId\x12\x1d\n\x05level\x18\x02 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x86\x03\n\x06Policy\x12\x18\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\x02id\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0b\x64\x65scription\x12-\n\rlegal_grounds\x18\x04 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0clegalGrounds\x12\x30\n\x0eretention_days\x18\x05 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04(\x01@\x01R\rretentionDays\x12\x44\n\x05state\x18\x06 \x01(\x0e\x32).strmprivacy.api.entities.v1.Policy.StateB\x03\xe0\x41\x03R\x05state\"U\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATE_DRAFT\x10\x01\x12\x10\n\x0cSTATE_ACTIVE\x10\x02\x12\x12\n\x0eSTATE_ARCHIVED\x10\x03\"\xb6\x01\n\x12WindowedEventCount\x12>\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstartTime\x12:\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\x07\x65ndTime\x12$\n\x0b\x65vent_count\x18\x03 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\xaf\x01\n\tSchemaRef\x12\x1b\n\x06handle\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x06handle\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name\x12\x1d\n\x07version\x18\x03 \x01(\tB\x03\xe0\x41\x02R\x07version\x12M\n\x0bschema_type\x18\x04 \x01(\x0e\x32\'.strmprivacy.api.entities.v1.SchemaTypeB\x03\xe0\x41\x03R\nschemaType\"\xe9\x06\n\x06Schema\x12\x42\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x44\n\x05state\x18\x02 \x01(\x0e\x32).strmprivacy.api.entities.v1.Schema.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x03 \x01(\x08R\x08isPublic\x12\x1e\n\ndefinition\x18\x04 \x01(\tR\ndefinition\x12%\n\x0b\x66ingerprint\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x0b\x66ingerprint\x12G\n\x08metadata\x18\x06 \x01(\x0b\x32+.strmprivacy.api.entities.v1.SchemaMetadataR\x08metadata\x12_\n\rsimple_schema\x18\x07 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionR\x0csimpleSchema\x12\x13\n\x02id\x18\x08 \x01(\tB\x03\xe0\x41\x03R\x02id\x1a\xbf\x02\n\x16SimpleSchemaDefinition\x12$\n\x04name\x18\x01 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12]\n\tnamespace\x18\x02 \x01(\tB?\xfa\x42<r:25^([a-zA-Z_][a-zA-Z0-9_]*)(\\.[a-zA-Z_][a-zA-Z0-9_]*)*$\xd0\x01\x01R\tnamespace\x12\x1a\n\x03\x64oc\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\x12\x43\n\x05nodes\x18\x04 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12?\n\tavro_name\x18\x05 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe3\x02\n\x10SimpleSchemaNode\x12O\n\x04type\x18\x01 \x01(\x0e\x32\x31.strmprivacy.api.entities.v1.SimpleSchemaNodeTypeB\x08\xfa\x42\x05\x82\x01\x02 \x00R\x04type\x12$\n\x04name\x18\x02 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12?\n\tavro_name\x18\x07 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\x12\x1a\n\x08repeated\x18\x03 \x01(\x08R\x08repeated\x12\x1a\n\x08required\x18\x04 \x01(\x08R\x08required\x12\x43\n\x05nodes\x18\x05 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12\x1a\n\x03\x64oc\x18\x06 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\"\xd5\x02\n\x0eSchemaMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12*\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x30\n\x08icon_uri\x18\x04 \x01(\tB\x15\xfa\x42\x12r\x10:\x08https://\xd0\x01\x01\x88\x01\x01R\x07iconUri\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\x9a\x01\n\x10\x45ventContractRef\x12\x1f\n\x06handle\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x04R\x06handle\x12\x33\n\x04name\x18\x02 \x01(\tB\x1f\xfa\x42\x1cr\x1a\x10\x04\x18\x64\x32\x14^[\\pL\\pN\\pS\\pM\\pP]+$R\x04name\x12\x30\n\x07version\x18\x03 \x01(\tB\x16\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x82\x06\n\rEventContract\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x03\xe0\x41\x02R\x03ref\x12K\n\x05state\x18\x02 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.EventContract.StateB\x03\xe0\x41\x03R\x05state\x12J\n\nschema_ref\x18\x03 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x03\xe0\x41\x02R\tschemaRef\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12 \n\tkey_field\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x08keyField\x12X\n\npii_fields\x18\x06 \x03(\x0b\x32\x39.strmprivacy.api.entities.v1.EventContract.PiiFieldsEntryR\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12N\n\x08metadata\x18\x08 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.EventContractMetadataR\x08metadata\x12\x0e\n\x02id\x18\t \x01(\tR\x02id\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"b\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\"\xc0\x02\n\x15\x45ventContractMetadata\x12\x19\n\x05title\x18\x01 \x01(\tB\x03\xe0\x41\x01R\x05title\x12%\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x03\xe0\x41\x01R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x1e\n\x08icon_uri\x18\x04 \x01(\tB\x03\xe0\x41\x01R\x07iconUri\x12?\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelB\x03\xe0\x41\x01R\x06labels\x12\x1d\n\x07\x64omains\x18\x06 \x03(\tB\x03\xe0\x41\x01R\x07\x64omains\x12#\n\nindustries\x18\x07 \x03(\tB\x03\xe0\x41\x01R\nindustries\"8\n\x05Label\x12\x19\n\x03key\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"l\n\nValidation\x12\x1d\n\x05\x66ield\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05\x66ield\x12 \n\x04type\x18\x02 \x01(\tB\x0c\xfa\x42\tr\x07R\x05regexR\x04type\x12\x1d\n\x05value\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05value\"\xfe\x02\n\nStreamTree\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x02R\x06stream\x12\x45\n\nkey_stream\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.KeyStreamR\tkeyStream\x12=\n\x07\x64\x65rived\x18\x03 \x03(\x0b\x32#.strmprivacy.api.entities.v1.StreamR\x07\x64\x65rived\x12S\n\x0f\x62\x61tch_exporters\x18\x04 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12S\n\x0fkafka_exporters\x18\x05 \x03(\x0b\x32*.strmprivacy.api.entities.v1.KafkaExporterR\x0ekafkaExporters\"\x9f\x01\n\x08SinkTree\x12:\n\x04sink\x18\x01 \x01(\x0b\x32!.strmprivacy.api.entities.v1.SinkB\x03\xe0\x41\x02R\x04sink\x12S\n\x0f\x62\x61tch_exporters\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters:\x02\x18\x01\"\xc8\x06\n\x08\x42\x61tchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12N\n\x07\x63onsent\x18\x04 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x07\x63onsent\x12W\n\nencryption\x18\x05 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EncryptionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nencryption\x12\x65\n\x12\x65vent_contract_ref\x18\x06 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x65ventContractRef\x12[\n\x0e\x65ncrypted_data\x18\x07 \x01(\x0b\x32*.strmprivacy.api.entities.v1.EncryptedDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\rencryptedData\x12k\n\x14\x65ncryption_keys_data\x18\x08 \x01(\x0b\x32/.strmprivacy.api.entities.v1.EncryptionKeysDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x12\x65ncryptionKeysData\x12K\n\x0c\x64\x65rived_data\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.DerivedDataR\x0b\x64\x65rivedData\x12(\n\tpolicy_id\x18\n \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xf0\x01\n\x0f\x42\x61tchJobWrapper\x12Y\n\x14\x65ncryption_batch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobH\x00R\x12\x65ncryptionBatchJob\x12v\n\x1bmicro_aggregation_batch_job\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobH\x00R\x18microAggregationBatchJobB\n\n\x03job\x12\x03\xf8\x42\x01\"\x9a\x01\n\x10\x45xtendedBatchJob\x12\x46\n\tbatch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobB\x02\x18\x01R\x08\x62\x61tchJob\x12>\n\x03job\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.BatchJobWrapperR\x03job\"y\n\x0b\x42\x61tchJobRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x13\n\x02id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb9\x01\n\rBatchJobState\x12>\n\nstate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstateTime\x12I\n\x05state\x18\x02 \x01(\x0e\x32..strmprivacy.api.entities.v1.BatchJobStateTypeB\x03\xe0\x41\x03R\x05state\x12\x1d\n\x07message\x18\x03 \x01(\tB\x03\xe0\x41\x01R\x07message\"\xda\x02\n\x14\x44\x61taConnectorAndType\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRef\x12[\n\x0bpath_prefix\x18\x02 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x30\n\tfile_name\x18\x03 \x01(\tB\x13\xfa\x42\x10r\x0e\x32\t^[^\\pC]+$\xd0\x01\x01R\x08\x66ileName\x12L\n\tdata_type\x18\x04 \x01(\x0b\x32%.strmprivacy.api.entities.v1.DataTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x08\x64\x61taType\"}\n\x0e\x44\x61tabaseConfig\x12\"\n\x06schema\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\x06schema\x12\x1d\n\x05table\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05table\x12(\n\x07\x63olumns\x18\x03 \x03(\tB\x0e\xfa\x42\x0b\x92\x01\x08\"\x04r\x02\x10\x01(\x01R\x07\x63olumns\"\xbb\x01\n\rConsentConfig\x12\x39\n\x16\x64\x65\x66\x61ult_consent_levels\x18\x01 \x03(\x05\x42\x03\xe0\x41\x01R\x14\x64\x65\x66\x61ultConsentLevels\x12o\n\x17\x63onsent_level_extractor\x18\x02 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.ConsentLevelExtractorB\x03\xe0\x41\x01R\x15\x63onsentLevelExtractor\"\x89\x02\n\x15\x43onsentLevelExtractor\x12\x14\n\x05\x66ield\x18\x01 \x01(\tR\x05\x66ield\x12l\n\x0e\x66ield_patterns\x18\x02 \x03(\x0b\x32\x45.strmprivacy.api.entities.v1.ConsentLevelExtractor.FieldPatternsEntryR\rfieldPatterns\x1al\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12@\n\x05value\x18\x02 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentLevelsR\x05value:\x02\x38\x01\"\xa2\x01\n\x10\x45ncryptionConfig\x12\x61\n\x10timestamp_config\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.TimestampConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0ftimestampConfig\x12+\n\x12\x62\x61tch_job_group_id\x18\x02 \x01(\tR\x0f\x62\x61tchJobGroupId\"\xa1\x01\n\x0fTimestampConfig\x12*\n\x05\x66ield\x18\x01 \x01(\tB\x14\xfa\x42\x11r\x0f\x10\x04\x18\x32\x32\t^[^\\pC]+$R\x05\x66ield\x12\x1f\n\x06\x66ormat\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x66ormat\x12\x41\n\x11\x64\x65\x66\x61ult_time_zone\x18\x03 \x01(\x0b\x32\x15.google.type.TimeZoneR\x0f\x64\x65\x66\x61ultTimeZone\"d\n\rEncryptedData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"i\n\x12\x45ncryptionKeysData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"\xb1\x02\n\x0b\x44\x65rivedData\x12N\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x03\xe0\x41\x02R\x06target\x12%\n\x0e\x63onsent_levels\x18\x02 \x03(\x05R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x03 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12N\n\rmasked_fields\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\"\xb7\x04\n\x18MicroAggregationBatchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12\\\n\x0btarget_data\x18\x04 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\ntargetData\x12\x62\n\x11\x64\x61ta_contract_ref\x18\x05 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0f\x64\x61taContractRef\x12l\n\x12\x61ggregation_config\x18\x06 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.MicroAggregationConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x11\x61ggregationConfig\"\x80\x01\n\x16MicroAggregationConfig\x12\x37\n\x13minimum_k_anonymity\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x02R\x11minimumKAnonymity\x12-\n\x12\x61ggregation_fields\x18\x02 \x03(\tR\x11\x61ggregationFields\"\x92\x01\n\x0f\x44\x61taContractRef\x12\"\n\x06handle\x18\x01 \x01(\tB\n\xe0\x41\x02\xfa\x42\x04r\x02\x10\x04R\x06handle\x12&\n\x04name\x18\x02 \x01(\tB\x12\xfa\x42\x0fr\r\x10\x04\x18\x64\x32\x07^[^/]+$R\x04name\x12\x33\n\x07version\x18\x03 \x01(\tB\x19\xe0\x41\x02\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x94\x07\n\x0c\x44\x61taContract\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12H\n\x03ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12J\n\x05state\x18\x03 \x01(\x0e\x32/.strmprivacy.api.entities.v1.DataContract.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12$\n\tkey_field\x18\x05 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08keyField\x12[\n\npii_fields\x18\x06 \x03(\x0b\x32\x38.strmprivacy.api.entities.v1.DataContract.PiiFieldsEntryB\x02\x18\x01R\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12M\n\x08metadata\x18\x08 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataContractMetadataR\x08metadata\x12\x45\n\x06schema\x18\t \x01(\x0b\x32#.strmprivacy.api.entities.v1.SchemaB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06schema\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x12\'\n\nproject_id\x18\x0b \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\x12Q\n\x0e\x66ield_metadata\x18\x0c \x03(\x0b\x32*.strmprivacy.api.entities.v1.FieldMetadataR\rfieldMetadata\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\r\n\tIN_REVIEW\x10\x02\x12\n\n\x06\x41\x43TIVE\x10\x03\x12\x0c\n\x08\x41RCHIVED\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe1\x06\n\rFieldMetadata\x12\x1d\n\nfield_name\x18\x01 \x01(\tR\tfieldName\x12o\n\x14personal_data_config\x18\x02 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.PersonalDataConfigR\x12personalDataConfig\x12\x64\n\x15statistical_data_type\x18\x03 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.StatisticalDataTypeR\x13statisticalDataType\x12%\n\x0eordinal_values\x18\x04 \x03(\tR\rordinalValues\x12o\n\x14null_handling_config\x18\x05 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfigR\x12nullHandlingConfig\x1a\xc0\x01\n\x12PersonalDataConfig\x12\x1a\n\x06is_pii\x18\x01 \x01(\x08\x42\x03\xe0\x41\x02R\x05isPii\x12#\n\x0bis_quasi_id\x18\x02 \x01(\x08\x42\x03\xe0\x41\x02R\tisQuasiId\x12#\n\rpurpose_level\x18\x03 \x01(\x05R\x0cpurposeLevel\x12\x44\n\x1fgdpr_special_personal_data_type\x18\x04 \x01(\tR\x1bgdprSpecialPersonalDataType\x1a\xfe\x01\n\x12NullHandlingConfig\x12g\n\x04type\x18\x01 \x01(\x0e\x32N.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfig.NullHandlingTypeB\x03\xe0\x41\x02R\x04type\x12#\n\rdefault_value\x18\x02 \x01(\tR\x0c\x64\x65\x66\x61ultValue\"Z\n\x10NullHandlingType\x12\"\n\x1eNULL_HANDLING_TYPE_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x44ROP_RECORD\x10\x01\x12\x11\n\rDEFAULT_VALUE\x10\x02\"\x9f\x02\n\x14\x44\x61taContractMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\xbd\x02\n\x07Project\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x02\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12,\n\x0forganization_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x0eorganizationId\x12\x45\n\x05state\x18\x05 \x01(\x0e\x32*.strmprivacy.api.entities.v1.Project.StateB\x03\xe0\x41\x03R\x05state\"E\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bOPERATIONAL\x10\x01\x12\x14\n\x10PENDING_DELETION\x10\x02\"\xbe\x02\n\x04User\x12 \n\x05\x65mail\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\xd0\x01\x01`\x01R\x05\x65mail\x12\x1d\n\nfirst_name\x18\x02 \x01(\tR\tfirstName\x12\x1b\n\tlast_name\x18\x03 \x01(\tR\x08lastName\x12\x44\n\nuser_roles\x18\x04 \x03(\x0e\x32%.strmprivacy.api.entities.v1.UserRoleR\tuserRoles\x12\x35\n\x10\x65xternal_user_id\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12\x34\n\x0forganization_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0eorganizationId\x12%\n\x0e\x66unction_title\x18\x07 \x01(\tR\rfunctionTitle\"\x82\x01\n\x0ePurposeMapping\x12\x1d\n\x05level\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12#\n\x07purpose\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x02\x18\x64R\x07purpose\x12,\n\x0b\x64\x65scription\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x02\xd0\x01\x01R\x0b\x64\x65scription\"\xaf\x01\n\nGenericRef\x12J\n\x04type\x18\x01 \x01(\x0e\x32\x36.strmprivacy.api.entities.v1.GenericRef.GenericRefTypeR\x04type\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\"E\n\x0eGenericRefType\x12 \n\x1cGENERIC_REF_TYPE_UNSPECIFIED\x10\x00\x12\x11\n\rDATA_CONTRACT\x10\x01\"\xac\x02\n\x07\x43omment\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x45\n\x07\x63reator\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x00R\x07\x63reator\"\xb0\x02\n\x0f\x41uditTrailEntry\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x41\n\x05\x61\x63tor\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05\x61\x63tor*]\n\x08UserRole\x12\x19\n\x15USER_ROLE_UNSPECIFIED\x10\x00\x12\t\n\x05\x41\x44MIN\x10\x01\x12\x11\n\rPROJECT_ADMIN\x10\x02\x12\x0c\n\x08\x41PPROVER\x10\x03\x12\n\n\x06MEMBER\x10\x04*\x8d\x01\n\x11\x42\x61tchJobStateType\x12$\n BATCH_JOB_STATE_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0b\n\x07STARTED\x10\x02\x12\x12\n\x0e\x45RROR_STARTING\x10\x03\x12\x0b\n\x07RUNNING\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05\x12\t\n\x05\x45RROR\x10\x06*T\n\x10\x43onsentLevelType\x12\"\n\x1e\x43ONSENT_LEVEL_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nCUMULATIVE\x10\x01\x12\x0c\n\x08GRANULAR\x10\x02*=\n\x08SinkType\x12\x19\n\x15SINK_TYPE_UNSPECIFIED\x10\x00\x12\x06\n\x02S3\x10\x01\x12\n\n\x06GCLOUD\x10\x02\x1a\x02\x18\x01*M\n\rAuthMechanism\x12\x1e\n\x1a\x41UTH_MECHANISM_UNSPECIFIED\x10\x00\x12\x0e\n\nSASL_PLAIN\x10\x01\x12\x0c\n\x08SASL_SSL\x10\x02*C\n\nSchemaType\x12\x1b\n\x17SCHEMA_TYPE_UNSPECIFIED\x10\x00\x12\x08\n\x04\x41VRO\x10\x01\x12\x0e\n\nJSONSCHEMA\x10\x02*\x84\x01\n\x14SimpleSchemaNodeType\x12\'\n#SIMPLE_SCHEMA_NODE_TYPE_UNSPECIFIED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07INTEGER\x10\x04\x12\x08\n\x04LONG\x10\x05\x12\x08\n\x04NODE\x10\n*_\n\x13\x46ilterPublicPrivate\x12%\n!FILTER_PUBLIC_PRIVATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bONLY_PUBLIC\x10\x01\x12\x10\n\x0cONLY_PRIVATE\x10\x02*e\n\x13StatisticalDataType\x12%\n!STATISTICAL_DATA_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07NOMINAL\x10\x01\x12\x0b\n\x07ORDINAL\x10\x02\x12\r\n\tNUMERICAL\x10\x03*\x92\x01\n\x10SubscriptionPlan\x12!\n\x1dSUBSCRIPTION_PLAN_UNSPECIFIED\x10\x00\x12\x08\n\x04\x46REE\x10\x01\x12\x0c\n\x08\x42USINESS\x10\x02\x12\x0f\n\x0bSELF_HOSTED\x10\x03\x12\x18\n\x14\x41WS_MARKETPLACE_PAYG\x10\x04\x12\x18\n\x14\x41WS_MARKETPLACE_BYOL\x10\x05*c\n\x0c\x44\x61tabaseType\x12\x1d\n\x19\x44\x41TABASE_TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\t\n\x05MYSQL\x10\x02\x12\x0c\n\x08\x42IGQUERY\x10\x03\x12\r\n\tSNOWFLAKE\x10\x04\x42i\n\x1eio.strmprivacy.api.entities.v1P\x01ZEgithub.com/strmprivacy/api-definitions-go/v2/api/entities/v1;entitiesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-strmprivacy/api/entities/v1/entities_v1.proto\x12\x1bstrmprivacy.api.entities.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1agoogle/type/datetime.proto\x1a\x17validate/validate.proto\"\xab\x05\n\x06Stream\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x0b\xe0\x41\x02\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12-\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x0b\xfa\x42\x08r\x06\x18\xe8\x07\xd0\x01\x01R\x0b\x64\x65scription\x12/\n\x0e\x63onsent_levels\x18\x03 \x03(\x05\x42\x08\xfa\x42\x05\x92\x01\x02\x10\x32R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x04 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12\x1d\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x03\xe0\x41\x03R\x07\x65nabled\x12@\n\x06limits\x18\x06 \x01(\x0b\x32#.strmprivacy.api.entities.v1.LimitsB\x03\xe0\x41\x03R\x06limits\x12#\n\rlinked_stream\x18\x07 \x01(\tR\x0clinkedStream\x12$\n\x04tags\x18\x08 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x10\x14\x18\x01\"\x04r\x02\x18\x64R\x04tags\x12O\n\x0b\x63redentials\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.CredentialsB\x03\xe0\x41\x03R\x0b\x63redentials\x12N\n\rmasked_fields\x18\n \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\x12&\n\x0bkafka_topic\x18\x0b \x01(\tB\x05\x18\x01\xe0\x41\x03R\nkafkaTopic\x12(\n\tpolicy_id\x18\x0c \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xaa\x01\n\x0e\x45xtendedStream\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x03R\x06stream\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12\x17\n\x04uuid\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\"\n\nkey_stream\x18\x04 \x01(\x08\x42\x03\xe0\x41\x03R\tkeyStream\"\xc2\x01\n\x13\x45xtendedStreamGroup\x12U\n\rsource_stream\x18\x01 \x01(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamB\x03\xe0\x41\x03R\x0csourceStream\x12T\n\x0f\x64\x65rived_streams\x18\x02 \x03(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamR\x0e\x64\x65rivedStreams\"\x91\x03\n\x0cMaskedFields\x12\x1b\n\thash_type\x18\x01 \x01(\tR\x08hashType\x12\x37\n\x04seed\x18\x02 \x01(\tB#\xfa\x42 r\x1e\x18\xe8\x07\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04seed\x12\x63\n\x0e\x66ield_patterns\x18\x03 \x03(\x0b\x32<.strmprivacy.api.entities.v1.MaskedFields.FieldPatternsEntryR\rfieldPatterns\x1aw\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12K\n\x05value\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MaskedFields.PatternListR\x05value:\x02\x38\x01\x1aM\n\x0bPatternList\x12>\n\x0e\x66ield_patterns\x18\x01 \x03(\tB\x17\xfa\x42\x14\x92\x01\x11\x18\x01\"\rr\x0b\xba\x01\x08strmMetaR\rfieldPatterns\"R\n\x06Limits\x12\"\n\nevent_rate\x18\x01 \x01(\x03\x42\x03\xe0\x41\x03R\teventRate\x12$\n\x0b\x65vent_count\x18\x02 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\x92\x01\n\tKeyStream\x12@\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefB\x03\xe0\x41\x03R\x03ref\x12\x1d\n\x06status\x18\x02 \x01(\tB\x05\x18\x01\xe0\x41\x03R\x06status\x12$\n\x0bkafka_topic\x18\x03 \x01(\tB\x03\xe0\x41\x03R\nkafkaTopic\"\x9c\x01\n\tStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x9f\x01\n\x0cKeyStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xa1\x01\n\x0b\x43redentials\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\tbillingId\x12 \n\tclient_id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12\"\n\nproject_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"\xdf\x01\n\x04Sink\x12;\n\x03ref\x18\x01 \x01(\x0b\x32$.strmprivacy.api.entities.v1.SinkRefB\x03\xe0\x41\x02R\x03ref\x12G\n\tsink_type\x18\x02 \x01(\x0e\x32%.strmprivacy.api.entities.v1.SinkTypeB\x03\xe0\x41\x02R\x08sinkType\x12\x43\n\x06\x62ucket\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.BucketConfigH\x00R\x06\x62ucket:\x02\x18\x01\x42\x08\n\x06\x63onfig\"J\n\x07SinkRef\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name:\x02\x18\x01\"\x83\x01\n\x0c\x42ucketConfig\x12$\n\x0b\x62ucket_name\x18\x04 \x01(\tB\x03\xe0\x41\x02R\nbucketName\x12%\n\x0b\x63redentials\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x0b\x63redentials\x12&\n\x0f\x61ssume_role_arn\x18\x06 \x01(\tR\rassumeRoleArn\"\x9f\x05\n\rDataConnector\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\ts3_bucket\x18\x02 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.AwsS3BucketLocationH\x00R\x08s3Bucket\x12~\n\x1bgoogle_cloud_storage_bucket\x18\x03 \x01(\x0b\x32=.strmprivacy.api.entities.v1.GoogleCloudStorageBucketLocationH\x00R\x18googleCloudStorageBucket\x12\x81\x01\n\x1c\x61zure_blob_storage_container\x18\x04 \x01(\x0b\x32>.strmprivacy.api.entities.v1.AzureBlobStorageContainerLocationH\x00R\x19\x61zureBlobStorageContainer\x12P\n\rjdbc_location\x18\x07 \x01(\x0b\x32).strmprivacy.api.entities.v1.JdbcLocationH\x00R\x0cjdbcLocation\x12\x1f\n\x04uuid\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x04uuid\x12j\n\x12\x64\x65pendent_entities\x18\x06 \x01(\x0b\x32;.strmprivacy.api.entities.v1.DataConnectorDependentEntitiesR\x11\x64\x65pendentEntitiesB\x0f\n\x08location\x12\x03\xf8\x42\x01\"\xa0\x01\n\x10\x44\x61taConnectorRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb3\x02\n\x1e\x44\x61taConnectorDependentEntities\x12S\n\x0f\x62\x61tch_exporters\x18\x01 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12\x44\n\nbatch_jobs\x18\x02 \x03(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobR\tbatchJobs\x12v\n\x1cmicro_aggregation_batch_jobs\x18\x03 \x03(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobR\x19microAggregationBatchJobs\"\x9e\x01\n\x13\x41wsS3BucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\x12\x32\n\x0f\x61ssume_role_arn\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\rassumeRoleArn\"w\n GoogleCloudStorageBucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\"\x8a\x02\n!AzureBlobStorageContainerLocation\x12\x37\n\x13storage_account_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x11storageAccountUri\x12.\n\x0e\x63ontainer_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\rcontainerName\x12|\n\x18\x63lient_secret_credential\x18\x03 \x01(\x0b\x32\x38.strmprivacy.api.entities.v1.AzureClientSecretCredentialB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x16\x63lientSecretCredential\"\x97\x01\n\x1b\x41zureClientSecretCredential\x12$\n\ttenant_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08tenantId\x12$\n\tclient_id\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x63lientId\x12,\n\rclient_secret\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0c\x63lientSecret\"\xad\x01\n\x0cJdbcLocation\x12\"\n\x08jdbc_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07jdbcUri\x12)\n\x0bprivate_key\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xd0\x01\x01R\nprivateKey\x12N\n\rdatabase_type\x18\x03 \x01(\x0e\x32).strmprivacy.api.entities.v1.DatabaseTypeR\x0c\x64\x61tabaseType\"\xa3\x01\n\x08\x44\x61taType\x12:\n\x03\x63sv\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.CsvConfigH\x00R\x03\x63sv\x12I\n\x08\x64\x61tabase\x18\x02 \x01(\x0b\x32+.strmprivacy.api.entities.v1.DatabaseConfigH\x00R\x08\x64\x61tabaseB\x10\n\tdata_type\x12\x03\xf8\x42\x01\"%\n\tCsvConfig\x12\x18\n\x07\x63harset\x18\x01 \x01(\tR\x07\x63harset\"\x8a\x05\n\rBatchExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.BatchExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefH\x00R\tstreamRef\x12Q\n\x0ekey_stream_ref\x18\x03 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefH\x00R\x0ckeyStreamRef\x12I\n\x08interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x12\xe0\x41\x02\xfa\x42\x0c\xaa\x01\t\"\x03\x08\x90\x1c\x32\x02\x08\x1eR\x08interval\x12*\n\tsink_name\x18\x05 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\x08sinkName\x12[\n\x0bpath_prefix\x18\x06 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x36\n\x17include_existing_events\x18\x07 \x01(\x08R\x15includeExistingEvents\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x08 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRefB\x1f\n\x18stream_or_key_stream_ref\x12\x03\xf8\x42\x01\"\x98\x01\n\x15\x45xtendedBatchExporter\x12\x17\n\x04uuid\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12K\n\x08\x65xporter\x18\x03 \x01(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterB\x03\xe0\x41\x03R\x08\x65xporter\"\xa3\x01\n\x10\x42\x61tchExporterRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xfa\x01\n\x0cKafkaCluster\x12\x43\n\x03ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x02R\x03ref\x12\x30\n\x11\x62ootstrap_servers\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x10\x62ootstrapServers\x12V\n\x0e\x61uth_mechanism\x18\x03 \x01(\x0e\x32*.strmprivacy.api.entities.v1.AuthMechanismB\x03\xe0\x41\x02R\rauthMechanism\x12\x1b\n\ttoken_uri\x18\x04 \x01(\tR\x08tokenUri\"\x93\x01\n\x0fKafkaClusterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\xb3\x02\n\rKafkaExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.KafkaExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tstreamRef\x12H\n\x06target\x18\x03 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.KafkaExporterTargetR\x06target\x12<\n\x05users\x18\x04 \x03(\x0b\x32&.strmprivacy.api.entities.v1.KafkaUserR\x05users\"v\n\x10KafkaExporterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\x87\x02\n\x13KafkaExporterTarget\x12W\n\x0b\x63luster_ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nclusterRef\x12\x34\n\x05topic\x18\x02 \x01(\tB\x1e\xfa\x42\x1br\x19\x18\xf9\x01\x32\x11^[a-zA-Z0-9._-]+$\xd0\x01\x01R\x05topic\x12(\n\tclient_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08\x63lientId\x12\x37\n\rclient_secret\x18\x04 \x01(\tB\x12\xfa\x42\x0fr\r2\x08^[ -~]+$\xd0\x01\x01R\x0c\x63lientSecret\"\xc2\x02\n\tKafkaUser\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KafkaUserRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x33\n\x13kafka_exporter_name\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x11kafkaExporterName\x12\x19\n\x05topic\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12 \n\tclient_id\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x06 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12R\n\x0b\x63luster_ref\x18\x07 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x03R\nclusterRef\"n\n\x0cKafkaUserRef\x12!\n\nbilling_id\x18\x01 \x01(\tB\x02\x18\x01R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12\"\n\nproject_id\x18\x03 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"6\n\rConsentLevels\x12%\n\x0e\x63onsent_levels\x18\x01 \x03(\x05R\rconsentLevels\"\x9d\x01\n\x13\x43onsentLevelMapping\x12O\n\x03ref\x18\x01 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.ConsentLevelMappingRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\"\x8d\x01\n\x16\x43onsentLevelMappingRef\x12+\n\nbilling_id\x18\x01 \x01(\tB\x0c\x18\x01\xfa\x42\x07r\x05\x18\x00\xd0\x01\x01R\tbillingId\x12\x1d\n\x05level\x18\x02 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x86\x03\n\x06Policy\x12\x18\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\x02id\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0b\x64\x65scription\x12-\n\rlegal_grounds\x18\x04 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0clegalGrounds\x12\x30\n\x0eretention_days\x18\x05 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04(\x01@\x01R\rretentionDays\x12\x44\n\x05state\x18\x06 \x01(\x0e\x32).strmprivacy.api.entities.v1.Policy.StateB\x03\xe0\x41\x03R\x05state\"U\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATE_DRAFT\x10\x01\x12\x10\n\x0cSTATE_ACTIVE\x10\x02\x12\x12\n\x0eSTATE_ARCHIVED\x10\x03\"\xb6\x01\n\x12WindowedEventCount\x12>\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstartTime\x12:\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\x07\x65ndTime\x12$\n\x0b\x65vent_count\x18\x03 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\xaf\x01\n\tSchemaRef\x12\x1b\n\x06handle\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x06handle\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name\x12\x1d\n\x07version\x18\x03 \x01(\tB\x03\xe0\x41\x02R\x07version\x12M\n\x0bschema_type\x18\x04 \x01(\x0e\x32\'.strmprivacy.api.entities.v1.SchemaTypeB\x03\xe0\x41\x03R\nschemaType\"\xe9\x06\n\x06Schema\x12\x42\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x44\n\x05state\x18\x02 \x01(\x0e\x32).strmprivacy.api.entities.v1.Schema.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x03 \x01(\x08R\x08isPublic\x12\x1e\n\ndefinition\x18\x04 \x01(\tR\ndefinition\x12%\n\x0b\x66ingerprint\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x0b\x66ingerprint\x12G\n\x08metadata\x18\x06 \x01(\x0b\x32+.strmprivacy.api.entities.v1.SchemaMetadataR\x08metadata\x12_\n\rsimple_schema\x18\x07 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionR\x0csimpleSchema\x12\x13\n\x02id\x18\x08 \x01(\tB\x03\xe0\x41\x03R\x02id\x1a\xbf\x02\n\x16SimpleSchemaDefinition\x12$\n\x04name\x18\x01 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12]\n\tnamespace\x18\x02 \x01(\tB?\xfa\x42<r:25^([a-zA-Z_][a-zA-Z0-9_]*)(\\.[a-zA-Z_][a-zA-Z0-9_]*)*$\xd0\x01\x01R\tnamespace\x12\x1a\n\x03\x64oc\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\x12\x43\n\x05nodes\x18\x04 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12?\n\tavro_name\x18\x05 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe3\x02\n\x10SimpleSchemaNode\x12O\n\x04type\x18\x01 \x01(\x0e\x32\x31.strmprivacy.api.entities.v1.SimpleSchemaNodeTypeB\x08\xfa\x42\x05\x82\x01\x02 \x00R\x04type\x12$\n\x04name\x18\x02 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12?\n\tavro_name\x18\x07 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\x12\x1a\n\x08repeated\x18\x03 \x01(\x08R\x08repeated\x12\x1a\n\x08required\x18\x04 \x01(\x08R\x08required\x12\x43\n\x05nodes\x18\x05 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12\x1a\n\x03\x64oc\x18\x06 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\"\xd5\x02\n\x0eSchemaMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12*\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x30\n\x08icon_uri\x18\x04 \x01(\tB\x15\xfa\x42\x12r\x10:\x08https://\xd0\x01\x01\x88\x01\x01R\x07iconUri\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\x9a\x01\n\x10\x45ventContractRef\x12\x1f\n\x06handle\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x04R\x06handle\x12\x33\n\x04name\x18\x02 \x01(\tB\x1f\xfa\x42\x1cr\x1a\x10\x04\x18\x64\x32\x14^[\\pL\\pN\\pS\\pM\\pP]+$R\x04name\x12\x30\n\x07version\x18\x03 \x01(\tB\x16\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x82\x06\n\rEventContract\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x03\xe0\x41\x02R\x03ref\x12K\n\x05state\x18\x02 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.EventContract.StateB\x03\xe0\x41\x03R\x05state\x12J\n\nschema_ref\x18\x03 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x03\xe0\x41\x02R\tschemaRef\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12 \n\tkey_field\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x08keyField\x12X\n\npii_fields\x18\x06 \x03(\x0b\x32\x39.strmprivacy.api.entities.v1.EventContract.PiiFieldsEntryR\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12N\n\x08metadata\x18\x08 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.EventContractMetadataR\x08metadata\x12\x0e\n\x02id\x18\t \x01(\tR\x02id\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"b\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\"\xc0\x02\n\x15\x45ventContractMetadata\x12\x19\n\x05title\x18\x01 \x01(\tB\x03\xe0\x41\x01R\x05title\x12%\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x03\xe0\x41\x01R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x1e\n\x08icon_uri\x18\x04 \x01(\tB\x03\xe0\x41\x01R\x07iconUri\x12?\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelB\x03\xe0\x41\x01R\x06labels\x12\x1d\n\x07\x64omains\x18\x06 \x03(\tB\x03\xe0\x41\x01R\x07\x64omains\x12#\n\nindustries\x18\x07 \x03(\tB\x03\xe0\x41\x01R\nindustries\"8\n\x05Label\x12\x19\n\x03key\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"l\n\nValidation\x12\x1d\n\x05\x66ield\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05\x66ield\x12 \n\x04type\x18\x02 \x01(\tB\x0c\xfa\x42\tr\x07R\x05regexR\x04type\x12\x1d\n\x05value\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05value\"\xfe\x02\n\nStreamTree\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x02R\x06stream\x12\x45\n\nkey_stream\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.KeyStreamR\tkeyStream\x12=\n\x07\x64\x65rived\x18\x03 \x03(\x0b\x32#.strmprivacy.api.entities.v1.StreamR\x07\x64\x65rived\x12S\n\x0f\x62\x61tch_exporters\x18\x04 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12S\n\x0fkafka_exporters\x18\x05 \x03(\x0b\x32*.strmprivacy.api.entities.v1.KafkaExporterR\x0ekafkaExporters\"\x9f\x01\n\x08SinkTree\x12:\n\x04sink\x18\x01 \x01(\x0b\x32!.strmprivacy.api.entities.v1.SinkB\x03\xe0\x41\x02R\x04sink\x12S\n\x0f\x62\x61tch_exporters\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters:\x02\x18\x01\"\xc8\x06\n\x08\x42\x61tchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12N\n\x07\x63onsent\x18\x04 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x07\x63onsent\x12W\n\nencryption\x18\x05 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EncryptionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nencryption\x12\x65\n\x12\x65vent_contract_ref\x18\x06 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x65ventContractRef\x12[\n\x0e\x65ncrypted_data\x18\x07 \x01(\x0b\x32*.strmprivacy.api.entities.v1.EncryptedDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\rencryptedData\x12k\n\x14\x65ncryption_keys_data\x18\x08 \x01(\x0b\x32/.strmprivacy.api.entities.v1.EncryptionKeysDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x12\x65ncryptionKeysData\x12K\n\x0c\x64\x65rived_data\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.DerivedDataR\x0b\x64\x65rivedData\x12(\n\tpolicy_id\x18\n \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xf0\x01\n\x0f\x42\x61tchJobWrapper\x12Y\n\x14\x65ncryption_batch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobH\x00R\x12\x65ncryptionBatchJob\x12v\n\x1bmicro_aggregation_batch_job\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobH\x00R\x18microAggregationBatchJobB\n\n\x03job\x12\x03\xf8\x42\x01\"\x9a\x01\n\x10\x45xtendedBatchJob\x12\x46\n\tbatch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobB\x02\x18\x01R\x08\x62\x61tchJob\x12>\n\x03job\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.BatchJobWrapperR\x03job\"y\n\x0b\x42\x61tchJobRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x13\n\x02id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb9\x01\n\rBatchJobState\x12>\n\nstate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstateTime\x12I\n\x05state\x18\x02 \x01(\x0e\x32..strmprivacy.api.entities.v1.BatchJobStateTypeB\x03\xe0\x41\x03R\x05state\x12\x1d\n\x07message\x18\x03 \x01(\tB\x03\xe0\x41\x01R\x07message\"\xda\x02\n\x14\x44\x61taConnectorAndType\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRef\x12[\n\x0bpath_prefix\x18\x02 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x30\n\tfile_name\x18\x03 \x01(\tB\x13\xfa\x42\x10r\x0e\x32\t^[^\\pC]+$\xd0\x01\x01R\x08\x66ileName\x12L\n\tdata_type\x18\x04 \x01(\x0b\x32%.strmprivacy.api.entities.v1.DataTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x08\x64\x61taType\"}\n\x0e\x44\x61tabaseConfig\x12\"\n\x06schema\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\x06schema\x12\x1d\n\x05table\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05table\x12(\n\x07\x63olumns\x18\x03 \x03(\tB\x0e\xfa\x42\x0b\x92\x01\x08\"\x04r\x02\x10\x01(\x01R\x07\x63olumns\"\xbb\x01\n\rConsentConfig\x12\x39\n\x16\x64\x65\x66\x61ult_consent_levels\x18\x01 \x03(\x05\x42\x03\xe0\x41\x01R\x14\x64\x65\x66\x61ultConsentLevels\x12o\n\x17\x63onsent_level_extractor\x18\x02 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.ConsentLevelExtractorB\x03\xe0\x41\x01R\x15\x63onsentLevelExtractor\"\x89\x02\n\x15\x43onsentLevelExtractor\x12\x14\n\x05\x66ield\x18\x01 \x01(\tR\x05\x66ield\x12l\n\x0e\x66ield_patterns\x18\x02 \x03(\x0b\x32\x45.strmprivacy.api.entities.v1.ConsentLevelExtractor.FieldPatternsEntryR\rfieldPatterns\x1al\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12@\n\x05value\x18\x02 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentLevelsR\x05value:\x02\x38\x01\"\xa2\x01\n\x10\x45ncryptionConfig\x12\x61\n\x10timestamp_config\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.TimestampConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0ftimestampConfig\x12+\n\x12\x62\x61tch_job_group_id\x18\x02 \x01(\tR\x0f\x62\x61tchJobGroupId\"\xa1\x01\n\x0fTimestampConfig\x12*\n\x05\x66ield\x18\x01 \x01(\tB\x14\xfa\x42\x11r\x0f\x10\x04\x18\x32\x32\t^[^\\pC]+$R\x05\x66ield\x12\x1f\n\x06\x66ormat\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x66ormat\x12\x41\n\x11\x64\x65\x66\x61ult_time_zone\x18\x03 \x01(\x0b\x32\x15.google.type.TimeZoneR\x0f\x64\x65\x66\x61ultTimeZone\"d\n\rEncryptedData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"i\n\x12\x45ncryptionKeysData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"\xb1\x02\n\x0b\x44\x65rivedData\x12N\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x03\xe0\x41\x02R\x06target\x12%\n\x0e\x63onsent_levels\x18\x02 \x03(\x05R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x03 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12N\n\rmasked_fields\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\"\xb7\x04\n\x18MicroAggregationBatchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12\\\n\x0btarget_data\x18\x04 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\ntargetData\x12\x62\n\x11\x64\x61ta_contract_ref\x18\x05 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0f\x64\x61taContractRef\x12l\n\x12\x61ggregation_config\x18\x06 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.MicroAggregationConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x11\x61ggregationConfig\"\x80\x01\n\x16MicroAggregationConfig\x12\x37\n\x13minimum_k_anonymity\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x02R\x11minimumKAnonymity\x12-\n\x12\x61ggregation_fields\x18\x02 \x03(\tR\x11\x61ggregationFields\"\x92\x01\n\x0f\x44\x61taContractRef\x12\"\n\x06handle\x18\x01 \x01(\tB\n\xe0\x41\x02\xfa\x42\x04r\x02\x10\x04R\x06handle\x12&\n\x04name\x18\x02 \x01(\tB\x12\xfa\x42\x0fr\r\x10\x04\x18\x64\x32\x07^[^/]+$R\x04name\x12\x33\n\x07version\x18\x03 \x01(\tB\x19\xe0\x41\x02\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x94\x07\n\x0c\x44\x61taContract\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12H\n\x03ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12J\n\x05state\x18\x03 \x01(\x0e\x32/.strmprivacy.api.entities.v1.DataContract.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12$\n\tkey_field\x18\x05 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08keyField\x12[\n\npii_fields\x18\x06 \x03(\x0b\x32\x38.strmprivacy.api.entities.v1.DataContract.PiiFieldsEntryB\x02\x18\x01R\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12M\n\x08metadata\x18\x08 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataContractMetadataR\x08metadata\x12\x45\n\x06schema\x18\t \x01(\x0b\x32#.strmprivacy.api.entities.v1.SchemaB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06schema\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x12\'\n\nproject_id\x18\x0b \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\x12Q\n\x0e\x66ield_metadata\x18\x0c \x03(\x0b\x32*.strmprivacy.api.entities.v1.FieldMetadataR\rfieldMetadata\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\r\n\tIN_REVIEW\x10\x02\x12\n\n\x06\x41\x43TIVE\x10\x03\x12\x0c\n\x08\x41RCHIVED\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe1\x06\n\rFieldMetadata\x12\x1d\n\nfield_name\x18\x01 \x01(\tR\tfieldName\x12o\n\x14personal_data_config\x18\x02 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.PersonalDataConfigR\x12personalDataConfig\x12\x64\n\x15statistical_data_type\x18\x03 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.StatisticalDataTypeR\x13statisticalDataType\x12%\n\x0eordinal_values\x18\x04 \x03(\tR\rordinalValues\x12o\n\x14null_handling_config\x18\x05 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfigR\x12nullHandlingConfig\x1a\xc0\x01\n\x12PersonalDataConfig\x12\x1a\n\x06is_pii\x18\x01 \x01(\x08\x42\x03\xe0\x41\x02R\x05isPii\x12#\n\x0bis_quasi_id\x18\x02 \x01(\x08\x42\x03\xe0\x41\x02R\tisQuasiId\x12#\n\rpurpose_level\x18\x03 \x01(\x05R\x0cpurposeLevel\x12\x44\n\x1fgdpr_special_personal_data_type\x18\x04 \x01(\tR\x1bgdprSpecialPersonalDataType\x1a\xfe\x01\n\x12NullHandlingConfig\x12g\n\x04type\x18\x01 \x01(\x0e\x32N.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfig.NullHandlingTypeB\x03\xe0\x41\x02R\x04type\x12#\n\rdefault_value\x18\x02 \x01(\tR\x0c\x64\x65\x66\x61ultValue\"Z\n\x10NullHandlingType\x12\"\n\x1eNULL_HANDLING_TYPE_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x44ROP_RECORD\x10\x01\x12\x11\n\rDEFAULT_VALUE\x10\x02\"\x9f\x02\n\x14\x44\x61taContractMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\xbd\x02\n\x07Project\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x02\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12,\n\x0forganization_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x0eorganizationId\x12\x45\n\x05state\x18\x05 \x01(\x0e\x32*.strmprivacy.api.entities.v1.Project.StateB\x03\xe0\x41\x03R\x05state\"E\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bOPERATIONAL\x10\x01\x12\x14\n\x10PENDING_DELETION\x10\x02\"\xbe\x02\n\x04User\x12 \n\x05\x65mail\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\xd0\x01\x01`\x01R\x05\x65mail\x12\x1d\n\nfirst_name\x18\x02 \x01(\tR\tfirstName\x12\x1b\n\tlast_name\x18\x03 \x01(\tR\x08lastName\x12\x44\n\nuser_roles\x18\x04 \x03(\x0e\x32%.strmprivacy.api.entities.v1.UserRoleR\tuserRoles\x12\x35\n\x10\x65xternal_user_id\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12\x34\n\x0forganization_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0eorganizationId\x12%\n\x0e\x66unction_title\x18\x07 \x01(\tR\rfunctionTitle\"\x82\x01\n\x0ePurposeMapping\x12\x1d\n\x05level\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12#\n\x07purpose\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x02\x18\x64R\x07purpose\x12,\n\x0b\x64\x65scription\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x02\xd0\x01\x01R\x0b\x64\x65scription\"\xaf\x01\n\nGenericRef\x12J\n\x04type\x18\x01 \x01(\x0e\x32\x36.strmprivacy.api.entities.v1.GenericRef.GenericRefTypeR\x04type\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\"E\n\x0eGenericRefType\x12 \n\x1cGENERIC_REF_TYPE_UNSPECIFIED\x10\x00\x12\x11\n\rDATA_CONTRACT\x10\x01\"\xac\x02\n\x07\x43omment\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x45\n\x07\x63reator\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x00R\x07\x63reator\"\xfd\x02\n\x0f\x41uditTrailEntry\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x41\n\x05\x61\x63tor\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05\x61\x63tor\x12*\n\nproject_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\x12\x1f\n\x0b\x65ntity_name\x18\x07 \x01(\tR\nentityName*]\n\x08UserRole\x12\x19\n\x15USER_ROLE_UNSPECIFIED\x10\x00\x12\t\n\x05\x41\x44MIN\x10\x01\x12\x11\n\rPROJECT_ADMIN\x10\x02\x12\x0c\n\x08\x41PPROVER\x10\x03\x12\n\n\x06MEMBER\x10\x04*\x8d\x01\n\x11\x42\x61tchJobStateType\x12$\n BATCH_JOB_STATE_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0b\n\x07STARTED\x10\x02\x12\x12\n\x0e\x45RROR_STARTING\x10\x03\x12\x0b\n\x07RUNNING\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05\x12\t\n\x05\x45RROR\x10\x06*T\n\x10\x43onsentLevelType\x12\"\n\x1e\x43ONSENT_LEVEL_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nCUMULATIVE\x10\x01\x12\x0c\n\x08GRANULAR\x10\x02*=\n\x08SinkType\x12\x19\n\x15SINK_TYPE_UNSPECIFIED\x10\x00\x12\x06\n\x02S3\x10\x01\x12\n\n\x06GCLOUD\x10\x02\x1a\x02\x18\x01*M\n\rAuthMechanism\x12\x1e\n\x1a\x41UTH_MECHANISM_UNSPECIFIED\x10\x00\x12\x0e\n\nSASL_PLAIN\x10\x01\x12\x0c\n\x08SASL_SSL\x10\x02*C\n\nSchemaType\x12\x1b\n\x17SCHEMA_TYPE_UNSPECIFIED\x10\x00\x12\x08\n\x04\x41VRO\x10\x01\x12\x0e\n\nJSONSCHEMA\x10\x02*\x84\x01\n\x14SimpleSchemaNodeType\x12\'\n#SIMPLE_SCHEMA_NODE_TYPE_UNSPECIFIED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07INTEGER\x10\x04\x12\x08\n\x04LONG\x10\x05\x12\x08\n\x04NODE\x10\n*_\n\x13\x46ilterPublicPrivate\x12%\n!FILTER_PUBLIC_PRIVATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bONLY_PUBLIC\x10\x01\x12\x10\n\x0cONLY_PRIVATE\x10\x02*e\n\x13StatisticalDataType\x12%\n!STATISTICAL_DATA_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07NOMINAL\x10\x01\x12\x0b\n\x07ORDINAL\x10\x02\x12\r\n\tNUMERICAL\x10\x03*\x92\x01\n\x10SubscriptionPlan\x12!\n\x1dSUBSCRIPTION_PLAN_UNSPECIFIED\x10\x00\x12\x08\n\x04\x46REE\x10\x01\x12\x0c\n\x08\x42USINESS\x10\x02\x12\x0f\n\x0bSELF_HOSTED\x10\x03\x12\x18\n\x14\x41WS_MARKETPLACE_PAYG\x10\x04\x12\x18\n\x14\x41WS_MARKETPLACE_BYOL\x10\x05*c\n\x0c\x44\x61tabaseType\x12\x1d\n\x19\x44\x41TABASE_TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\t\n\x05MYSQL\x10\x02\x12\x0c\n\x08\x42IGQUERY\x10\x03\x12\r\n\tSNOWFLAKE\x10\x04\x42i\n\x1eio.strmprivacy.api.entities.v1P\x01ZEgithub.com/strmprivacy/api-definitions-go/v2/api/entities/v1;entitiesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'strmprivacy.api.entities.v1.entities_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036io.strmprivacy.api.entities.v1P\001ZEgithub.com/strmprivacy/api-definitions-go/v2/api/entities/v1;entities'
@@ -478,36 +478,38 @@
   _AUDITTRAILENTRY.fields_by_name['create_time']._serialized_options = b'\372B\005\262\001\002\010\000'
   _AUDITTRAILENTRY.fields_by_name['entity_ref']._options = None
   _AUDITTRAILENTRY.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _AUDITTRAILENTRY.fields_by_name['content']._options = None
   _AUDITTRAILENTRY.fields_by_name['content']._serialized_options = b'\372B\007r\005\020\001\030\350\007'
   _AUDITTRAILENTRY.fields_by_name['actor']._options = None
   _AUDITTRAILENTRY.fields_by_name['actor']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _USERROLE._serialized_start=20071
-  _USERROLE._serialized_end=20164
-  _BATCHJOBSTATETYPE._serialized_start=20167
-  _BATCHJOBSTATETYPE._serialized_end=20308
-  _CONSENTLEVELTYPE._serialized_start=20310
-  _CONSENTLEVELTYPE._serialized_end=20394
-  _SINKTYPE._serialized_start=20396
-  _SINKTYPE._serialized_end=20457
-  _AUTHMECHANISM._serialized_start=20459
-  _AUTHMECHANISM._serialized_end=20536
-  _SCHEMATYPE._serialized_start=20538
-  _SCHEMATYPE._serialized_end=20605
-  _SIMPLESCHEMANODETYPE._serialized_start=20608
-  _SIMPLESCHEMANODETYPE._serialized_end=20740
-  _FILTERPUBLICPRIVATE._serialized_start=20742
-  _FILTERPUBLICPRIVATE._serialized_end=20837
-  _STATISTICALDATATYPE._serialized_start=20839
-  _STATISTICALDATATYPE._serialized_end=20940
-  _SUBSCRIPTIONPLAN._serialized_start=20943
-  _SUBSCRIPTIONPLAN._serialized_end=21089
-  _DATABASETYPE._serialized_start=21091
-  _DATABASETYPE._serialized_end=21190
+  _AUDITTRAILENTRY.fields_by_name['project_id']._options = None
+  _AUDITTRAILENTRY.fields_by_name['project_id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
+  _USERROLE._serialized_start=20148
+  _USERROLE._serialized_end=20241
+  _BATCHJOBSTATETYPE._serialized_start=20244
+  _BATCHJOBSTATETYPE._serialized_end=20385
+  _CONSENTLEVELTYPE._serialized_start=20387
+  _CONSENTLEVELTYPE._serialized_end=20471
+  _SINKTYPE._serialized_start=20473
+  _SINKTYPE._serialized_end=20534
+  _AUTHMECHANISM._serialized_start=20536
+  _AUTHMECHANISM._serialized_end=20613
+  _SCHEMATYPE._serialized_start=20615
+  _SCHEMATYPE._serialized_end=20682
+  _SIMPLESCHEMANODETYPE._serialized_start=20685
+  _SIMPLESCHEMANODETYPE._serialized_end=20817
+  _FILTERPUBLICPRIVATE._serialized_start=20819
+  _FILTERPUBLICPRIVATE._serialized_end=20914
+  _STATISTICALDATATYPE._serialized_start=20916
+  _STATISTICALDATATYPE._serialized_end=21017
+  _SUBSCRIPTIONPLAN._serialized_start=21020
+  _SUBSCRIPTIONPLAN._serialized_end=21166
+  _DATABASETYPE._serialized_start=21168
+  _DATABASETYPE._serialized_end=21267
   _STREAM._serialized_start=230
   _STREAM._serialized_end=913
   _EXTENDEDSTREAM._serialized_start=916
   _EXTENDEDSTREAM._serialized_end=1086
   _EXTENDEDSTREAMGROUP._serialized_start=1089
   _EXTENDEDSTREAMGROUP._serialized_end=1283
   _MASKEDFIELDS._serialized_start=1286
@@ -677,9 +679,9 @@
   _GENERICREF._serialized_start=19284
   _GENERICREF._serialized_end=19459
   _GENERICREF_GENERICREFTYPE._serialized_start=19390
   _GENERICREF_GENERICREFTYPE._serialized_end=19459
   _COMMENT._serialized_start=19462
   _COMMENT._serialized_end=19762
   _AUDITTRAILENTRY._serialized_start=19765
-  _AUDITTRAILENTRY._serialized_end=20069
+  _AUDITTRAILENTRY._serialized_end=20146
 # @@protoc_insertion_point(module_scope)
```

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/entities_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/paging_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/paging_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/PKG-INFO` & `strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.3.0
+Version: 3.4.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/SOURCES.txt` & `strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

