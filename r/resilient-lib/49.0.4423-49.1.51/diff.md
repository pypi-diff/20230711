# Comparing `tmp/resilient_lib-49.0.4423.tar.gz` & `tmp/resilient_lib-49.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_lib-49.0.4423.tar", last modified: Thu Jun  1 15:58:36 2023, max compression
+gzip compressed data, was "resilient_lib-49.1.51.tar", last modified: Tue Jul 11 16:14:33 2023, max compression
```

## Comparing `resilient_lib-49.0.4423.tar` & `resilient_lib-49.1.51.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6305 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.425552 resilient_lib-49.0.4423/resilient_lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/resilient_lib/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/function_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/integration_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/poller_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/requests_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/resilient_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/templates_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/workflow_status.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/resilient_lib/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/tab.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/resilient_lib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/util/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.425552 resilient_lib-49.0.4423/resilient_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-06-01 15:58:36.433552 resilient_lib-49.0.4423/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/data/default_template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/data/override_template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/cert.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/key.open.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_payload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      981 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6409 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.861333 resilient_lib-49.1.51/resilient_lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.861333 resilient_lib-49.1.51/resilient_lib/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/function_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/integration_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/poller_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/requests_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/resilient_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/templates_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/components/workflow_status.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/resilient_lib/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/ui/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/ui/conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/ui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/ui/tab.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/resilient_lib/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/resilient_lib/util/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.861333 resilient_lib-49.1.51/resilient_lib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2023-07-11 16:14:33.000000 resilient_lib-49.1.51/resilient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-07-11 16:14:33.000000 resilient_lib-49.1.51/resilient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:14:33.000000 resilient_lib-49.1.51/resilient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-07-11 16:14:33.000000 resilient_lib-49.1.51/resilient_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-07-11 16:14:33.000000 resilient_lib-49.1.51/resilient_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-07-11 16:14:33.000000 resilient_lib-49.1.51/resilient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/data/default_template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/data/override_template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/shared_mock_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/tests/shared_mock_data/mock_certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/shared_mock_data/mock_certs/cert.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/shared_mock_data/mock_certs/key.open.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_payload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:14:33.865332 resilient_lib-49.1.51/tests/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/ui/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/ui/test_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/ui/test_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tests/ui/test_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      981 2023-07-11 16:13:50.000000 resilient_lib-49.1.51/tox.ini
```

### Comparing `resilient_lib-49.0.4423/CHANGES` & `resilient_lib-49.1.51/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-07: version 49.1**
+
+* No major changes. Just bumping build number to coincide with other builds
+
 **2023-05: version 49.0**
 
 * Added new functions for pollers to interact with SOAR
 
 **2023-04: version 48.1**
 
 * Updated SOAR case default filters for poller helper methods
```

### Comparing `resilient_lib-49.0.4423/PKG-INFO` & `resilient_lib-49.1.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_lib
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-49.0.4423/README.md` & `resilient_lib-49.1.51/README.md`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/__init__.py` & `resilient_lib-49.1.51/resilient_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/function_metrics.py` & `resilient_lib-49.1.51/resilient_lib/components/function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/function_result.py` & `resilient_lib-49.1.51/resilient_lib/components/function_result.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/html2markdown.py` & `resilient_lib-49.1.51/resilient_lib/components/html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/integration_errors.py` & `resilient_lib-49.1.51/resilient_lib/components/integration_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/oauth2_client_credentials_session.py` & `resilient_lib-49.1.51/resilient_lib/components/oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/poller_common.py` & `resilient_lib-49.1.51/resilient_lib/components/poller_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/requests_common.py` & `resilient_lib-49.1.51/resilient_lib/components/requests_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/resilient_common.py` & `resilient_lib-49.1.51/resilient_lib/components/resilient_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/templates_common.py` & `resilient_lib-49.1.51/resilient_lib/components/templates_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/components/workflow_status.py` & `resilient_lib-49.1.51/resilient_lib/components/workflow_status.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/ui/common.py` & `resilient_lib-49.1.51/resilient_lib/ui/common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/ui/conditions.py` & `resilient_lib-49.1.51/resilient_lib/ui/conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/ui/elements.py` & `resilient_lib-49.1.51/resilient_lib/ui/elements.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/ui/tab.py` & `resilient_lib-49.1.51/resilient_lib/ui/tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib/util/config.py` & `resilient_lib-49.1.51/resilient_lib/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/resilient_lib.egg-info/PKG-INFO` & `resilient_lib-49.1.51/resilient_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-lib
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-49.0.4423/resilient_lib.egg-info/SOURCES.txt` & `resilient_lib-49.1.51/resilient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/setup.cfg` & `resilient_lib-49.1.51/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient      >= 49.0
+	resilient      >= 49.1
 	
 	pytz           ~= 2023.3
 	deprecated     ~= 1.2
 	beautifulsoup4 ~= 4.9
 	
 	jinja2         ~= 3.0; python_version >= "3.6"
```

### Comparing `resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/cert.pem` & `resilient_lib-49.1.51/tests/shared_mock_data/mock_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/key.open.pem` & `resilient_lib-49.1.51/tests/shared_mock_data/mock_certs/key.open.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_common.py` & `resilient_lib-49.1.51/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_function_metrics.py` & `resilient_lib-49.1.51/tests/test_function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_html2markdown.py` & `resilient_lib-49.1.51/tests/test_html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_oauth2_client_credentials_session.py` & `resilient_lib-49.1.51/tests/test_oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_payload.py` & `resilient_lib-49.1.51/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_poller.py` & `resilient_lib-49.1.51/tests/test_poller.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_requests.py` & `resilient_lib-49.1.51/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/test_templates.py` & `resilient_lib-49.1.51/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/ui/test_common.py` & `resilient_lib-49.1.51/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/ui/test_conditions.py` & `resilient_lib-49.1.51/tests/ui/test_conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/ui/test_permissions.py` & `resilient_lib-49.1.51/tests/ui/test_permissions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tests/ui/test_tab.py` & `resilient_lib-49.1.51/tests/ui/test_tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-49.0.4423/tox.ini` & `resilient_lib-49.1.51/tox.ini`

 * *Files identical despite different names*

