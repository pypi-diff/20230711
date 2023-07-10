# Comparing `tmp/modelaapi-0.6.221.tar.gz` & `tmp/modelaapi-0.6.223.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.221.tar", last modified: Mon Jul 10 19:36:06 2023, max compression
+gzip compressed data, was "modelaapi-0.6.223.tar", last modified: Mon Jul 10 23:33:40 2023, max compression
```

## Comparing `modelaapi-0.6.221.tar` & `modelaapi-0.6.223.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.221/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.221/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.221/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.221/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.221/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.221/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.221/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 19:36:06.135758 modelaapi-0.6.221/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.221/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22695 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    56885 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4692 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-10 19:35:45.000000 modelaapi-0.6.221/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.221/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.221/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-10 19:36:06.139758 modelaapi-0.6.221/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.221/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.467099 modelaapi-0.6.223/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.223/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.223/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.223/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.223/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.223/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.223/MANIFEST.in
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.223/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 23:33:40.467099 modelaapi-0.6.223/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.223/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.419099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22698 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.423099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    56885 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4692 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.427099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.431099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.435099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.439099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.443099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.447099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.451099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.455099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-10 23:06:08.000000 modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-10 23:06:08.000000 modelaapi-0.6.223/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-10 23:06:08.000000 modelaapi-0.6.223/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 23:06:08.000000 modelaapi-0.6.223/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/api/apps/v1/generated_pb2.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.459099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.463099 modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-10 23:06:08.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.467099 modelaapi-0.6.223/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.223/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.223/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.223/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.223/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.223/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-10 23:33:36.000000 modelaapi-0.6.223/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 23:33:40.467099 modelaapi-0.6.223/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 23:33:40.000000 modelaapi-0.6.223/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-10 23:33:40.000000 modelaapi-0.6.223/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-10 23:33:40.000000 modelaapi-0.6.223/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-10 23:33:40.000000 modelaapi-0.6.223/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.223/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-10 23:33:40.000000 modelaapi-0.6.223/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-10 23:33:40.000000 modelaapi-0.6.223/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.223/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-10 23:33:40.467099 modelaapi-0.6.223/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.223/setup.py
```

### Comparing `modelaapi-0.6.221/CONTRIBUTING.rst` & `modelaapi-0.6.223/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/LICENSE.txt` & `modelaapi-0.6.223/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/Makefile` & `modelaapi-0.6.223/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/PKG-INFO` & `modelaapi-0.6.223/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.221
+Version: 0.6.223
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.221
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.223
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.221
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.223
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.221/README.md` & `modelaapi-0.6.223/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.223/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_training_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xd2\x06\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12R\n\x05input\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12;\n\x0eservingSiteRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08modelRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rcreateDataset\x18\x07 \x01(\x08\x12\x0f\n\x07labeled\x18\x08 \x01(\x08\x12U\n\tunitTests\x18\t \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12\r\n\x05\x61\x62ort\x18\x0c \x01(\x08\x12g\n\x0c\x66orecastSpec\x18\r \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12v\n\x11partitionLocation\x18\x0e \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x16\n\x0emodelClassName\x18\x0f \x01(\t\"\xcb\x05\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xd8\x06\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12R\n\x05input\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12;\n\x0eservingSiteRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08modelRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rcreateDataset\x18\x07 \x01(\x08\x12\x0f\n\x07labeled\x18\x08 \x01(\x08\x12[\n\tunitTests\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12\r\n\x05\x61\x62ort\x18\x0c \x01(\x08\x12g\n\x0c\x66orecastSpec\x18\r \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12v\n\x11partitionLocation\x18\x0e \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x16\n\x0emodelClassName\x18\x0f \x01(\t\"\xcb\x05\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1'
@@ -89,25 +89,25 @@
   _PREDICTIONCACHESPEC._serialized_start=5972
   _PREDICTIONCACHESPEC._serialized_end=6103
   _PREDICTIONLIST._serialized_start=6106
   _PREDICTIONLIST._serialized_end=6274
   _PREDICTIONLOGGINGSPEC._serialized_start=6277
   _PREDICTIONLOGGINGSPEC._serialized_end=6536
   _PREDICTIONSPEC._serialized_start=6539
-  _PREDICTIONSPEC._serialized_end=7389
-  _PREDICTIONSTATUS._serialized_start=7392
-  _PREDICTIONSTATUS._serialized_end=8107
-  _PREDICTOR._serialized_start=8110
-  _PREDICTOR._serialized_end=8369
-  _PREDICTORLIST._serialized_start=8372
-  _PREDICTORLIST._serialized_end=8538
-  _PREDICTORSPEC._serialized_start=8541
-  _PREDICTORSPEC._serialized_end=10254
-  _PREDICTORSTATUS._serialized_start=10257
-  _PREDICTORSTATUS._serialized_end=11111
-  _PREDICTORLETSTATUS._serialized_start=11114
-  _PREDICTORLETSTATUS._serialized_end=11504
-  _PROGRESSIVESPEC._serialized_start=11506
-  _PROGRESSIVESPEC._serialized_end=11588
-  _VALIDATIONERROR._serialized_start=11590
-  _VALIDATIONERROR._serialized_end=11681
+  _PREDICTIONSPEC._serialized_end=7395
+  _PREDICTIONSTATUS._serialized_start=7398
+  _PREDICTIONSTATUS._serialized_end=8113
+  _PREDICTOR._serialized_start=8116
+  _PREDICTOR._serialized_end=8375
+  _PREDICTORLIST._serialized_start=8378
+  _PREDICTORLIST._serialized_end=8544
+  _PREDICTORSPEC._serialized_start=8547
+  _PREDICTORSPEC._serialized_end=10260
+  _PREDICTORSTATUS._serialized_start=10263
+  _PREDICTORSTATUS._serialized_end=11117
+  _PREDICTORLETSTATUS._serialized_start=11120
+  _PREDICTORLETSTATUS._serialized_end=11510
+  _PROGRESSIVESPEC._serialized_start=11512
+  _PROGRESSIVESPEC._serialized_end=11594
+  _VALIDATIONERROR._serialized_start=11596
+  _VALIDATIONERROR._serialized_end=11687
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.223/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/google/api/annotations_pb2.py` & `modelaapi-0.6.223/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/google/api/http_pb2.py` & `modelaapi-0.6.223/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.223/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/modelaapi/consts.py` & `modelaapi-0.6.223/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/modelaapi/custom_transformers.py` & `modelaapi-0.6.223/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/modelaapi/graykite_model.py` & `modelaapi-0.6.223/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/modelaapi/ts.py` & `modelaapi-0.6.223/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/modelaapi/version.py` & `modelaapi-0.6.223/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 221,
+    "micro": 223,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.221/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.223/modelaapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.221
+Version: 0.6.223
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.221
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.223
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.221
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.223
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.221/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.223/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/setup.cfg` & `modelaapi-0.6.223/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.221/setup.py` & `modelaapi-0.6.223/setup.py`

 * *Files identical despite different names*

