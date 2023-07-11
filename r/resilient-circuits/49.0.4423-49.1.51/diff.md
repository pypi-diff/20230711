# Comparing `tmp/resilient_circuits-49.0.4423.tar.gz` & `tmp/resilient_circuits-49.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_circuits-49.0.4423.tar", last modified: Thu Jun  1 15:58:50 2023, max compression
+gzip compressed data, was "resilient_circuits-49.1.51.tar", last modified: Tue Jul 11 16:14:47 2023, max compression
```

## Comparing `resilient_circuits-49.0.4423.tar` & `resilient_circuits-49.1.51.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12779 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/README
--rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/action_message.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    59967 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/actions_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/actions_test_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11442 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12400 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app_argument_parser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6658 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app_function_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app_restartable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/res_action_test.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/resilient_circuits_cmd.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/service_wrapper.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/cmds/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15923 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/cmds/selftest.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2824 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/data/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/data/app.config.base
--rwxrwxr-x   0 travis    (2000) travis    (2000)    19901 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11958 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/helpers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/keyring_arguments.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/rest_helper.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/stomp_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/stomp_events.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/stomp_transport.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/template_functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/util/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/util/resilient_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/util/resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/validate_configs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/top_level.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-06-01 15:58:50.237552 resilient_circuits-49.0.4423/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/cmds/test_selftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/selftest_tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/mocked_fail_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/mocked_success_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/mocked_unimplemented_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_commented_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_import_definition.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_action_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_actions_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2491 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_app_restartable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_resilient_circuits_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_rest_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_stomp_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/util/test_resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12883 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2939 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.621333 resilient_circuits-49.1.51/resilient_circuits/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/README
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/action_message.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    59967 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/actions_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/actions_test_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11478 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12400 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/app_argument_parser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6658 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/app_function_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/app_restartable.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.621333 resilient_circuits-49.1.51/resilient_circuits/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/bin/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/bin/res_action_test.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/bin/resilient_circuits_cmd.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/bin/service_wrapper.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.621333 resilient_circuits-49.1.51/resilient_circuits/cmds/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15953 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/cmds/selftest.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2824 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.621333 resilient_circuits-49.1.51/resilient_circuits/data/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/data/app.config.base
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    19901 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11958 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/helpers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/keyring_arguments.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/rest_helper.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/stomp_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/stomp_events.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/stomp_transport.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/template_functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.621333 resilient_circuits-49.1.51/resilient_circuits/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/util/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/util/resilient_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/util/resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/resilient_circuits/validate_configs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.621333 resilient_circuits-49.1.51/resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2939 2023-07-11 16:14:47.000000 resilient_circuits-49.1.51/resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-07-11 16:14:47.000000 resilient_circuits-49.1.51/resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:14:47.000000 resilient_circuits-49.1.51/resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-07-11 16:14:47.000000 resilient_circuits-49.1.51/resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-07-11 16:14:47.000000 resilient_circuits-49.1.51/resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-07-11 16:14:47.000000 resilient_circuits-49.1.51/resilient_circuits.egg-info/top_level.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/tests/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/cmds/test_selftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/tests/selftest_tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/selftest_tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/selftest_tests/mocked_fail_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/selftest_tests/mocked_success_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/selftest_tests/mocked_unimplemented_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_commented_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_import_definition.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_action_message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_actions_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2491 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_app_restartable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_resilient_circuits_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_rest_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_stomp_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:47.625332 resilient_circuits-49.1.51/tests/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tests/util/test_resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2023-07-11 16:13:50.000000 resilient_circuits-49.1.51/tox.ini
```

### Comparing `resilient_circuits-49.0.4423/CHANGES` & `resilient_circuits-49.1.51/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-07: version 49.1**
+
+* No major changes. Just bumping build number to coincide with other builds
+
 **2023-05: version 49.0**
 
 * Improved logging on restarts
 * Improved obfuscation of sensitive information from app.config in logs
 * Added ability to disable persistent sessions for ``resilient-lib.RequestsCommon`` in app functions using new optional ``rc_use_persistent_sessions`` configuration parameter
 * Added ``resilient-app-config-plugins`` as a new package to manage third party credentials within SOAR apps
