# Comparing `tmp/tierkreis-0.1.0.tar.gz` & `tmp/tierkreis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tierkreis-0.1.0.tar", last modified: Mon Nov  7 18:00:38 2022, max compression
+gzip compressed data, was "tierkreis-0.2.0.tar", last modified: Tue Jul 11 11:13:42 2023, max compression
```

## Comparing `tierkreis-0.1.0.tar` & `tierkreis-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-11-07 18:00:38.460405 tierkreis-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-11-07 18:00:13.000000 tierkreis-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-11-07 18:00:13.000000 tierkreis-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 18:00:38.460405 tierkreis-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.456405 tierkreis-0.1.0/tierkreis/
--rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.456405 tierkreis-0.1.0/tierkreis/_build/
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/_build/generate_protos.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    29054 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    10530 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.456405 tierkreis-0.1.0/tierkreis/client/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/client/runtime_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10154 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/client/server_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.456405 tierkreis-0.1.0/tierkreis/common_types/
--rw-r--r--   0 runner    (1001) docker     (121)     4569 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23524 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/common_types/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/function.py
--rw-r--r--   0 runner    (1001) docker     (121)    14567 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/graphviz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/protos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis/core/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.456405 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/graph/
--rw-r--r--   0 runner    (1001) docker     (121)     6739 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)    10390 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/signature/
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/worker/
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/signature.py
--rw-r--r--   0 runner    (1001) docker     (121)    22257 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/tierkreis_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/tierkreis_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)     6781 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/type_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/type_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)    14425 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    20740 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/core/values.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/pyruntime/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/pyruntime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23098 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/pyruntime/python_builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9448 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/pyruntime/python_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.460405 tierkreis-0.1.0/tierkreis/worker/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/callback.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8977 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/prelude.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)     9663 2022-11-07 18:00:13.000000 tierkreis-0.1.0/tierkreis/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:00:38.456405 tierkreis-0.1.0/tierkreis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-07 18:00:38.000000 tierkreis-0.1.0/tierkreis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-11 11:13:42.257420 tierkreis-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-11 11:13:20.000000 tierkreis-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-11 11:13:20.000000 tierkreis-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 11:13:42.257420 tierkreis-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.253419 tierkreis-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31703 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_commontypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_pyruntime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_pytket_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_tierkreis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tests/test_type_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.253419 tierkreis-0.2.0/tierkreis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.253419 tierkreis-0.2.0/tierkreis/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/_build/generate_protos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.253419 tierkreis-0.2.0/tierkreis/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/client/runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/client/server_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.253419 tierkreis-0.2.0/tierkreis/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/common_types/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis/core/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.249420 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/signature/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/tierkreis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/tierkreis_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/type_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/type_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/core/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/pyruntime/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/pyruntime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/pyruntime/python_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/pyruntime/python_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.257420 tierkreis-0.2.0/tierkreis/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/prelude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-11 11:13:20.000000 tierkreis-0.2.0/tierkreis/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:13:42.253419 tierkreis-0.2.0/tierkreis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 11:13:42.000000 tierkreis-0.2.0/tierkreis.egg-info/top_level.txt
```

### Comparing `tierkreis-0.1.0/PKG-INFO` & `tierkreis-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tierkreis
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python client and utilities for tierkreis.
 Author-email: Seyon Sivarajah <seyon.sivarajah@quantinuum.com>, Lukas Heidemann <lukas.heidemann@quantinuum.com>, John Children <john.children@quantinuum.com>, Alan Lawrence <alan.lawrence@quantinuum.com>
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docker
 Provides-Extra: telemetry
 Provides-Extra: commontypes
```

### Comparing `tierkreis-0.1.0/README.md` & `tierkreis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/pyproject.toml` & `tierkreis-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     "betterproto[compiler]==2.0.0b5",
     "protobuf>=3.19,<4",  # Restrict version to maintain compatibility with opentelemetry
     "grpclib>=0.4.3rc,<0.5", # pre-release to support python 3.10
     "networkx>=2.6.3,<3",
     "graphviz>=0.18,<0.19",
     "keyring==23.2",
     "keyrings.alt==4.1",
-    "click>=8.0.3,<9",
+    "click==8.1.3", # 8.1.4 causes mypy fails
     "yachalk>=0.1.4,<0.2",
+    "requests>=2.31,<3"
 ]
 
 [project.scripts]
 tkrs = 'tierkreis.cli:cli'
 
 [project.optional-dependencies]
 docker = [ "docker>=5,<6"]
@@ -39,14 +40,15 @@
 ]
 lint = [
     "black>=22.1,<23",
     "mypy>=0.981,<0.982",
     "pylint~=2.13,!=2.13.6",
     "isort~=5.10",
     "types-setuptools>=57.4.2,<58",
+    "types-requests>=2.31,<3",
     "types-python-dateutil>=2.8.2,<3",
     "tierkreis[sc22-example,telemetry,docker]"
 ]
 test = [
     "pytest>=6.2,<7",
     "pytest-asyncio>=0.16,<0.17",
 ]
```

### Comparing `tierkreis-0.1.0/tierkreis/__init__.py` & `tierkreis-0.2.0/tierkreis/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/_build/generate_protos.py` & `tierkreis-0.2.0/tierkreis/_build/generate_protos.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/builder.py` & `tierkreis-0.2.0/tierkreis/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from abc import ABC, abstractmethod
 from contextlib import AbstractContextManager
 from contextvars import ContextVar, Token
 from dataclasses import dataclass
-from functools import update_wrapper, wraps
+from functools import cached_property
 from itertools import count
 from types import FrameType, TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -47,15 +47,15 @@
     TierkreisNode,
     to_nodeport,
 )
 from tierkreis.core.tierkreis_struct import TierkreisStruct
 from tierkreis.core.type_errors import TierkreisTypeErrors
 from tierkreis.core.type_inference import infer_graph_types
 from tierkreis.core.types import TypeScheme
-from tierkreis.core.utils import map_vals
+from tierkreis.core.utils import graph_from_func, map_vals, rename_ports_graph
 from tierkreis.core.values import TierkreisValue, TKVal1, tkvalue_to_tktype
 
 if TYPE_CHECKING:
     from tierkreis.core.types import GraphType, TierkreisType
 
 
 # magic for lazily creating nodes (and returning ports thereof)
@@ -317,16 +317,19 @@
         str,
         dict,
         TierkreisStruct,
         TierkreisValue,
         TierkreisGraph,
         tuple,
         list,
+        "LazyGraph",
     ]
 ) -> NodePort:
+    if isinstance(val, LazyGraph):
+        val = val.graph
     n = current_builder().add_node_to_graph(ConstNode(TierkreisValue.from_python(val)))
     return n[Labels.VALUE]
 
 
 @dataclass(frozen=True)
 class _CallAddNode:
     node: TierkreisNode
@@ -337,26 +340,14 @@
         bg = current_builder()
         kwds = _combine_args_with_kwargs(self.input_order, *args, **kwds)
 
         n = bg.add_node_to_graph(self.node, **kwds)
         return NodeRef(n.idx, n.graph, self.output_order)
 
 
-class Box(_CallAddNode):
-    graph: TierkreisGraph
-
-    def __init__(self, graph: TierkreisGraph, location: Location = Location([])):
-        self.graph = graph
-        super().__init__(
-            BoxNode(graph, location=location),
-            graph.input_order,
-            graph.output_order,
-        )
-
-
 class Scope(CaptureBuilder, ABC):
     location: Location
 
     def __init__(self, location: Union[str, Location] = Location([])):
         if isinstance(location, str):
             self.location = Location(location.split("/"))
         else:
@@ -369,17 +360,16 @@
         __exc_value: Optional[BaseException],
         __traceback: Optional[TracebackType],
     ) -> None:
         super().__exit__(__exc_type, __exc_value, __traceback)
 
         if not any((__exc_type, __exc_value, __traceback)):
             graph = self.graph
-            box = Box(graph, self.location)
             inputs = {v: k for k, v in self.captured.items()}
