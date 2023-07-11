# Comparing `tmp/ai_transform-0.32.1.tar.gz` & `tmp/ai_transform-0.32.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.32.1.tar", last modified: Tue Jun 13 06:47:09 2023, max compression
+gzip compressed data, was "ai_transform-0.32.2.tar", last modified: Tue Jul 11 03:23:42 2023, max compression
```

## Comparing `ai_transform-0.32.1.tar` & `ai_transform-0.32.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-13 06:46:50.000000 ai_transform-0.32.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 06:47:09.457221 ai_transform-0.32.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-13 06:46:50.000000 ai_transform-0.32.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 06:46:50.000000 ai_transform-0.32.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:47:09.457221 ai_transform-0.32.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 06:46:50.000000 ai_transform-0.32.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.648690 ai_transform-0.32.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-11 03:23:26.000000 ai_transform-0.32.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 03:23:42.648690 ai_transform-0.32.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-11 03:23:26.000000 ai_transform-0.32.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.624689 ai_transform-0.32.2/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.628689 ai_transform-0.32.2/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.632689 ai_transform-0.32.2/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.632689 ai_transform-0.32.2/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.632689 ai_transform-0.32.2/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.636689 ai_transform-0.32.2/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.636689 ai_transform-0.32.2/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.636689 ai_transform-0.32.2/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.628689 ai_transform-0.32.2/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 03:23:26.000000 ai_transform-0.32.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 03:23:42.648690 ai_transform-0.32.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 03:23:26.000000 ai_transform-0.32.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.640689 ai_transform-0.32.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.640689 ai_transform-0.32.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.640689 ai_transform-0.32.2/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.32.1/LICENSE` & `ai_transform-0.32.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/README.md` & `ai_transform-0.32.2/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/__init__.py` & `ai_transform-0.32.2/ai_transform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.32.1"
+__version__ = "0.32.2"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.32.1/ai_transform/api/api.py` & `ai_transform-0.32.2/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/api/client.py` & `ai_transform-0.32.2/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/api/helpers.py` & `ai_transform-0.32.2/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/api/wrappers.py` & `ai_transform-0.32.2/ai_transform/api/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     pass
 
 
 class ResultNotOKError(Exception):
     pass
 
 
+class OrgEntitlementError(Exception):
+    pass
+
+
 def is_response_bad(
     result: Response,
     key_for_error: str = None,
     output_to_stdout: bool = False,  # support output to stdout to ensure logging is working
 ):
     try:
         json_response = result.json()
@@ -51,15 +55,14 @@
     timeout: int = 30,
     output_to_stdout: bool = False,  # support output to stdout to ensure logging is working
     exponential_backoff: float = 1,
     retry_func: Callable = None,
     key_for_error: str = None,
     is_json_decodable: bool = False,
 ) -> Response:
-
     if args is None:
         args = ()
 
     if kwargs is None:
         kwargs = {}
 
     if retry_func is None:
@@ -68,17 +71,24 @@
     result: requests.Response = None
 
     for n in range(1, num_retries + 1):
         try:
             result = fn(*args, **kwargs)
 
             if not result.ok:
-                to_log = format_logging_info({"message": result.content.decode(), "status_code": result.status_code})
+                content = result.content.decode()
+                status_code = result.status_code
+
+                to_log = format_logging_info({"message": content, "status_code": result.status_code})
                 if output_to_stdout:
                     ic(to_log)
+
+                if status_code == 400 and "Organization Entitlement setting documents" in content:
+                    raise OrgEntitlementError(to_log)
+
                 raise ResultNotOKError(to_log)
 
             if retry_func(result):
                 to_log_for_retry = "Manual Retry Triggered..."
                 if output_to_stdout:
                     ic(to_log_for_retry)
                 raise ManualRetryError(to_log_for_retry)
```

### Comparing `ai_transform-0.32.1/ai_transform/components/components.py` & `ai_transform-0.32.2/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/config.py` & `ai_transform-0.32.2/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/dataset/dataset.py` & `ai_transform-0.32.2/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/dataset/field.py` & `ai_transform-0.32.2/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/engine/abstract_engine.py` & `ai_transform-0.32.2/ai_transform/engine/abstract_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.abstract_operator import AbstractOperator
 
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
 from ai_transform.errors import MaxRetriesError
