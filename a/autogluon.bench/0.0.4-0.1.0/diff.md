# Comparing `tmp/autogluon.bench-0.0.4.tar.gz` & `tmp/autogluon.bench-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.bench-0.0.4.tar", last modified: Wed Jun  7 23:47:01 2023, max compression
+gzip compressed data, was "autogluon.bench-0.1.0.tar", last modified: Tue Jul 11 00:14:43 2023, max compression
```

## Comparing `autogluon.bench-0.0.4.tar` & `autogluon.bench-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-07 23:47:01.386952 autogluon.bench-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 23:47:01.386952 autogluon.bench-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.378952 autogluon.bench-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.378952 autogluon.bench-0.0.4/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/stack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/dataset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19773 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/multimodal_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/object_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/runbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 23:47:00.000000 autogluon.bench-0.0.4/src/autogluon/bench/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14697 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.248561 autogluon.bench-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.252561 autogluon.bench-0.1.0/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19890 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/multimodal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/output_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/evaluate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/runbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/scripts/generate_cloud_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 00:14:42.000000 autogluon.bench-0.1.0/src/autogluon/bench/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.252561 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14697 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/zip-safe
```

### Comparing `autogluon.bench-0.0.4/LICENSE` & `autogluon.bench-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/PKG-INFO` & `autogluon.bench-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.0.4
+Version: 0.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/autogluon/autogluon-bench
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-bench/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-bench/
 Description: <div align="left">
@@ -37,26 +37,30 @@
         git clone https://github.com/autogluon/autogluon-bench.git
         cd autogluon-bench
         
         # install from source in editable mode
         pip install -e .
         ```
         
-        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). To ensure that your local changes are reflected in the installed package, you may need to adjust the installation command as necessary. A recommended approach is to push your changes to a remote git branch and then pull from this branch, installing the package from source in the scripts.
+        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
+        
+        ```
+        agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+        ```
         
         
         ## Run benchmarks locally
         
         To run the benchmarks on your local machine, use the following command:
         
         ```
         agbench run path/to/local_config_file
         ```
         
-        Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
+        Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
         
         The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
         
         
         ### Tabular Benchmark
         
         To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
@@ -83,15 +87,39 @@
         3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
         ```bash
         nvm install $VERSION  # install Node.js
         npm install -g aws-cdk  # install aws-cdk
         cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
         ```
         
-        To initiate benchmarking on the cloud, use the command below:
+        If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
+        
+        ```bash
+        cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
+        ```
+        
+        You will need a cloud configuration file to run the benchmarks. You can edit the provided [sample cloud config files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs), or use the CLI tool to generate the cloud config files locally.
+        
+        For multimodal:
+        
+        ```
+        agbench generate-cloud-config --module multimodal --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --git-uri-branch <GIT_URI#BRANCH> --dataset-names DATASET_1,DATASET_2 --presets <PRESET_1>,<PRESET_2> --time-limit <TIME_LIMIT_1>,<TIME_LIMIT_2> --hyperparameters "key_1:value_1,key_2:value_2;key_1:value_3,key_2:value_4"
+        ```
+        
+        For tabular:
+        ```
+        agbench generate-cloud-config --module tabular --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --framework <FRAMEWORK>:<LABEL> --amlb-benchmark <BENCHMARK1>,<BENCHMARK2> --amlb-task "BENCHMARK1:DATASET1,DATASET2;BENCHMARK2:DATASET3" --amlb-constraint <CONSTRAINT>
+        ```
+        
+        For more details, you can run
+        ```
+        agbench generate-cloud-config --help
+        ```
+        
+        After having the configuration file ready, use the command below to initiate benchmark runs on cloud:
         
         ```
         agbench run /path/to/cloud_config_file
         ```
         
         This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
         
@@ -108,81 +136,98 @@
         ```bash
         agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
         
         ```
         
         Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
         
+        A cloud configuration file with time-stamped `benchmark_name` is also saved under `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml`
+        
         By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
         
         ```bash
-        agbench run path/to/cloud_config_file --remove_resources
+        agbench run path/to/cloud_config_file --remove-resources
         ```
         
         This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
         
         If you want to manually remove resources later, use:
         
         ```bash
-        agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
+        agbench destroy-stack --config-file `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`
         ```
         
+        Or you can remove specific stacks by running:
+        
+        ```bash
+        agbench destroy-stack --static-resource-stack STATIC_RESOURCE_STACK_NAME --batch-stack BATCH_STACK_NAME --cdk-deploy-account CDK_DEPLOY_ACCOUNT --cdk-deploy-region CDK_DEPLOY_REGION
+        ```
         where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
         
         
         ### Configure the AWS infrastructure
         
         The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
         
         where:
         - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
         - `PREFIX` is used as an identifier for the stack and resources created.
         - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
         - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
         - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
         
-        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
+        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabular_cloud_configs.yaml) for reference.
+        
         
         ## Evaluating bechmark runs
         
-        Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
-        Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
+        Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
+        In a future release, we intend to add evaluation support for multimodal benchmark results.
+        
         
         ### Evaluation Steps
         
-        Clone the `autogluon-benchmark` repository:
+        Begin by setting up AWS credentials for the default profile for the AWS account that has the benchmark results in S3.
+        
+        Step 1: Aggregate AMLB results on S3. After running the benchmark in [AWS mode](#run-benchmarks-on-aws), take note of the `benchmark_name` with timestamp in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml` and run the command below:
         ```
-        git clone https://github.com/gidler/autogluon-benchmark.git
+        agbench aggregate-amlb-results {METRICS_BUCKET} {module} {benchmark_name} --constraint {constraint}
         ```
         
-        Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
-        
-        Run the `aggregate_all.py` script
+        This will create a new file on S3 with this signature:
         ```
-        python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
-        
-        # example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
+        s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/results_automlbenchmark_{constraint}_{benchmark_name}.csv
         ```
         
-        This will create a new file in S3 with this signature:
+        Currently, aggregation is also supported for multimodal benchmark results without the `--constratint` option.
+        
+        For more details, run:
         ```
-        s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
+        agbench aggregate-amlb-results --help
         ```
         
-        Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
+        Step 2: Further clean the aggregated results.
+        
+        If the file is still on S3 from the previous step, run:
         ```
-        python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
+        agbench clean-amlb-results {benchmark_name} --results-dir-input s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/ --benchmark-name-in-input-path --constraints constratint_1 --constraints constratint_2 --results-dir-output {results_dir_output} 
+        --out-path-prefix {out_path_prefix} --out-path-suffix {out_path_suffix}
         ```
-        This will create a local file of results in the `data/results/input/prepared/openml/` directory.
+        where `{results_dir_input}` can also be a local directory. This will create a local file `{results_dir_output}/{out_path_prefix}{benchmark_name}{out_path_suffix}`.
         
-        Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
+        For more details, run:
         ```
-        python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
+        agbench clean-amlb-results --help
         ```
         
+        Step 3: Run evaluation on multiple cleaned files from `Step 2`
+        
+        ```
+        agbench evaluate-amlb-results --frameworks_run framework_1 --frameworks_run framework_2 --results-dir-input data/results/input/prepared/openml --paths file_name_1.csv --paths file_name_2.csv --no-clean-data
+        ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
```

### Comparing `autogluon.bench-0.0.4/README.md` & `autogluon.bench-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,26 +28,30 @@
 git clone https://github.com/autogluon/autogluon-bench.git
 cd autogluon-bench
 
 # install from source in editable mode
 pip install -e .
 ```
 
-For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). To ensure that your local changes are reflected in the installed package, you may need to adjust the installation command as necessary. A recommended approach is to push your changes to a remote git branch and then pull from this branch, installing the package from source in the scripts.
+For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
+
+```
+agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+```
 
 
 ## Run benchmarks locally
 
 To run the benchmarks on your local machine, use the following command:
 
 ```
 agbench run path/to/local_config_file
 ```
 
-Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
+Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
 
 The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
 
 
 ### Tabular Benchmark
 
 To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
@@ -74,15 +78,39 @@
 3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
 ```bash
 nvm install $VERSION  # install Node.js
 npm install -g aws-cdk  # install aws-cdk
 cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
 ```
 
-To initiate benchmarking on the cloud, use the command below:
+If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
+
+```bash
+cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
+```
+
+You will need a cloud configuration file to run the benchmarks. You can edit the provided [sample cloud config files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs), or use the CLI tool to generate the cloud config files locally.
+
+For multimodal:
+
+```
+agbench generate-cloud-config --module multimodal --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --git-uri-branch <GIT_URI#BRANCH> --dataset-names DATASET_1,DATASET_2 --presets <PRESET_1>,<PRESET_2> --time-limit <TIME_LIMIT_1>,<TIME_LIMIT_2> --hyperparameters "key_1:value_1,key_2:value_2;key_1:value_3,key_2:value_4"
+```
+
+For tabular:
+```
+agbench generate-cloud-config --module tabular --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --framework <FRAMEWORK>:<LABEL> --amlb-benchmark <BENCHMARK1>,<BENCHMARK2> --amlb-task "BENCHMARK1:DATASET1,DATASET2;BENCHMARK2:DATASET3" --amlb-constraint <CONSTRAINT>
+```
+
+For more details, you can run
+```
+agbench generate-cloud-config --help
+```
+
+After having the configuration file ready, use the command below to initiate benchmark runs on cloud:
 
 ```
 agbench run /path/to/cloud_config_file
 ```
 
 This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
 
@@ -99,74 +127,91 @@
 ```bash
 agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
 
 ```
 
 Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
 
+A cloud configuration file with time-stamped `benchmark_name` is also saved under `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml`
+
 By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
 
 ```bash