-            node_ref = box(**inputs)
+            node_ref = _build_box(graph, self.location, **inputs)
             for inner_graph, captured in self.inner_scopes.items():
                 current_builder().inner_scopes[inner_graph] = CaptureOutwards(
                     graph, node_ref, captured
                 )
             current_builder().inner_scopes[graph] = CaptureOutwards(graph, node_ref)
 
 
@@ -480,15 +470,14 @@
 class Input(Generic[TKVal1], NodePort):
     def __init__(self, port: PortID) -> None:
         np = current_builder().graph.input[port]
         super().__init__(np.node_ref, np.port)
 
 
 _GraphDef = Callable[..., Output]
-_GraphDecoratorType = Callable[[_GraphDef], Callable[[], TierkreisGraph]]
 
 
 def _get_edge_annotations(
     f: _GraphDef,
 ) -> tuple[dict[str, Optional["TierkreisType"]], dict[str, Optional["TierkreisType"]],]:
     f_sig = inspect.signature(f)
     inps = map_vals(
@@ -504,45 +493,75 @@
     return in_types, out_types
 
 
 class CapturedError(Exception):
     pass
 
 
-def graph(
+@dataclass(frozen=True)
+class LazyGraph:
+    _builder: Callable[[], TierkreisGraph]
+
+    @cached_property
+    def graph(self) -> TierkreisGraph:
+        return self._builder()
+
+    def __call__(self, *args: ValueSource, **kwargs: ValueSource) -> NodeRef:
+        return self.graph(*args, **kwargs)
+
+    def _repr_svg_(self) -> str:
+        return getattr(self.graph, "_repr_svg_")()
+
+
+_GraphDecoratorType = Callable[[_GraphDef], TierkreisGraph]
+_LazyGraphDecoratorType = Callable[[_GraphDef], LazyGraph]
+
+
+def lazy_graph(
     name: Optional[str] = None,
     type_check_sig: Optional[Signature] = None,
     debug: bool = True,
-) -> _GraphDecoratorType:
-    def decorator_graph(f: _GraphDef) -> Callable[[], TierkreisGraph]:
+) -> _LazyGraphDecoratorType:
+    def decorator_graph(f: _GraphDef) -> LazyGraph:
         in_types, out_types = _get_edge_annotations(f)
         # Use getattr as _GraphDef doesn't specify that it has a __name__
         graph_name = name or getattr(f, "__name__")
         # graph_name = name or f.__name__  # type: ignore  # the alternative
 
-        @wraps(f)
         def wrapper() -> TierkreisGraph:
             gb = GraphBuilder(in_types, out_types, name=graph_name, debug=debug)
 
             with gb as sub_build:
                 f(*(Input(port) for port in in_types))
 
             return (
                 sub_build.graph
                 if type_check_sig is None
                 else sub_build.type_check(type_check_sig)
             )
 
-        wrapper.__annotations__ = {}
-        return wrapper
+        return LazyGraph(wrapper)
+
+    return decorator_graph
+
+
+def graph(
+    name: Optional[str] = None,
+    type_check_sig: Optional[Signature] = None,
+    debug: bool = True,
+) -> _GraphDecoratorType:
+    dec = lazy_graph(name, type_check_sig, debug)
+
+    def decorator_graph(f: _GraphDef) -> TierkreisGraph:
+        return dec(f).graph
 
     return decorator_graph
 
 
-class Thunk(_CallAddNode):
+class Thunk(_CallAddNode, PortFunc):
     graph_src: ValueSource
 
     def __init__(
         self, graph_src: ValueSource, input_order: list[str], output_order: list[str]
     ):
         self.graph_src = graph_src
         super().__init__(FunctionNode(FunctionName("eval")), input_order, output_order)
@@ -551,33 +570,36 @@
         assert "thunk" not in kwargs
         return super().__call__(*args, thunk=self.graph_src, **kwargs)
 
     def copyable(self) -> "Thunk":
         self.graph_src = Copyable(self.graph_src)
         return self
 
+    def resolve(self) -> NodePort:
+        """Return a NodePort, creating nodes as necessary in source graph."""
+        return _resolve(self.graph_src)
+
+    def source_graph(self) -> TierkreisGraph:
+        """The graph the port belongs to (or will)."""
+        return _source_graph(self.graph_src)
+
 
 def closure(
     name: Optional[str] = None, debug: bool = True
 ) -> Callable[[_GraphDef], Thunk]:
     def decorator_graph(f: _GraphDef) -> Thunk:
         in_types, out_types = _get_edge_annotations(f)
         # Use getattr as _GraphDef doesn't specify that it has a __name__
         graph_name = name or getattr(f, "__name__")
         # graph_name = name or f.__name__  # type: ignore  # the alternative
 
         gb = CaptureBuilder(in_types, out_types, name=graph_name, debug=debug)
 
         with gb as sub_build:
             f(*(Input(port) for port in in_types))
-        # Copy docstring, etc., onto the TierkreisGraph.
-        # (Of course such will be lost if the graph is serialized.)
-        wrapper = sub_build.graph
-        update_wrapper(wrapper, f)
-        wrapper.__annotations__ = {}
         return Thunk(
             _partial_thunk(sub_build, sub_build.captured),
             list(in_types.keys()),
             list(out_types.keys()),
         )
 
     return decorator_graph
@@ -590,15 +612,14 @@
             raise ValueError("Loop body graph can only have one input.")
 
         # the loop node has input port "value"
         # allow body definitions to use any input names and map it
         in_types = {Labels.VALUE: in_types.popitem()[1]}
         graph_name = name or getattr(f, "__name__")
 
-        @wraps(f)
         def wrapper(initial: ValueSource) -> NodePort:
             gb = CaptureBuilder(in_types, out_types, name=graph_name, debug=debug)
             with gb as sub_build:
                 f(Input(Labels.VALUE))
 
             loop_node = current_builder().add_node_to_graph(
                 FunctionNode(FunctionName("loop")),
@@ -874,14 +895,21 @@
         self.f = f
         self.name = name
         super().__init__(FunctionNode(name), f.input_order, f.output_order)
 
     def signature_string(self) -> str:
         return _func_sig(self.name.name, self.f)
 
+    def to_graph(
+        self,
+        input_map: Optional[dict[str, str]] = None,
+        output_map: Optional[dict[str, str]] = None,
+    ) -> TierkreisGraph:
+        return graph_from_func(self.name, self.f, input_map, output_map)
+
 
 class Namespace(Mapping[str, "Namespace"]):
     @overload
     def __init__(self, args: Signature, /):
         ...
 
     @overload
@@ -913,7 +941,49 @@
         return self.__subspaces[__k]
 
     def __len__(self) -> int:
         return self.__subspaces.__len__()
 
     def __iter__(self) -> Iterator[str]:
         return self.__subspaces.__iter__()
+
+
+def _rename_ports(
+    thunk: ValueSource, map_old_to_new: dict[str, str], is_inputs: bool
+) -> NodePort:
+    bg = current_builder()
+    rename_g = Const(rename_ports_graph(map_old_to_new))
+    f, s = (rename_g, thunk) if is_inputs else (thunk, rename_g)
+    seq = bg.add_node_to_graph(
+        FunctionNode(FunctionName("sequence")), first=f, second=s
+    )
+
+    return seq["sequenced"]
+
+
+def RenameInputs(thunk: ValueSource, rename_map: dict[str, str]) -> NodePort:
+    return _rename_ports(thunk, {v: k for k, v in rename_map.items()}, True)
+
+
+def RenameOuputs(thunk: ValueSource, rename_map: dict[str, str]) -> NodePort:
+    return _rename_ports(thunk, rename_map, False)
+
+
+def _build_box(
+    g: TierkreisGraph, __tk_loc: Location, *args: ValueSource, **kwargs: ValueSource
+) -> NodeRef:
+    bx = _CallAddNode(
+        BoxNode(g, __tk_loc),
+        g.input_order,
+        g.output_order,
+    )
+    return bx(*args, **kwargs)
+
+
+def __graph_call__(
+    self: TierkreisGraph, *args: ValueSource, **kwargs: ValueSource
+) -> NodeRef:
+    return _build_box(self, Location([]), *args, **kwargs)
+
+
+# mypy is not happy with assignment to a method
+setattr(TierkreisGraph, "__call__", __graph_call__)
```

### Comparing `tierkreis-0.1.0/tierkreis/cli.py` & `tierkreis-0.2.0/tierkreis/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,24 @@
     @wraps(f)
     def wrapper(*args, **kwargs):
         return asyncio.run(f(*args, **kwargs))
 
     return wrapper
 
 
-def _inputs(source: str) -> Dict[str, TierkreisValue]:
-    if source == "":
-        return {}
-    path = Path(source)
+def _inputs(proto_file: str, py_source: str) -> Dict[str, TierkreisValue]:
+    if proto_file == "":
+        return (
+            {}
+            if py_source == ""
+            else {k: TierkreisValue.from_python(v) for k, v in eval(py_source).items()}
+        )
+    if py_source != "":
+        raise ValueError("Cannot provide both inputs and --py-inputs")
+    path = Path(proto_file)
     with open(path, "rb") as f:
         v: StructValue = StructValue.from_proto(pg.StructValue().parse(f.read()))
         return v.values
 
 
 async def _parse(source: Path) -> TierkreisGraph:
     with open(source, "rb") as f:
@@ -178,44 +184,46 @@
 def _print_typeerrs(errs: str):
     print(chalk.red(errs), file=sys.stderr)
 
 
 @cli.command()
 @click.argument("proto", type=click.Path(exists=True))
 @click.argument("inputs", default="")
+@click.option("-p", "--py-inputs", default="")
 @click.pass_context
 @coro
-async def run(ctx: click.Context, proto: Path, inputs: str):
+async def run(ctx: click.Context, proto: Path, inputs: str, py_inputs: str):
     """Run PROTO binary on runtime with optional INPUTS and output to console."""
     async with ctx.obj["client_manager"] as client:
         client = cast(ServerRuntime, client)
         tkg = await _parse(proto)
-        py_inputs = _inputs(inputs)
+        input_dict = _inputs(inputs, py_inputs)
         try:
-            outputs = await client.run_graph(tkg, **py_inputs)
+            outputs = await client.run_graph(tkg, **input_dict)
             _print_outputs(outputs)
         except TierkreisTypeErrors:
             _print_typeerrs(traceback.format_exc(0))
             sys.exit(1)
 
 
 @cli.command()
 @click.argument("proto", type=click.Path(exists=True))
 @click.argument("inputs", default="")
+@click.option("-p", "--py-inputs", default="")
 @click.pass_context
 @coro
-async def submit(ctx: click.Context, proto: Path, inputs: str):
+async def submit(ctx: click.Context, proto: Path, inputs: str, py_inputs: str):
     """Submit PROTO binary and optional
     INPUTS to runtime and print task id to console."""
     async with ctx.obj["client_manager"] as client:
         client = cast(ServerRuntime, client)
         tkg = await _parse(proto)
-        py_inputs = _inputs(inputs)
+        input_dict = _inputs(inputs, py_inputs)
         try:
-            task_handle = await client.start_task(tkg, py_inputs)
+            task_handle = await client.start_task(tkg, input_dict)
             print(chalk.bold.yellow("Task id:"), task_handle.task_id)
         except TierkreisTypeErrors:
             _print_typeerrs(traceback.format_exc(0))
             sys.exit(1)
 
 
 @cli.command()
```

### Comparing `tierkreis-0.1.0/tierkreis/client/runtime_client.py` & `tierkreis-0.2.0/tierkreis/client/runtime_client.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/client/server_client.py` & `tierkreis-0.2.0/tierkreis/client/server_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,25 @@
     Dict,
     Type,
     TypeVar,
     cast,
 )
 
 import betterproto
-import keyring
 from grpclib.client import Channel
-from grpclib.events import SendRequest, listen
+from grpclib.events import SendRequest
 
 import tierkreis.core.protos.tierkreis.v1alpha.graph as pg
 import tierkreis.core.protos.tierkreis.v1alpha.runtime as pr
 import tierkreis.core.protos.tierkreis.v1alpha.signature as ps
 from tierkreis.client.runtime_client import RuntimeClient
 from tierkreis.core.signature import Signature
 from tierkreis.core.tierkreis_graph import Location, TierkreisGraph
 from tierkreis.core.type_errors import TierkreisTypeErrors
 from tierkreis.core.values import IncompatiblePyType, StructValue, TierkreisValue
-from tierkreis.worker import CallbackHook
 
 if TYPE_CHECKING:
     from betterproto.grpc.grpclib_client import ServiceStub
 
 
 @dataclass
 class RuntimeHTTPError(Exception):
@@ -97,17 +95,17 @@
     def _runtime_stub(self) -> pr.RuntimeStub:
         return self._stub_gen("runtime", pr.RuntimeStub)
 
     @property
     def _type_stub(self) -> ps.TypeInferenceStub:
         return self._stub_gen("type", ps.TypeInferenceStub)
 
-    async def get_signature(self) -> Signature:
+    async def get_signature(self, loc: Location = Location([])) -> Signature:
         return Signature.from_proto(
-            await self._signature_stub.list_functions(ps.ListFunctionsRequest())
+            await self._signature_stub.list_functions(ps.ListFunctionsRequest(loc))
         )
 
     async def start_task(
         self, graph: TierkreisGraph, py_inputs: Dict[str, Any]
     ) -> TaskHandle:
         """
         Spawn a task that runs a graph and return the task's id. The id can
@@ -182,14 +180,15 @@
         :param task: The id of the task to delete.
         """
         await self._runtime_stub.delete_task(pr.DeleteTaskRequest(id=task.task_id))
 
     async def run_graph(
         self,
         graph: TierkreisGraph,
+        loc: Location = Location([]),
         /,
         **py_inputs: Any,
     ) -> Dict[str, TierkreisValue]:
         """
         Run a graph and return results. This combines `start_task` and `await_task`.
 
         :param gb: Graph to run.
@@ -205,15 +204,15 @@
                 raise InputConversionError(key, val) from err
 
         decoded = await self._runtime_stub.run_graph(
             pr.RunGraphRequest(
                 graph=graph.to_proto(),
                 inputs=pg.StructValue(map=StructValue(inputs).to_proto_dict()),
                 type_check=True,
-                loc=Location([]),
+                loc=loc,
             )
         )
 
         status, status_value = betterproto.which_one_of(decoded, "result")
         assert status_value is not None
         if status == "type_errors":
             raise TierkreisTypeErrors.from_proto(status_value, graph)
@@ -234,18 +233,22 @@
             port: int,
         ):
             async with Channel(host, port) as channel:
                 return await ServerRuntime(channel).run_graph(graph, **py_inputs)
 
         return async_to_sync(_run)(self._channel._host, self._channel._port)
 
-    async def type_check_graph(self, graph: TierkreisGraph) -> TierkreisGraph:
+    async def type_check_graph(
+        self, graph: TierkreisGraph, loc: Location = Location([])
+    ) -> TierkreisGraph:
         value = TierkreisValue.from_python(graph).to_proto()
 
-        response = await self._type_stub.infer_type(ps.InferTypeRequest(value=value))
+        response = await self._type_stub.infer_type(
+            ps.InferTypeRequest(value=value, loc=loc)
+        )
         name, message = betterproto.which_one_of(response, "response")
 
         if name == "success":
             message = cast(ps.InferTypeSuccess, message)
             assert message.value.graph is not None
             return TierkreisValue.from_proto(message.value).to_python(TierkreisGraph)
 
@@ -257,44 +260,14 @@
     async def _inject_auth(event: SendRequest) -> None:
         event.metadata["token"] = login
         event.metadata["key"] = pwd
 
     return _inject_auth
 
 
-def with_runtime_client(callback: CallbackHook) -> Callable:
-    from tierkreis.worker.worker import _KEYRING_SERVICE
-
-    def decorator(func: Callable) -> Callable:
-        @wraps(func)
-        async def wrapped_func(*args, **kwargs):
-            if callback.callback is None:
-                raise RuntimeError(
-                    "Callback address has not been extracted from request."
-                )
-            async with Channel(*callback.callback) as channel:
-                _token = keyring.get_password(_KEYRING_SERVICE, "token")
-                _key = keyring.get_password(_KEYRING_SERVICE, "key")
-                if not (_token is None or _key is None):
-                    listen(channel, SendRequest, _gen_auth_injector(_token, _key))
-                args = (ServerRuntime(channel),) + args
-                return await func(*args, **kwargs)
-
-        try:
-            wrapped_func.__annotations__.pop("client")
-        except KeyError as e:
-            raise RuntimeError(
-                "Function to be wrapped must have"
-                " 'channel: RuntimeClient' as first argument"
-            ) from e
-        return wrapped_func
-
-    return decorator
-
-
 class RuntimeLaunchFailed(Exception):
     """Starting server locally failed."""
 
 
 CallableReturn = TypeVar("CallableReturn")
```

### Comparing `tierkreis-0.1.0/tierkreis/common_types/__init__.py` & `tierkreis-0.2.0/tierkreis/common_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/common_types/circuit.py` & `tierkreis-0.2.0/tierkreis/common_types/circuit.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/__init__.py` & `tierkreis-0.2.0/tierkreis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/function.py` & `tierkreis-0.2.0/tierkreis/core/function.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/graphviz.py` & `tierkreis-0.2.0/tierkreis/core/graphviz.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/internal.py` & `tierkreis-0.2.0/tierkreis/core/internal.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py` & `tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,25 @@
     vec: "VecValue" = betterproto.message_field(5, group="value")
     map: "MapValue" = betterproto.message_field(7, group="value")
     struct: "StructValue" = betterproto.message_field(8, group="value")
     variant: "VariantValue" = betterproto.message_field(12, group="value")
 
 
 @dataclass(eq=False, repr=False)
+class Output(betterproto.Message):
+    edge: "Edge" = betterproto.message_field(1)
+    value: "Value" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class OutputStream(betterproto.Message):
+    stream: List["Output"] = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
 class Type(betterproto.Message):
     var: str = betterproto.string_field(1, group="type")
     int: "Empty" = betterproto.message_field(2, group="type")
     bool: "Empty" = betterproto.message_field(3, group="type")
     graph: "GraphType" = betterproto.message_field(4, group="type")
     pair: "PairType" = betterproto.message_field(5, group="type")
     vec: "Type" = betterproto.message_field(6, group="type")
```

### Comparing `tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py` & `tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 if TYPE_CHECKING:
     import grpclib.server
     from betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class Callback(betterproto.Message):
+    uri: str = betterproto.string_field(1)
+    loc: "_graph__.Location" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
 class RunTaskRequest(betterproto.Message):
     graph: "_graph__.Graph" = betterproto.message_field(1)
     inputs: "_graph__.StructValue" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class RunTaskResponse(betterproto.Message):
@@ -89,14 +95,15 @@
 
 @dataclass(eq=False, repr=False)
 class RunGraphRequest(betterproto.Message):
     graph: "_graph__.Graph" = betterproto.message_field(1)
     inputs: "_graph__.StructValue" = betterproto.message_field(2)
     type_check: bool = betterproto.bool_field(3)
     loc: "_graph__.Location" = betterproto.message_field(4)
+    escape: "Callback" = betterproto.message_field(5)
 
 
 @dataclass(eq=False, repr=False)
 class RunGraphResponse(betterproto.Message):
     success: "_graph__.StructValue" = betterproto.message_field(1, group="result")
     error: str = betterproto.string_field(2, group="result")
     type_errors: "_signature__.TypeErrors" = betterproto.message_field(
```

### Comparing `tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py` & `tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,29 +28,30 @@
     description: str = betterproto.string_field(3)
     input_order: List[str] = betterproto.string_field(4)
     output_order: List[str] = betterproto.string_field(5)
 
 
 @dataclass(eq=False, repr=False)
 class ListFunctionsRequest(betterproto.Message):
-    pass
+    loc: "_graph__.Location" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class ListFunctionsResponse(betterproto.Message):
     root: "Namespace" = betterproto.message_field(1)
     aliases: Dict[str, "_graph__.TypeScheme"] = betterproto.map_field(
         2, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
     scopes: List["_graph__.Location"] = betterproto.message_field(3)
 
 
 @dataclass(eq=False, repr=False)
 class InferTypeRequest(betterproto.Message):
     value: "_graph__.Value" = betterproto.message_field(1)
+    loc: "_graph__.Location" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class InferTypeResponse(betterproto.Message):
     success: "InferTypeSuccess" = betterproto.message_field(1, group="response")
     error: "TypeErrors" = betterproto.message_field(2, group="response")
```

### Comparing `tierkreis-0.1.0/tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py` & `tierkreis-0.2.0/tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,32 @@
     Optional,
 )
 
 import betterproto
 import grpclib
 from betterproto.grpc.grpclib_server import ServiceBase
 
-from .. import graph as _graph__
+from .. import (
+    graph as _graph__,
+    runtime as _runtime__,
+)
 
 
 if TYPE_CHECKING:
     import grpclib.server
     from betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
 class RunFunctionRequest(betterproto.Message):
     function: "_graph__.FunctionName" = betterproto.message_field(1)
     inputs: "_graph__.StructValue" = betterproto.message_field(2)
     loc: "_graph__.Location" = betterproto.message_field(3)
+    callback: "_runtime__.Callback" = betterproto.message_field(4)
 
 
 @dataclass(eq=False, repr=False)
 class RunFunctionResponse(betterproto.Message):
     outputs: "_graph__.StructValue" = betterproto.message_field(1)
```

### Comparing `tierkreis-0.1.0/tierkreis/core/python.py` & `tierkreis-0.2.0/tierkreis/core/python.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/signature.py` & `tierkreis-0.2.0/tierkreis/core/signature.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/tierkreis_graph.py` & `tierkreis-0.2.0/tierkreis/core/tierkreis_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import tierkreis.core.protos.tierkreis.v1alpha.graph as pg
 from tierkreis.core.function import FunctionName
 from tierkreis.core.types import TierkreisType
 from tierkreis.core.values import T, TierkreisValue
 
 if TYPE_CHECKING:
-    from tierkreis.builder import Unpack
+    from tierkreis.builder import Unpack, ValueSource
 
 PortID = str
 Location = pg.Location
 
 
 class TierkreisNode(ABC):
     @abstractmethod
@@ -324,78 +324,42 @@
         return self.add_node(TagNode(tag), value=value)
 
     def insert_graph(
         self,
         graph: "TierkreisGraph",
         /,
         **kwargs: IncomingWireType,
-    ) -> Dict[str, NodePort]:
+    ) -> Dict[str, IncomingWireType]:
+        """Given a graph and wires to connect to that graph's inputs,
+        inline that graph into <self>, and return the outputs of
+        the inserted graph."""
 
-        # gather maps from I/O name to node ports
-        input_wires = {
-            e.source.port: (e.target.node_ref.idx, e.target.port)
-            for e in graph.out_edges(graph.input_node_idx)
-        }
-        output_wires = {
-            e.target.port: (e.source.node_ref.idx, e.source.port)
-            for e in graph.in_edges(graph.output_node_idx)
-        }
-
-        # return a map from subgraph outputs to inserted nodeports
-        return_outputs: Dict[str, NodePort] = dict()
         index_map: Dict[int, int] = dict()
         for node_idx, node in enumerate(graph.nodes()):
-            if node_idx in {graph.input_node_idx, graph.output_node_idx}:
-                continue
+            if node_idx not in {graph.input_node_idx, graph.output_node_idx}:
+                index_map[node_idx] = self.add_node(node).idx
 
-            # find any provided incoming wires to wire to this node
-            input_ports = {
-                input_port: kwargs[graph_input]
-                for graph_input, (
-                    input_node,
-                    input_port,
-                ) in input_wires.items()
-                if input_node == node_idx and graph_input in kwargs
-            }
-
-            # find any node ports that are graph outputs
-            output_ports = {
-                graph_output: output_port
-                for graph_output, (
-                    output_node,
-                    output_port,
-                ) in output_wires.items()
-                if output_node == node_idx
-            }
-            node_ref = self.add_node(node, **input_ports)
-            index_map[node_idx] = node_ref.idx
-            return_outputs.update(
-                {
-                    graph_output: NodePort(node_ref, output_port)
-                    for graph_output, output_port in output_ports.items()
-                }
-            )
+        return_outputs: Dict[str, IncomingWireType] = {}
 
         for edge in graph.edges():
             source_node = edge.source.node_ref.idx
             target_node = edge.target.node_ref.idx
-            if (
-                source_node == graph.input_node_idx
-                or target_node == graph.output_node_idx
-            ):
-                continue
-            source_node = index_map[source_node]
-            target_node = index_map[target_node]
-
-            self.add_edge(
-                NodeRef(source_node, self)[edge.source.port],
-                NodeRef(target_node, self)[edge.target.port],
-                edge.type_,
+            source_port = (
+                kwargs[edge.source.port]
+                if source_node == graph.input_node_idx
+                else NodeRef(index_map[source_node], self)[edge.source.port]
             )
 
+            if target_node == graph.output_node_idx:
+                return_outputs[edge.target.port] = source_port
+            else:
+                target_port = NodeRef(index_map[target_node], self)[edge.target.port]
+
+                self.add_edge(source_port, target_port, edge.type_)
+
         return return_outputs
 
     def inline_boxes(self, recursive=False) -> "TierkreisGraph":
         """Inline boxes by inserting the graphs they contain in to the parent
         graph. Optionally do this recursively.
 
         :return: Inlined graph
@@ -639,14 +603,21 @@
         return tk_graph
 
     def to_python(self, type_: typing.Type[T]) -> T:
         if isinstance(type_, typing.TypeVar) or type_ is TierkreisGraph:
             return cast(T, self)
         raise TypeError()
 
+    def __call__(
+        self: "TierkreisGraph", *args: "ValueSource", **kwargs: "ValueSource"
+    ) -> NodeRef:
+        raise NotImplementedError(
+            "TierkreisGraph can only be called inside builder contexts."
+        )
+
 
 def _to_tierkreis_type(
     edge_type: Optional[Union[Type, TierkreisType]]
 ) -> Optional[TierkreisType]:
     if edge_type is None:
         return None
     else:
```

### Comparing `tierkreis-0.1.0/tierkreis/core/type_errors.py` & `tierkreis-0.2.0/tierkreis/core/type_errors.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/type_inference.py` & `tierkreis-0.2.0/tierkreis/core/type_inference.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/types.py` & `tierkreis-0.2.0/tierkreis/core/types.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/core/values.py` & `tierkreis-0.2.0/tierkreis/core/values.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/pyruntime/python_builtin.py` & `tierkreis-0.2.0/tierkreis/pyruntime/python_builtin.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from typing import Generic, TypeVar, cast
 
 from tierkreis.core.protos.tierkreis.v1alpha.graph import (
     Constraint,
     Empty,
     GraphType,
     Kind,
-    PairType,
     PartitionConstraint,
     RowType,
     StructType,
     Type,
     TypeScheme,
     TypeSchemeVar,
 )
 from tierkreis.core.protos.tierkreis.v1alpha.signature import FunctionDeclaration
+from tierkreis.core.python import RuntimeGraph
 from tierkreis.core.tierkreis_graph import GraphValue, IncomingWireType, TierkreisGraph
 from tierkreis.core.tierkreis_struct import TierkreisStruct
 from tierkreis.core.types import StarKind
 from tierkreis.core.utils import map_vals
-from tierkreis.core.values import MapValue, StructValue
+from tierkreis.core.values import StructValue
 from tierkreis.worker.namespace import Function, Namespace
 
 namespace = Namespace()
 
 a = TypeVar("a")
 b = TypeVar("b")
 val = TypeVar("val")
@@ -70,15 +70,15 @@
 
 @namespace.function(type_vars={"val": StarKind()})
 async def eq(value_0: val, value_1: val) -> EqOut:
     """Check two values for equality."""
     return EqOut(value_0 == value_1)
 
 
-async def _eval(_x: StructValue) -> StructValue:
+async def _eval(_, _x: StructValue) -> StructValue:
     # implemented as part of runtime
     raise NotImplementedError
 
 
 namespace.functions["eval"] = Function(
     run=_eval,
     declaration=FunctionDeclaration(
@@ -227,64 +227,26 @@
 
 @namespace.function()
 async def imul(a: int, b: int) -> int:
     """Multiply integers a and b together; a * b"""
     return a * b
 
 
-async def _insert_key(ins: StructValue) -> StructValue:
-    # Extract the arguments to the operation
-    inner_map = cast(MapValue, ins.values["map"])
-    key = ins.values["key"]
-    val = ins.values["val"]
-
-    # Perform update (destructively is fine)
-    inner_map.values[key] = val
-    return StructValue({"map": inner_map})
+@dataclass()
+class _InsertOut(TierkreisStruct, Generic[a, b]):
+    map: dict[a, b]
 
 
-namespace.functions["insert_key"] = Function(
-    run=_insert_key,
-    declaration=FunctionDeclaration(
-        type_scheme=TypeScheme(
-            variables=[
-                TypeSchemeVar(name="key", kind=Kind(star=Empty())),
-                TypeSchemeVar(name="val", kind=Kind(star=Empty())),
-            ],
-            body=Type(
-                graph=GraphType(
-                    inputs=RowType(
-                        content={
-                            "map": Type(
-                                map=PairType(
-                                    first=Type(var="key"), second=Type(var="val")
-                                )
-                            ),
-                            "val": Type(var="val"),
-                            "key": Type(var="key"),
-                        }
-                    ),
-                    outputs=RowType(
-                        content={
-                            "map": Type(
-                                map=PairType(
-                                    first=Type(var="key"), second=Type(var="val")
-                                )
-                            )
-                        }
-                    ),
-                )
-            ),
-        ),
-        description="Insert a key value pair in to a map."
-        " Existing keys will have their values replaced.",
-        input_order=["map", "key", "val"],
-        output_order=["map"],
-    ),
-)
+@namespace.function(type_vars={"a": StarKind(), "b": StarKind()})
+async def insert_key(map: dict[a, b], key: a, val: b) -> _InsertOut[a, b]:
+    # pylint: disable=redefined-builtin
+    """Insert a key value pair in to a map.\
+ Existing keys will have their values replaced."""
+    map[key] = val
+    return _InsertOut(map)
 
 
 @namespace.function()
 async def int_to_float(int: int) -> float:
     # pylint: disable=redefined-builtin
     """Convert an integer to a float"""
     return float(int)
@@ -298,15 +260,15 @@
 
 @namespace.function()
 async def isub(a: int, b: int) -> int:
     """Subtract integer b from integer a; a - b"""
     return a - b
 
 
-async def _loop(_x: StructValue) -> StructValue:
+async def _loop(_, _x: StructValue) -> StructValue:
     # implemented as part of runtime
     raise NotImplementedError
 
 
 namespace.functions["loop"] = Function(
     run=_loop,
     declaration=FunctionDeclaration(
@@ -362,15 +324,15 @@
 
 @namespace.function(type_vars={"a": StarKind(), "b": StarKind()})
 async def make_pair(first: a, second: b) -> _MakePairOut[a, b]:
     "Creates a new pair."
     return _MakePairOut((first, second))
 
 
-async def make_struct(ins: StructValue) -> StructValue:
+async def make_struct(_, ins: StructValue) -> StructValue:
     """Construct a struct from incoming ports."""
     return StructValue({"struct": ins})
 
 
 namespace.functions["make_struct"] = Function(
     run=make_struct,
     declaration=FunctionDeclaration(
@@ -403,23 +365,23 @@
 
 @namespace.function("or")
 async def _or(a: bool, b: bool) -> bool:
     """Check a or b are true; a || b"""
     return a or b
 
 
-async def _partial(inputs: StructValue) -> StructValue:
+async def _partial(_, inputs: StructValue) -> StructValue:
     invals = inputs.values
     thunk = deepcopy(cast(GraphValue, invals.pop("thunk")).value)
     newg = TierkreisGraph()
     rest_inputs = [port for port in thunk.inputs() if port not in invals]
     inports = map_vals(invals, lambda x: newg.add_const(x)["value"])
     inports.update({port: newg.input[port] for port in rest_inputs})
-    box = newg.add_box(thunk, **inports)
-    newg.set_outputs(**{port: box[port] for port in thunk.outputs()})
+    outs = newg.insert_graph(thunk, **inports)
+    newg.set_outputs(**outs)
     return StructValue({"value": GraphValue(newg)})
 
 
 namespace.functions["partial"] = Function(
     run=_partial,
     declaration=FunctionDeclaration(
         type_scheme=TypeScheme(
@@ -493,70 +455,39 @@
 @namespace.function(type_vars={"a": StarKind()})
 async def push(vec: list[a], item: a) -> _PushOut[a]:
     """Push an item on to end of a Vec."""
     vec.append(item)
     return _PushOut(vec)
 
 
-async def _remove_key(ins: StructValue) -> StructValue:
-    inner_map = cast(MapValue, ins.values["map"])
-    val = inner_map.values.pop(ins.values["key"])
-
-    return StructValue({"map": inner_map, "val": val})
+@dataclass
+class _RemoveOut(TierkreisStruct, Generic[a, b]):
+    map: dict[a, b]
+    val: b
 
 
-namespace.functions["remove_key"] = Function(
-    run=_remove_key,
-    declaration=FunctionDeclaration(
-        type_scheme=TypeScheme(
-            variables=[
-                TypeSchemeVar(name="key", kind=Kind(star=Empty())),
-                TypeSchemeVar(name="val", kind=Kind(star=Empty())),
-            ],
-            body=Type(
-                graph=GraphType(
-                    inputs=RowType(
-                        content={
-                            "key": Type(var="key"),
-                            "map": Type(
-                                map=PairType(
-                                    first=Type(var="key"), second=Type(var="val")
-                                )
-                            ),
-                        }
-                    ),
-                    outputs=RowType(
-                        content={
-                            "val": Type(var="val"),
-                            "map": Type(
-                                map=PairType(
-                                    first=Type(var="key"), second=Type(var="val")
-                                )
-                            ),
-                        }
-                    ),
-                )
-            ),
-        ),
-        description="Remove a key value pair from a map and return the map and value.",
-        input_order=["map", "key"],
-        output_order=["map", "val"],
-    ),
-)
+@namespace.function(type_vars={"a": StarKind(), "b": StarKind()})
+async def remove_key(map: dict[a, b], key: a) -> _RemoveOut[a, b]:
+    # pylint: disable=redefined-builtin
+    """Remove a key value pair from a map and return the map and value."""
+    val = map.pop(key)
+    return _RemoveOut(map, val)
 
 
-async def _sequence(inputs: StructValue) -> StructValue:
+async def _sequence(_, inputs: StructValue) -> StructValue:
     invals = cast(dict[str, IncomingWireType], inputs.values)
     first = deepcopy(cast(GraphValue, invals.pop("first")).value)
     second = deepcopy(cast(GraphValue, invals.pop("second")).value)
     newg = TierkreisGraph()
-    box1 = newg.add_box(first, **{port: newg.input[port] for port in first.inputs()})
-    box2 = newg.add_box(second, **{port: box1[port] for port in first.outputs()})
-    newg.set_outputs(**{port: box2[port] for port in second.outputs()})
-    return StructValue({"sequenced": GraphValue(newg.inline_boxes())})
+    outs1 = newg.insert_graph(
+        first, **{port: newg.input[port] for port in first.inputs()}
+    )
+    outs2 = newg.insert_graph(second, **outs1)
+    newg.set_outputs(**outs2)
+    return StructValue({"sequenced": GraphValue(newg)})
 
 
 namespace.functions["sequence"] = Function(
     run=_sequence,
     declaration=FunctionDeclaration(
         type_scheme=TypeScheme(
             variables=[
@@ -599,27 +530,27 @@
         " outputs of the first graph match the inputs of the second.",
         input_order=["first", "second"],
         output_order=["sequenced"],
     ),
 )
 
 
-async def _parallel(inputs: StructValue) -> StructValue:
+async def _parallel(_, inputs: StructValue) -> StructValue:
     invals = inputs.values
     left = deepcopy(cast(GraphValue, invals.pop("left")).value)
     right = deepcopy(cast(GraphValue, invals.pop("right")).value)
     newg = TierkreisGraph()
-    box1 = newg.add_box(left, **{port: newg.input[port] for port in left.inputs()})
-    box2 = newg.add_box(right, **{port: newg.input[port] for port in right.inputs()})
-    outputs = dict(
-        {port: box1[port] for port in left.outputs()},
-        **{port: box2[port] for port in right.outputs()}
+    outs1 = newg.insert_graph(
+        left, **{port: newg.input[port] for port in left.inputs()}
+    )
+    outs2 = newg.insert_graph(
+        right, **{port: newg.input[port] for port in right.inputs()}
     )
-    newg.set_outputs(**outputs)
-    return StructValue({"value": GraphValue(newg.inline_boxes())})
+    newg.set_outputs(**outs1, **outs2)
+    return StructValue({"value": GraphValue(newg)})
 
 
 namespace.functions["parallel"] = Function(
     run=_parallel,
     declaration=FunctionDeclaration(
         type_scheme=TypeScheme(
             variables=[
@@ -698,15 +629,15 @@
 
 @namespace.function(type_vars={"a": StarKind(), "b": StarKind()})
 async def unpack_pair(pair: tuple[a, b]) -> _UnpackPairOut[a, b]:
     "Unpacks a pair."
     return _UnpackPairOut(*pair)
 
 
-async def _unpack_struct(ins: StructValue) -> StructValue:
+async def _unpack_struct(_, ins: StructValue) -> StructValue:
     return cast(StructValue, ins.values["struct"])
 
 
 namespace.functions["unpack_struct"] = Function(
     run=_unpack_struct,
     declaration=FunctionDeclaration(
         type_scheme=TypeScheme(
@@ -730,7 +661,25 @@
 )
 
 
 @namespace.function()
 async def xor(a: bool, b: bool) -> bool:
     """Check either a or b are true; a ^ b"""
     return a ^ b
+
+
+@dataclass
+class GraphIn(TierkreisStruct, Generic[a]):
+    value: a
+
+
+@dataclass
+class GraphOut(TierkreisStruct, Generic[b]):
+    value: b
+
+
+@namespace.function(name="map", type_vars={"a": StarKind(), "b": StarKind()})
+async def _map(thunk: RuntimeGraph[GraphIn[a], GraphOut[b]], value: list[a]) -> list[b]:
+    """Runs a graph on each element of a Vec and collects the results in a Vec"""
+    # We avoid the use of callbacks in the python builtins and so must
+    # define map in the pyruntime
+    raise NotImplementedError()
```

### Comparing `tierkreis-0.1.0/tierkreis/pyruntime/python_runtime.py` & `tierkreis-0.2.0/tierkreis/pyruntime/python_runtime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Implementation of simple python-only runtime."""
 import asyncio
 from copy import deepcopy
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Tuple, cast
 
 import networkx as nx  # type: ignore
+import requests
 
 from tierkreis.client.runtime_client import RuntimeClient
 from tierkreis.core import Labels
 from tierkreis.core.function import FunctionName
+from tierkreis.core.protos.tierkreis.v1alpha.graph import Output, OutputStream
 from tierkreis.core.signature import Signature
 from tierkreis.core.tierkreis_graph import (
     BoxNode,
     ConstNode,
     FunctionNode,
     GraphValue,
     IncomingWireType,
     InputNode,
     MatchNode,
     OutputNode,
     TagNode,
     TierkreisEdge,
     TierkreisGraph,
 )
+from tierkreis.core.type_errors import TierkreisTypeErrors
 from tierkreis.core.type_inference import _TYPE_CHECK, infer_graph_types
 from tierkreis.core.utils import map_vals
-from tierkreis.core.values import StructValue, TierkreisValue, VariantValue
+from tierkreis.core.values import StructValue, TierkreisValue, VariantValue, VecValue
 from tierkreis.pyruntime import python_builtin
 
 if TYPE_CHECKING:
     from tierkreis.core.tierkreis_graph import _EdgeData
     from tierkreis.worker.namespace import Namespace
 
 
@@ -116,19 +119,21 @@
             inps = {e.target.port: val for e, val in in_values}
             if isinstance(tk_node, FunctionNode):
                 fname = tk_node.function_name
                 if fname.namespaces == [] and fname.name == "eval":
                     return await self._run_eval(inps)
                 elif fname.namespaces == [] and fname.name == "loop":
                     return await self._run_loop(inps)
+                elif fname.namespaces == [] and fname.name == "map":
+                    return await self._run_map(inps)
                 else:
                     function = self.root.get_function(fname)
                     if function is None:
                         raise FunctionNotFound(fname)
-                    return (await function.run(StructValue(inps))).values
+                    return (await function.run(self, StructValue(inps))).values
 
             elif isinstance(tk_node, BoxNode):
                 return await self.run_graph(
                     tk_node.graph,
                     **inps,
                 )
 
@@ -217,14 +222,28 @@
             )
             nxt = {"value": out.value}
             if out.tag == Labels.BREAK:
                 return nxt
             else:
                 ins = nxt
 
+    async def _run_map(
+        self, ins: dict[str, TierkreisValue]
+    ) -> dict[str, TierkreisValue]:
+        body = cast(GraphValue, ins.pop("thunk")).value
+        inputs = cast(VecValue, ins.pop("value")).values
+
+        async def task(x):
+            return (await self.run_graph(body, value=x))[Labels.VALUE]
+
+        tasks = [asyncio.create_task(task(x)) for x in inputs]
+        out = await asyncio.gather(*tasks)
+        ret = {"value": cast(TierkreisValue, VecValue(out))}
+        return ret
+
     def _run_match(self, ins: dict[str, TierkreisValue]) -> dict[str, TierkreisValue]:
         variant = cast(VariantValue, ins[Labels.VARIANT_VALUE])
         thunk = cast(GraphValue, ins[variant.tag]).value
 
         newg = TierkreisGraph()
         boxinps: dict[str, IncomingWireType] = {
             inp: newg.input[inp] for inp in thunk.inputs()
@@ -233,18 +252,73 @@
         box = newg.add_box(thunk, **boxinps)
         newg.set_outputs(**{out: box[out] for out in thunk.outputs()})
         return {Labels.THUNK: GraphValue(newg)}
 
     async def get_signature(self) -> Signature:
         return self.root.extract_signature(True)
 
-    async def type_check_graph(self, tg) -> TierkreisGraph:
+    async def type_check_graph(self, tg: TierkreisGraph) -> TierkreisGraph:
         return infer_graph_types(tg, await self.get_signature())
 
     async def type_check_graph_with_inputs(
         self, tg, inputs: StructValue
     ) -> Tuple[TierkreisGraph, StructValue]:
         return infer_graph_types(tg, await self.get_signature(), inputs)
 
     @property
     def can_type_check(self) -> bool:
         return _TYPE_CHECK
+
+
+class VizRuntime(PyRuntime):
+    """Child class of ``PyRuntime`` that can interact with a tierkreis-viz instance
+    for live graph visulization."""
+
+    def __init__(self, url: str, roots: Iterable["Namespace"], num_workers: int = 1):
+        """`url` is the address of the running tierkreis-viz instance. See
+        `PyRuntime` for remaining parameters
+        """
+        self.url = url
+        super().__init__(roots, num_workers)
+
+    def _post(self, endpoint: str, data):
+        proto_dat = data.to_proto() if hasattr(data, "to_proto") else data
+        requests.post(
+            self.url + endpoint,
+            data=bytes(proto_dat),
+            headers={"content-type": "application/protobuf"},
+        )
+
+    async def type_check_graph(self, tg: TierkreisGraph) -> TierkreisGraph:
+        """See ``PyRuntime.type_check_graph``. Additionally updates
+        vizualized graph with type annotations."""
+        try:
+            typedg = await super().type_check_graph(tg)
+        except TierkreisTypeErrors as e:
+            self._post("/api/typeErrors", e)
+            raise e
+        self.viz_graph(typedg)
+        return typedg
+
+    def viz_graph(self, tg: TierkreisGraph):
+        """Send graph to be visualized."""
+        self._post("/api/graph", tg)
+        self._post("/api/streamList", OutputStream())
+        self._post("/api/typeErrors", TierkreisTypeErrors([]))
+
+    async def run_graph(
+        self,
+        run_g: TierkreisGraph,
+        /,
+        **py_inputs: Any,
+    ) -> dict[str, TierkreisValue]:
+        """See ``PyRuntime.type_check_graph``. Additionally updates the
+        visualization with the outputs of each node when they are available."""
+        lst = OutputStream()
+
+        def _psh(edge: TierkreisEdge, val):
+            lst.stream.append(Output(edge=edge.to_proto(), value=val.to_proto()))
+            self._post("/api/streamList", lst)
+
+        self.set_callback(_psh)
+
+        return await super().run_graph(run_g, **py_inputs)
```

### Comparing `tierkreis-0.1.0/tierkreis/worker/exceptions.py` & `tierkreis-0.2.0/tierkreis/worker/exceptions.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/worker/namespace.py` & `tierkreis-0.2.0/tierkreis/worker/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Namespace class for holding namespace definitions of python Tierkreis worker."""
 
 import dataclasses
 import typing
+from ctypes import ArgumentError
 from dataclasses import dataclass, make_dataclass
 from functools import wraps
 from inspect import getdoc, isclass
 from typing import Awaitable, Callable, Dict, List, Mapping, Optional, Type, Union, cast
 
+from tierkreis.client.runtime_client import RuntimeClient
 from tierkreis.core.function import FunctionDeclaration, FunctionName
 from tierkreis.core.signature import Namespace as SigNamespace
 from tierkreis.core.signature import Signature
 from tierkreis.core.tierkreis_graph import Location
 from tierkreis.core.tierkreis_struct import TierkreisStruct
 from tierkreis.core.types import (
     Constraint,
@@ -39,15 +41,15 @@
 tracer = get_tracer(__name__)
 
 
 @dataclass
 class Function:
     """Registered python function."""
 
-    run: Callable[[StructValue], Awaitable[StructValue]]
+    run: Callable[[RuntimeClient, StructValue], Awaitable[StructValue]]
     declaration: FunctionDeclaration
 
 
 def _snake_to_pascal(name: str) -> str:
     return name.replace("_", " ").title().replace(" ", "")
 
 
@@ -153,14 +155,15 @@
         return ns.functions.get(name.name)
 
     def function(
         self,
         name: Optional[str] = None,
         constraints: Optional[List[Constraint]] = None,
         type_vars: Optional[Dict[Union[str, typing.TypeVar], Kind]] = None,
+        callback: bool = False,
     ) -> Callable[[Callable], Callable]:
         """Decorator to mark python function as available Namespace."""
 
         def decorator(func: Callable) -> Callable:
             func_name = name or func.__name__
 
             # Get input and output type hints
@@ -170,14 +173,22 @@
                 raise ValueError("Tierkreis function needs return type hint.")
             return_hint = type_hints.pop("return")
 
             struct_input = "inputs" in type_hints and _check_tkstruct_hint(
                 type_hints["inputs"]
             )
 
+            if callback:
+                try:
+                    type_hints.pop("client", None)
+                except IndexError:
+                    raise ArgumentError(
+                        "Functions with callbacks must have an argument 'client'"
+                    )
+
             hint_inputs: Type = (
                 type_hints["inputs"]
                 if struct_input
                 else make_dataclass(
                     f"{_snake_to_pascal(func_name)}Inputs", type_hints.items()
                 )
             )
@@ -193,30 +204,35 @@
 
             # Convert type hints into tierkreis types
             type_inputs = Row.from_python(hint_inputs)
             type_outputs = Row.from_python(hint_outputs)
 
             # Wrap function with input and output conversions
             @wraps(func)
-            async def wrapped_func(inputs: StructValue) -> StructValue:
+            async def wrapped_func(
+                runtime: RuntimeClient, inputs: StructValue
+            ) -> StructValue:
                 try:
                     with span(tracer, name="decoding inputs to python type"):
                         python_inputs = (
                             {"inputs": inputs.to_python(hint_inputs)}
                             if struct_input
                             else {
                                 name: val.to_python(type_hints[name])
                                 for name, val in inputs.values.items()
                             }
                         )
                 except Exception as error:
                     raise DecodeInputError(str(error)) from error
 
                 try:
-                    python_outputs = await func(**python_inputs)
+                    if callback:
+                        python_outputs = await func(client=runtime, **python_inputs)
+                    else:
+                        python_outputs = await func(**python_inputs)
                 except Exception as error:
                     raise NodeExecutionError(error) from error
 
                 try:
                     with span(tracer, name="encoding outputs from python type"):
                         outputs = TierkreisValue.from_python(python_outputs)
                 except Exception as error:
```

### Comparing `tierkreis-0.1.0/tierkreis/worker/prelude.py` & `tierkreis-0.2.0/tierkreis/worker/prelude.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Prelude definitions and functions for server executable scripts.
 """
 
 import argparse
 import asyncio
 import os
-from typing import Optional
 
-from .callback import CallbackHook
 from .namespace import Namespace
 from .tracing import _TRACING
 from .worker import Worker
 
 parser = argparse.ArgumentParser(description="Parse worker server cli.")
 parser.add_argument(
     "--port", help="If specified listen on network port rather than UDP."
@@ -42,24 +40,20 @@
         span_exporter = OTLPSpanExporter(endpoint=endpoint)
 
         tracer_provider.add_span_processor(SimpleSpanProcessor(span_exporter))
 
         opentelemetry.trace.set_tracer_provider(tracer_provider)
 
 
-def start_worker_server(
-    worker_name: str, namespace: Namespace, callback: Optional[CallbackHook] = None
-):
+def start_worker_server(worker_name: str, namespace: Namespace):
     """Set up tracing and run the worker server with the provided namespaces.
     Expects a port specified on the command line, and reports succesful start to
     stdout"""
 
-    cb_hook = callback or CallbackHook()
-
     async def main():
         args = parser.parse_args()
         setup_tracing(worker_name)
-        worker = Worker(cb_hook, namespace)
+        worker = Worker(namespace)
         await worker.start(args.port)
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
```

### Comparing `tierkreis-0.1.0/tierkreis/worker/tracing.py` & `tierkreis-0.2.0/tierkreis/worker/tracing.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.1.0/tierkreis/worker/worker.py` & `tierkreis-0.2.0/tierkreis/worker/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Worker server implementation."""
 
 import sys
 from tempfile import TemporaryDirectory
-from typing import Any, Awaitable, Callable, Coroutine, Optional
+from typing import Any, Callable, Coroutine, Optional
 
 import grpclib
 import grpclib.events
 import grpclib.server
 import keyring
 from grpclib.const import Status as StatusCode
 from grpclib.exceptions import GRPCError
@@ -21,16 +21,16 @@
     RunFunctionResponse,
     WorkerBase,
 )
 from tierkreis.core.tierkreis_graph import TierkreisGraph
 from tierkreis.core.type_errors import TierkreisTypeErrors
 from tierkreis.core.values import StructValue
 from tierkreis.pyruntime.python_runtime import PyRuntime
+from tierkreis.worker.callback import callback_server
 
-from .callback import CallbackHook
 from .exceptions import (
     DecodeInputError,
     EncodeOutputError,
     FunctionNotFound,
     NodeExecutionError,
 )
 from .namespace import Namespace
@@ -95,48 +95,38 @@
 
 
 class Worker:
     """Worker server."""
 
     root: Namespace
     server: Server
-    callback_hook: CallbackHook
     pyruntime: PyRuntime
 
-    def __init__(self, callback_hook, root_namespace):
+    def __init__(self, root_namespace):
         self.root = root_namespace
-        self.callback_hook = callback_hook
         self.pyruntime = PyRuntime([root_namespace])
         self.server = Server(
             [SignatureServerImpl(self), WorkerServerImpl(self), RuntimeServerImpl(self)]
         )
 
         # Attach event listener for tracing
         self._add_request_listener(_event_recv_request)
-        # Attach event listener to pick up callback address
-        self._add_request_listener(self._extract_callback)
         # Attach event listener to extract auth credentials
         self._add_request_listener(self._extract_auth)
 
-    def run(
-        self, function: FunctionName, inputs: StructValue
-    ) -> Awaitable[StructValue]:
+    async def run(
+        self, function: FunctionName, inputs: StructValue, callback: pr.Callback
+    ) -> StructValue:
         """Run function."""
         func = self.root.get_function(function)
         if func is None:
             raise FunctionNotFound(function)
 
-        return func.run(inputs)
-
-    async def _extract_callback(self, request: grpclib.events.RecvRequest):
-        if self.callback_hook.callback is None:
-            callback_host = str(request.metadata.get("tierkreis_callback_host"))
-            callback_port = int(request.metadata.get("tierkreis_callback_port"))  # type: ignore
-
-            self.callback_hook.callback = (callback_host, callback_port)
+        async with callback_server(callback) as cb:
+            return await func.run(cb, inputs)
 
     async def _extract_auth(self, request: grpclib.events.RecvRequest) -> None:
         if keyring.get_password(_KEYRING_SERVICE, "token") is None:
             token = request.metadata.pop("token", None)
             key = request.metadata.pop("key", None)
             if (token is not None) and (key is not None):
                 keyring.set_password(_KEYRING_SERVICE, "token", str(token))
@@ -186,18 +176,21 @@
 
     async def run_function(
         self,
         run_function_request: pw.RunFunctionRequest,
     ) -> RunFunctionResponse:
         function = run_function_request.function
         inputs = run_function_request.inputs
+        callback = run_function_request.callback
         try:
             function_name = FunctionName.from_proto(function)
             inputs_struct = StructValue.from_proto_dict(inputs.map)
-            outputs_struct = await self.worker.run(function_name, inputs_struct)
+            outputs_struct = await self.worker.run(
+                function_name, inputs_struct, callback
+            )
             with span(tracer, name="encoding python type in RunFunctionResponse proto"):
                 res = RunFunctionResponse(
                     outputs=pg.StructValue(outputs_struct.to_proto_dict())
                 )
             return res
         except DecodeInputError as err:
             raise GRPCError(
```

### Comparing `tierkreis-0.1.0/tierkreis.egg-info/PKG-INFO` & `tierkreis-0.2.0/tierkreis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tierkreis
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python client and utilities for tierkreis.
 Author-email: Seyon Sivarajah <seyon.sivarajah@quantinuum.com>, Lukas Heidemann <lukas.heidemann@quantinuum.com>, John Children <john.children@quantinuum.com>, Alan Lawrence <alan.lawrence@quantinuum.com>
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docker
 Provides-Extra: telemetry
 Provides-Extra: commontypes
```

### Comparing `tierkreis-0.1.0/tierkreis.egg-info/SOURCES.txt` & `tierkreis-0.2.0/tierkreis.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 README.md
 pyproject.toml
+tests/test_builder.py
+tests/test_commontypes.py
+tests/test_frontend.py
+tests/test_pyruntime.py
+tests/test_pytket_worker.py
+tests/test_tierkreis_graph.py
+tests/test_type_check.py
 tierkreis/__init__.py
 tierkreis/_version.py
 tierkreis/builder.py
 tierkreis/cli.py
 tierkreis.egg-info/PKG-INFO
 tierkreis.egg-info/SOURCES.txt
 tierkreis.egg-info/dependency_links.txt
```

### Comparing `tierkreis-0.1.0/tierkreis.egg-info/requires.txt` & `tierkreis-0.2.0/tierkreis.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 betterproto[compiler]==2.0.0b5
 protobuf<4,>=3.19
 grpclib<0.5,>=0.4.3rc
 networkx<3,>=2.6.3
 graphviz<0.19,>=0.18
 keyring==23.2
 keyrings.alt==4.1
-click<9,>=8.0.3
+click==8.1.3
 yachalk<0.2,>=0.1.4
+requests<3,>=2.31
 
 [commontypes]
 pytket>=1.0
 
 [docker]
 docker<6,>=5
 
 [lint]
 black<23,>=22.1
 mypy<0.982,>=0.981
 pylint!=2.13.6,~=2.13
 isort~=5.10
 types-setuptools<58,>=57.4.2
+types-requests<3,>=2.31
 types-python-dateutil<3,>=2.8.2
 tierkreis[docker,sc22-example,telemetry]
 
 [sc22-example]
 numpy<2,>=1.20
 pytket>=1.0
```

