# Comparing `tmp/datumaro-1.4.0rc1.tar.gz` & `tmp/datumaro-1.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.4.0rc1.tar", last modified: Fri Jul  7 13:23:30 2023, max compression
+gzip compressed data, was "datumaro-1.4.0rc2.tar", last modified: Tue Jul 11 06:20:52 2023, max compression
```

## Comparing `datumaro-1.4.0rc1.tar` & `datumaro-1.4.0rc2.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.620827 datumaro-1.4.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)   375078 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-07 13:23:30.620827 datumaro-1.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:23:30.620827 datumaro-1.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.544827 datumaro-1.4.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.560827 datumaro-1.4.0rc1/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.560827 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.572827 datumaro-1.4.0rc1/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.572827 datumaro-1.4.0rc1/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.572827 datumaro-1.4.0rc1/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29044 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.580827 datumaro-1.4.0rc1/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.580827 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.580827 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.592827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28677 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.592827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.592827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31336 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    46895 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.616827 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.616827 datumaro-1.4.0rc1/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)   375078 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.674769 datumaro-1.4.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.698771 datumaro-1.4.0rc2/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.702771 datumaro-1.4.0rc2/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.702771 datumaro-1.4.0rc2/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.710772 datumaro-1.4.0rc2/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29610 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.718772 datumaro-1.4.0rc2/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.718772 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.718772 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.722772 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.722772 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28677 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16682 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31336 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.702771 datumaro-1.4.0rc2/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.4.0rc1/3rd-party.txt` & `datumaro-1.4.0rc2/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/LICENSE` & `datumaro-1.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/PKG-INFO` & `datumaro-1.4.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc1/README.md` & `datumaro-1.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/pyproject.toml` & `datumaro-1.4.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/requirements-core.txt` & `datumaro-1.4.0rc2/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/setup.py` & `datumaro-1.4.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/capi/pybind.cpp` & `datumaro-1.4.0rc2/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/__main__.py` & `datumaro-1.4.0rc2/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/compare.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/convert.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/download.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/explain.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/explore.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/filter.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/generate.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging as log
 import os
 import os.path as osp
 from shutil import rmtree
 
 from datumaro.cli.util.errors import CliException
 from datumaro.plugins.synthetic_data import FractalImageGenerator
-from datumaro.util.definitions import DATUMARO_CACHE_DIR
+from datumaro.util.definitions import get_datumaro_cache_dir
 
 from ..util import MultilineFormatter
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Generate synthetic dataset",
@@ -54,15 +54,15 @@
         default="image",
         choices=["image"],
         help="Specify type of data to generate (default: %(default)s)",
     )
     parser.add_argument(
         "--model-dir",
         type=str,
-        default=DATUMARO_CACHE_DIR,
+        default=get_datumaro_cache_dir(),
         help="Path to load the colorization model from. "
         "If no model is found, the model will be downloaded (default: %(default)s)",
     )
     parser.add_argument(
         "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
     )
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/info.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/merge.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/patch.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/prune.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/stats.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/transform.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/commands/validate.py` & `datumaro-1.4.0rc2/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/contexts/model.py` & `datumaro-1.4.0rc2/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/contexts/source.py` & `datumaro-1.4.0rc2/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/contexts/util.py` & `datumaro-1.4.0rc2/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/util/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/util/compare.py` & `datumaro-1.4.0rc2/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/cli/util/project.py` & `datumaro-1.4.0rc2/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/abstracts/merger.py` & `datumaro-1.4.0rc2/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.4.0rc2/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,19 +156,19 @@
                     if center_dict.get(label_) is None:
                         center_dict[label_] = item
             if all(center_dict.values()):
                 break
 
         item_id_list = [item.id.split("/")[-1] for item in item_list]
         centroids = [
-            database_keys[item_id_list.index(i.id.split(":")[-1])]
-            for i in list(center_dict.values())
-            if i
+            database_keys[item_id_list.index(item.id)] for item in center_dict.values() if item
         ]