-agbench run path/to/cloud_config_file --remove_resources
+agbench run path/to/cloud_config_file --remove-resources
 ```
 
 This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
 
 If you want to manually remove resources later, use:
 
 ```bash
-agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
+agbench destroy-stack --config-file `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`
 ```
 
+Or you can remove specific stacks by running:
+
+```bash
+agbench destroy-stack --static-resource-stack STATIC_RESOURCE_STACK_NAME --batch-stack BATCH_STACK_NAME --cdk-deploy-account CDK_DEPLOY_ACCOUNT --cdk-deploy-region CDK_DEPLOY_REGION
+```
 where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
 
 
 ### Configure the AWS infrastructure
 
 The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
 
 where:
 - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
 - `PREFIX` is used as an identifier for the stack and resources created.
 - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
 - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
 - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
 
-To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
+To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabular_cloud_configs.yaml) for reference.
+
 
 ## Evaluating bechmark runs
 
-Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
-Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
+Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
+In a future release, we intend to add evaluation support for multimodal benchmark results.
+
 
 ### Evaluation Steps
 
-Clone the `autogluon-benchmark` repository:
+Begin by setting up AWS credentials for the default profile for the AWS account that has the benchmark results in S3.
+
+Step 1: Aggregate AMLB results on S3. After running the benchmark in [AWS mode](#run-benchmarks-on-aws), take note of the `benchmark_name` with timestamp in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml` and run the command below:
 ```
-git clone https://github.com/gidler/autogluon-benchmark.git
+agbench aggregate-amlb-results {METRICS_BUCKET} {module} {benchmark_name} --constraint {constraint}
 ```
 
-Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
-
-Run the `aggregate_all.py` script
+This will create a new file on S3 with this signature:
 ```
-python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
-
-# example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
+s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/results_automlbenchmark_{constraint}_{benchmark_name}.csv
 ```
 
-This will create a new file in S3 with this signature:
+Currently, aggregation is also supported for multimodal benchmark results without the `--constratint` option.
+
+For more details, run:
 ```
-s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
+agbench aggregate-amlb-results --help
 ```
 
-Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
+Step 2: Further clean the aggregated results.
+
+If the file is still on S3 from the previous step, run:
 ```
-python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
+agbench clean-amlb-results {benchmark_name} --results-dir-input s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/ --benchmark-name-in-input-path --constraints constratint_1 --constraints constratint_2 --results-dir-output {results_dir_output} 
+--out-path-prefix {out_path_prefix} --out-path-suffix {out_path_suffix}
 ```
-This will create a local file of results in the `data/results/input/prepared/openml/` directory.
+where `{results_dir_input}` can also be a local directory. This will create a local file `{results_dir_output}/{out_path_prefix}{benchmark_name}{out_path_suffix}`.
 
-Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
+For more details, run:
 ```
-python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
+agbench clean-amlb-results --help
 ```
 
+Step 3: Run evaluation on multiple cleaned files from `Step 2`
+
+```
+agbench evaluate-amlb-results --frameworks_run framework_1 --frameworks_run framework_2 --results-dir-input data/results/input/prepared/openml --paths file_name_1.csv --paths file_name_2.csv --no-clean-data
+```
```

### Comparing `autogluon.bench-0.0.4/setup.py` & `autogluon.bench-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 AUTOGLUON = "autogluon"
 BENCH = "bench"
 
 PYTHON_REQUIRES = ">=3.8, <3.10"
 
 
@@ -62,15 +62,15 @@
         zip_safe=True,
         include_package_data=True,
         python_requires=PYTHON_REQUIRES,
         package_data={
             "": ["Dockerfile", "*.sh", "*.txt", "*.yaml"],
             AUTOGLUON: [
                 "LICENSE",
-            ]
+            ],
         },
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Education",
             "Intended Audience :: Developers",
             "Intended Audience :: Science/Research",
             "Intended Audience :: Customer Service",
@@ -98,15 +98,15 @@
             [console_scripts]
             agbench=autogluon.bench.main:app
         """,
     )
     return setup_args
 
 
-version = "0.0.4"
+version = "0.1.0"
 version = update_version(version, use_file_if_exists=False, create_file=True)
 
 install_requires = [
     "autogluon.common>=0.7,<1.0",
     "awscliv2>=2.2.0,<2.3.0",
     "pandas>=1.2.5,<2.0",
     "boto3>=1.26.0,<1.26.99",
@@ -116,14 +116,18 @@
     "pyyaml>=5.4,<=6.0",
     "tqdm>4.60.0,<=4.65.0",
     "twine>=4.0.0,<=4.0.2",
     "typer>=0.9.0,<1.0.0",
     "requests>2.20.0,<=2.30.0",
     "pyarrow>11.0.0,<=12.0.0",
     "wheel>0.38.0,<=0.40.0",
+    "ray[default]>=2.3.0,<2.4.0",
+    "fsspec>=2023.5.0",
+    "s3fs>=0.4.2",
+    "matplotlib>=3.4,<3.7",
 ]
 
 test_requirements = ["pytest", "pytest-mock", "tox"]
 extras_require = {}
 extras_require["tests"] = test_requirements
 
 if __name__ == "__main__":
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/app.py` & `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/app.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py` & `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py` & `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py` & `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,28 +200,25 @@
     for common_combination in product(*[common_configs[key] for key in common_configs.keys()]):
         for module_combination in product(*[module_configs[key] for key in module_configs.keys()]):
             keys = list(common_configs.keys()) + list(module_configs.keys())
             combination = common_combination + module_combination
 
             if common_configs["module"][0] == "tabular":
                 for amlb_benchmark in amlb_benchmarks:
-                    amlb_task_values = amlb_tasks[amlb_benchmark]
-                    if amlb_task_values is None:
-                        amlb_task_values = [None]
-                    for amlb_task in amlb_task_values:
-                        extended_combination = combination + (amlb_benchmark, amlb_task)
-                        extended_keys = keys + ["amlb_benchmark", "amlb_task"]
-                        job_id, config_s3_path = process_combination(
-                            extended_combination,
-                            extended_keys,
-                            metrics_bucket,
-                            batch_job_queue,
-                            batch_job_definition,
-                        )
-                        job_configs[job_id] = config_s3_path
+                    amlb_task_values = amlb_tasks.get(amlb_benchmark)
+                    extended_combination = combination + (amlb_benchmark, amlb_task_values)
+                    extended_keys = keys + ["amlb_benchmark", "amlb_task"]
+                    job_id, config_s3_path = process_combination(
+                        extended_combination,
+                        extended_keys,
+                        metrics_bucket,
+                        batch_job_queue,
+                        batch_job_definition,
+                    )
+                    job_configs[job_id] = config_s3_path
             else:
                 job_id, config_s3_path = process_combination(
                     combination,
                     keys,
                     metrics_bucket,
                     batch_job_queue,
                     batch_job_definition,
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/stack.py` & `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         tag = self.node.try_get_context("STACK_NAME_TAG")
         instance_types = self.node.try_get_context("INSTANCE_TYPES")
         compute_env_maxv_cpus = int(self.node.try_get_context("COMPUTE_ENV_MAXV_CPUS"))
         container_gpu = self.node.try_get_context("CONTAINER_GPU")
         container_vcpu = self.node.try_get_context("CONTAINER_VCPU")
         container_memory = self.node.try_get_context("CONTAINER_MEMORY")
         block_device_volume = self.node.try_get_context("BLOCK_DEVICE_VOLUME")
-        lambda_function_name = self.node.try_get_context("LAMBDA_FUNCTION_NAME")
+        lambda_function_name = self.node.try_get_context("LAMBDA_FUNCTION_NAME") + "-" + prefix
 
         instances = []
         for instance in instance_types:
             instances.append(ec2.InstanceType(instance))
 
         vpc = static_stack.vpc
 
@@ -150,27 +150,34 @@
         # https://github.com/aws/aws-cdk/issues/12597
         # TODO: use https://github.com/cdklabs/cdk-docker-image-deployment
         docker_image_asset = ecr_assets.DockerImageAsset(
             self,
             f"{prefix}-ecr-docker-image-asset",
             directory=docker_base_dir,
             follow_symlinks=core.SymlinkFollowMode.ALWAYS,
-            build_args={"AG_BENCH_VERSION": os.getenv("AG_BENCH_VERSION", "latest")},
+            build_args={
+                "AG_BENCH_VERSION": os.getenv("AG_BENCH_VERSION", "latest"),
+                "AG_BENCH_DEV_URL": os.getenv("AG_BENCH_DEV_URL", ""),
+            },
         )
 
         docker_container_image = ecs.ContainerImage.from_docker_image_asset(docker_image_asset)
 
         container = batch.JobDefinitionContainer(
             image=docker_container_image,
             gpu_count=container_gpu,
             vcpus=container_vcpu,
             memory_limit_mib=container_memory,
             # Bug that this parameter is not rending in the CF stack under cdk.out
             # https://github.com/aws/aws-cdk/issues/13023
             linux_params=ecs.LinuxParameters(self, f"{prefix}-linux_params", shared_memory_size=container_memory),
+            environment={
+                "AG_BENCH_VERSION": os.getenv("AG_BENCH_VERSION", "latest"),
+                "AG_BENCH_DEV_URL": os.getenv("AG_BENCH_DEV_URL", ""),
+            },
         )
 
         job_definition = batch.JobDefinition(
             self,
             "job-definition",
             container=container,
             retry_attempts=3,
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/stack_handler.py` & `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/stack_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,26 +2,43 @@
 import json
 import os
 import shutil
 import subprocess
 import tempfile
 from typing import Optional
 
+import boto3
 import typer
 import yaml
 
-from autogluon.bench.cloud.aws.constants import gpu_map, memory_map, vcpu_map
-
 with importlib.resources.path("autogluon.bench.cloud.aws", "stack_handler.py") as file_path:
     module_base_dir = os.path.dirname(file_path)
 CONTEXT_FILE = "./cdk.context.json"
 
 app = typer.Typer()
 
 
+def get_instance_type_specs(instance_type, region):
+    ec2_client = boto3.client("ec2", region_name=region)
+    response = ec2_client.describe_instance_types(InstanceTypes=[instance_type])
+
+    instance_type_info = response["InstanceTypes"][0]
+
+    gpu_info_list = instance_type_info.get("GpuInfo", [])
+    gpu_count = sum(gpu_info.get("Count", 0) for gpu_info in gpu_info_list["Gpus"])
+
+    vcpu_info = instance_type_info.get("VCpuInfo", {})
+    vcpu_count = vcpu_info.get("DefaultVCpus", 0)
+
+    memory_info = instance_type_info.get("MemoryInfo", {})
+    memory = memory_info.get("SizeInMiB", 0)
+
+    return gpu_count, vcpu_count, memory
+
+
 def _get_temp_cdk_app_path():
     temp_dir = tempfile.mkdtemp()
     temp_cdk_app_path = os.path.join(temp_dir, "app.py")
     with importlib.resources.path("autogluon.bench.cloud.aws", "app.py") as cdk_app_path:
         shutil.copy2(cdk_app_path, temp_cdk_app_path)
     os.chmod(temp_cdk_app_path, 0o755)
     return temp_cdk_app_path
@@ -41,29 +58,32 @@
     """
     default_config_file = os.path.join(module_base_dir, "default_config.yaml")
     configs = {}
     with open(default_config_file, "r") as f:
         configs = yaml.safe_load(f)
     configs.update(custom_configs)
     prefix = configs["PREFIX"]