+from ai_transform.api.wrappers import OrgEntitlementError
 
 
 class AbstractEngine(ABC):
     MAX_SCHEMA_UPDATE_LIMITER: int = 1
 
     def __init__(
         self,
@@ -322,33 +323,19 @@
         for i in range(num_chunks):
             start = i * chunksize
             end = (i + 1) * chunksize
             chunk = documents[start:end]
             if len(chunk) > 0:
                 yield chunk
 
-    def update_chunk(
-        self,
-        chunk: List[Document],
-        max_retries: int = 3,
-        ingest_in_background: bool = True,
-        update_schema: bool = False,
-    ):
+    def update_chunk(self, chunk: List[Document], ingest_in_background: bool = True, update_schema: bool = False):
         if chunk:
-            for _ in range(max_retries):
-                try:
-                    update_json = self._dataset.update_documents(
-                        documents=chunk, ingest_in_background=ingest_in_background, update_schema=update_schema
-                    )
-                except Exception as e:
-                    ic(e)
-                else:
-                    return update_json
-
-            raise MaxRetriesError("max number of retries exceeded")
+            return self._dataset.update_documents(
+                documents=chunk, ingest_in_background=ingest_in_background, update_schema=update_schema
+            )
 
     def api_progress(
         self,
         iterator: Iterator,
         show_progress_bar: bool = True,
         n_total: int = None,
         n_passes: int = 1,
```

### Comparing `ai_transform-0.32.1/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.32.2/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.32.2/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/engine/multipass_engine.py` & `ai_transform-0.32.2/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.32.2/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/engine/stable_engine.py` & `ai_transform-0.32.2/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/errors.py` & `ai_transform-0.32.2/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/logger.py` & `ai_transform-0.32.2/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/operator/abstract_operator.py` & `ai_transform-0.32.2/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/operator/dense_operator.py` & `ai_transform-0.32.2/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/timer.py` & `ai_transform-0.32.2/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/types.py` & `ai_transform-0.32.2/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/utils/document.py` & `ai_transform-0.32.2/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/utils/document_list.py` & `ai_transform-0.32.2/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/utils/example_documents.py` & `ai_transform-0.32.2/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/utils/json_encoder.py` & `ai_transform-0.32.2/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/utils/keyphrase.py` & `ai_transform-0.32.2/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.32.2/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform/workflow/context_manager.py` & `ai_transform-0.32.2/ai_transform/workflow/context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from ai_transform.api.api import API
 from ai_transform.types import Credentials
 from ai_transform.dataset import dataset
 from ai_transform.operator import abstract_operator
 from ai_transform.engine import abstract_engine
 from ai_transform.logger import ic
+from ai_transform.api.wrappers import OrgEntitlementError
 
 
 WORKFLOW_PROCESSED_MESSAGE = "Workflow processed {:.2f}%" + " of documents. "
 
 WORKFLOW_FAIL_MESSAGE = WORKFLOW_PROCESSED_MESSAGE + "This is less than the success threshold of {:.2f}%"
 
 
 class WorkflowContextManager:
-
     FAILED = "failed"
     COMPLETE = "complete"
     IN_PROGRESS = "inprogress"
 
     def __init__(
         self,
         workflow_name: str,
@@ -36,15 +36,14 @@
         credentials: Credentials = None,
         dataset: dataset.Dataset = None,
         operators: List[abstract_operator.AbstractOperator] = None,
         engine: abstract_engine.AbstractEngine = None,
         metadata: Dict[str, Any] = None,
         output: dict = None,
     ):
-
         self.credentials = credentials
         self.engine = engine
         self.dataset = dataset
 
         if self.dataset is not None:
             self.api = self.dataset.api
         else:
@@ -89,15 +88,14 @@
         workflow_id = script_path.split("/")[0]
         return {"job_id": self.job_id, "workflow_id": workflow_id}
 
     def _set_field_children_recursively(self):
         for operator in self.operators:
             if operator.update_field_children:
                 for input_field in operator.input_fields:
-
                     metadata = {}
                     metadata.update(self.field_children_metadata)
                     if isinstance(operator.output_fields, dict):
                         metadata.update(operator.output_fields)
 
                     output_fields = list(operator.output_fields)
 
@@ -196,15 +194,26 @@
             regular_workflow_failed = self.engine.success_ratio < self.success_threshold
 
             if regular_workflow_failed:
                 user_errors = WORKFLOW_FAIL_MESSAGE.format(
                     100 * self.engine.success_ratio, 100 * self.success_threshold
                 )
 
-        if exc_type is not None or regular_workflow_failed:
+        # Here is where we should define all the errors than could occur
+        # outside of the Operators transform function
+        #
+        # Since OrgEntitlementError occurs when upserting and not transforming,
+        # the logic for error handling it is defined here.
+        if isinstance(exc_value, OrgEntitlementError):
+            user_errors = "Organization Entitlement setting documents"
+
+        if exc_type is not None or user_errors is not None:
+            regular_workflow_failed = True
+
+        if regular_workflow_failed:
             return self._handle_workflow_fail(exc_type, exc_value, traceback, user_errors)
         else:
             n_processed_pricing = self._n_processed_pricing or self._calculate_pricing()
             if n_processed_pricing is not None:
                 self.update_workflow_pricing(n_processed_pricing)
             return self._handle_workflow_complete()
```

### Comparing `ai_transform-0.32.1/ai_transform/workflow/helpers.py` & `ai_transform-0.32.2/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.32.2/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/setup.py` & `ai_transform-0.32.2/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/conftest.py` & `ai_transform-0.32.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,14 +421,35 @@
     config_string = json.dumps(config)
     config_bytes = config_string.encode()
     workflow_token = base64.b64encode(config_bytes).decode()
     yield workflow_token
     test_client.delete_dataset(dataset_id)
 
 
+@pytest.fixture(scope="function")
+def test_org_error_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(incomplete_documents(20))
+    job_id = str(uuid.uuid4())
+    print(job_id)
+    config = dict(
+        job_id=job_id,
+        authorizationToken=test_client.credentials.token,
+        dataset_id=dataset_id,
+        vector_fields=["sample_1_vector_"],
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
 @pytest.fixture()
 def test_keyphrases() -> List[Dict]:
     return [
         {
             "text": "word",
             "_id": "word",
             "ancestors": [],
```

### Comparing `ai_transform-0.32.1/tests/core/test_api/test_client.py` & `ai_transform-0.32.2/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_api/test_endpoints.py` & `ai_transform-0.32.2/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.32.2/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_api/test_wrappers.py` & `ai_transform-0.32.2/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.32.2/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_dataset/test_field.py` & `ai_transform-0.32.2/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.32.2/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.32.2/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_engine/test_engine.py` & `ai_transform-0.32.2/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.32.2/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.32.2/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.32.2/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.32.2/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.32.2/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.32.2/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.1/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.32.2/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

