# Comparing `tmp/sensenova-1.0.0.tar.gz` & `tmp/sensenova-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensenova-1.0.0.tar", last modified: Thu Jun 29 09:13:39 2023, max compression
+gzip compressed data, was "sensenova-1.0.1.tar", last modified: Tue Jul 11 11:00:14 2023, max compression
```

## Comparing `sensenova-1.0.0.tar` & `sensenova-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 09:13:39.313519 sensenova-1.0.0/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.0/LICENSE
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2466 2023-06-29 09:13:39.317520 sensenova-1.0.0/PKG-INFO
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2198 2023-06-29 07:30:41.000000 sensenova-1.0.0/README.md
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.0/pyproject.toml
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 09:13:39.273519 sensenova-1.0.0/sensenova/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/_sensenova_scripts.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_requestor.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 09:13:39.281519 sensenova-1.0.0/sensenova/api_resources/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/__init__.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 09:13:39.285519 sensenova-1.0.0/sensenova/api_resources/abstract/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      691 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/createable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/deletable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/downloadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/engine_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/fileable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/listable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/abstract/uploadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/dataset.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/error_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/fine_tune.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      507 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/knowledge_base.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/model.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/api_resources/serving.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    16914 2023-06-29 07:30:41.000000 sensenova-1.0.0/sensenova/cli.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/error.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/object_classes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/sensenova_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/sensenova_response.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 09:13:39.313519 sensenova-1.0.0/sensenova/tests/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      867 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3730 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_datasets.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1158 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_fine_tunes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2066 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_knowlege_bases.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      348 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_models.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_prepare_data.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      973 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/tests/test_servings.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/upload_progress.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/util.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-06-29 07:11:49.000000 sensenova-1.0.0/sensenova/validators.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-06-29 09:13:13.000000 sensenova-1.0.0/sensenova/version.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 09:13:39.277519 sensenova-1.0.0/sensenova.egg-info/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2466 2023-06-29 09:13:39.000000 sensenova-1.0.0/sensenova.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1725 2023-06-29 09:13:39.000000 sensenova-1.0.0/sensenova.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-06-29 09:13:39.000000 sensenova-1.0.0/sensenova.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       65 2023-06-29 09:13:39.000000 sensenova-1.0.0/sensenova.egg-info/entry_points.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       71 2023-06-29 09:13:39.000000 sensenova-1.0.0/sensenova.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-06-29 09:13:39.000000 sensenova-1.0.0/sensenova.egg-info/top_level.txt
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      613 2023-06-29 09:13:39.317520 sensenova-1.0.0/setup.cfg
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.0/setup.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.821371 sensenova-1.0.1/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.1/LICENSE
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-11 11:00:14.821371 sensenova-1.0.1/PKG-INFO
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2124 2023-07-11 10:58:41.000000 sensenova-1.0.1/README.md
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.1/pyproject.toml
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.801371 sensenova-1.0.1/sensenova/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/_sensenova_scripts.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_requestor.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.813371 sensenova-1.0.1/sensenova/api_resources/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/__init__.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.817371 sensenova-1.0.1/sensenova/api_resources/abstract/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      691 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/createable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/deletable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/downloadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/engine_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/fileable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/listable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/uploadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/dataset.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/error_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/fine_tune.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      507 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/knowledge_base.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/model.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/serving.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    16914 2023-06-29 07:30:41.000000 sensenova-1.0.1/sensenova/cli.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/error.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/object_classes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/sensenova_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/sensenova_response.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.821371 sensenova-1.0.1/sensenova/tests/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      867 2023-07-11 10:58:01.000000 sensenova-1.0.1/sensenova/tests/test_chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3730 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_datasets.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1158 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_fine_tunes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2066 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_knowlege_bases.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      348 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_models.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_prepare_data.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      973 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_servings.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/upload_progress.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-07-11 10:58:24.000000 sensenova-1.0.1/sensenova/util.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/validators.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-11 10:59:24.000000 sensenova-1.0.1/sensenova/version.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.809371 sensenova-1.0.1/sensenova.egg-info/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1725 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       65 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/entry_points.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       71 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/top_level.txt
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      613 2023-07-11 11:00:14.825371 sensenova-1.0.1/setup.cfg
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.1/setup.py
```

### Comparing `sensenova-1.0.0/LICENSE` & `sensenova-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/PKG-INFO` & `sensenova-1.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-Metadata-Version: 2.1
-Name: sensenova
-Version: 1.0.0
-Summary: Python client library for the Sensenova API
-Home-page: UNKNOWN
-Author: Sensetime
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Sensenova Python Library
 
 The Sensenova Python library provides convenient access to the Sensenova API from applications written in the Python
 language.
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
-pip install -i http://spring.sensetime.com/pypi/ --trusted-host spring.sensetime.com --upgrade sensenova 
+pip install --upgrade sensenova
 ```
 
 Install from source with:
 
 ```sh
 python setup.py install
 ```
@@ -111,9 +99,8 @@
 
 ```sh
 sensenova tools fine_tunes.prepare_data -f data.json
 ```
 
 ## Requirements
 
-- Python 3.7.1+
-
+- Python 3.7.1+
```