+    gpu_count, vcpu_count, memory = get_instance_type_specs(
+        instance_type=configs["INSTANCE"], region=configs["CDK_DEPLOY_REGION"]
+    )
     context_to_parse = {
         "CDK_DEPLOY_ACCOUNT": configs["CDK_DEPLOY_ACCOUNT"],
         "CDK_DEPLOY_REGION": configs["CDK_DEPLOY_REGION"],
         "STACK_NAME_PREFIX": prefix,  # aws resource tag key, also used as name prefix for resources created
         "STACK_NAME_TAG": "benchmark",  # aws resource tag value
         "STATIC_RESOURCE_STACK_NAME": f"{prefix}-static-resource-stack",
         "BATCH_STACK_NAME": f"{prefix}-batch-stack",
         "METRICS_BUCKET": configs["METRICS_BUCKET"],  # bucket to upload metrics
         "DATA_BUCKET": configs.get("DATA_BUCKET", None),  # bucket to download data
         "INSTANCE_TYPES": [configs["INSTANCE"]],  # can be a list of instance families or instance types
-        "COMPUTE_ENV_MAXV_CPUS": vcpu_map[configs["INSTANCE"]]
+        "COMPUTE_ENV_MAXV_CPUS": vcpu_count
         * configs["MAX_MACHINE_NUM"],  # total max v_cpus in batch compute environment
-        "CONTAINER_GPU": gpu_map[configs["INSTANCE"]],  # GPU reserved for container
-        "CONTAINER_VCPU": vcpu_map[configs["INSTANCE"]],  # v_cpus reserved for container
-        "CONTAINER_MEMORY": memory_map[configs["INSTANCE"]]
+        "CONTAINER_GPU": gpu_count,  # GPU reserved for container
+        "CONTAINER_VCPU": vcpu_count,  # v_cpus reserved for container
+        "CONTAINER_MEMORY": memory
         - configs[
             "RESERVED_MEMORY_SIZE"
         ],  # memory in MB reserved for container, also used for shm_size, i.e. `shared_memory_size`
         "BLOCK_DEVICE_VOLUME": configs["BLOCK_DEVICE_VOLUME"],  # device attached to instance, in GB
         "LAMBDA_FUNCTION_NAME": f"{prefix}-batch-job-function",
         "VPC_NAME": configs.get(
             "VPC_NAME", None
@@ -80,29 +100,28 @@
     # set environment variables
     os.environ["CDK_DEPLOY_ACCOUNT"] = str(configs["CDK_DEPLOY_ACCOUNT"])
     os.environ["CDK_DEPLOY_REGION"] = configs["CDK_DEPLOY_REGION"]
 
     return context_to_parse
 
 
-def deploy_stack(configs: Optional[dict] = None) -> dict:
+def deploy_stack(custom_configs: dict) -> dict:
     """
     Deploys the AWS CloudFormation stack containing the benchmarking infrastructure by calling the deploy.sh
     script and passing it the required command line arguments. Constructs the CDK context using the custom
     configuration settings specified in the configs parameter, or the default configuration settings if no
     custom settings are provided.
 
     Args:
         configs (dict, optional): A dictionary containing custom configuration settings. Defaults to None.
 
     Returns:
         dict: A dictionary containing the CDK context settings used for the deployment.
     """
     cdk_path = _get_temp_cdk_app_path()
-    custom_configs = {} if configs is None else configs
     infra_configs = construct_context(custom_configs=custom_configs)
 
     subprocess.check_call(
         [
             os.path.join(module_base_dir, "deploy.sh"),
             infra_configs["STACK_NAME_PREFIX"],
             infra_configs["STACK_NAME_TAG"],
@@ -116,30 +135,45 @@
     shutil.rmtree(os.path.dirname(cdk_path))
 
     return infra_configs
 
 
 @app.command()
 def destroy_stack(
-    static_resource_stack: str = typer.Argument(..., help="The static resource stack name."),
-    batch_stack: str = typer.Argument(..., help="The batch stack name."),
-    cdk_deploy_account: str = typer.Argument(..., help="The CDK deploy account ID."),
-    cdk_deploy_region: str = typer.Argument(..., help="The CDK deploy region."),
+    static_resource_stack: Optional[str] = typer.Option(None, help="The static resource stack name."),
+    batch_stack: Optional[str] = typer.Option(None, help="The batch stack name."),
+    cdk_deploy_account: Optional[str] = typer.Option(None, help="The CDK deploy account ID."),
+    cdk_deploy_region: Optional[str] = typer.Option(None, help="The CDK deploy region."),
+    config_file: Optional[str] = typer.Option(None, help="Path to YAML config file containing stack information."),
 ):
     """
     This function destroys AWS CloudFormation stacks using the AWS Cloud Development Kit (CDK).
 
     It first sets up the necessary environment variables for the CDK, then calls a shell script
     that uses the CDK to destroy the specified static resource stack and batch stack. Finally, it
     removes the temporary directory that was used to deploy the CDK app.
 
     If you have previously deployed with `agbench run CONFIG_FILE,`
     you can find the AWS configs saved under {root_dir}/{module}/{prefix}_{timestamp}/aws_configs.yaml"
     """
     cdk_path = _get_temp_cdk_app_path()
+
+    if config_file is not None:
+        with open(config_file, "r") as f:
+            config = yaml.safe_load(f)
+            static_resource_stack = config.get("STATIC_RESOURCE_STACK_NAME", static_resource_stack)
+            batch_stack = config.get("BATCH_STACK_NAME", batch_stack)
+            cdk_deploy_account = config.get("CDK_DEPLOY_ACCOUNT", cdk_deploy_account)
+            cdk_deploy_region = config.get("CDK_DEPLOY_REGION", cdk_deploy_region)
+
+    if static_resource_stack is None or batch_stack is None or cdk_deploy_account is None or cdk_deploy_region is None:
+        raise ValueError(
+            "static_resource_stack, batch_stack, cdk_deploy_account and cdk_deploy_region must be specified or configured in the config_file."
+        )
+
     os.environ["CDK_DEPLOY_ACCOUNT"] = cdk_deploy_account
     os.environ["CDK_DEPLOY_REGION"] = cdk_deploy_region
     subprocess.check_call(
         [
             os.path.join(module_base_dir, "destroy.sh"),
             static_resource_stack,
             batch_stack,
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/datasets/multimodal_dataset.py` & `autogluon.bench-0.1.0/src/autogluon/bench/datasets/multimodal_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+import logging
 import os
 
 import pandas as pd
 
 from autogluon.bench.utils.dataset_utils import get_data_home_dir, get_repo_url
 from autogluon.common.loaders import load_zip
 from autogluon.common.loaders._utils import download
@@ -32,21 +33,46 @@
     "AEPricePrediction",
     "IMDBGenrePrediction",
     "JCPennyCategory",
     "NewsPopularity",
     "NewsChannel",
 ]
 
+logger = logging.getLogger(__name__)
+
 
 def _path_expander(path, base_folder):
     path_l = path.split(";")
     return ";".join([os.path.abspath(os.path.join(base_folder, path)) for path in path_l])
 
 
 class BaseMultiModalDataset(abc.ABC):
+    def __init__(self, split: str, dataset_name: str, data_info: dict):
+        """
+        Initializes the class.
+
+        Args:
+            split (str): Specifies the dataset split. It should be one of the following options: 'train', 'val', 'test'.
+        """
+        try:
+            ext = os.path.splitext(data_info[split]["url"])[-1]
+            self._path = os.path.join(get_data_home_dir(), dataset_name, f"{split}{ext}")
+            download(data_info[split]["url"], path=self._path, sha1_hash=data_info[split]["sha1sum"])
+            if ext == ".csv":
+                self._data = pd.read_csv(self._path)
+            elif ext == ".pq":
+                self._data = pd.read_parquet(self._path)
+            else:
+                raise NotImplementedError(f"File extension {ext} is not supported.")
+        except Exception:
+            logger.warn(f"The data split {split} is not available.")
+            self._data = None
+
+        self._split = split
+
     @property
     @abc.abstractmethod
     def feature_columns(self):
         pass
 
     @property
     @abc.abstractmethod
@@ -104,16 +130,23 @@
     _registry_name = "shopee"
 
     def __init__(self, split="train"):
         self._split = split
         self._path = os.path.join(get_data_home_dir(), "shopee")
         load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path, sha1sum=self._INFO["data"]["sha1sum"])
         self._base_folder = os.path.join(self._path, "shopee")
-        self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"))
-        self._data["image"] = self._data["image"].apply(lambda ele: _path_expander(ele, base_folder=self._base_folder))
+        try:
+            data_path = os.path.join(self._base_folder, f"{self._split}.csv")
+            self._data = pd.read_csv(data_path)
+            self._data["image"] = self._data["image"].apply(
+                lambda ele: _path_expander(ele, base_folder=self._base_folder)
+            )
+        except FileNotFoundError as e:
+            logger.warn(e)
+            self._data = None
 
     @property
     def base_folder(self):
         """Base folder that contains images"""
         return self._base_folder
 
     @property
@@ -153,20 +186,24 @@
     _registry_name = "stanford_online"
 
     def __init__(self, split="train"):
         self._split = split
         self._path = os.path.join(get_data_home_dir(), "Stanford_Online_Products")
         load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path, sha1sum=self._INFO["data"]["sha1sum"])
         self._base_folder = os.path.join(self._path, "Stanford_Online_Products")
-        self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
-        self._image_columns = ["Image1", "Image2"]
-        for image_col in self._image_columns:
-            self._data[image_col] = self._data[image_col].apply(
-                lambda ele: _path_expander(ele, base_folder=self._base_folder)
-            )
+        try:
+            self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
+            self._image_columns = ["Image1", "Image2"]
+            for image_col in self._image_columns:
+                self._data[image_col] = self._data[image_col].apply(
+                    lambda ele: _path_expander(ele, base_folder=self._base_folder)
+                )
+        except FileNotFoundError as e:
+            logger.warn(e)
+            self._data = None
 
     @property
     def image_columns(self):
         """List of image columns"""
         return self._image_columns
 
     @property
@@ -202,23 +239,28 @@
     _registry_name = "flickr30k"
 
     def __init__(self, split="train"):
         self._split = split
         self._path = os.path.join(get_data_home_dir(), "flickr30k")
         load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path)
         self._base_folder = os.path.join(self._path, "flickr30k_processed")
-        self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
-        self._image_col = "image"
-        self._text_col = "caption"
-
-        self._data[self._image_col] = self._data[self._image_col].apply(
-            lambda ele: _path_expander(ele, base_folder=self._base_folder)
-        )
-        self._label_col = "relevance"
-        self._data[self._label_col] = [1] * len(self._data)
+
+        try:
+            self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
+            self._image_col = "image"
+            self._text_col = "caption"
+
+            self._data[self._image_col] = self._data[self._image_col].apply(
+                lambda ele: _path_expander(ele, base_folder=self._base_folder)
+            )
+            self._label_col = "relevance"
+            self._data[self._label_col] = [1] * len(self._data)
+        except FileNotFoundError as e:
+            logger.warn(e)
+            self._data = None
 
     @property
     def image_columns(self):
         """List of image columns"""
         return [self._image_col]
 
     @property
@@ -261,16 +303,20 @@
         "test": {"url": get_repo_url() + "snli/snli_test.csv", "sha1sum": "87d304ad75b3d64f0f58e316befc7aeba4729b8f"},
     }
     _registry_name = "snli"
 
     def __init__(self, split="train"):
         self._split = split
         self._path = os.path.join(get_data_home_dir(), "snli", f"{split}.csv")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_csv(self._path, delimiter="|")
+        try:
+            download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
+            self._data = pd.read_csv(self._path, delimiter="|")
+        except Exception:
+            logger.warn(f"The data split {self._split} is not available.")
+            self._data = None
 
     @property
     def text_columns(self):
         """List of text columns"""
         return ["premise", "hypothesis"]
 
     @property
@@ -309,18 +355,15 @@
             "url": get_repo_url() + "ner/mit-movies/test_v2.csv",
             "sha1sum": "99040f5f9d4990f62498ad0deeebc472a97e7885",
         },
     }
     _registry_name = "mit_movies"
 
     def __init__(self, split="train"):
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "mit-movies", f"{split}.csv")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_csv(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def feature_columns(self):
         return ["text_snippet"]
 
     @property
     def label_columns(self):
@@ -350,18 +393,15 @@
             "url": get_repo_url() + "women_clothing_review/test.pq",
             "sha1sum": "fbc84f757b8a08210a772613ca8342f3990eb1f7",
         },
     }
     _registry_name = "women_clothing_review"
 
     def __init__(self, split="train"):
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "women_clothing_review", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_parquet(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @classmethod
     def splits(cls):
         return cls._INFO.keys()
 
     @property
     def feature_columns(self):
@@ -408,18 +448,15 @@
             "url": get_repo_url() + "airbnb_melbourne/test.pq",
             "sha1sum": "c28611514b659295fe4b345c3995005719499946",
         },
     }
     _registry_name = "melbourne_airbnb"
 
     def __init__(self, split="train"):
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "airbnb_melbourne", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_parquet(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @classmethod
     def splits(cls):
         return cls._INFO.keys()
 
     @property
     def ignore_columns(self):
@@ -480,19 +517,15 @@
             "url": get_repo_url() + "ae_price_prediction/test.pq",
             "sha1sum": "7bebcaae48410386f610fd7a9c37ba0e89602858",
         },
     }
     _registry_name = "ae_price_prediction"
 
     def __init__(self, split="train"):
