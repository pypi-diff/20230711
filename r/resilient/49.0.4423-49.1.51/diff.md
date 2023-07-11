# Comparing `tmp/resilient-49.0.4423.tar.gz` & `tmp/resilient-49.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient-49.0.4423.tar", last modified: Thu Jun  1 15:58:22 2023, max compression
+gzip compressed data, was "resilient-49.1.51.tar", last modified: Tue Jul 11 16:14:18 2023, max compression
```

## Comparing `resilient-49.0.4423.tar` & `resilient-49.1.51.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8556 2023-06-01 15:57:43.000000 resilient-49.0.4423/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-06-01 15:58:22.933552 resilient-49.0.4423/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-06-01 15:57:43.000000 resilient-49.0.4423/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.925552 resilient-49.0.4423/co3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-06-01 15:57:43.000000 resilient-49.0.4423/co3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient-49.0.4423/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/resilient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11460 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/app_config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/resilient/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/res_keyring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12784 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39318 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1758 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17717 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/resilient_rest_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/resilient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      379 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-06-01 15:58:22.933552 resilient-49.0.4423/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-06-01 15:57:43.000000 resilient-49.0.4423/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/shared_mock_data/mock_plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_plugins/mock_plugins.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_responses/session.JSON
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/.jwk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/API_KEY
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/EMAIL
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/EMPTY
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/PASSWORD
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/URL
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/template_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6071 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3_ii.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19399 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11144 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/xtest_gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/xtest_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/xtest_res_keyring.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-06-01 15:57:43.000000 resilient-49.0.4423/tools/res_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-06-01 15:57:43.000000 resilient-49.0.4423/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.793332 resilient-49.1.51/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8638 2023-07-11 16:13:50.000000 resilient-49.1.51/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2023-07-11 16:14:18.793332 resilient-49.1.51/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-07-11 16:13:50.000000 resilient-49.1.51/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.785333 resilient-49.1.51/co3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-07-11 16:13:50.000000 resilient-49.1.51/co3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-11 16:13:50.000000 resilient-49.1.51/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/resilient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11561 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/app_config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/resilient/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/bin/finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/bin/gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/bin/res_keyring.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12784 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/co3argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39318 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1758 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17717 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-07-11 16:13:50.000000 resilient-49.1.51/resilient/resilient_rest_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/resilient.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2023-07-11 16:14:18.000000 resilient-49.1.51/resilient.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2023-07-11 16:14:18.000000 resilient-49.1.51/resilient.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:14:18.000000 resilient-49.1.51/resilient.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-07-11 16:14:18.000000 resilient-49.1.51/resilient.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      379 2023-07-11 16:14:18.000000 resilient-49.1.51/resilient.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-07-11 16:14:18.000000 resilient-49.1.51/resilient.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-07-11 16:14:18.793332 resilient-49.1.51/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-07-11 16:13:50.000000 resilient-49.1.51/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/tests/shared_mock_data/mock_plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_plugins/mock_plugins.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.789332 resilient-49.1.51/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_responses/session.JSON
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.793332 resilient-49.1.51/tests/shared_mock_data/mock_secrets/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.793332 resilient-49.1.51/tests/shared_mock_data/mock_secrets/.jwk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/API_KEY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/EMAIL
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/EMPTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/PASSWORD
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/shared_mock_data/mock_secrets/URL
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/template_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6896 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_co3_ii.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19399 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11144 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/xtest_gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/xtest_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-07-11 16:13:50.000000 resilient-49.1.51/tests/xtest_res_keyring.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:18.793332 resilient-49.1.51/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-07-11 16:13:50.000000 resilient-49.1.51/tools/res_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-07-11 16:13:50.000000 resilient-49.1.51/tox.ini
```

### Comparing `resilient-49.0.4423/CHANGES` & `resilient-49.1.51/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-07: version 49.1**
+
+* Bug fix for protected secrets which ended in ``$}``
+
 **2023-05: version 49.0**
 
 * Added logic to skip retry logic for failed API calls in :class:`resilient.SimpleClient.post() <resilient.co3.SimpleClient.post>`, :class:`resilient.SimpleClient.put() <resilient.co3.SimpleClient.put>` and :class:`resilient.SimpleClient.getput() <resilient.co3.SimpleClient.getput>`
 * Added ``resilient-app-config-plugins`` as a new package to manage third party credentials within SOAR apps
 
 **2023-05: version 48.2**
```

### Comparing `resilient-49.0.4423/PKG-INFO` & `resilient-49.1.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-49.0.4423/README.md` & `resilient-49.1.51/README.md`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/LICENSE` & `resilient-49.1.51/resilient/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/__init__.py` & `resilient-49.1.51/resilient/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/app_config.py` & `resilient-49.1.51/resilient/app_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         if secret_prefix not in item:
             return item
         start = item.index(secret_prefix)
 
         # loop through any prefixed values in the item and substitute them
         # the loop here is required for multiple values in a line
         while start < len(item):
-            end = item.index("}", start) if "}" in item else len(item)
+            end = item.index("}", start) if "}" in item[start:] else len(item)
             prefixed_item = item[start:end+1]
             unprefixed_item = prefixed_item.replace(secret_prefix, "").replace("}", "")
             secret_value = secret_manager.get(unprefixed_item, prefixed_item)
 
             # since we set prefixed_item to be the default value that will
             # be returned when no value is found, log a warning telling the
             # user that their value wasn't found
@@ -255,11 +255,12 @@
                           prefixed_item, manager_type_str, prefixed_item)
             else:
                 LOG.debug("Substituting value for '%s' in %s", prefixed_item, original_item)
 
             item = u"{0}{1}{2}".format(item[0:start], secret_value, item[end+1:])
 
             # restart the search from the one beyond where we just subbed in the found value
-            start = item.index(secret_prefix, start+1) if secret_prefix in item[start+1:] else len(item)
+            length_secret = len(secret_value) if secret_value else 0
+            start = item.index(secret_prefix, start+length_secret) if secret_prefix in item[start+length_secret:] else len(item)
         return item
```