```

### Comparing `resilient_circuits-49.0.4423/PKG-INFO` & `resilient_circuits-49.1.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_circuits
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-49.0.4423/README.md` & `resilient_circuits-49.1.51/README.md`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/LICENSE` & `resilient_circuits-49.1.51/resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/__init__.py` & `resilient_circuits-49.1.51/resilient_circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/action_message.py` & `resilient_circuits-49.1.51/resilient_circuits/action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/actions_component.py` & `resilient_circuits-49.1.51/resilient_circuits/actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/actions_test_component.py` & `resilient_circuits-49.1.51/resilient_circuits/actions_test_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/app.py` & `resilient_circuits-49.1.51/resilient_circuits/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         if self.opts.get("api_key_id", None):
             LOG.info("Resilient api key id: %s", self.opts.get("api_key_id"))
         if self.opts.get("api_key_id", None) and self.opts.get("email", None):
             LOG.warning("The user and api key configuration settings are both enabled. Credentials will default to the "
                         "api key settings.")
         LOG.info("Resilient org: %s", self.opts.get("org"))
         LOG.info("Logging Level: %s", self.opts.get("loglevel"))
-        LOG.info("App Config plugin: %s", self.opts.pam_plugin.__class__.__name__)
+        LOG.info("App Config plugin: %s", self.opts.pam_plugin.__class__.__name__ if self.opts.pam_plugin else "None")
         if self.opts.get("test_actions", False):
             # Make all components aware that we are in test mode
             ResilientComponent.test_mode = True
 
         # Make all components aware that we are in selftest mode
         ResilientComponent.IS_SELFTEST = self.IS_SELFTEST
```

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/app_argument_parser.py` & `resilient_circuits-49.1.51/resilient_circuits/app_argument_parser.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/app_function_component.py` & `resilient_circuits-49.1.51/resilient_circuits/app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/app_restartable.py` & `resilient_circuits-49.1.51/resilient_circuits/app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/bin/res_action_test.py` & `resilient_circuits-49.1.51/resilient_circuits/bin/res_action_test.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/bin/resilient_circuits_cmd.py` & `resilient_circuits-49.1.51/resilient_circuits/bin/resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/bin/service_wrapper.py` & `resilient_circuits-49.1.51/resilient_circuits/bin/service_wrapper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/cmds/selftest.py` & `resilient_circuits-49.1.51/resilient_circuits/cmds/selftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     the second element is a reason if it is incorrectly configured.
 
     :param app_configs: app configs for the app -- should contain a .pam_plugin object
     :type app_configs: ``resilient.app_config.AppConfigManager``
     """
     LOG.info("{0}Testing PAM Plugin details{0}".format(constants.LOG_DIVIDER))
 
-    if not app_configs or not hasattr(app_configs, "pam_plugin"):
+    if not app_configs or not hasattr(app_configs, "pam_plugin") or not app_configs.pam_plugin:
         LOG.info("{0}No Plugin specified. Skipping test{0}".format(constants.LOG_DIVIDER))
         return
 
     try:
         LOG.info("- Running pam plugin selftest")
         result = app_configs.pam_plugin.selftest()
     except NotImplementedError:
```

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/component_loader.py` & `resilient_circuits-49.1.51/resilient_circuits/component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/constants.py` & `resilient_circuits-49.1.51/resilient_circuits/constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/data/app.config.base` & `resilient_circuits-49.1.51/resilient_circuits/data/app.config.base`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/decorators.py` & `resilient_circuits-49.1.51/resilient_circuits/decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/helpers.py` & `resilient_circuits-49.1.51/resilient_circuits/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/rest_helper.py` & `resilient_circuits-49.1.51/resilient_circuits/rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/stomp_component.py` & `resilient_circuits-49.1.51/resilient_circuits/stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/stomp_events.py` & `resilient_circuits-49.1.51/resilient_circuits/stomp_events.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/stomp_transport.py` & `resilient_circuits-49.1.51/resilient_circuits/stomp_transport.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/template_functions.py` & `resilient_circuits-49.1.51/resilient_circuits/template_functions.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/util/__init__.py` & `resilient_circuits-49.1.51/resilient_circuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/util/resilient_config.py` & `resilient_circuits-49.1.51/resilient_circuits/util/resilient_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/util/resilient_customize.py` & `resilient_circuits-49.1.51/resilient_circuits/util/resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits/validate_configs.py` & `resilient_circuits-49.1.51/resilient_circuits/validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/resilient_circuits.egg-info/PKG-INFO` & `resilient_circuits-49.1.51/resilient_circuits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-circuits
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-49.0.4423/resilient_circuits.egg-info/SOURCES.txt` & `resilient_circuits-49.1.51/resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/setup.cfg` & `resilient_circuits-49.1.51/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient     >= 49.0
-	resilient-lib >= 49.0
+	resilient     >= 49.1
+	resilient-lib >= 49.1
 	
 	stompest      ~= 2.3
 	circuits      ~= 3.2
 	pysocks       ~= 1.6
 	filelock      ~= 3.2
 	
 	watchdog      ~= 2.1;  python_version >= "3.6"
```

### Comparing `resilient_circuits-49.0.4423/tests/cmds/test_selftest.py` & `resilient_circuits-49.1.51/tests/cmds/test_selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/conftest.py` & `resilient_circuits-49.1.51/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/helpers.py` & `resilient_circuits-49.1.51/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_config` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_function_component.py` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_commented_app_config` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_commented_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_component.py` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_constants.py` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_function_component.py` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_import_definition.txt` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_import_definition.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_paths.py` & `resilient_circuits-49.1.51/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_action_message.py` & `resilient_circuits-49.1.51/tests/test_action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_actions_component.py` & `resilient_circuits-49.1.51/tests/test_actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_app_config.py` & `resilient_circuits-49.1.51/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_app_function_component.py` & `resilient_circuits-49.1.51/tests/test_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_app_restartable.py` & `resilient_circuits-49.1.51/tests/test_app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_component_loader.py` & `resilient_circuits-49.1.51/tests/test_component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_decorators.py` & `resilient_circuits-49.1.51/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_errors.py` & `resilient_circuits-49.1.51/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_helpers.py` & `resilient_circuits-49.1.51/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_resilient_circuits_cmd.py` & `resilient_circuits-49.1.51/tests/test_resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_rest_helper.py` & `resilient_circuits-49.1.51/tests/test_rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_stomp_component.py` & `resilient_circuits-49.1.51/tests/test_stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/test_templates.py` & `resilient_circuits-49.1.51/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tests/util/test_resilient_customize.py` & `resilient_circuits-49.1.51/tests/util/test_resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-49.0.4423/tox.ini` & `resilient_circuits-49.1.51/tox.ini`

 * *Files identical despite different names*