-        super().__init__()
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "ae_price_prediction", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_parquet(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @classmethod
     def splits(cls):
         return cls._INFO.keys()
 
     @property
     def data(self):
@@ -534,19 +567,15 @@
             "url": get_repo_url() + "imdb_genre_prediction/test.csv",
             "sha1sum": "0e435e917159542d725d21135cfa514ae936d2c1",
         },
     }
     _registry_name = "imdb_genre_prediction"
 
     def __init__(self, split="train"):
-        super().__init__()
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "imdb_genre_prediction", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_csv(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def data(self):
         return self._data
 
     @classmethod
     def splits(cls):
@@ -588,19 +617,15 @@
             "url": get_repo_url() + "jc_penney_products/test.csv",
             "sha1sum": "23bca284354deec13a11ef7bd726d35a01eb1332",
         },
     }
     _registry_name = "jc_penney_products"
 
     def __init__(self, split="train"):
-        super().__init__()
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "jc_penney_products", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_csv(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def data(self):
         return self._data
 
     @classmethod
     def splits(cls):
@@ -642,19 +667,15 @@
             "url": get_repo_url() + "news_popularity2/test.csv",
             "sha1sum": "297253bdca18f6aafbaee0262be430126c1f9044",
         },
     }
     _registry_name = "news_popularity"
 
     def __init__(self, split="train"):