### Comparing `resilient-49.0.4423/resilient/bin/finfo.py` & `resilient-49.1.51/resilient/bin/finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/bin/gadget.py` & `resilient-49.1.51/resilient/bin/gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/bin/res_keyring.py` & `resilient-49.1.51/resilient/bin/res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/co3.py` & `resilient-49.1.51/resilient/co3.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/co3argparse.py` & `resilient-49.1.51/resilient/co3argparse.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/co3base.py` & `resilient-49.1.51/resilient/co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/co3sslutil.py` & `resilient-49.1.51/resilient/co3sslutil.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/constants.py` & `resilient-49.1.51/resilient/constants.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/definitions.py` & `resilient-49.1.51/resilient/definitions.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/helpers.py` & `resilient-49.1.51/resilient/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/patch.py` & `resilient-49.1.51/resilient/patch.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient/resilient_rest_mock.py` & `resilient-49.1.51/resilient/resilient_rest_mock.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/resilient.egg-info/PKG-INFO` & `resilient-49.1.51/resilient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-49.0.4423/resilient.egg-info/SOURCES.txt` & `resilient-49.1.51/resilient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/setup.cfg` & `resilient-49.1.51/setup.cfg`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/conftest.py` & `resilient-49.1.51/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/helpers.py` & `resilient-49.1.51/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/shared_mock_data/mock_paths.py` & `resilient-49.1.51/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/shared_mock_data/mock_plugins/mock_plugins.py` & `resilient-49.1.51/tests/shared_mock_data/mock_plugins/mock_plugins.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/shared_mock_data/mock_responses/session.JSON` & `resilient-49.1.51/tests/shared_mock_data/mock_responses/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/test_app_config.py` & `resilient-49.1.51/tests/test_app_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,19 +26,22 @@
     nothing = psm.get("$DOESNT_EXIST")
 
     assert key == MOCK_API_KEY_VALUE
     assert nothing is None
 
 def test_protected_secrets_manager_PY27(fx_reset_environmental_variables):
     os.environ["UNPROTECTED_API_KEY"] = "passw0rd"
+    os.environ["UNPROTECTED_SECRET_WITH_BRACKETS"] = "A[xyz)e}K,/MabS1}:NbJ$("
     psm = ProtectedSecretsManager()
 
     key = psm.get("$UNPROTECTED_API_KEY")
+    key2 = psm.get("$UNPROTECTED_SECRET_WITH_BRACKETS")
 
     assert key == "passw0rd"
+    assert key2 == "A[xyz)e}K,/MabS1}:NbJ$("
 
 def test_app_config_manager_no_plugin():
     original_dict = {
         "a": 1,
         "b": 2,
         "c": 3,
         "d": {
@@ -126,14 +129,29 @@
 ])
 def test_replace_secret_in_config_pam_plugin(item, prefix, expected):
     manager = MyMockPlugin()
     replaced = AppConfigManager.replace_secret_in_config(item, manager, prefix)
 
     assert replaced == expected
 
+@pytest.mark.parametrize("item, prefix, secret, expected", [
+    ("$SECRET", "$", "A[xyz)e}K,/MabS1}:NbJ$(}$", "A[xyz)e}K,/MabS1}:NbJ$(}$"),
+    ("${SECRET}${SECRET_2}", "${", "A[xyz)e}K,/MabS1}:NbJ$(}${", "A[xyz)e}K,/MabS1}:NbJ$(}${2")
+])
+def test_replace_secret_in_config_protected_secret_env_only(item, prefix, secret, expected, fx_reset_environmental_variables, caplog):
+    manager = ProtectedSecretsManager()
+    os.environ["SECRET"] = secret
+    os.environ["SECRET_2"] = "2"
+
+    replaced = AppConfigManager.replace_secret_in_config(item, manager, prefix)
+
+    assert replaced == expected
+    assert "Failed to find" not in caplog.text
+
+
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
 def test_replace_secret_in_config_protected_secret(fx_write_protected_secrets, fx_reset_environmental_variables):
     os.environ[constants.ENV_VAR_APP_HOST_CONTAINER] = "1"
     path_secrets_dir = fx_write_protected_secrets
     path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key.jwk")
     manager = ProtectedSecretsManager(path_secrets_dir=path_secrets_dir, path_jwk_file=path_jwk_file)
```

### Comparing `resilient-49.0.4423/tests/test_co3.py` & `resilient-49.1.51/tests/test_co3.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/test_co3_ii.py` & `resilient-49.1.51/tests/test_co3_ii.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/test_co3base.py` & `resilient-49.1.51/tests/test_co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/test_finfo.py` & `resilient-49.1.51/tests/test_finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/test_helpers.py` & `resilient-49.1.51/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/xtest_gadget.py` & `resilient-49.1.51/tests/xtest_gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/xtest_patch.py` & `resilient-49.1.51/tests/xtest_patch.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tests/xtest_res_keyring.py` & `resilient-49.1.51/tests/xtest_res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tools/res_utils.py` & `resilient-49.1.51/tools/res_utils.py`

 * *Files identical despite different names*

### Comparing `resilient-49.0.4423/tox.ini` & `resilient-49.1.51/tox.ini`

 * *Files identical despite different names*