-        kmeans = KMeans(n_clusters=num_centers, n_init=1, init=centroids, random_state=0)
+        kmeans = KMeans(
+            n_clusters=num_centers, n_init=1, init=np.stack(centroids, axis=0), random_state=0
+        )
 
         clusters = kmeans.fit_predict(database_keys)
         cluster_centers = kmeans.cluster_centers_
         cluster_ids, cluster_num_item_list = np.unique(clusters, return_counts=True)
 
         norm_cluster_num_item_list = match_num_item_for_cluster(
             ratio, len(database_keys), cluster_num_item_list
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/algorithms/rise.py` & `datumaro-1.4.0rc2/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/annotation.py` & `datumaro-1.4.0rc2/src/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/annotations/matcher.py` & `datumaro-1.4.0rc2/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/annotations/merger.py` & `datumaro-1.4.0rc2/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/cli_plugin.py` & `datumaro-1.4.0rc2/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/comparator.py` & `datumaro-1.4.0rc2/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/config.py` & `datumaro-1.4.0rc2/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/config_model.py` & `datumaro-1.4.0rc2/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/crypter.py` & `datumaro-1.4.0rc2/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/dataset.py` & `datumaro-1.4.0rc2/src/datumaro/components/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
     Dataset is supposed to have a single media type for its items. If the
     dataset is filled manually or from extractors, and media type does not
     match, an error is raised.
     """
 
     _global_eager: bool = False
+    _stream = False
 
     @classmethod
     def from_iterable(
         cls,
         iterable: Iterable[DatasetItem],
         infos: Optional[DatasetInfo] = None,
         categories: Union[CategoriesInfo, List[str], None] = None,
@@ -189,16 +190,17 @@
                 return infos
 
             def categories(self):
                 return categories
 
         return cls.from_extractors(_extractor(), env=env)
 
-    @staticmethod
+    @classmethod
     def from_extractors(
+        cls,
         *sources: IDataset,
         env: Optional[Environment] = None,
         merge_policy: str = DEFAULT_MERGE_POLICY,
     ) -> Dataset:
         """
         Creates a new dataset from one or several `Extractor`s.
 
@@ -215,15 +217,15 @@
 
         Returns:
             dataset: A new dataset with contents produced by input extractors
         """
 
         if len(sources) == 1:
             source = sources[0]
-            dataset = Dataset(source=source, env=env)
+            dataset = cls(source=source, env=env)
         else:
             from datumaro.components.hl_ops import HLOps
 
             return HLOps.merge(*sources, merge_policy=merge_policy)
 
         return dataset
 
@@ -596,17 +598,17 @@
                 except TypeError as e:
                     # TODO: for backward compatibility. To be removed after 0.3
                     if "unexpected keyword argument 'ctx'" not in str(e):
                         raise
 
                     if has_ctx_args:
                         warnings.warn(
-                            "It seems that '%s' exporter "
+                            f"It seems that '{format}' exporter "
                             "does not support progress and error reporting, "
-                            "it will be disabled" % format,
+                            "It will be disabled in datumaro==1.5.0.",
                             DeprecationWarning,
                         )
                     exporter_kwargs.pop("ctx")
 
                     exporter.convert(self, save_dir=save_dir, **exporter_kwargs)
             else:
                 try:
@@ -614,17 +616,17 @@
                 except TypeError as e:
                     # TODO: for backward compatibility. To be removed after 0.3
                     if "unexpected keyword argument 'ctx'" not in str(e):
                         raise
 
                     if has_ctx_args:
                         warnings.warn(
-                            "It seems that '%s' exporter "
+                            f"It seems that '{format}' exporter "
                             "does not support progress and error reporting, "
-                            "it will be disabled" % format,
+                            "It will be disabled in datumaro==1.5.0.",
                             DeprecationWarning,
                         )
                     exporter_kwargs.pop("ctx")
 
                     exporter.patch(self, self.get_patch(), save_dir=save_dir, **exporter_kwargs)
         except _ExportFail as e:
             raise e.__cause__
@@ -673,19 +675,25 @@
 
         if env is None:
             env = DEFAULT_ENVIRONMENT
 
         if not format:
             format = cls.detect(path, env=env)
 
+        extractor_merger = None
         # TODO: remove importers, put this logic into extractors
         if format in env.importers:
             importer = env.make_importer(format)
             with logging_disabled(log.INFO):
-                detected_sources = importer(path, **kwargs)
+                detected_sources = (
+                    importer(path, stream=cls._stream, **kwargs)
+                    if importer.can_stream
+                    else importer(path, **kwargs)
+                )
+            extractor_merger = importer.get_extractor_merger()
         elif format in env.extractors:
             detected_sources = [{"url": path, "format": format, "options": kwargs}]
         else:
             raise UnknownFormatError(format)
 
         # TODO: probably, should not be available in lazy mode, because it
         # becomes unreliable and error-prone. For progress reporting it
@@ -720,26 +728,30 @@
                 except TypeError as e:
                     # TODO: for backward compatibility. To be removed after 0.3
                     if "unexpected keyword argument 'ctx'" not in str(e):
                         raise
 
                     if has_ctx_args:
                         warnings.warn(
-                            "It seems that '%s' extractor "
-                            "does not support progress and error reporting, "
-                            "it will be disabled" % src_conf.format,
+                            f"It seems that '{src_conf.format}' extractor "
+                            "does not support progress and error reporting. "
+                            "It will be disabled in datumaro==1.5.0.",
                             DeprecationWarning,
                         )
                     extractor_kwargs.pop("ctx")
 
                     extractors.append(
                         env.make_extractor(src_conf.format, src_conf.url, **extractor_kwargs)
                     )
 
-            dataset = cls.from_extractors(*extractors, env=env, merge_policy=merge_policy)
+            dataset = (
+                cls(source=extractor_merger(*extractors), env=env)
+                if extractor_merger is not None
+                else cls.from_extractors(*extractors, env=env, merge_policy=merge_policy)
+            )
             if eager:
                 dataset.init_cache()
         except _ImportFail as e:
             cause = e.__cause__ if getattr(e, "__cause__", None) is not None else e
             cause.__traceback__ = e.__traceback__
             raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from cause
         except Exception as e:
@@ -776,14 +788,18 @@
         if not matches:
             raise NoMatchingFormatsError()
         elif 1 < len(matches):
             raise MultipleFormatsMatchError(matches)
         else:
             return matches[0]
 
+    @property
+    def is_stream(self) -> bool:
+        return self._data.is_stream
+
 
 class StreamDataset(Dataset):
     def __init__(
         self,
         source: Optional[IDataset] = None,
         *,
         infos: Optional[DatasetInfo] = None,
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/dataset_base.py` & `datumaro-1.4.0rc2/src/datumaro/components/dataset_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import attr
 import numpy as np
 from attr import attrs, field
 
 from datumaro.components.annotation import Annotation, AnnotationType, Categories
 from datumaro.components.cli_plugin import CliPlugin
-from datumaro.components.importer import ImportContext, NullImportContext
+from datumaro.components.importer import ImportContext, NullImportContext, _ImportFail
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util.attrs_util import default_if_none, not_empty
 from datumaro.util.definitions import DEFAULT_SUBSET_NAME
 
 T = TypeVar("T", bound=MediaElement)
 
 
@@ -52,37 +52,40 @@
         attributes: Dict[str, Any] = None,
         image=None,
         point_cloud=None,
         related_images=None,
     ):
         if image is not None:
             warnings.warn(
-                "'image' is deprecated and will be " "removed in future. Use 'media' instead.",
+                "'image' is deprecated and will be removed in future. Use 'media' instead. "
+                "It will be deprecated in datumaro==1.5.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             if isinstance(image, str):
                 image = Image.from_file(path=image)
             elif isinstance(image, np.ndarray):
                 image = Image.from_numpy(data=image)
             elif isinstance(image, bytes) or callable(image):
                 image = Image.from_bytes(data=image)
             assert isinstance(image, Image)
             media = image
         elif point_cloud is not None:
             warnings.warn(
                 "'point_cloud' is deprecated and will be "
-                "removed in future. Use 'media' instead.",
+                "removed in future. Use 'media' instead. "
+                "It will be deprecated in datumaro==1.5.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             if related_images is not None:
                 warnings.warn(
                     "'related_images' is deprecated and will be "
-                    "removed in future. Use 'media' instead.",
+                    "removed in future. Use 'media' instead. "
+                    "It will be deprecated in datumaro==1.5.0.",
                     DeprecationWarning,
                     stacklevel=2,
                 )
             if isinstance(point_cloud, str):
                 point_cloud = PointCloud.from_file(path=point_cloud, extra_images=related_images)
             elif isinstance(point_cloud, bytes):
                 point_cloud = PointCloud.from_bytes(data=point_cloud, extra_images=related_images)
@@ -94,65 +97,70 @@
         )
 
     # Deprecated. Provided for backward compatibility.
     @property
     def image(self) -> Optional[Image]:
         warnings.warn(
             "'DatasetItem.image' is deprecated and will be "
-            "removed in future. Use '.media' and '.media_as()' instead.",
+            "removed in future. Use '.media' and '.media_as()' instead. "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
         if not isinstance(self.media, Image):
             return None
         return self.media_as(Image)
 
     # Deprecated. Provided for backward compatibility.
     @property
     def point_cloud(self) -> Optional[str]:
         warnings.warn(
             "'DatasetItem.point_cloud' is deprecated and will be "
-            "removed in future. Use '.media' and '.media_as()' instead.",
+            "removed in future. Use '.media' and '.media_as()' instead. "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
         if not isinstance(self.media, PointCloud):
             return None
         return getattr(self.media_as(PointCloud), "path", None)
 
     # Deprecated. Provided for backward compatibility.
     @property
     def related_images(self) -> List[Image]:
         warnings.warn(
             "'DatasetItem.related_images' is deprecated and will be "
-            "removed in future. Use '.media' and '.media_as()' instead.",
+            "removed in future. Use '.media' and '.media_as()' instead. "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
         if not isinstance(self.media, PointCloud):
             return []
         return self.media_as(PointCloud).extra_images
 
     # Deprecated. Provided for backward compatibility.
     @property
     def has_image(self):
         warnings.warn(
             "'DatasetItem.has_image' is deprecated and will be "
-            "removed in future. Use '.media' and '.media_as()' instead.",
+            "removed in future. Use '.media' and '.media_as()' instead. "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
         return isinstance(self.media, Image)
 
     # Deprecated. Provided for backward compatibility.
     @property
     def has_point_cloud(self):
         warnings.warn(
             "'DatasetItem.has_point_cloud' is deprecated and will be "
-            "removed in future. Use '.media' and '.media_as()' instead.",
+            "removed in future. Use '.media' and '.media_as()' instead. "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
         return isinstance(self.media, PointCloud)
 
 
 DatasetInfo = Dict[str, Any]
@@ -241,15 +249,15 @@
         return self._length
 
     def subsets(self) -> Dict[str, IDataset]:
         if self._subsets is None:
             self._init_cache()
         return {name or DEFAULT_SUBSET_NAME: self.get_subset(name) for name in self._subsets}
 
-    def get_subset(self, name):
+    def get_subset(self, name: str) -> IDataset:
         if self._subsets is None:
             self._init_cache()
         if name in self._subsets:
             if len(self._subsets) == 1:
                 return self
 
             subset = self.select(lambda item: item.subset == name)
@@ -349,7 +357,65 @@
 
     def __len__(self):
         return len(self._items)
 
     def get(self, id, subset=None):
         assert subset == self._subset, "%s != %s" % (subset, self._subset)
         return super().get(id, subset or self._subset)
+
+    @property
+    def subset(self) -> str:
+        """Subset name of this instance."""
+        return self._subset
+
+
+class ExtractorMerger(DatasetBase):
+    """A simple class to merge single-subset extractors."""
+
+    def __init__(
+        self,
+        *sources: Sequence[SubsetBase],
+    ):
+        if len(sources) == 0:
+            raise _ImportFail("It should not be empty.")
+
+        self._infos = self._check_identicalness(*[s.infos() for s in sources])
+        self._categories = self._check_identicalness(*[s.categories() for s in sources])
+        self._media_type = self._check_identicalness(*[s.media_type() for s in sources])
+        self._is_stream = self._check_identicalness(*[s.is_stream for s in sources])
+        self._subsets = {s.subset: s for s in sources}
+
+    def _check_identicalness(self, *seq: Sequence[T]) -> T:
+        if len(seq) == 0:
+            raise _ImportFail("It should not be empty.")
+
+        if seq.count(seq[0]) != len(seq):
+            raise _ImportFail("All items in the sequence should be identical.")
+
+        return seq[0]
+
+    def infos(self):
+        return self._infos
+
+    def categories(self):
+        return self._categories
+
+    def __iter__(self):
+        for subset in self._subsets.values():
+            yield from subset
+
+    def __len__(self):
+        return sum(len(subset) for subset in self._subsets.values())
+
+    def get(self, id: str, subset: Optional[str] = None):
+        if subset is None:
+            for s in self._subsets.values():
+                item = s.get(id)
+                if item is not None:
+                    return item
+
+        s = self._subset[subset]
+        return s.get(id)
+
+    @property
+    def is_stream(self) -> bool:
+        return self._is_stream
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.4.0rc2/src/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/dataset_storage.py` & `datumaro-1.4.0rc2/src/datumaro/components/dataset_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/environment.py` & `datumaro-1.4.0rc2/src/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/errors.py` & `datumaro-1.4.0rc2/src/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/components/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,16 @@
 
         if save_media is not None:
             self._save_media = save_media
         elif save_images is not None:
             self._save_media = save_images
             warnings.warn(
                 "'save-images' is deprecated and will be "
-                "removed in future. Use 'save-media' instead.",
+                "removed in future. Use 'save-media' instead. "
+                "It will be deprecated in datumaro==1.5.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
         else:
             self._save_media = False
 
         self._image_ext = image_ext
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/extractor_tfds.py` & `datumaro-1.4.0rc2/src/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/filter.py` & `datumaro-1.4.0rc2/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/format_detection.py` & `datumaro-1.4.0rc2/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/generator.py` & `datumaro-1.4.0rc2/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/importer.py` & `datumaro-1.4.0rc2/src/datumaro/components/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import os
 import os.path as osp
 from contextlib import contextmanager
 from functools import wraps
 from glob import iglob
-from typing import Callable, Dict, List, NoReturn, Optional, Tuple, TypeVar
+from typing import Callable, Dict, List, NoReturn, Optional, Tuple, Type, TypeVar
 
 import attr
 from attr import define, field
 
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.errors import (
     AnnotationImportError,
@@ -23,14 +23,17 @@
     ItemImportError,
 )
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
 from datumaro.util.definitions import SUBSET_NAME_BLACKLIST
 
 T = TypeVar("T")
+# TODO: we should refactor code to import `ExtractorMerger` from datumaro.component.dataset_base
+# Currently, it is impossible due to a circular import.
+ExtractorMerger = TypeVar("ExtractorMerger")
 
 
 class _ImportFail(DatumaroError):
     pass
 
 
 class ImportErrorPolicy:
@@ -107,26 +110,34 @@
     def find_sources(cls, path: str) -> List[Dict]:
         raise NotImplementedError()
 
     @classmethod
     def find_sources_with_params(cls, path: str, **extra_params) -> List[Dict]:
         return cls.find_sources(path)
 
-    def __call__(self, path, **extra_params):
+    def __call__(self, path, stream: bool = False, **extra_params):
         if not path or not osp.exists(path):
             raise DatasetNotFoundError(path, self.NAME)
 
         found_sources = self.find_sources_with_params(osp.normpath(path), **extra_params)
         if not found_sources:
             raise DatasetNotFoundError(path, self.NAME)
 
         sources = []
         for desc in found_sources:
             params = dict(extra_params)
             params.update(desc.get("options", {}))
+
+            if stream and self.can_stream:
+                params.update({"stream": True})
+            elif stream and not self.can_stream:
+                raise DatasetImportError(
+                    f"{self.__class__.__name__} cannot stream, but stream=True."
+                )
+
             desc["options"] = params
             sources.append(desc)
 
         return sources
 
     @classmethod
     def _find_sources_recursive(
@@ -185,14 +196,32 @@
                     )
                     if (callable(file_filter) and file_filter(p)) or (not callable(file_filter))
                 )
                 if sources:
                     break
         return sources
 
+    @property
+    def can_stream(self) -> bool:
+        """Flag to indicate whether the importer can stream the dataset item or not."""
+        return False
+
+    def get_extractor_merger(self) -> Optional[Type[ExtractorMerger]]:
+        """Extractor merger dedicated for the data format
+
+        Datumaro import process spawns multiple `DatasetBase` for the detected sources.
+        We can find a bunch of the detected sources from the given directory path.
+        It is usually each detected source is corresponded to the subset of dataset in many data formats.
+
+        Returns:
+            If None, use `Dataset.from_extractors()` to merge the extractors,
+            Otherwise, use the return type to merge the extractors.
+        """
+        return None
+
 
 def with_subset_dirs(input_cls: Importer):
     @wraps(input_cls, updated=())
     class WrappedImporter(input_cls):
         NAME = input_cls.NAME
 
         @classmethod
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/launcher.py` & `datumaro-1.4.0rc2/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/lazy_plugin.py` & `datumaro-1.4.0rc2/src/datumaro/components/lazy_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/media.py` & `datumaro-1.4.0rc2/src/datumaro/components/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,16 @@
         path: Optional[str] = None,
         ext: Optional[str] = None,
         size: Optional[Tuple[int, int]] = None,
         crypter: Crypter = NULL_CRYPTER,
     ):
         warnings.warn(
             f"Using {self.__class__.__name__} is deprecated. "
-            "Please use 'Image.from_bytes()' instead.",
+            "Please use 'Image.from_bytes()' instead. "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
 
         if not isinstance(data, bytes):
             assert path or callable(data), "Image can not be empty"
             assert data is None or callable(data)
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/media_manager.py` & `datumaro-1.4.0rc2/src/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/merge/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/merge/base.py` & `datumaro-1.4.0rc2/src/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.4.0rc2/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.4.0rc2/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/merge/union_merge.py` & `datumaro-1.4.0rc2/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/operations.py` & `datumaro-1.4.0rc2/src/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/progress_reporting.py` & `datumaro-1.4.0rc2/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/project.py` & `datumaro-1.4.0rc2/src/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/shift_analyzer.py` & `datumaro-1.4.0rc2/src/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/transformer.py` & `datumaro-1.4.0rc2/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/validator.py` & `datumaro-1.4.0rc2/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/components/visualizer.py` & `datumaro-1.4.0rc2/src/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
-from typing import List, Optional, Tuple, Type, TypeVar
+from typing import Dict, List, Optional, Tuple, Type, TypeVar
 
 import numpy as np
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
@@ -51,14 +51,15 @@
         self,
         path: str,
         task: Optional[VocTask] = VocTask.voc,
         *,
         subset: Optional[str] = None,
         voc_importer_type: VocImporterType = VocImporterType.default,
         ctx: Optional[ImportContext] = None,
+        **kwargs,
     ):
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
 
         super().__init__(subset=subset, ctx=ctx)
 
         if voc_importer_type == VocImporterType.default:
@@ -373,15 +374,15 @@
                     )
 
                 image = self._lazy_extract_mask(class_mask, label_id)
                 item_annotations.append(Mask(image=image, label=label_id))
 
         return item_annotations
 
-    def _parse_labels(self):
+    def _parse_labels(self) -> Dict[str, List[Label]]:
         annotations = {}
         task_dir = osp.dirname(self._path)
         for label_id, label in enumerate(self._categories[AnnotationType.label]):
             ann_file = osp.join(task_dir, f"{label.name}_{self._subset}.txt")
             if not osp.isfile(ann_file):
                 continue
 
@@ -407,14 +408,18 @@
                         )
 
                     if present == "1":
                         annotations.setdefault(item, []).append(Label(label_id))
 
         return annotations
 
+    @property
+    def is_stream(self) -> bool:
+        return True
+
 
 class VocClassificationBase(VocBase):
     def __init__(self, path, **kwargs):
         super().__init__(path, task=VocTask.voc_classification, **kwargs)
 
 
 class VocDetectionBase(VocBase):
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
+from typing import Optional, Type
 
+from datumaro.components.dataset_base import ExtractorMerger
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import Importer
 
 from .format import VocPath, VocTask
 
 
 class _VocImporter(Importer):
@@ -59,14 +61,21 @@
             subsets.extend(task_subsets)
 
             if not root_path:
                 root_path = osp.dirname(osp.dirname(osp.dirname(task_subsets[0]["url"])))
 
         return subsets
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
+    def get_extractor_merger(self) -> Optional[Type[ExtractorMerger]]:
+        return ExtractorMerger
+
 
 class VocImporter(_VocImporter):
     _TASK = VocTask.voc
     _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
 
 
 class VocClassificationImporter(_VocImporter):
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import os.path as osp
-import re
 from collections import OrderedDict
-from typing import Dict, List, Optional, Type, TypeVar, Union
+from typing import Dict, Iterator, List, Optional, Type, TypeVar, Union
 
 import yaml
 
 from datumaro.components.annotation import Annotation, AnnotationType, Bbox, LabelCategories
-from datumaro.components.dataset_base import DatasetBase, DatasetItem, SubsetBase
+from datumaro.components.dataset_base import CategoriesInfo, DatasetBase, DatasetItem, SubsetBase
 from datumaro.components.errors import (
     DatasetImportError,
     InvalidAnnotationError,
     UndeclaredLabelError,
 )
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, ImageFromFile
@@ -29,246 +28,248 @@
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 from datumaro.util.os_util import extract_subset_name_from_parent, find_files, split_path
 
 from .format import YoloLoosePath, YoloPath, YoloUltralyticsPath
 
 T = TypeVar("T")
 
+__all__ = ["YoloStrictBase", "YoloLooseBase", "YoloUltralyticsBase"]
 
-class YoloStrictBase(SubsetBase):
-    class _Subset(DatasetBase):
-        def __init__(self, name: str, parent: YoloStrictBase):
-            super().__init__()
-            self._name = name
-            self._parent = parent
-            self.items: Dict[str, Union[str, DatasetItem]] = OrderedDict()
-
-        def __iter__(self):
-            for item_id in self.items:
-                item = self._parent._get(item_id, self._name)
-                if item is not None:
-                    yield item
 
-        def __len__(self):
-            return len(self.items)
+def localize_path(path: str) -> str:
+    """
+    Removes the "data/" prefix from the path
+    """
+
+    path = osp.normpath(path.strip()).replace("\\", "/")
+    default_base = "data/"
+    if path.startswith(default_base):
+        path = path[len(default_base) :]
+    return path
 
-        def categories(self):
-            return self._parent.categories()
 
+# TODO: Need to clean this dirty structure (SubsetBase has _Subset).
+class _Subset(DatasetBase):
+    def __init__(
+        self,
+        subset_name: str,
+        path: str,
+        items: OrderedDict[str, str],
+        categories: CategoriesInfo,
+        image_info: ImageMeta,
+    ):
+        super().__init__()
+        self._subset_name = subset_name
+        self._path = path
+        self._items = items
+        self._categories = categories
+        self._image_info = image_info
+
+    def __iter__(self) -> Iterator[DatasetItem]:
+        for item_id in self._items:
+            item = self._get(item_id)
+            if item is not None:
+                yield item
+
+    def __len__(self):
+        return len(self._items)
+
+    def categories(self):
+        return self._parent.categories()
+
+    def _get(self, item_id: str) -> Optional[DatasetItem]:
+        item = self._items.get(item_id)
+
+        if not isinstance(item, str):
+            return None
+
+        try:
+            image_size = self._image_info.get(item_id)
+            image = Image.from_file(path=osp.join(self._path, item), size=image_size)
+
+            anno_path = osp.splitext(image.path)[0] + ".txt"
+            annotations = self._parse_annotations(
+                anno_path,
+                image,
+                label_categories=self._categories[AnnotationType.label],
+            )
+
+            item = DatasetItem(
+                id=item_id, subset=self._subset_name, media=image, annotations=annotations
+            )
+            return item
+        except (UndeclaredLabelError, InvalidAnnotationError) as e:
+            self._ctx.error_policy.report_annotation_error(e, item_id=(item_id, self._subset_name))
+        except Exception as e:
+            self._ctx.error_policy.report_item_error(e, item_id=(item_id, self._subset_name))
+
+        return None
+
+    @classmethod
+    def _parse_annotations(
+        cls,
+        anno_path: str,
+        image: ImageFromFile,
+        *,
+        label_categories: LabelCategories,
+    ) -> List[Annotation]:
+        lines = []
+        with open(anno_path, "r", encoding="utf-8") as f:
+            for line in f:
+                line = line.strip()
+                if line:
+                    lines.append(line)
+
+        annotations = []
+
+        if lines:
+            # Use image info as late as possible to avoid unnecessary image loading
+            if image.size is None:
+                raise DatasetImportError(f"Can't find image info for '{localize_path(image.path)}'")
+            image_height, image_width = image.size
+
+        for idx, line in enumerate(lines):
+            parts = line.split()
+            if len(parts) != 5:
+                raise InvalidAnnotationError(
+                    f"Unexpected field count {len(parts)} in the bbox description. "
+                    "Expected 5 fields (label, xc, yc, w, h)."
+                )
+            label_id, xc, yc, w, h = parts
+
+            label_id = cls._parse_field(label_id, int, "bbox label id")
+            if label_id not in label_categories:
+                raise UndeclaredLabelError(str(label_id))
+
+            w = cls._parse_field(w, float, "bbox width")
+            h = cls._parse_field(h, float, "bbox height")
+            x = cls._parse_field(xc, float, "bbox center x") - w * 0.5
+            y = cls._parse_field(yc, float, "bbox center y") - h * 0.5
+            annotations.append(
+                Bbox(
+                    x * image_width,
+                    y * image_height,
+                    w * image_width,
+                    h * image_height,
+                    label=label_id,
+                    id=idx,
+                    group=idx,
+                )
+            )
+
+        return annotations
+
+    @classmethod
+    def _parse_field(cls, value: str, desired_type: Type[T], field_name: str) -> T:
+        try:
+            return desired_type(value)
+        except Exception as e:
+            raise InvalidAnnotationError(
+                f"Can't parse {field_name} from '{value}'. Expected {desired_type}"
+            ) from e
+
+
+class YoloStrictBase(SubsetBase):
     def __init__(
         self,
         config_path: str,
         image_info: Union[None, str, ImageMeta] = None,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
+        **kwargs,
     ) -> None:
         super().__init__(subset=subset, ctx=ctx)
 
         if not osp.isfile(config_path):
             raise DatasetImportError(f"Can't read dataset descriptor file '{config_path}'")
 
         rootpath = osp.dirname(config_path)
         self._path = rootpath
 
         self._image_info = self.parse_image_info(rootpath, image_info)
 
-        config = self._parse_config(config_path)
+        config = YoloPath._parse_config(config_path)
 
         names_path = config.get("names")
         if not names_path:
             raise InvalidAnnotationError("Failed to parse names file path from config")
 
+        self._categories = {
+            AnnotationType.label: self._load_categories(
+                osp.join(self._path, localize_path(names_path))
+            )
+        }
+
         # The original format is like this:
         #
         # classes = 2
         # train  = data/train.txt
         # valid  = data/test.txt
         # names = data/obj.names
         # backup = backup/
         #
         # To support more subset names, we disallow subsets
         # called 'classes', 'names' and 'backup'.
         subsets = {k: v for k, v in config.items() if k not in YoloPath.RESERVED_CONFIG_KEYS}
+        self._subsets: Dict[str, self._Subset] = {}
 
         for subset_name, list_path in subsets.items():
-            list_path = osp.join(self._path, self.localize_path(list_path))
+            if subset_name != subset:
+                continue
+
+            list_path = osp.join(self._path, localize_path(list_path))
             if not osp.isfile(list_path):
                 raise InvalidAnnotationError(f"Can't find '{subset_name}' subset list file")
 
-            subset = self._Subset(subset_name, self)
             with open(list_path, "r", encoding="utf-8") as f:
-                subset.items = OrderedDict(
-                    (self.name_from_path(p), self.localize_path(p)) for p in f if p.strip()
+                items = OrderedDict(
+                    (self.name_from_path(p), localize_path(p)) for p in f if p.strip()
                 )
-            subsets[subset_name] = subset
-
-        self._subsets: Dict[str, self._Subset] = subsets
 
-        self._categories = {
-            AnnotationType.label: self._load_categories(
-                osp.join(self._path, self.localize_path(names_path))
+            subset = _Subset(
+                subset_name=subset_name,
+                path=self._path,
+                items=items,
+                categories=self._categories,
+                image_info=self._image_info,
             )
-        }
+            self._subsets[subset_name] = subset
 
     @staticmethod
-    def parse_image_info(rootpath: str, image_info: Optional[Union[str, ImageMeta]] = None):
+    def parse_image_info(
+        rootpath: str, image_info: Optional[Union[str, ImageMeta]] = None
+    ) -> ImageMeta:
         assert image_info is None or isinstance(image_info, (str, dict))
         if image_info is None:
             image_info = osp.join(rootpath, DEFAULT_IMAGE_META_FILE_NAME)
             if not osp.isfile(image_info):
                 image_info = {}
         if isinstance(image_info, str):
             image_info = load_image_meta_file(image_info)
 
         return image_info
 
-    @staticmethod
-    def _parse_config(path: str) -> Dict[str, str]:
-        with open(path, "r", encoding="utf-8") as f:
-            config_lines = f.readlines()
-
-        config = {}
-
-        for line in config_lines:
-            match = re.match(r"^\s*(\w+)\s*=\s*(.+)$", line)
-            if not match:
-                continue
-
-            key = match.group(1)
-            value = match.group(2)
-            config[key] = value
-
-        return config
-
-    @staticmethod
-    def localize_path(path: str) -> str:
-        """
-        Removes the "data/" prefix from the path
-        """
-
-        path = osp.normpath(path.strip()).replace("\\", "/")
-        default_base = "data/"
-        if path.startswith(default_base):
-            path = path[len(default_base) :]
-        return path
-
     @classmethod
     def name_from_path(cls, path: str) -> str:
         """
         Obtains <image name> from the path like [data/]<subset>_obj/<image_name>.ext
 
         <image name> can be <a/b/c/filename>, so it is
         more involved than just calling "basename()".
         """
 
-        path = cls.localize_path(path)
+        path = localize_path(path)
 
         parts = split_path(path)
         if 1 < len(parts) and not osp.isabs(path):
             path = osp.join(*parts[1:])  # pylint: disable=no-value-for-parameter
 
         return osp.splitext(path)[0]
 
-    def _get(self, item_id: str, subset_name: str) -> Optional[DatasetItem]:
-        subset = self._subsets[subset_name]
-        item = subset.items[item_id]
-
-        if isinstance(item, str):
-            try:
-                image_size = self._image_info.get(item_id)
-                image = Image.from_file(path=osp.join(self._path, item), size=image_size)
-
-                anno_path = osp.splitext(image.path)[0] + ".txt"
-                annotations = self._parse_annotations(
-                    anno_path,
-                    image,
-                    label_categories=self._categories[AnnotationType.label],
-                )
-
-                item = DatasetItem(
-                    id=item_id, subset=subset_name, media=image, annotations=annotations
-                )
-                subset.items[item_id] = item
-            except (UndeclaredLabelError, InvalidAnnotationError) as e:
-                self._ctx.error_policy.report_annotation_error(e, item_id=(item_id, subset_name))
-                subset.items.pop(item_id)
-                item = None
-            except Exception as e:
-                self._ctx.error_policy.report_item_error(e, item_id=(item_id, subset_name))
-                subset.items.pop(item_id)
-                item = None
-
-        return item
-
-    @classmethod
-    def _parse_field(cls, value: str, desired_type: Type[T], field_name: str) -> T:
-        try:
-            return desired_type(value)
-        except Exception as e:
-            raise InvalidAnnotationError(
-                f"Can't parse {field_name} from '{value}'. Expected {desired_type}"
-            ) from e
-
-    @classmethod
-    def _parse_annotations(
-        cls,
-        anno_path: str,
-        image: ImageFromFile,
-        *,
-        label_categories: LabelCategories,
-    ) -> List[Annotation]:
-        lines = []
-        with open(anno_path, "r", encoding="utf-8") as f:
-            for line in f:
-                line = line.strip()
-                if line:
-                    lines.append(line)
-
-        annotations = []
-
-        if lines:
-            # Use image info as late as possible to avoid unnecessary image loading
-            if image.size is None:
-                raise DatasetImportError(
-                    f"Can't find image info for '{cls.localize_path(image.path)}'"
-                )
-            image_height, image_width = image.size
-
-        for idx, line in enumerate(lines):
-            parts = line.split()
-            if len(parts) != 5:
-                raise InvalidAnnotationError(
-                    f"Unexpected field count {len(parts)} in the bbox description. "
-                    "Expected 5 fields (label, xc, yc, w, h)."
-                )
-            label_id, xc, yc, w, h = parts
-
-            label_id = cls._parse_field(label_id, int, "bbox label id")
-            if label_id not in label_categories:
-                raise UndeclaredLabelError(str(label_id))
-
-            w = cls._parse_field(w, float, "bbox width")
-            h = cls._parse_field(h, float, "bbox height")
-            x = cls._parse_field(xc, float, "bbox center x") - w * 0.5
-            y = cls._parse_field(yc, float, "bbox center y") - h * 0.5
-            annotations.append(
-                Bbox(
-                    x * image_width,
-                    y * image_height,
-                    w * image_width,
-                    h * image_height,
-                    label=label_id,
-                    id=idx,
-                    group=idx,
-                )
-            )
-
-        return annotations
-
     @staticmethod
     def _load_categories(names_path):
         if has_meta_file(osp.dirname(names_path)):
             return LabelCategories.from_iterable(parse_meta_file(osp.dirname(names_path)).keys())
 
         label_categories = LabelCategories()
 
@@ -276,27 +277,31 @@
             for label in f:
                 label = label.strip()
                 if label:
                     label_categories.add(label)
 
         return label_categories
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[DatasetItem]:
         subsets = self._subsets
         pbars = self._ctx.progress_reporter.split(len(subsets))
         for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
             for item in pbar.iter(subset, desc=f"Parsing '{subset_name}'"):
                 yield item
 
     def __len__(self):
         return sum(len(s) for s in self._subsets.values())
 
     def get_subset(self, name):
         return self._subsets[name]
 
+    @property
+    def is_stream(self) -> bool:
+        return True
+
 
 class YoloLooseBase(SubsetBase):
     META_FILE = YoloLoosePath.NAMES_FILE
 
     def __init__(
         self,
         config_path: str,
@@ -315,58 +320,67 @@
 
         self._image_info = YoloStrictBase.parse_image_info(rootpath, image_info)
 
         # Init label categories
         label_categories = self._load_categories(osp.join(rootpath, self.META_FILE))
         self._categories = {AnnotationType.label: label_categories}
 
-        img_files = self._load_img_files(rootpath)
+        self._urls = urls
+        self._img_files = self._load_img_files(rootpath)
 
-        for url in urls:
+    def __iter__(self) -> Iterator[DatasetItem]:
+        label_categories = self._categories.get(AnnotationType.label)
+        if label_categories is None:
+            raise DatasetImportError("label_categories should be not None.")
+
+        for url in self._urls:
             try:
                 fname = self._get_fname(url)
-                img = Image.from_file(path=img_files[fname])
+                img = Image.from_file(path=self._img_files[fname])
                 anns = self._parse_annotations(
                     url,
                     img,
                     label_categories=label_categories,
                 )
-                self._items.append(
-                    DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
-                )
+                yield DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(fname, self._subset))
 
+    def __len__(self) -> int:
+        return len(self._urls)
+
     def _get_rootpath(self, config_path: str) -> str:
         return config_path
 
     def _load_categories(self, names_path: str) -> LabelCategories:
         return YoloStrictBase._load_categories(names_path)
 
     def _get_fname(self, fpath: str) -> str:
         return osp.splitext(osp.basename(fpath))[0]
 
-    def _load_img_files(self, rootpath: str) -> Dict:
+    def _load_img_files(self, rootpath: str) -> Dict[str, str]:
         return {
             self._get_fname(img_file): img_file
             for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
             if extract_subset_name_from_parent(img_file, rootpath) == self._subset
         }
 
     def _parse_annotations(
         self, anno_path: str, image: ImageFromFile, label_categories: LabelCategories
     ) -> List[Annotation]:
-        return YoloStrictBase._parse_annotations(
+        return _Subset._parse_annotations(
             anno_path=anno_path, image=image, label_categories=label_categories
         )
 
     def _parse_field(self, value: str, desired_type: Type[T], field_name: str) -> T:
-        return YoloStrictBase._parse_field(
-            value=value, desired_type=desired_type, field_name=field_name
-        )
+        return _Subset._parse_field(value=value, desired_type=desired_type, field_name=field_name)
+
+    @property
+    def is_stream(self) -> bool:
+        return True
 
 
 class YoloUltralyticsBase(YoloLooseBase):
     META_FILE = YoloUltralyticsPath.META_FILE
 
     def __init__(
         self,
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from collections import defaultdict
 from io import TextIOWrapper
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional, Type
 
+from datumaro.components.dataset_base import ExtractorMerger
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 from datumaro.util.os_util import extract_subset_name_from_parent
 
-from .format import YoloFormatType, YoloLoosePath, YoloUltralyticsPath
+from .format import YoloFormatType, YoloLoosePath, YoloPath, YoloUltralyticsPath
 
 
 class _YoloStrictImporter(Importer):
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         context.require_file("obj.data")
 
     @classmethod
-    def find_sources(cls, path):
-        return cls._find_sources_recursive(path, ".data", YoloFormatType.yolo_strict.name)
+    def find_sources(cls, path: str) -> List[Dict]:
+        found = cls._find_sources_recursive(path, ".data", YoloFormatType.yolo_strict.name)
+        if len(found) == 0:
+            return []
+
+        config_path = found[0]["url"]
+        config = YoloPath._parse_config(config_path)
+        subsets = [k for k in config if k not in YoloPath.RESERVED_CONFIG_KEYS]
+        return [
+            {
+                "url": config_path,
+                "format": YoloFormatType.yolo_strict.name,
+                "options": {"subset": subset},
+            }
+            for subset in subsets
+        ]
 
 
 class _YoloLooseImporter(Importer):
     META_FILE = YoloLoosePath.NAMES_FILE
     FORMAT = YoloFormatType.yolo_loose.name
 
     @classmethod
@@ -131,14 +146,18 @@
 
         sources = cls._find_loose(path, "[Ll]abels")
         if sources:
             return sources
 
         return []
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
 
 class _YoloUltralyticsImporter(_YoloLooseImporter):
     META_FILE = YoloUltralyticsPath.META_FILE
     FORMAT = YoloFormatType.yolo_ultralytics.name
 
 
 class YoloImporter(Importer):
@@ -163,7 +182,10 @@
             # TODO: From Python >= 3.8, we can use
             # "if (sources := importer_cls.find_sources(path)): return sources"
             sources = importer_cls.find_sources(path)
             if sources:
                 return sources
 
         return []
+
+    def get_extractor_merger(self) -> Optional[Type[ExtractorMerger]]:
+        return ExtractorMerger
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/explorer.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/ndr.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from openvino.runtime import Core
 from tqdm import tqdm
 
 from datumaro.components.abstracts.model_interpreter import ModelPred
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.launcher import LauncherWithModelInterpreter
 from datumaro.errors import DatumaroError
-from datumaro.util.definitions import DATUMARO_CACHE_DIR
+from datumaro.util.definitions import get_datumaro_cache_dir
 from datumaro.util.samples import get_samples_path
 
 
 class _OpenvinoImporter(CliPlugin):
     @staticmethod
     def _parse_output_layers(s):
         return [s.strip() for s in s.split(",")]
@@ -97,15 +97,15 @@
 
     @classmethod
     def create_from_model_name(cls, model_name: str) -> "BuiltinOpenvinoModelInfo":
         openvino_plugin_samples_dir = get_samples_path()
         interpreter = osp.join(openvino_plugin_samples_dir, model_name + "_interp.py")
         interpreter = interpreter if osp.exists(interpreter) else interpreter
 
-        model_dir = DATUMARO_CACHE_DIR
+        model_dir = get_datumaro_cache_dir()
 
         # Please visit open-model-zoo repository for OpenVINO public models if you are interested in
         # https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md
         url_folder = "https://storage.openvinotoolkit.org/repositories/datumaro/models/"
 
         description = osp.join(model_dir, model_name + ".xml")
         if not osp.exists(description):
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/specs.json` & `datumaro-1.4.0rc2/src/datumaro/plugins/specs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961832061068703%*

 * *Differences: {'insert': "[(47, OrderedDict([('import_path', "*

 * *           "'datumaro.components.dataset_base.ExtractorMerger'), ('plugin_name', "*

 * *           "'extractor_merger'), ('plugin_type', 'DatasetBase'), ('extra_deps', [])]))]"}*

```diff
@@ -283,14 +283,20 @@
         "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.yolo.base.YoloUltralyticsBase",
         "plugin_name": "yolo_ultralytics",
         "plugin_type": "DatasetBase"
     },
     {
         "extra_deps": [],
+        "import_path": "datumaro.components.dataset_base.ExtractorMerger",
+        "plugin_name": "extractor_merger",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.yolo.base.YoloLooseBase",
         "plugin_name": "yolo_loose",
         "plugin_type": "DatasetBase"
     },
     {
         "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.yolo.base.YoloStrictBase",
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/specs.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/splitter.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import List, Optional, Tuple
 
 import cv2 as cv
 import numpy as np
 import requests
 
 from datumaro.components.generator import DatasetGenerator
-from datumaro.util.definitions import DATUMARO_CACHE_DIR
+from datumaro.util.definitions import get_datumaro_cache_dir
 from datumaro.util.image import save_image
 from datumaro.util.scope import on_error_do, on_exit_do, scope_add, scoped
 
 from .utils import IFSFunction, augment, colorize, suppress_computation_warnings
 
 
 class FractalImageGenerator(DatasetGenerator):
@@ -35,15 +35,15 @@
     _COLORS_FILE = "background_colors.txt"
 
     def __init__(
         self,
         output_dir: str,
         count: int,
         shape: Tuple[int, int],
-        model_path: str = DATUMARO_CACHE_DIR,
+        model_path: str = get_datumaro_cache_dir(),
     ) -> None:
         assert 0 < count, "Image count cannot be lesser than 1"
         self._count = count
 
         self._output_dir = output_dir
         self._model_dir = model_path
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/tiling/util.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/transforms.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/plugins/validators.py` & `datumaro-1.4.0rc2/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/__init__.py` & `datumaro-1.4.0rc2/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/annotation_util.py` & `datumaro-1.4.0rc2/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/attrs_util.py` & `datumaro-1.4.0rc2/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/file_utils.py` & `datumaro-1.4.0rc2/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/image.py` & `datumaro-1.4.0rc2/src/datumaro/util/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 from datumaro.util.os_util import find_files
 
 
 def __getattr__(name: str):
     if name in {"Image", "ByteImage"}:
         warnings.warn(
             f"Using {name} from 'util.image' is deprecated, "
-            "the class is moved to 'components.media'",
+            "the class is moved to 'components.media' "
+            "It will be deprecated in datumaro==1.5.0.",
             DeprecationWarning,
             stacklevel=2,
         )
 
         import datumaro.components.media as media_module
 
         return getattr(media_module, name)
```

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/image_cache.py` & `datumaro-1.4.0rc2/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/log_utils.py` & `datumaro-1.4.0rc2/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/mask_tools.py` & `datumaro-1.4.0rc2/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/meta_file_util.py` & `datumaro-1.4.0rc2/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/os_util.py` & `datumaro-1.4.0rc2/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/pickle_util.py` & `datumaro-1.4.0rc2/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/scope.py` & `datumaro-1.4.0rc2/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/telemetry_stub.py` & `datumaro-1.4.0rc2/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/telemetry_utils.py` & `datumaro-1.4.0rc2/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro/util/tf_util.py` & `datumaro-1.4.0rc2/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.4.0rc2/src/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc1/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.4.0rc2/src/datumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc1/src/datumaro.egg-info/requires.txt` & `datumaro-1.4.0rc2/src/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