-        super().__init__()
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "news_popularity2", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_csv(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def data(self):
         return self._data
 
     @classmethod
     def splits(cls):
@@ -696,19 +717,15 @@
             "url": get_repo_url() + "news_channel/test.csv",
             "sha1sum": "a71516784ce6e168bd9933e9ec50080f65cb05fd",
         },
     }
     _registry_name = "news_channel"
 
     def __init__(self, split="train"):
-        super().__init__()
-        self._split = split
-        self._path = os.path.join(get_data_home_dir(), "news_channel", f"{split}.pq")
-        download(self._INFO[split]["url"], path=self._path, sha1_hash=self._INFO[split]["sha1sum"])
-        self._data = pd.read_csv(self._path)
+        super().__init__(split=split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def data(self):
         return self._data
 
     @classmethod
     def splits(cls):
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/datasets/object_detection_dataset.py` & `autogluon.bench-0.1.0/src/autogluon/bench/datasets/object_detection_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,38 @@
 import abc
+import logging
 import os
 
 from autogluon.bench.utils.dataset_utils import get_data_home_dir, get_repo_url
 from autogluon.common.loaders import load_zip
 
 from .constants import _OBJECT_DETECTION
 
 # Add dataset class names here
 __all__ = ["TinyMotorbike", "Clipart"]
 
+logger = logging.getLogger(__name__)
+
 
 class BaseObjectDetectionDataset(abc.ABC):
+    def __init__(self, split: str, dataset_name: str, data_info: dict):
+        """
+        Initializes the class.
+
+        Args:
+            split (str): Specifies the dataset split. It should be one of the following options: 'train', 'val', 'test'.
+        """
+        self._path = os.path.join(get_data_home_dir(), dataset_name)
+        load_zip.unzip(data_info["data"]["url"], unzip_dir=self._path, sha1sum=data_info["data"]["sha1sum"])
+        self._base_folder = os.path.join(self._path, dataset_name)
+        self._data_path = os.path.join(self._base_folder, "Annotations", f"{split}_cocoformat.json")
+        if not os.path.exists(self._data_path):
+            logger.warn(f"No annotation found at {self._data_path}")
+            self._data_path = None
+
     @property
     @abc.abstractmethod
     def base_folder(self):
         pass
 
     @property
     @abc.abstractmethod
@@ -39,18 +57,15 @@
             "sha1sum": "45c883b2feb0721d6eef29055fa28fb46b6e5346",
         },
     }
     _registry_name = "tiny_motorbike"
 
     def __init__(self, split="train"):
         self._split = f"{split}val" if split == "train" else split
-        self._path = os.path.join(get_data_home_dir(), "tiny_motorbike")
-        load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path, sha1sum=self._INFO["data"]["sha1sum"])
-        self._base_folder = os.path.join(self._path, "tiny_motorbike")
-        self._data_path = os.path.join(self._base_folder, "Annotations", f"{self._split}_cocoformat.json")
+        super().__init__(split=self._split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def base_folder(self):
         return self._base_folder
 
     @property
     def data(self):
@@ -69,18 +84,15 @@
             "sha1sum": "d25b2f905da597d7857297ac8e3efe4555e0bf32",
         },
     }
     _registry_name = "clipart"
 
     def __init__(self, split="train"):
         self._split = split
-        self._path = os.path.join(get_data_home_dir(), "clipart")
-        load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path, sha1sum=self._INFO["data"]["sha1sum"])
-        self._base_folder = os.path.join(self._path, "clipart")
-        self._data_path = os.path.join(self._base_folder, "Annotations", f"{self._split}_cocoformat.json")
+        super().__init__(split=self._split, dataset_name=self._registry_name, data_info=self._INFO)
 
     @property
     def base_folder(self):
         return self._base_folder
 
     @property
     def data(self):
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/datasets/registry.py` & `autogluon.bench-0.1.0/src/autogluon/bench/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/benchmark.py` & `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
                 relative_path = os.path.relpath(local_path, self.metrics_dir)
                 s3_path = os.path.join(s3_dir, relative_path)
 
                 # upload the file to S3
                 s3.upload_file(local_path, s3_bucket, s3_path)
 
-        logging.info("Metrics under %s has been saved to %s/%s.", self.metrics_dir, s3_bucket, s3_dir)
+        logging.info("Metrics under %s have been saved to s3://%s/%s.", self.metrics_dir, s3_bucket, s3_dir)
 
     def cleanup_metrics(self):
         """
         Remove benchmark metrics from local and S3 storage.
 
         This method removes the directory specified by `self.benchmark_dir` from the local file system.
         If `self.benchmark_dir_s3` is also specified, it removes the corresponding directory from S3.
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/exec.py` & `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/exec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 import argparse
+import csv
 import json
 import logging
 import os
 import time
 from datetime import datetime
 from typing import Optional
 
 from autogluon.bench.datasets.constants import (
     _IMAGE_SIMILARITY,
     _IMAGE_TEXT_SIMILARITY,
     _OBJECT_DETECTION,
     _TEXT_SIMILARITY,
 )
 from autogluon.bench.datasets.dataset_registry import multimodal_dataset_registry
-from autogluon.bench.utils.general_utils import NumpyEncoder
 from autogluon.multimodal import MultiModalPredictor
+from autogluon.multimodal import __version__ as ag_version
 
 logger = logging.getLogger(__name__)
 
 
+def _flatten_dict(data, separator="_", prefix=""):
+    flattened = {}
+    for key, value in data.items():
+        if isinstance(value, dict):
+            flattened.update(_flatten_dict(value, separator, prefix + key + separator))
+        else:
+            flattened[prefix + key] = value
+    return flattened
+
+
 def get_args():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "--dataset_name",
         type=str,
         help="Dataset that has been registered with multimodal_dataset_registry.",
     )
-
+    parser.add_argument("--framework", type=str, help="Framework (and) branch/version.")
     parser.add_argument("--benchmark_dir", type=str, help="Directory to save benchmarking run.")
     parser.add_argument("--metrics_dir", type=str, help="Directory to save benchmarking metrics.")
     parser.add_argument(
         "--time_limit", type=int, default=None, help="Time limit for the AutoGluon benchmark (in seconds)."
     )
     parser.add_argument("--presets", type=str, default=None, help="Preset configurations to use in the benchmark.")
     parser.add_argument("--hyperparameters", type=str, default=None, help="Hyperparameters to use in the benchmark.")
@@ -48,20 +59,21 @@
     Args:
         dataset_name (str): The name of the dataset to load.
 
     Returns:
         Tuple[pd.DataFrame, pd.DataFrame]: A tuple containing the training and test datasets.
     """
     train_data = multimodal_dataset_registry.create(dataset_name, "train")
+    val_data = multimodal_dataset_registry.create(dataset_name, "val")
     test_data = multimodal_dataset_registry.create(dataset_name, "test")
 
-    return train_data, test_data
+    return train_data, val_data, test_data
 
 
-def save_metrics(metrics_path: str, metrics):
+def save_metrics(metrics_path: str, metrics: dict):
     """Saves evaluation metrics to a JSON file.
 
     Args:
         metrics_path (str): The path to the directory where the metrics should be saved.
         metrics: The evaluation metrics to save.
 
     Returns:
@@ -69,23 +81,29 @@
     """
     if metrics is None:
         logger.warning("No metrics were created.")
         return
 
     if not os.path.exists(metrics_path):
         os.makedirs(metrics_path)
-    file = os.path.join(metrics_path, "metrics.json")
-    with open(file, "w") as f:
-        json.dump(metrics, f, indent=2, cls=NumpyEncoder)
-        logger.info("Metrics saved to %s.", metrics_path)
+    file = os.path.join(metrics_path, "results.csv")
+    flat_metrics = _flatten_dict(metrics)
+    field_names = flat_metrics.keys()
+
+    with open(file, "w", newline="") as f:
+        writer = csv.DictWriter(f, fieldnames=field_names)
+        writer.writeheader()
+        writer.writerow(flat_metrics)
+    logger.info("Metrics saved to %s.", file)
     f.close()
 
 
 def run(
     dataset_name: str,
+    framework: str,
     benchmark_dir: str,
     metrics_dir: str,
     time_limit: Optional[int] = None,
     presets: Optional[str] = None,
     hyperparameters: Optional[dict] = None,
 ):
     """Runs the AutoGluon multimodal benchmark on a given dataset.
@@ -102,15 +120,15 @@
         time_limit (int): The maximum amount of time (in seconds) to spend training the predictor (default: 10).
         presets (str): The name of the AutoGluon preset to use (default: "None").
         hyperparameters (str): A JSON of hyperparameters to use for training (default: None).
 
     Returns:
         None
     """