### Comparing `sensenova-1.0.0/README.md` & `sensenova-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+Metadata-Version: 2.1
+Name: sensenova
+Version: 1.0.1
+Summary: Python client library for the Sensenova API
+Home-page: UNKNOWN
+Author: Sensetime
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.7.1
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Sensenova Python Library
 
 The Sensenova Python library provides convenient access to the Sensenova API from applications written in the Python
 language.
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
-pip install -i http://spring.sensetime.com/pypi/ --trusted-host spring.sensetime.com --upgrade sensenova 
+pip install --upgrade sensenova
 ```
 
 Install from source with:
 
 ```sh
 python setup.py install
 ```
@@ -99,8 +111,9 @@
 
 ```sh
 sensenova tools fine_tunes.prepare_data -f data.json
 ```
 
 ## Requirements
 
-- Python 3.7.1+
+- Python 3.7.1+
+
```

### Comparing `sensenova-1.0.0/sensenova/__init__.py` & `sensenova-1.0.1/sensenova/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/_sensenova_scripts.py` & `sensenova-1.0.1/sensenova/_sensenova_scripts.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_requestor.py` & `sensenova-1.0.1/sensenova/api_requestor.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/__init__.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/createable_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/deletable_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/downloadable_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/downloadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/engine_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/fileable_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/fileable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/listable_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/abstract/uploadable_api_resource.py` & `sensenova-1.0.1/sensenova/api_resources/abstract/uploadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/chat_completion.py` & `sensenova-1.0.1/sensenova/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/error_object.py` & `sensenova-1.0.1/sensenova/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/fine_tune.py` & `sensenova-1.0.1/sensenova/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/finetune_completion.py` & `sensenova-1.0.1/sensenova/api_resources/finetune_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/api_resources/serving.py` & `sensenova-1.0.1/sensenova/api_resources/serving.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/cli.py` & `sensenova-1.0.1/sensenova/cli.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/error.py` & `sensenova-1.0.1/sensenova/error.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/sensenova_object.py` & `sensenova-1.0.1/sensenova/sensenova_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/tests/test_chat_completion.py` & `sensenova-1.0.1/sensenova/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/tests/test_datasets.py` & `sensenova-1.0.1/sensenova/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/tests/test_fine_tunes.py` & `sensenova-1.0.1/sensenova/tests/test_fine_tunes.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/tests/test_knowlege_bases.py` & `sensenova-1.0.1/sensenova/tests/test_knowlege_bases.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/tests/test_prepare_data.py` & `sensenova-1.0.1/sensenova/tests/test_prepare_data.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/tests/test_servings.py` & `sensenova-1.0.1/sensenova/tests/test_servings.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/upload_progress.py` & `sensenova-1.0.1/sensenova/upload_progress.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/util.py` & `sensenova-1.0.1/sensenova/util.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova/validators.py` & `sensenova-1.0.1/sensenova/validators.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/sensenova.egg-info/PKG-INFO` & `sensenova-1.0.1/sensenova.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python client library for the Sensenova API
 Home-page: UNKNOWN
 Author: Sensetime
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
-pip install -i http://spring.sensetime.com/pypi/ --trusted-host spring.sensetime.com --upgrade sensenova 
+pip install --upgrade sensenova
 ```
 
 Install from source with:
 
 ```sh
 python setup.py install
 ```
```

### Comparing `sensenova-1.0.0/sensenova.egg-info/SOURCES.txt` & `sensenova-1.0.1/sensenova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.0/setup.cfg` & `sensenova-1.0.1/setup.cfg`

 * *Files identical despite different names*