-    train_data, test_data = load_dataset(dataset_name=dataset_name)
+    train_data, val_data, test_data = load_dataset(dataset_name=dataset_name)
 
     try:
         label_column = train_data.label_columns[0]
     except (AttributeError, IndexError):  # Object Detection does not have label columns
         label_column = None
 
     predictor_args = {
@@ -124,26 +142,26 @@
         predictor_args["query"] = train_data.image_columns[0]
         predictor_args["response"] = train_data.image_columns[1]
         predictor_args["match_label"] = train_data.match_label
     elif train_data.problem_type == _IMAGE_TEXT_SIMILARITY:
         predictor_args["query"] = train_data.text_columns[0]
         predictor_args["response"] = train_data.image_columns[0]
         predictor_args["eval_metric"] = train_data.metric
-        predictor_args["match_label"] = train_data.match_label
         del predictor_args["label"]
     elif train_data.problem_type == _TEXT_SIMILARITY:
         predictor_args["query"] = train_data.text_columns[0]
         predictor_args["response"] = train_data.text_columns[1]
         predictor_args["match_label"] = train_data.match_label
     elif train_data.problem_type == _OBJECT_DETECTION:
         predictor_args["sample_data_path"] = train_data.data
     predictor = MultiModalPredictor(**predictor_args)
 
     fit_args = {
         "train_data": train_data.data,
+        "tuning_data": val_data.data,
         "hyperparameters": hyperparameters,
         "time_limit": time_limit,
     }
 
     utc_time = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S")
     start_time = time.time()
     predictor.fit(**fit_args)
@@ -161,30 +179,39 @@
         evaluate_args["cutoffs"] = [1, 5, 10]
 
     start_time = time.time()
     scores = predictor.evaluate(**evaluate_args)
     end_time = time.time()
     predict_duration = round(end_time - start_time, 1)
 
+    if "#" in framework:
+        framework, version = framework.split("#")
+    else:
+        framework, version = framework, ag_version
+
     metrics = {
-        "problem_type": predictor.problem_type,
+        "task": dataset_name,
+        "framework": framework,
+        "version": version,
+        "type": predictor.problem_type,
         "utc_time": utc_time,
         "training_duration": training_duration,
         "predict_duration": predict_duration,
         "scores": scores,
     }
-    save_metrics(metrics_dir, metrics)
+    save_metrics(os.path.join(metrics_dir, "scores"), metrics)
 
 
 if __name__ == "__main__":
     args = get_args()
     if args.hyperparameters is not None:
         args.hyperparameters = json.loads(args.hyperparameters)
 
     run(
         dataset_name=args.dataset_name,
+        framework=args.framework,
         benchmark_dir=args.benchmark_dir,
         metrics_dir=args.metrics_dir,
         time_limit=args.time_limit,
         presets=args.presets,
         hyperparameters=args.hyperparameters,
     )
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py` & `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,37 +25,44 @@
         run(): Runs the benchmark on a given dataset.
     """
 
     def setup(
         self,
         git_uri: str = "https://github.com/autogluon/autogluon.git",
         git_branch: str = "master",
+        agbench_dev_url: str = None,
     ):
         """
         Sets up the virtual environment for running the benchmark.
 
         Args:
             git_uri (str): The URI of the Git repository to clone (default: "https://github.com/autogluon/autogluon.git").
             git_branch (str): The branch of the Git repository to clone (default: "master").
 
         Returns:
             None
         """
         setup_script_path = os.path.abspath(os.path.dirname(__file__)) + "/setup.sh"
-        command = [setup_script_path, git_uri, git_branch, self.benchmark_dir, agbench_version]
+        command = [setup_script_path, git_uri, git_branch, self.benchmark_dir]
+        if agbench_dev_url is not None:
+            command.append(f"--AGBENCH_DEV_URL={agbench_dev_url}")
+        else:
+            command.append(f"--AG_BENCH_VER={agbench_version}")
         result = subprocess.run(command)
-        if result.stdout:
-            logger.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
-        elif result.stderr:
+        if result.returncode != 0:
             logger.error(result.stderr)
             sys.exit(1)
+        else:
+            logger.info(result.stdout)
+            logger.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
 
     def run(
         self,
         dataset_name: str,
+        framework: str,
         presets: Optional[str] = None,
         hyperparameters: Optional[dict] = None,
         time_limit: Optional[int] = None,
     ):
         """
         Runs the benchmark on a given dataset.
 
@@ -72,19 +79,27 @@
         PY_EXC_PATH = self.benchmark_dir + "/.venv/bin/python"
         exec_path = os.path.abspath(os.path.dirname(__file__)) + "/exec.py"
         command = [
             PY_EXC_PATH,
             exec_path,
             "--dataset_name",
             dataset_name,
+            "--framework",
+            framework,
             "--benchmark_dir",
             self.benchmark_dir,
             "--metrics_dir",
             self.metrics_dir,
         ]
         if presets is not None and len(presets) > 0:
             command += ["--presets", presets]
         if hyperparameters is not None:
             command += ["--hyperparameters", json.dumps(hyperparameters)]
         if time_limit is not None:
             command += ["--time_limit", str(time_limit)]
-        subprocess.run(command)
+        result = subprocess.run(command)
+        if result.returncode != 0:
+            logger.error(result.stderr)
+            sys.exit(1)
+        else:
+            logger.info(result.stdout)
+            logger.info(f"Benchmark {self.benchmark_name} on dataset {dataset_name} is complete.")
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py` & `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import subprocess
-import tempfile
+import sys
+from typing import List
 
 import yaml
 
 from autogluon.bench.frameworks.benchmark import Benchmark
 
 logger = logging.getLogger(__name__)
 
@@ -14,71 +15,84 @@
     def setup(
         self,
     ):
         """Sets up the virtual environment for tabular benchmark."""
         setup_script_path = os.path.abspath(os.path.dirname(__file__)) + "/setup.sh"
         command = [setup_script_path, self.benchmark_dir]
         result = subprocess.run(command)
-        if result.stdout:
-            logging.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
-        elif result.stderr:
-            logging.error(result.stderr)
+        if result.returncode != 0:
+            logger.error(result.stderr)
+            sys.exit(1)
+        else:
+            logger.info(result.stdout)
+            logger.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
 
     def run(
         self,
-        framework: str = "AutoGluon:latest",
         benchmark: str = "test",
         constraint: str = "test",
-        task: str = None,
+        task: List[str] = None,
+        framework: str = None,
         custom_branch: str = None,
     ):
         """Runs the tabular benchmark.
 
         Args:
-            framework (str): The name of the framework to use (default: "AutoGluon:latest").
             benchmark (str): The name of the benchmark to run (default: "test").
             constraint (str): The name of the constraint to use (default: "test").
-            task (str): The name of the task to run (default: None).
+            task (List[str]): The name of the task to run (default: None).
+            framework (str): The name of the framework to use (default: None). Examples: "AutoGluon:latest", "AutoGluon:stable".
             custom_branch (str): The name of the custom branch to use (default: None).
 
         Returns:
             None
         """
-        exec_script_path = os.path.abspath(os.path.dirname(__file__)) + "/exec.sh"
-        command = [
-            exec_script_path,
-            framework,
-            benchmark,
-            constraint,
-            self.benchmark_dir,
-        ]
-
-        if task is not None:
-            command += ["-t", task]
+        if framework is None and custom_branch is None:
+            raise KeyError("Either 'framework' or 'custom_branch' should be provided.")
 
+        custom_branch_dir = None
         if custom_branch is not None:
             custom_repo, custom_branch_name = tuple(custom_branch.split("#"))
+            custom_branch_dir = self.benchmark_dir
 
-            temp_dirpath = tempfile.mkdtemp()
-            custom_framework_name = "AutoGluon_dev"
-            command[1] = custom_framework_name
+            framework = "AutoGluon_dev"
 
             custom_config_contents = {
                 "frameworks": {
                     "definition_file": ["{root}/resources/frameworks.yaml", "{user}/frameworks.yaml"],
                     "allow_duplicates": "true",
                 }
             }
 
-            with open(os.path.join(temp_dirpath, "config.yaml"), "w") as fo:
+            with open(os.path.join(custom_branch_dir, "amlb_configs.yaml"), "w") as fo:
                 yaml.dump(custom_config_contents, fo)
 
             custom_framework_contents = {
-                custom_framework_name: {"extends": "AutoGluon", "repo": custom_repo, "version": custom_branch_name}
+                framework: {"extends": "AutoGluon", "repo": custom_repo, "version": custom_branch_name}
             }
 
-            with open(os.path.join(temp_dirpath, "frameworks.yaml"), "w") as fo:
+            with open(os.path.join(custom_branch_dir, "frameworks.yaml"), "w") as fo:
                 yaml.dump(custom_framework_contents, fo)
 
-            command += ["-c", temp_dirpath]
+        exec_script_path = os.path.abspath(os.path.dirname(__file__)) + "/exec.sh"
+        command = [
+            exec_script_path,
+            framework,
+            benchmark,
+            constraint,
+            self.benchmark_dir,
+            self.metrics_dir,
+        ]
+
+        if custom_branch_dir is not None:
+            command += ["-c", custom_branch_dir]
 
-        subprocess.run(command)
+        if task is not None:
+            command += ["-t", " ".join(task)]
+
+        result = subprocess.run(command)
+        if result.returncode != 0:
+            logger.error(result.stderr)
+            sys.exit(1)
+        else:
+            logger.info(result.stdout)
+            logger.info(f"Benchmark {self.benchmark_name} is complete.")
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/runbenchmark.py` & `autogluon.bench-0.1.0/src/autogluon/bench/runbenchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 app = typer.Typer()
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
-def get_kwargs(module: str, configs: dict):
+def get_kwargs(module: str, configs: dict, agbench_dev_url: str):
     """Returns a dictionary of keyword arguments to be used for setting up and running the benchmark.
 
     Args:
         module (str): The name of the module to benchmark (either "multimodal" or "tabular").
         configs (dict): A dictionary of configuration options for the benchmark.
 
     Returns:
@@ -36,46 +36,44 @@
 
     if module == "multimodal":
         git_uri, git_branch = configs["git_uri#branch"].split("#")
         return {
             "setup_kwargs": {
                 "git_uri": git_uri,
                 "git_branch": git_branch,
+                "agbench_dev_url": agbench_dev_url,
             },
             "run_kwargs": {
                 "dataset_name": configs["dataset_name"],
+                "framework": configs["git_uri#branch"].split("/")[-1],
                 "presets": configs.get("presets"),
                 "hyperparameters": configs.get("hyperparameters"),
                 "time_limit": configs.get("time_limit"),
             },
         }
     elif module == "tabular":
         return {
             "setup_kwargs": {},
             "run_kwargs": {
-                "framework": f'{configs["framework"]}:{configs["label"]}',
                 "benchmark": configs["amlb_benchmark"],
                 "constraint": configs["amlb_constraint"],
-                "task": configs.get("amlb_task"),
+                "task": configs.get("amlb_task") if configs.get("amlb_task") else None,
+                "framework": configs.get("framework"),
                 "custom_branch": configs.get("amlb_custom_branch"),
             },
         }
 
 
 def _get_benchmark_name(configs: dict) -> str:
     default_benchmark_name = "ag_bench"
     benchmark_name = configs.get("benchmark_name", default_benchmark_name) or default_benchmark_name
     return benchmark_name
 
 
-def run_benchmark(
-    benchmark_name: str,
-    benchmark_dir: str,
-    configs: dict,
-):
+def run_benchmark(benchmark_name: str, benchmark_dir: str, configs: dict, agbench_dev_url: str = None):
     """Runs a benchmark based on the provided configuration options.
 
     Args:
         configs (dict): A dictionary of configuration options for the benchmark.
 
     Returns:
         None
@@ -89,22 +87,22 @@
 
     benchmark_class = module_to_benchmark.get(module_name, None)
     if benchmark_class is None:
         raise NotImplementedError
 
     benchmark = benchmark_class(benchmark_name=benchmark_name, benchmark_dir=benchmark_dir)
 
-    module_kwargs = get_kwargs(module=module_name, configs=configs)
+    module_kwargs = get_kwargs(module=module_name, configs=configs, agbench_dev_url=agbench_dev_url)
     benchmark.setup(**module_kwargs.get("setup_kwargs", {}))
     benchmark.run(**module_kwargs.get("run_kwargs", {}))
     logger.info(f"Backing up benchmarking configs to {benchmark.metrics_dir}/configs.yaml")
     _dump_configs(benchmark_dir=benchmark.metrics_dir, configs=configs, file_name="configs.yaml")
 
     if configs.get("METRICS_BUCKET", None):
-        s3_dir = f"{module_name}{benchmark_dir.split(module_name)[-1]}"
+        s3_dir = f"{module_name}{benchmark_dir.split(module_name, 1)[-1]}"
         benchmark.upload_metrics(s3_bucket=configs["METRICS_BUCKET"], s3_dir=s3_dir)
 
 
 def upload_config(bucket: str, benchmark_name: str, file: str):
     """Uploads a configuration file to an S3 bucket.
 
     Args:
@@ -152,39 +150,36 @@
 
     Returns:
         A dictionary containing Lambda response payload.
     """
 
     lambda_client = boto3.client("lambda", configs["CDK_DEPLOY_REGION"])
     payload = {"config_file": config_file}
+    lambda_function_name = configs["LAMBDA_FUNCTION_NAME"] + "-" + configs["STACK_NAME_PREFIX"]
     response = lambda_client.invoke(
-        FunctionName=configs["LAMBDA_FUNCTION_NAME"], InvocationType="RequestResponse", Payload=json.dumps(payload)
+        FunctionName=lambda_function_name, InvocationType="RequestResponse", Payload=json.dumps(payload)
     )
     response = json.loads(response["Payload"].read().decode("utf-8"))
     logger.info("AWS Batch jobs submitted by %s.", configs["LAMBDA_FUNCTION_NAME"])
 
     return response
 
 
 @app.command()
 def get_job_status(
     job_ids: Optional[List[str]] = typer.Option(None, "--job-ids", help="List of job ids, separated by space."),
-    cdk_deploy_region: Optional[str] = typer.Option(
-        None, "--cdk_deploy_region", help="AWS region that the Batch jobs run in."
-    ),
-    config_file: Optional[str] = typer.Option(
-        None, "--config-file", help="Path to YAML config file containing job ids."
-    ),
+    cdk_deploy_region: Optional[str] = typer.Option(None, help="AWS region that the Batch jobs run in."),
+    config_file: Optional[str] = typer.Option(None, help="Path to YAML config file containing job ids."),
 ):
     """
     Query the status of AWS Batch job ids.
     The job ids can either be passed in directly or read from a YAML configuration file.
 
     Args:
-        job_ids (list[str], optional):
+        job_ids (List[str], optional):
             A list of job ids to query the status for.
         cdk_deploy_region (str, optional):
             AWS region that the Batch jobs run in.
         config_file (str, optional):
             A path to a YAML config file containing job ids. The YAML file should have the structure:
                 job_configs:
                     <job_id>: <job_config>
@@ -213,15 +208,15 @@
         status_dict[job_id] = job["status"]
 
     logger.info(status_dict)
     return status_dict
 
 
 def wait_for_jobs_to_complete(
-    config_file: Optional[str] = None, job_ids: Optional[list[str]] = None, aws_region: Optional[str] = None
+    config_file: Optional[str] = None, job_ids: Optional[List[str]] = None, aws_region: Optional[str] = None
 ):
     while True:
         all_jobs_completed = True
         failed_jobs = []
 
         try:
             job_status = get_job_status(job_ids=job_ids, cdk_deploy_region=aws_region, config_file=config_file)
@@ -262,19 +257,20 @@
         yaml.dump(configs, file)
         logger.info(f"Configs have been saved to {config_path}")
     return config_path
 
 
 @app.command()
 def run(
-    config_file: Annotated[str, typer.Argument(help="Path to custom config file.")],
-    remove_resources: Annotated[bool, typer.Option("--remove_resources", help="Remove resources after run.")] = False,
+    config_file: str = typer.Argument(..., help="Path to custom config file."),
+    remove_resources: bool = typer.Option(False, help="Remove resources after run."),
+    wait: bool = typer.Option(False, help="Whether to block and wait for the benchmark to finish."),
+    dev_branch: Optional[str] = typer.Option(None, help="Path to a development AutoGluon-Bench branch."),
 ):
     """Main function that runs the benchmark based on the provided configuration options."""
-
     configs = {}
     if config_file.startswith("s3"):
         config_file = download_config(s3_path=config_file)
     with open(config_file, "r") as f:
         configs = yaml.safe_load(f)
 
     benchmark_name = _get_benchmark_name(configs=configs)
@@ -286,49 +282,67 @@
     benchmark_dir = os.path.join(root_dir, configs["module"], benchmark_name)
 
     if configs["mode"] == "aws":
         configs["benchmark_name"] = benchmark_name
         cloud_config_path = _dump_configs(
             benchmark_dir=benchmark_dir, configs=configs, file_name=os.path.basename(config_file)
         )
-        os.environ["AG_BENCH_VERSION"] = agbench_version  # set the installed version for Dockerfile to align with
-        infra_configs = deploy_stack(configs=configs.get("cdk_context", {}))
+        if dev_branch is not None:
+            os.environ["AG_BENCH_DEV_URL"] = dev_branch  # pull dev branch from GitHub
+        else:
+            os.environ["AG_BENCH_VERSION"] = agbench_version  # set the installed version for Dockerfile to align with
+        infra_configs = deploy_stack(custom_configs=configs.get("cdk_context", {}))
         config_s3_path = upload_config(
             bucket=infra_configs["METRICS_BUCKET"], benchmark_name=benchmark_name, file=cloud_config_path
         )
         lambda_response = invoke_lambda(configs=infra_configs, config_file=config_s3_path)
         aws_configs = {**infra_configs, **lambda_response}
         logger.info(f"Saving infra configs and submitted job configs under {benchmark_dir}.")
         aws_config_path = _dump_configs(benchmark_dir=benchmark_dir, configs=aws_configs, file_name="aws_configs.yaml")
 
         if remove_resources:
-            logger.info("Waiting for jobs to complete and then remove the AWS resources created.")
+            wait = True
+        if wait:
             logger.info(
-                "You can quit at anytime and run \n"
-                "`agbench destroy-stack STATIC_RESOURCE_STACK BATCH_STACK CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION` "
-                "to delete the stack after jobs have run to completion."
+                "Waiting for jobs to complete. You can quit at anytime and the benchmark will continue to run on the cloud"
             )
+            if remove_resources:
+                logger.info(
+                    "Resources will be deleted after the jobs are finished. You can also call \n"
+                    f"`agbench destroy-stack --config-file {aws_config_path}` "
+                    "to delete the stack after jobs have run to completion if you choose to quit now."
+                )
+
             failed_jobs = wait_for_jobs_to_complete(config_file=aws_config_path)
-            if failed_jobs:
-                logger.warning("Some jobs have failed: %s. Resources are not being removed.", failed_jobs)
+            if len(failed_jobs) > 0:
+                logger.warning("Some jobs have failed: %s.", failed_jobs)
+                if remove_resources:
+                    logger.warning("Resources will be kept so error logs can be accessed")
             elif failed_jobs is None:
-                logger.error("Resources are not being removed due to errors.")
+                if remove_resources:
+                    logger.error("Resources are not being removed due to errors.")
             else:
-                destroy_stack(
-                    static_resource_stack=infra_configs["STATIC_RESOURCE_STACK_NAME"],
-                    batch_stack=infra_configs["BATCH_STACK_NAME"],
-                    cdk_deploy_account=infra_configs["CDK_DEPLOY_ACCOUNT"],
-                    cdk_deploy_region=infra_configs["CDK_DEPLOY_REGION"],
-                )
+                logger.info("All job succeeded.")
+                if remove_resources:
+                    logger.info("Removing resoureces...")
+                    destroy_stack(
+                        static_resource_stack=infra_configs["STATIC_RESOURCE_STACK_NAME"],
+                        batch_stack=infra_configs["BATCH_STACK_NAME"],
+                        cdk_deploy_account=infra_configs["CDK_DEPLOY_ACCOUNT"],
+                        cdk_deploy_region=infra_configs["CDK_DEPLOY_REGION"],
+                        config_file=None,
+                    )
+                    logger.info("Resources removed successfully.")
 
     elif configs["mode"] == "local":
         split_id = _get_split_id(config_file)
         if split_id is not None:
             benchmark_name += "_" + split_id
             benchmark_dir = os.path.join(benchmark_dir, benchmark_name)
+        logger.info(f"Running benchmark {benchmark_name} at {benchmark_dir}.")
+        if dev_branch is not None:
+            logger.info(f"Using dev branch at {dev_branch}...")
         run_benchmark(
-            benchmark_name=benchmark_name,
-            benchmark_dir=benchmark_dir,
-            configs=configs,
+            benchmark_name=benchmark_name, benchmark_dir=benchmark_dir, configs=configs, agbench_dev_url=dev_branch
         )
     else:
         raise NotImplementedError
```

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/utils/dataset_utils.py` & `autogluon.bench-0.1.0/src/autogluon/bench/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/src/autogluon/bench/utils/general_utils.py` & `autogluon.bench-0.1.0/src/autogluon/bench/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.4/src/autogluon.bench.egg-info/PKG-INFO` & `autogluon.bench-0.1.0/src/autogluon.bench.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.0.4
+Version: 0.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/autogluon/autogluon-bench
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-bench/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-bench/
 Description: <div align="left">
@@ -37,26 +37,30 @@
         git clone https://github.com/autogluon/autogluon-bench.git
         cd autogluon-bench
         
         # install from source in editable mode
         pip install -e .
         ```
         
-        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). To ensure that your local changes are reflected in the installed package, you may need to adjust the installation command as necessary. A recommended approach is to push your changes to a remote git branch and then pull from this branch, installing the package from source in the scripts.
+        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
+        
+        ```
+        agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+        ```
         
         
         ## Run benchmarks locally
         
         To run the benchmarks on your local machine, use the following command:
         
         ```
         agbench run path/to/local_config_file
         ```
         
-        Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
+        Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
         
         The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
         
         
         ### Tabular Benchmark
         
         To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
@@ -83,15 +87,39 @@
         3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
         ```bash
         nvm install $VERSION  # install Node.js
         npm install -g aws-cdk  # install aws-cdk
         cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
         ```
         
-        To initiate benchmarking on the cloud, use the command below:
+        If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
+        
+        ```bash
+        cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
+        ```
+        
+        You will need a cloud configuration file to run the benchmarks. You can edit the provided [sample cloud config files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs), or use the CLI tool to generate the cloud config files locally.
+        
+        For multimodal:
+        
+        ```
+        agbench generate-cloud-config --module multimodal --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --git-uri-branch <GIT_URI#BRANCH> --dataset-names DATASET_1,DATASET_2 --presets <PRESET_1>,<PRESET_2> --time-limit <TIME_LIMIT_1>,<TIME_LIMIT_2> --hyperparameters "key_1:value_1,key_2:value_2;key_1:value_3,key_2:value_4"
+        ```
+        
+        For tabular:
+        ```
+        agbench generate-cloud-config --module tabular --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --framework <FRAMEWORK>:<LABEL> --amlb-benchmark <BENCHMARK1>,<BENCHMARK2> --amlb-task "BENCHMARK1:DATASET1,DATASET2;BENCHMARK2:DATASET3" --amlb-constraint <CONSTRAINT>
+        ```
+        
+        For more details, you can run
+        ```
+        agbench generate-cloud-config --help
+        ```
+        
+        After having the configuration file ready, use the command below to initiate benchmark runs on cloud:
         
         ```
         agbench run /path/to/cloud_config_file
         ```
         
         This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
         
@@ -108,81 +136,98 @@
         ```bash
         agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
         
         ```
         
         Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
         
+        A cloud configuration file with time-stamped `benchmark_name` is also saved under `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml`
+        
         By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
         
         ```bash
-        agbench run path/to/cloud_config_file --remove_resources
+        agbench run path/to/cloud_config_file --remove-resources
         ```
         
         This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
         
         If you want to manually remove resources later, use:
         
         ```bash
-        agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
+        agbench destroy-stack --config-file `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`
         ```
         
+        Or you can remove specific stacks by running:
+        
+        ```bash
+        agbench destroy-stack --static-resource-stack STATIC_RESOURCE_STACK_NAME --batch-stack BATCH_STACK_NAME --cdk-deploy-account CDK_DEPLOY_ACCOUNT --cdk-deploy-region CDK_DEPLOY_REGION
+        ```
         where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
         
         
         ### Configure the AWS infrastructure
         
         The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
         
         where:
         - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
         - `PREFIX` is used as an identifier for the stack and resources created.
         - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
         - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
         - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
         
-        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
+        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabular_cloud_configs.yaml) for reference.
+        
         
         ## Evaluating bechmark runs
         
-        Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
-        Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
+        Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
+        In a future release, we intend to add evaluation support for multimodal benchmark results.
+        
         
         ### Evaluation Steps
         
-        Clone the `autogluon-benchmark` repository:
+        Begin by setting up AWS credentials for the default profile for the AWS account that has the benchmark results in S3.
+        
+        Step 1: Aggregate AMLB results on S3. After running the benchmark in [AWS mode](#run-benchmarks-on-aws), take note of the `benchmark_name` with timestamp in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml` and run the command below:
         ```
-        git clone https://github.com/gidler/autogluon-benchmark.git
+        agbench aggregate-amlb-results {METRICS_BUCKET} {module} {benchmark_name} --constraint {constraint}
         ```
         
-        Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
-        
-        Run the `aggregate_all.py` script
+        This will create a new file on S3 with this signature:
         ```
-        python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
-        
-        # example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
+        s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/results_automlbenchmark_{constraint}_{benchmark_name}.csv
         ```
         
-        This will create a new file in S3 with this signature:
+        Currently, aggregation is also supported for multimodal benchmark results without the `--constratint` option.
+        
+        For more details, run:
         ```
-        s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
+        agbench aggregate-amlb-results --help
         ```
         
-        Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
+        Step 2: Further clean the aggregated results.
+        
+        If the file is still on S3 from the previous step, run:
         ```
-        python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
+        agbench clean-amlb-results {benchmark_name} --results-dir-input s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/ --benchmark-name-in-input-path --constraints constratint_1 --constraints constratint_2 --results-dir-output {results_dir_output} 
+        --out-path-prefix {out_path_prefix} --out-path-suffix {out_path_suffix}
         ```
-        This will create a local file of results in the `data/results/input/prepared/openml/` directory.
+        where `{results_dir_input}` can also be a local directory. This will create a local file `{results_dir_output}/{out_path_prefix}{benchmark_name}{out_path_suffix}`.
         
-        Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
+        For more details, run:
         ```
-        python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
+        agbench clean-amlb-results --help
         ```
         
+        Step 3: Run evaluation on multiple cleaned files from `Step 2`
+        
+        ```
+        agbench evaluate-amlb-results --frameworks_run framework_1 --frameworks_run framework_2 --results-dir-input data/results/input/prepared/openml --paths file_name_1.csv --paths file_name_2.csv --no-clean-data
+        ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
```

