# Comparing `tmp/saltext.azurerm-2.0.2.tar.gz` & `tmp/saltext.azurerm-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltext.azurerm-2.0.2.tar", last modified: Mon Feb 13 16:43:58 2023, max compression
+gzip compressed data, was "saltext.azurerm-3.0.0.tar", last modified: Mon Jul 10 22:00:42 2023, max compression
```

## Comparing `saltext.azurerm-2.0.2.tar` & `saltext.azurerm-3.0.0.tar`

### file list

```diff
@@ -1,121 +1,163 @@
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      708 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/.coveragerc
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.467614 saltext.azurerm-2.0.2/.github/
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1201 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      547 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      581 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      635 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      463 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      933 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/.github/workflows/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    12055 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/.github/workflows/test.yml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1991 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/.gitignore
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8848 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/.pre-commit-hooks/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2084 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1372 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    11890 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/.pylintrc
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      457 2022-06-22 00:54:47.000000 saltext.azurerm-2.0.2/.readthedocs.yaml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      925 2023-02-13 16:43:44.000000 saltext.azurerm-2.0.2/CHANGELOG.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5280 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/CODE-OF-CONDUCT.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      703 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/CONTRIBUTING.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    11352 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/LICENSE
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      481 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/NOTICE.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4438 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/PKG-INFO
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3115 2022-06-22 00:54:47.000000 saltext.azurerm-2.0.2/README.md
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/changelog/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       12 2022-06-22 01:31:35.000000 saltext.azurerm-2.0.2/changelog/.gitignore
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      634 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/docs/Makefile
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/_static/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/docs/_static/.gitkeep
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      238 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/docs/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5323 2022-06-22 01:22:05.000000 saltext.azurerm-2.0.2/docs/conf.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      252 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/docs/index.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      760 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/docs/make.bat
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/ref/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/docs/ref/.gitkeep
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/ref/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      143 2022-06-22 01:16:49.000000 saltext.azurerm-2.0.2/docs/ref/clouds/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      800 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/ref/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      270 2022-06-22 01:16:49.000000 saltext.azurerm-2.0.2/docs/ref/modules/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      816 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      497 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_dns.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2189 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1092 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/ref/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      277 2022-06-22 01:16:49.000000 saltext.azurerm-2.0.2/docs/ref/states/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      309 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/states/saltext.azurerm.states.azurerm_compute.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      322 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/states/saltext.azurerm.states.azurerm_dns.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      747 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/states/saltext.azurerm.states.azurerm_network.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      434 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/states/saltext.azurerm.states.azurerm_resource.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/ref/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      138 2022-06-22 01:16:49.000000 saltext.azurerm-2.0.2/docs/ref/utils/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      339 2022-06-22 00:33:58.000000 saltext.azurerm-2.0.2/docs/ref/utils/saltext.azurerm.utils.azurerm.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/docs/sitevars.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/docs/topics/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5885 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/docs/topics/authentication.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       80 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/docs/topics/index.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    17842 2023-02-10 04:03:05.000000 saltext.azurerm-2.0.2/noxfile.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1016 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/pyproject.toml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2519 2023-02-13 16:43:58.477614 saltext.azurerm-2.0.2/setup.cfg
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      568 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/setup.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.467614 saltext.azurerm-2.0.2/src/
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.467614 saltext.azurerm-2.0.2/src/saltext/
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/src/saltext/azurerm/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      863 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/src/saltext/azurerm/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/clouds/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    67026 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/clouds/azurerm.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      803 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/loader.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/src/saltext/azurerm/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       35 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/modules/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    19486 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_compute.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    20133 2022-09-26 21:20:25.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_dns.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    82568 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_network.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    37903 2023-02-13 16:43:44.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_resource.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/src/saltext/azurerm/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/states/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    10287 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_compute.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    25691 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_dns.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    88144 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_network.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    26674 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_resource.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/src/saltext/azurerm/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       39 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/utils/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    12153 2023-02-13 15:42:34.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/utils/azurerm.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       65 2023-02-13 16:43:44.000000 saltext.azurerm-2.0.2/src/saltext/azurerm/version.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.470947 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4438 2023-02-13 16:43:58.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/PKG-INFO
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2784 2023-02-13 16:43:58.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/SOURCES.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        1 2023-02-13 16:43:58.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/dependency_links.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       48 2023-02-13 16:43:58.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/entry_points.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        1 2022-06-22 00:15:20.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/not-zip-safe
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      900 2023-02-13 16:43:58.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/requires.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        8 2023-02-13 16:43:58.000000 saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/top_level.txt
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      775 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/conftest.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/integration/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/integration/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/integration/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/integration/clouds/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      457 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/integration/conftest.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/integration/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/integration/modules/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/integration/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/integration/states/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/integration/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/integration/utils/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/unit/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/unit/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/unit/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/unit/clouds/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/unit/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/unit/modules/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/unit/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/unit/states/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-02-13 16:43:58.474281 saltext.azurerm-2.0.2/tests/unit/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/unit/utils/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       40 2022-06-21 23:53:27.000000 saltext.azurerm-2.0.2/tests/unit/utils/test_azurerm.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      708 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/.coveragerc
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.227945 saltext.azurerm-3.0.0/.github/
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.227945 saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1201 2022-09-26 21:20:25.000000 saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      547 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      581 2022-09-26 21:20:25.000000 saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      635 2022-09-26 21:20:25.000000 saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      463 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      933 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.227945 saltext.azurerm-3.0.0/.github/workflows/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    12839 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/.github/workflows/test.yml
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1991 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/.gitignore
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8848 2023-02-13 15:42:34.000000 saltext.azurerm-3.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.227945 saltext.azurerm-3.0.0/.pre-commit-hooks/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2084 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1372 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    11890 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/.pylintrc
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      457 2022-06-22 00:54:47.000000 saltext.azurerm-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1208 2023-07-10 21:59:35.000000 saltext.azurerm-3.0.0/CHANGELOG.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5280 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      703 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/CONTRIBUTING.md
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    11352 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/LICENSE
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      481 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/NOTICE.txt
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4438 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/PKG-INFO
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3115 2022-06-22 00:54:47.000000 saltext.azurerm-3.0.0/README.md
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.227945 saltext.azurerm-3.0.0/changelog/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       12 2022-06-22 01:31:35.000000 saltext.azurerm-3.0.0/changelog/.gitignore
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.231279 saltext.azurerm-3.0.0/docs/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      634 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/docs/Makefile
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.231279 saltext.azurerm-3.0.0/docs/_static/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/docs/_static/.gitkeep
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      238 2022-09-26 21:20:25.000000 saltext.azurerm-3.0.0/docs/all.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5323 2022-06-22 01:22:05.000000 saltext.azurerm-3.0.0/docs/conf.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      252 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/docs/index.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      760 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/docs/make.bat
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.231279 saltext.azurerm-3.0.0/docs/ref/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/docs/ref/.gitkeep
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.231279 saltext.azurerm-3.0.0/docs/ref/clouds/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      143 2022-06-22 01:16:49.000000 saltext.azurerm-3.0.0/docs/ref/clouds/all.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      800 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.231279 saltext.azurerm-3.0.0/docs/ref/modules/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      778 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/all.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      816 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      369 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_availability_set.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      340 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_disk.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      327 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_image.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      733 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      391 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_extension.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      399 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_image.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      497 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_dns.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      620 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_key.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      613 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_secret.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      179 2023-06-13 12:36:09.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_vault.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2189 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1092 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/docs/ref/states/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      545 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/states/all.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      309 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_compute.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      290 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_compute_availability_set.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      287 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_compute_virtual_machine.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      322 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_dns.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      289 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_key.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      298 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_secret.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      176 2023-06-13 12:36:09.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_vault.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      747 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_network.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      434 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_resource.rst
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/docs/ref/utils/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      138 2022-06-22 01:16:49.000000 saltext.azurerm-3.0.0/docs/ref/utils/all.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      339 2022-06-22 00:33:58.000000 saltext.azurerm-3.0.0/docs/ref/utils/saltext.azurerm.utils.azurerm.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/docs/sitevars.rst
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/docs/topics/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5885 2022-09-26 21:20:25.000000 saltext.azurerm-3.0.0/docs/topics/authentication.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       80 2022-09-26 21:20:25.000000 saltext.azurerm-3.0.0/docs/topics/index.rst
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    17841 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/noxfile.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1016 2023-02-13 15:42:34.000000 saltext.azurerm-3.0.0/pyproject.toml
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2591 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/setup.cfg
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      568 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/setup.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.224612 saltext.azurerm-3.0.0/src/
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.224612 saltext.azurerm-3.0.0/src/saltext/
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/src/saltext/azurerm/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      863 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/src/saltext/azurerm/clouds/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/clouds/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    67166 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/clouds/azurerm.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/src/saltext/azurerm/fileserver/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    14404 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/fileserver/azurefs.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      803 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/loader.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       35 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    14063 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     7448 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute_availability_set.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5678 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute_disk.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8509 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute_image.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    59216 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     7037 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_extension.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     6331 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_image.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    20227 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_dns.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    23448 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_keyvault_key.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    16546 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_keyvault_secret.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    19494 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_keyvault_vault.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    83152 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_network.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    38085 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_resource.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/src/saltext/azurerm/states/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     6204 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_compute.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     9457 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_compute_availability_set.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    37179 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_compute_virtual_machine.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    25691 2023-02-13 15:42:34.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_dns.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8639 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_keyvault_key.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    10245 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_keyvault_secret.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    18314 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_keyvault_vault.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    88144 2023-02-13 15:42:34.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_network.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    26674 2023-02-13 15:42:34.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_resource.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/src/saltext/azurerm/utils/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       39 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/utils/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    12926 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/utils/azurerm.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       65 2023-07-10 21:59:35.000000 saltext.azurerm-3.0.0/src/saltext/azurerm/version.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.234612 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4438 2023-07-10 22:00:42.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/PKG-INFO
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5250 2023-07-10 22:00:42.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/SOURCES.txt
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        1 2023-07-10 22:00:42.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/dependency_links.txt
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       48 2023-07-10 22:00:42.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/entry_points.txt
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        1 2022-06-22 00:15:20.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/not-zip-safe
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      969 2023-07-10 22:00:42.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/requires.txt
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        8 2023-07-10 22:00:42.000000 saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/top_level.txt
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/tests/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      708 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/conftest.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/tests/integration/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/integration/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/tests/integration/clouds/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/integration/clouds/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5587 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/integration/conftest.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.237945 saltext.azurerm-3.0.0/tests/integration/modules/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/integration/modules/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/integration/states/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/integration/states/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2811 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/integration/states/test_compute_availability_set.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4379 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/integration/states/test_compute_virtual_machine.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5633 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_dns.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3566 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/integration/states/test_keyvault_key.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4256 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/integration/states/test_keyvault_secret.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     7796 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/integration/states/test_keyvault_vault.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3392 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_network_interface.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5874 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_network_route.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     6566 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_network_security_group.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4681 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_public_ip_address.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3316 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_resource_group.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8846 2023-06-13 12:36:03.000000 saltext.azurerm-3.0.0/tests/integration/states/test_virtual_network.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/integration/utils/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/integration/utils/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/unit/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/unit/clouds/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/unit/clouds/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/unit/modules/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/unit/modules/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/unit/states/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/unit/states/__init__.py
+drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-07-10 22:00:42.241279 saltext.azurerm-3.0.0/tests/unit/utils/
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-3.0.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8157 2023-07-10 10:59:30.000000 saltext.azurerm-3.0.0/tests/unit/utils/test_azurerm.py
```

### Comparing `saltext.azurerm-2.0.2/.coveragerc` & `saltext.azurerm-3.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/config.yml` & `saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/docs.md` & `saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/docs.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `saltext.azurerm-3.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.github/PULL_REQUEST_TEMPLATE.md` & `saltext.azurerm-3.0.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.github/workflows/test.yml` & `saltext.azurerm-3.0.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   Pre-Commit:
     runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v1
       with:
-        python-version: 3.9
+        python-version: "3.10"
     - name: Set Cache Key
       run: echo "PY=$(python --version --version | sha256sum | cut -d' ' -f1)" >> $GITHUB_ENV
     - name: Install System Deps
       run: |
         sudo apt-get update
         sudo apt-get install -y libxml2 libxml2-dev libxslt-dev
     - uses: actions/cache@v1
@@ -29,28 +29,28 @@
     needs: Pre-Commit
 
     timeout-minutes: 10
 
     steps:
     - uses: actions/checkout@v2
 
-    - name: Set up Python 3.9 For Nox
+    - name: Set up Python 3.10 For Nox
       uses: actions/setup-python@v1
       with:
-        python-version: 3.9
+        python-version: "3.10"
 
     - name: Install Nox
       run: |
         python -m pip install --upgrade pip
         pip uninstall -y distro-info
         pip install nox
 
     - name: Install Doc Requirements
       env:
-        SALT_REQUIREMENT: salt==3005.1
+        SALT_REQUIREMENT: salt==3006.1
       run: |
         nox --force-color -e docs --install-only
 
     - name: Build Docs
       env:
         SKIP_REQUIREMENTS_INSTALL: YES
       run: |
@@ -63,20 +63,17 @@
     timeout-minutes: 15
 
     strategy:
       fail-fast: false
       max-parallel: 4
       matrix:
         python-version:
-          - 3.7
-          - 3.8
-          - 3.9
           - "3.10"
         salt-version:
-          - 3005.1
+          - 3006.1
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
@@ -90,20 +87,28 @@
 
     - name: Install Test Requirements
       env:
         SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
       run: |
         nox --force-color -e tests-3 --install-only
 
-    - name: Test
+    - name: Unit Test
       env:
         SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
         SKIP_REQUIREMENTS_INSTALL: YES
       run: |
-        nox --force-color -e tests-3 -- -vv tests/
+        nox --force-color -e tests-3 -- -vv tests/unit
+
+    - name: Integration Test
+      if: false
+      env:
+        SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
+        SKIP_REQUIREMENTS_INSTALL: YES
+      run: |
+        nox --force-color -e tests-3 -- -vv tests/integration
 
     - name: Create CodeCov Flags
       if: always()
       id: codecov-flags
       run: |
         echo ::set-output name=flags::$(python -c "import sys; print('{},{},salt_{}'.format('${{ runner.os }}'.replace('-22.04', ''), 'py{}{}'.format(*sys.version_info), '_'.join(str(v) for v in '${{ matrix.salt-version }}'.replace('==', '_').split('.'))))")
 
@@ -175,27 +180,28 @@
       if: always()
       uses: actions/upload-artifact@main
       with:
         name: runtests-${{ runner.os }}-py${{ matrix.python-version }}-Salt${{ matrix.salt-version }}.log
         path: artifacts/runtests-*.log
 
   Windows:
+    if: false
     runs-on: windows-2019
     needs: Pre-Commit
 
     timeout-minutes: 40
 
     strategy:
       fail-fast: false
       max-parallel: 3
       matrix:
         python-version:
-          - 3.7
+          - "3.10"
         salt-version:
-          - 3004.2
+          - 3006.1
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
@@ -211,22 +217,32 @@
       env:
         SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
         EXTRA_REQUIREMENTS_INSTALL: Cython
       run: |
         export PATH="/C/Program Files (x86)/Windows Kits/10/bin/10.0.18362.0/x64;$PATH"
         nox --force-color -e tests-3 --install-only
 
-    - name: Test
+    - name: Unit Test
       shell: bash
       env:
         SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
         SKIP_REQUIREMENTS_INSTALL: YES
       run: |
         export PATH="/C/Program Files (x86)/Windows Kits/10/bin/10.0.18362.0/x64;$PATH"
-        nox --force-color -e tests-3 -- -vv tests/
+        nox --force-color -e tests-3 -- -vv tests/unit
+
+    - name: Integration Test
+      if: false
+      shell: bash
+      env:
+        SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
+        SKIP_REQUIREMENTS_INSTALL: YES
+      run: |
+        export PATH="/C/Program Files (x86)/Windows Kits/10/bin/10.0.18362.0/x64;$PATH"
+        nox --force-color -e tests-3 -- -vv tests/integration
 
     - name: Create CodeCov Flags
       if: always()
       id: codecov-flags
       run: |
         echo ::set-output name=flags::$(python -c "import sys; print('{},{},salt_{}'.format('${{ runner.os }}'.replace('-2019', ''), 'py{}{}'.format(*sys.version_info), '_'.join(str(v) for v in '${{ matrix.salt-version }}'.replace('==', '_').split('.'))))")
 
@@ -298,29 +314,28 @@
       if: always()
       uses: actions/upload-artifact@main
       with:
         name: runtests-${{ runner.os }}-py${{ matrix.python-version }}-Salt${{ matrix.salt-version }}.log
         path: artifacts/runtests-*.log
 
   macOS:
+    if: false
     runs-on: macOS-10.15
     needs: Pre-Commit
 
     timeout-minutes: 40
 
     strategy:
       fail-fast: false
       max-parallel: 3
       matrix:
         python-version:
-          - 3.7
-          - 3.8
-          - 3.9
+          - "3.10"
         salt-version:
-          - 3004.2
+          - 3006.1
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
@@ -333,20 +348,28 @@
 
     - name: Install Test Requirements
       env:
         SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
       run: |
         nox --force-color -e tests-3 --install-only
 
-    - name: Test
+    - name: Unit Test
+      env:
+        SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
+        SKIP_REQUIREMENTS_INSTALL: YES
+      run: |
+        nox --force-color -e tests-3 -- -vv tests/unit
+
+    - name: Integration Test
+      if: false
       env:
         SALT_REQUIREMENT: salt==${{ matrix.salt-version }}
         SKIP_REQUIREMENTS_INSTALL: YES
       run: |
-        nox --force-color -e tests-3 -- -vv tests/
+        nox --force-color -e tests-3 -- -vv tests/integration
 
     - name: Create CodeCov Flags
       if: always()
       id: codecov-flags
       run: |
         echo ::set-output name=flags::$(python -c "import sys; print('{},{},salt_{}'.format('${{ runner.os }}'.replace('-10.15', ''), 'py{}{}'.format(*sys.version_info), '_'.join(str(v) for v in '${{ matrix.salt-version }}'.replace('==', '_').split('.'))))")
```

### Comparing `saltext.azurerm-2.0.2/.gitignore` & `saltext.azurerm-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.pre-commit-config.yaml` & `saltext.azurerm-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.pre-commit-hooks/check-cli-examples.py` & `saltext.azurerm-3.0.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.pre-commit-hooks/make-autodocs.py` & `saltext.azurerm-3.0.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/.pylintrc` & `saltext.azurerm-3.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/CHANGELOG.md` & `saltext.azurerm-3.0.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 The changelog format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 This project uses [Semantic Versioning](https://semver.org/) - MAJOR.MINOR.PATCH
 
 # Changelog
 
+Saltext.Azurerm 3.0.0 (2023-07-10)
+==================================
+
+Added
+-----
+
+- Add more ARM compute functionality - VMs, disk, images (#34)
+- Port AzureFS backend from Salt (#31)
+- Add KeyVault operations (#28)
+
+Deprecated
+----------
+
+- Start to deprecate msrestazure (#32)
+
+
 Saltext.Azurerm 2.0.2 (2023-02-13)
 ==================================
 
 Fixed
 -----
 
 - Fix deployment resource validation function (#21)
```

### Comparing `saltext.azurerm-2.0.2/CODE-OF-CONDUCT.md` & `saltext.azurerm-3.0.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/CONTRIBUTING.md` & `saltext.azurerm-3.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/LICENSE` & `saltext.azurerm-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/PKG-INFO` & `saltext.azurerm-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.azurerm
-Version: 2.0.2
+Version: 3.0.0
 Summary: Salt Extension Modules for Azure Resource Manager
 Home-page: https://github.com/salt-extensions/saltext-azurerm
 Author: EITR Technologies, LLC
 Author-email: devops@eitr.tech
 License: Apache Software License
 Project-URL: Source, https://github.com/salt-extensions/saltext-azurerm
 Project-URL: Tracker, https://github.com/salt-extensions/saltext-azurerm/issues
```

### Comparing `saltext.azurerm-2.0.2/README.md` & `saltext.azurerm-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/Makefile` & `saltext.azurerm-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/conf.py` & `saltext.azurerm-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/make.bat` & `saltext.azurerm-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst` & `saltext.azurerm-3.0.0/docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst` & `saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst` & `saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst` & `saltext.azurerm-3.0.0/docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/ref/states/saltext.azurerm.states.azurerm_network.rst` & `saltext.azurerm-3.0.0/docs/ref/states/saltext.azurerm.states.azurerm_network.rst`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/docs/topics/authentication.rst` & `saltext.azurerm-3.0.0/docs/topics/authentication.rst`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/noxfile.py` & `saltext.azurerm-3.0.0/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     os.environ.get("JENKINS_URL") or os.environ.get("CI") or os.environ.get("DRONE") is not None
 )
 PIP_INSTALL_SILENT = CI_RUN is False
 SKIP_REQUIREMENTS_INSTALL = "SKIP_REQUIREMENTS_INSTALL" in os.environ
 EXTRA_REQUIREMENTS_INSTALL = os.environ.get("EXTRA_REQUIREMENTS_INSTALL")
 
 COVERAGE_VERSION_REQUIREMENT = "coverage==5.2"
-SALT_REQUIREMENT = os.environ.get("SALT_REQUIREMENT") or "salt>=3003rc1"
+SALT_REQUIREMENT = os.environ.get("SALT_REQUIREMENT") or "salt>=3006.1"
 if SALT_REQUIREMENT == "salt==master":
     SALT_REQUIREMENT = "git+https://github.com/saltstack/salt.git@master"
 
 # Prevent Python from writing bytecode
 os.environ["PYTHONDONTWRITEBYTECODE"] = "1"
 
 # Global Path Definitions
```

### Comparing `saltext.azurerm-2.0.2/pyproject.toml` & `saltext.azurerm-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/setup.cfg` & `saltext.azurerm-3.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,20 @@
 	azure-identity==1.10.0
 	azure-core==1.24.2
 	azure-mgmt-authorization==2.0.0
 	azure-mgmt-batch==16.2.0
 	azure-mgmt-compute==27.1.0
 	azure-mgmt-dns==8.0.0
 	azure-mgmt-privatedns==1.0.0
-	azure-mgmt-keyvault==10.0.0
+	azure-mgmt-keyvault==10.1.0
+	azure-mgmt-monitor==6.0.1
 	azure-mgmt-msi==6.0.1
 	azure-mgmt-network==20.0.0
 	azure-mgmt-resource==21.1.0
+	azure-mgmt-storage==21.0.0
 	azure-mgmt-subscription==3.0.0
 	azure-mgmt-web==6.1.0
 	azure-storage-blob==12.12.0
 	azure-storage-common==2.1.0
 	azure-storage-file==2.1.0
 	azure-storage-nspkg==3.1.0
 	azure-storage-queue==12.3.0
@@ -73,15 +75,16 @@
 salt.loader = 
 	saltext.azurerm = saltext.azurerm
 
 [options.extras_require]
 tests = 
 	mock>=3.0.5
 	pytest>=7.2.0
-	pytest-salt-factories>=1.0.0rc21
+	pytest-salt-factories>=1.0.0rc23
+	pytest-ordering
 	Jinja2
 dev = 
 	nox==2022.1.7
 	pre-commit==2.13.0
 	pylint<2.14.0
 	SaltPyLint
 docs =
```

### Comparing `saltext.azurerm-2.0.2/setup.py` & `saltext.azurerm-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/__init__.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/__init__.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/clouds/azurerm.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/clouds/azurerm.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 HAS_LIBS = False
 try:
     import azure.mgmt.compute.models as compute_models
     import azure.mgmt.network.models as network_models
 
     from azure.storage.blob import BlobServiceClient, ContainerClient
-    from msrestazure.azure_exceptions import CloudError
+    from azure.core.exceptions import HttpResponseError
 
     HAS_LIBS = True
 except ImportError:
     pass
 
 __virtualname__ = "azurerm"
 
@@ -179,15 +179,15 @@
             resource_provider_namespace=kwargs["resource_provider"]
         )
 
         for resource in provider_query.resource_types:
             if str(resource.resource_type) == kwargs["resource_type"]:
                 resource_dict = resource.as_dict()
                 api_versions = resource_dict["api_versions"]
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", exc.message)
 
     return api_versions
 
 
 def get_resource_by_id(resource_id, api_version, extract_value=None):
     """
@@ -201,15 +201,15 @@
             resource_id=resource_id, api_version=api_version
         )
         resource_dict = resource_query.as_dict()
         if extract_value is not None:
             ret = resource_dict[extract_value]
         else:
             ret = resource_dict
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", exc.message)
         ret = {"Error": exc.message}
 
     return ret
 
 
 def get_configured_provider():
@@ -321,15 +321,15 @@
         for resource in provider_query.resource_types:
             if str(resource.resource_type) == "virtualMachines":
                 resource_dict = resource.as_dict()
                 locations = resource_dict["locations"]
         for location in locations:
             lowercase = location.lower().replace(" ", "")
             ret["locations"].append(lowercase)
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", exc.message)
         ret = {"Error": exc.message}
 
     return ret
 
 
 def avail_images(call=None):
@@ -383,26 +383,26 @@
                         )
                         data[name] = {
                             "publisher": publisher,
                             "offer": offer["name"],
                             "sku": sku["name"],
                             "version": version["name"],
                         }
-        except CloudError as exc:
+        except HttpResponseError as exc:
             saltext.azurerm.utils.azurerm.log_cloud_error("compute", exc.message)
             data = {publisher: exc.message}
 
         return data
 
     try:
         publishers_query = compconn.virtual_machine_images.list_publishers(location=region)
         for publisher_obj in publishers_query:
             publisher = publisher_obj.as_dict()
             publishers.append(publisher["name"])
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("compute", exc.message)
 
     pool = ThreadPool(cpu_count() * 6)
     results = pool.map_async(_get_publisher_images, publishers)
     results.wait()
 
     ret = {k: v for result in results.get() for k, v in result.items()}
@@ -426,15 +426,15 @@
     location = get_location()
 
     try:
         sizes = compconn.virtual_machine_sizes.list(location=location)
         for size_obj in sizes:
             size = size_obj.as_dict()
             ret[size["name"]] = size
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("compute", exc.message)
         ret = {"Error": exc.message}
 
     return ret
 
 
 def list_nodes(call=None):
@@ -548,15 +548,15 @@
     ret = {}
     try:
         groups = resconn.resource_groups.list()
 
         for group_obj in groups:
             group = group_obj.as_dict()
             ret[group["name"]] = group
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", exc.message)
         ret = {"Error": exc.message}
 
     return ret
 
 
 def show_instance(name, call=None):
@@ -618,15 +618,15 @@
     """
     netconn = get_conn(client_type="network")
     try:
         pubip_query = netconn.public_ip_addresses.get(
             resource_group_name=resource_group, public_ip_address_name=name
         )
         pubip = pubip_query.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", exc.message)
         pubip = {"error": exc.message}
 
     return pubip
 
 
 def _get_network_interface(name, resource_group):
@@ -709,15 +709,15 @@
 
     try:
         subnet_obj = netconn.subnets.get(
             resource_group_name=kwargs["network_resource_group"],
             virtual_network_name=kwargs["network"],
             subnet_name=kwargs["subnet"],
         )
-    except CloudError as exc:
+    except HttpResponseError as exc:
         raise SaltCloudSystemExit(  # pylint: disable=raise-missing-from
             '{} (Resource Group: "{}", VNET: "{}", Subnet: "{}")'.format(
                 exc.message,
                 kwargs["network_resource_group"],
                 kwargs["network"],
                 kwargs["subnet"],
             )
@@ -735,15 +735,15 @@
                     try:
                         lbbep_data = netconn.load_balancer_backend_address_pools.get(
                             kwargs["resource_group"],
                             load_bal,
                             pool,
                         )
                         pool_ids.append({"id": lbbep_data.as_dict()["id"]})
-                    except CloudError as exc:
+                    except HttpResponseError as exc:
                         log.error("There was a cloud error: %s", str(exc))
                     except KeyError as exc:
                         log.error(
                             "There was an error getting the Backend Pool ID: %s",
                             str(exc),
                         )
             ip_kwargs["load_balancer_backend_address_pools"] = pool_ids
@@ -780,15 +780,15 @@
                         NetworkInterfaceIPConfiguration(
                             name="{}-ip".format(kwargs["iface_name"]),
                             subnet=subnet_obj,
                             **ip_kwargs
                         )
                     ]
                     break
-            except CloudError as exc:
+            except HttpResponseError as exc:
                 log.error("There was a cloud error: %s", exc)
             count += 1
             if count > 120:
                 raise ValueError("Timed out waiting for public IP Address.")
             time.sleep(5)
     else:
         priv_ip_name = "{}-ip".format(kwargs["iface_name"])
@@ -821,15 +821,15 @@
             exc,
         )
 
     count = 0
     while True:
         try:
             return _get_network_interface(kwargs["iface_name"], kwargs["resource_group"])
-        except CloudError:
+        except HttpResponseError:
             count += 1
             if count > 120:
                 raise ValueError(  # pylint: disable=raise-missing-from
                     "Timed out waiting for operation to complete."
                 )  # pylint: disable=raise-missing-from
             time.sleep(5)
 
@@ -1219,15 +1219,15 @@
             polling=True,
         )
         vm_create.wait()
         vm_result = vm_create.result()
         vm_result = vm_result.as_dict()
         if custom_extension:
             create_or_update_vmextension(kwargs=custom_extension)
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("compute", exc.message)
         vm_result = {}
 
     return vm_result
 
 
 def create(vm_):
@@ -1515,15 +1515,15 @@
 
     ret = {}
     try:
         accounts_query = storconn.storage_accounts.list()
         accounts = saltext.azurerm.utils.azurerm.paged_object_to_list(accounts_query)
         for account in accounts:
             ret[account["name"]] = account
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("storage", exc.message)
         ret = {"Error": exc.message}
 
     return ret
 
 
 def _get_cloud_environment():
@@ -1690,15 +1690,15 @@
     netconn = get_conn(client_type="network")
     resource_groups = list_resource_groups()
 
     ret = {}
     for group in resource_groups:
         try:
             networks = netconn.virtual_networks.list(resource_group_name=group)
-        except CloudError:
+        except HttpResponseError:
             networks = {}
         for network_obj in networks:
             network = network_obj.as_dict()
             ret[network["name"]] = network
             ret[network["name"]]["subnets"] = list_subnets(
                 kwargs={"resource_group": group, "network": network["name"]}
             )
@@ -1833,15 +1833,15 @@
             kwargs["virtual_machine_name"],
             kwargs["extension_name"],
             params,
         )
         ret = poller.result()
         ret = ret.as_dict()
 
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error(
             "compute",
             "Error attempting to create the VM extension: {}".format(exc.message),
         )
         ret = {"error": exc.message}
 
     return ret
@@ -1876,15 +1876,15 @@
                 instance = compconn.virtual_machines.deallocate(
                     vm_name=name, resource_group_name=group
                 )
                 instance.wait()
                 vm_result = instance.result()
                 ret = vm_result.as_dict()
                 break
-            except CloudError as exc:
+            except HttpResponseError as exc:
                 if "was not found" in exc.message:
                     continue
                 else:
                     ret = {"error": exc.message}
         if not ret:
             saltext.azurerm.utils.azurerm.log_cloud_error(
                 "compute", "Unable to find virtual machine with name: {}".format(name)
@@ -1894,15 +1894,15 @@
         try:
             instance = compconn.virtual_machines.deallocate(
                 vm_name=name, resource_group_name=resource_group
             )
             instance.wait()
             vm_result = instance.result()
             ret = vm_result.as_dict()
-        except CloudError as exc:
+        except HttpResponseError as exc:
             saltext.azurerm.utils.azurerm.log_cloud_error(
                 "compute", "Error attempting to stop {}: {}".format(name, exc.message)
             )
             ret = {"error": exc.message}
 
     return ret
 
@@ -1934,15 +1934,15 @@
         for group in groups:
             try:
                 instance = compconn.virtual_machines.start(vm_name=name, resource_group_name=group)
                 instance.wait()
                 vm_result = instance.result()
                 ret = vm_result.as_dict()
                 break
-            except CloudError as exc:
+            except HttpResponseError as exc:
                 if "was not found" in exc.message:
                     continue
                 else:
                     ret = {"error": exc.message}
         if not ret:
             saltext.azurerm.utils.azurerm.log_cloud_error(
                 "compute", "Unable to find virtual machine with name: {}".format(name)
@@ -1952,15 +1952,15 @@
         try:
             instance = compconn.virtual_machines.start(
                 vm_name=name, resource_group_name=resource_group
             )
             instance.wait()
             vm_result = instance.result()
             ret = vm_result.as_dict()
-        except CloudError as exc:
+        except HttpResponseError as exc:
             saltext.azurerm.utils.azurerm.log_cloud_error(
                 "compute",
                 "Error attempting to start {}: {}".format(name, exc.message),
             )
             ret = {"error": exc.message}
 
     return ret
```

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/loader.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/loader.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_dns.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_dns.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,15 @@
 import saltext.azurerm.utils.azurerm
 
 # Azure libs
 HAS_LIBS = False
 try:
     import azure.mgmt.dns.models  # pylint: disable=unused-import
     import azure.mgmt.privatedns.models  # pylint: disable=unused-import
-    from msrest.exceptions import SerializationError
-    from msrestazure.azure_exceptions import CloudError
-    from azure.core.exceptions import ResourceNotFoundError
+    from azure.core.exceptions import ResourceNotFoundError, HttpResponseError, SerializationError
 
     HAS_LIBS = True
 except ImportError:
     pass
 
 __virtualname__ = "azurerm_dns"
 
@@ -134,15 +132,15 @@
                 resource_group_name=resource_group,
                 record_type=record_type,
                 parameters=record_set_model,
                 if_match=kwargs.get("if_match"),
                 if_none_match=kwargs.get("if_none_match"),
             )
         result = record_set.as_dict()
-    except ResourceNotFoundError as exc:
+    except (HttpResponseError, ResourceNotFoundError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -178,30 +176,31 @@
     client = "dns"
     if zone_type.lower() == "private":
         client = "privatedns"
 
     dnsconn = saltext.azurerm.utils.azurerm.get_client(client, **kwargs)
     try:
         if zone_type.lower() == "private":
-            result = dnsconn.record_sets.delete(
+            dnsconn.record_sets.delete(
                 relative_record_set_name=name,
                 private_zone_name=zone_name,
                 resource_group_name=resource_group,
                 record_type=record_type,
                 if_match=kwargs.get("if_match"),
             )
         else:
-            result = dnsconn.record_sets.delete(
+            dnsconn.record_sets.delete(
                 relative_record_set_name=name,
                 zone_name=zone_name,
                 resource_group_name=resource_group,
                 record_type=record_type,
                 if_match=kwargs.get("if_match"),
             )
-    except CloudError as exc:
+        result = True
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
 
     return result
 
 
 def record_set_get(name, zone_name, resource_group, record_type, zone_type="Public", **kwargs):
     """
@@ -246,15 +245,15 @@
             record_set = dnsconn.record_sets.get(
                 relative_record_set_name=name,
                 zone_name=zone_name,
                 resource_group_name=resource_group,
                 record_type=record_type,
             )
         result = record_set.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error(client, str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def record_sets_list_by_type(
@@ -322,15 +321,15 @@
                     record_type=record_type,
                     top=top,
                     recordsetnamesuffix=recordsetnamesuffix,
                 )
             )
         for record_set in record_sets:
             result[record_set["name"]] = record_set
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def record_sets_list_by_dns_zone(
@@ -387,15 +386,15 @@
                     top=top,
                     recordsetnamesuffix=recordsetnamesuffix,
                 )
             )
 
         for record_set in record_sets:
             result[record_set["name"]] = record_set
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def zone_create_or_update(name, resource_group, zone_type="Public", **kwargs):
@@ -463,15 +462,15 @@
                 zone_name=name,
                 resource_group_name=resource_group,
                 parameters=zone_model,
                 if_match=kwargs.get("if_match"),
                 if_none_match=kwargs.get("if_none_match"),
             )
             result = zone.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -507,22 +506,22 @@
             zone = dnsconn.private_zones.begin_delete(
                 private_zone_name=name,
                 resource_group_name=resource_group,
                 if_match=kwargs.get("if_match"),
                 polling=True,
             )
         else:
-            zone = dnsconn.zones.delete(
+            zone = dnsconn.zones.begin_delete(
                 zone_name=name,
                 resource_group_name=resource_group,
                 if_match=kwargs.get("if_match"),
             )
         zone.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
 
     return result
 
 
 def zone_get(name, resource_group, zone_type="Public", **kwargs):
     """
@@ -555,15 +554,15 @@
                 private_zone_name=name, resource_group_name=resource_group
             )
             result = zone.as_dict()
         else:
             zone = dnsconn.zones.get(zone_name=name, resource_group_name=resource_group)
             result = zone.as_dict()
 
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def zones_list_by_resource_group(resource_group, zone_type="Public", top=None, **kwargs):
@@ -604,15 +603,15 @@
         else:
             zones = saltext.azurerm.utils.azurerm.paged_object_to_list(
                 dnsconn.zones.list_by_resource_group(resource_group_name=resource_group, top=top)
             )
 
         for zone in zones:
             result[zone["name"]] = zone
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def zones_list(top=None, zone_type="Public", **kwargs):
@@ -647,12 +646,12 @@
                 dnsconn.private_zones.list(top=top)
             )
         else:
             zones = saltext.azurerm.utils.azurerm.paged_object_to_list(dnsconn.zones.list(top=top))
 
         for zone in zones:
             result[zone["name"]] = zone
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
```

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_network.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
 import saltext.azurerm.utils.azurerm
 
 # Azure libs
 HAS_LIBS = False
 try:
     import azure.mgmt.network.models  # pylint: disable=unused-import
-    from msrest.exceptions import SerializationError
-    from msrestazure.azure_exceptions import CloudError
-    from azure.core.exceptions import ResourceNotFoundError
+    from azure.core.exceptions import ResourceNotFoundError, HttpResponseError, SerializationError
 
     HAS_LIBS = True
 except ImportError:
     pass
 
 __virtualname__ = "azurerm_network"
 
@@ -86,15 +84,15 @@
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         check_dns_name = netconn.check_dns_name_availability(
             location=region, domain_name_label=name
         )
         result = check_dns_name.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def check_ip_address_availability(ip_address, virtual_network, resource_group, **kwargs):
@@ -123,15 +121,15 @@
     try:
         check_ip = netconn.virtual_networks.check_ip_address_availability(
             resource_group_name=resource_group,
             virtual_network_name=virtual_network,
             ip_address=ip_address,
         )
         result = check_ip.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def default_security_rule_get(name, security_group, resource_group, **kwargs):
@@ -234,15 +232,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         secrules = netconn.security_rules.list(
             network_security_group_name=security_group,
             resource_group_name=resource_group,
         )
         result = saltext.azurerm.utils.azurerm.paged_object_to_list(secrules)
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def security_rule_create_or_update(
@@ -370,24 +368,24 @@
             **kwargs
         )
     except TypeError as exc:
         result = {"error": "The object model could not be built. ({})".format(str(exc))}
         return result
 
     try:
-        secrule = netconn.security_rules.create_or_update(
+        secrule = netconn.security_rules.begin_create_or_update(
             resource_group_name=resource_group,
             network_security_group_name=security_group,
             security_rule_name=name,
             security_rule_parameters=rulemodel,
         )
         secrule.wait()
         secrule_result = secrule.result()
         result = secrule_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -420,15 +418,15 @@
             network_security_group_name=security_group,
             resource_group_name=resource_group,
             security_rule_name=security_rule,
             polling=True,
         )
         secrule.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def security_rule_get(security_rule, security_group, resource_group, **kwargs):
     """
@@ -455,15 +453,15 @@
     try:
         secrule = netconn.security_rules.get(
             network_security_group_name=security_group,
             resource_group_name=resource_group,
             security_rule_name=security_rule,
         )
         result = secrule.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def network_security_group_create_or_update(
@@ -510,15 +508,15 @@
             network_security_group_name=name,
             parameters=secgroupmodel,
             polling=True,
         )
         secgroup.wait()
         secgroup_result = secgroup.result()
         result = secgroup_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -545,15 +543,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         secgroup = netconn.network_security_groups.begin_delete(
             resource_group_name=resource_group, network_security_group_name=name, polling=True
         )
         secgroup.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def network_security_group_get(name, resource_group, **kwargs):
     """
@@ -606,15 +604,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         secgroups = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.network_security_groups.list(resource_group_name=resource_group)
         )
         for secgroup in secgroups:
             result[secgroup["name"]] = secgroup
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def network_security_groups_list_all(**kwargs):  # pylint: disable=invalid-name
@@ -634,15 +632,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         secgroups = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.network_security_groups.list_all()
         )
         for secgroup in secgroups:
             result[secgroup["name"]] = secgroup
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def subnets_list(virtual_network, resource_group, **kwargs):
@@ -670,15 +668,15 @@
             netconn.subnets.list(
                 resource_group_name=resource_group, virtual_network_name=virtual_network
             )
         )
 
         for subnet in subnets:
             result[subnet["name"]] = subnet
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def subnet_get(name, virtual_network, resource_group, **kwargs):
@@ -707,15 +705,15 @@
         subnet = netconn.subnets.get(
             resource_group_name=resource_group,
             virtual_network_name=virtual_network,
             subnet_name=name,
         )
 
         result = subnet.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def subnet_create_or_update(name, address_prefix, virtual_network, resource_group, **kwargs):
@@ -779,15 +777,15 @@
             subnet_name=name,
             subnet_parameters=snetmodel,
             polling=True,
         )
         subnet.wait()
         sn_result = subnet.result()
         result = sn_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -820,15 +818,15 @@
             resource_group_name=resource_group,
             virtual_network_name=virtual_network,
             subnet_name=name,
             polling=True,
         )
         subnet.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def virtual_networks_list_all(**kwargs):
     """
@@ -848,15 +846,15 @@
     try:
         vnets = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.virtual_networks.list_all()
         )
 
         for vnet in vnets:
             result[vnet["name"]] = vnet
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def virtual_networks_list(resource_group, **kwargs):
@@ -880,15 +878,15 @@
     try:
         vnets = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.virtual_networks.list(resource_group_name=resource_group)
         )
 
         for vnet in vnets:
             result[vnet["name"]] = vnet
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -950,15 +948,15 @@
             resource_group_name=resource_group,
             parameters=vnetmodel,
             polling=True,
         )
         vnet.wait()
         vnet_result = vnet.result()
         result = vnet_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -985,15 +983,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         vnet = netconn.virtual_networks.begin_delete(
             virtual_network_name=name, resource_group_name=resource_group, polling=True
         )
         vnet.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def virtual_network_get(name, resource_group, **kwargs):
     """
@@ -1015,15 +1013,15 @@
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         vnet = netconn.virtual_networks.get(
             virtual_network_name=name, resource_group_name=resource_group
         )
         result = vnet.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def load_balancers_list_all(**kwargs):
@@ -1044,15 +1042,15 @@
     try:
         load_balancers = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.load_balancers.list_all()
         )
 
         for load_balancer in load_balancers:
             result[load_balancer["name"]] = load_balancer
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def load_balancers_list(resource_group, **kwargs):
@@ -1076,15 +1074,15 @@
     try:
         load_balancers = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.load_balancers.list(resource_group_name=resource_group)
         )
 
         for load_balancer in load_balancers:
             result[load_balancer["name"]] = load_balancer
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def load_balancer_get(name, resource_group, **kwargs):
@@ -1107,15 +1105,15 @@
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         load_balancer = netconn.load_balancers.get(
             load_balancer_name=name, resource_group_name=resource_group
         )
         result = load_balancer.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def load_balancer_create_or_update(name, resource_group, **kwargs):
@@ -1279,15 +1277,15 @@
             load_balancer_name=name,
             parameters=lbmodel,
             polling=True,
         )
         load_balancer.wait()
         lb_result = load_balancer.result()
         result = lb_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -1314,15 +1312,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         load_balancer = netconn.load_balancers.begin_delete(
             load_balancer_name=name, resource_group_name=resource_group, polling=True
         )
         load_balancer.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def usages_list(location, **kwargs):
     """
@@ -1338,15 +1336,15 @@
 
         salt-call azurerm_network.usages_list westus
 
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         result = saltext.azurerm.utils.azurerm.paged_object_to_list(netconn.usages.list(location))
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def network_interface_delete(name, resource_group, **kwargs):
@@ -1372,15 +1370,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         nic = netconn.network_interfaces.begin_delete(
             network_interface_name=name, resource_group_name=resource_group, polling=True
         )
         nic.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def network_interface_get(name, resource_group, **kwargs):
     """
@@ -1402,15 +1400,15 @@
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         nic = netconn.network_interfaces.get(
             network_interface_name=name, resource_group_name=resource_group
         )
         result = nic.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -1511,15 +1509,15 @@
             network_interface_name=name,
             parameters=nicmodel,
             polling=True,
         )
         interface.wait()
         nic_result = interface.result()
         result = nic_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -1542,15 +1540,15 @@
     try:
         nics = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.network_interfaces.list_all()
         )
 
         for nic in nics:
             result[nic["name"]] = nic
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def network_interfaces_list(resource_group, **kwargs):
@@ -1574,15 +1572,15 @@
     try:
         nics = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.network_interfaces.list(resource_group_name=resource_group)
         )
 
         for nic in nics:
             result[nic["name"]] = nic
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -1602,22 +1600,22 @@
     .. code-block:: bash
 
         salt-call azurerm_network.network_interface_get_effective_route_table test-iface0 testgroup
 
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
-        nic = netconn.network_interfaces.get_effective_route_table(
+        nic = netconn.network_interfaces.begin_get_effective_route_table(
             network_interface_name=name, resource_group_name=resource_group
         )
         nic.wait()
         tables = nic.result()
         tables = tables.as_dict()
         result = tables["value"]
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -1637,22 +1635,22 @@
     .. code-block:: bash
 
         salt-call azurerm_network.network_interface_list_effective_network_security_groups test-iface0 testgroup
 
     """
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
-        nic = netconn.network_interfaces.list_effective_network_security_groups(
+        nic = netconn.network_interfaces.begin_list_effective_network_security_groups(
             network_interface_name=name, resource_group_name=resource_group
         )
         nic.wait()
         groups = nic.result()
         groups = groups.as_dict()
         result = groups["value"]
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -1687,15 +1685,15 @@
                 virtualmachine_index=vm_index,
                 resource_group_name=resource_group,
             )
         )
 
         for nic in nics:
             result[nic["name"]] = nic
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -1725,15 +1723,15 @@
                 virtual_machine_scale_set_name=scale_set,
                 resource_group_name=resource_group,
             )
         )
 
         for nic in nics:
             result[nic["name"]] = nic
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 # pylint: disable=invalid-name
@@ -1770,15 +1768,15 @@
             virtual_machine_scale_set_name=scale_set,
             virtualmachine_index=vm_index,
             resource_group_name=resource_group,
             exapnd=expand,
         )
 
         result = nic.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def public_ip_address_delete(name, resource_group, **kwargs):
@@ -1803,15 +1801,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         pub_ip = netconn.public_ip_addresses.begin_delete(
             public_ip_address_name=name, resource_group_name=resource_group, polling=True
         )
         pub_ip.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def public_ip_address_get(name, resource_group, **kwargs):
     """
@@ -1838,15 +1836,15 @@
     try:
         pub_ip = netconn.public_ip_addresses.get(
             public_ip_address_name=name,
             resource_group_name=resource_group,
             expand=expand,
         )
         result = pub_ip.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def public_ip_address_create_or_update(name, resource_group, **kwargs):
@@ -1891,15 +1889,15 @@
             public_ip_address_name=name,
             parameters=pub_ip_model,
             polling=True,
         )
         ip.wait()
         ip_result = ip.result()
         result = ip_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -1922,15 +1920,15 @@
     try:
         pub_ips = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.public_ip_addresses.list_all()
         )
 
         for ip in pub_ips:
             result[ip["name"]] = ip
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def public_ip_addresses_list(resource_group, **kwargs):
@@ -1954,15 +1952,15 @@
     try:
         pub_ips = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.public_ip_addresses.list(resource_group_name=resource_group)
         )
 
         for ip in pub_ips:
             result[ip["name"]] = ip
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_filter_rule_delete(name, route_filter, resource_group, **kwargs):
@@ -1991,15 +1989,15 @@
         rule = netconn.route_filter_rules.delete(
             resource_group_name=resource_group,
             route_filter_name=route_filter,
             rule_name=name,
         )
         rule.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def route_filter_rule_get(name, route_filter, resource_group, **kwargs):
     """
@@ -2027,15 +2025,15 @@
         rule = netconn.route_filter_rules.get(
             resource_group_name=resource_group,
             route_filter_name=route_filter,
             rule_name=name,
         )
 
         result = rule.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_filter_rule_create_or_update(
@@ -2093,15 +2091,15 @@
             route_filter_name=route_filter,
             rule_name=name,
             route_filter_rule_parameters=rule_model,
         )
         rule.wait()
         rule_result = rule.result()
         result = rule_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         message = str(exc)
         if kwargs.get("subscription_id") == str(message).strip():
             message = "Subscription not authorized for this operation!"
         saltext.azurerm.utils.azurerm.log_cloud_error("network", message, **kwargs)
         result = {"error": message}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
@@ -2134,15 +2132,15 @@
             netconn.route_filter_rules.list_by_route_filter(
                 resource_group_name=resource_group, route_filter_name=route_filter
             )
         )
 
         for rule in rules:
             result[rule["name"]] = rule
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_filter_delete(name, resource_group, **kwargs):
@@ -2167,15 +2165,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         route_filter = netconn.route_filters.delete(
             route_filter_name=name, resource_group_name=resource_group
         )
         route_filter.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def route_filter_get(name, resource_group, **kwargs):
     """
@@ -2200,15 +2198,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         route_filter = netconn.route_filters.get(
             route_filter_name=name, resource_group_name=resource_group, expand=expand
         )
         result = route_filter.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_filter_create_or_update(name, resource_group, **kwargs):
@@ -2252,15 +2250,15 @@
             resource_group_name=resource_group,
             route_filter_name=name,
             route_filter_parameters=rt_filter_model,
         )
         rt_filter.wait()
         rt_result = rt_filter.result()
         result = rt_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -2286,15 +2284,15 @@
     try:
         filters = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.route_filters.list_by_resource_group(resource_group_name=resource_group)
         )
 
         for route_filter in filters:
             result[route_filter["name"]] = route_filter
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_filters_list_all(**kwargs):
@@ -2313,15 +2311,15 @@
     result = {}
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         filters = saltext.azurerm.utils.azurerm.paged_object_to_list(netconn.route_filters.list())
 
         for route_filter in filters:
             result[route_filter["name"]] = route_filter
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_delete(name, route_table, resource_group, **kwargs):
@@ -2351,15 +2349,15 @@
             resource_group_name=resource_group,
             route_table_name=route_table,
             route_name=name,
             polling=True,
         )
         route.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def route_get(name, route_table, resource_group, **kwargs):
     """
@@ -2387,15 +2385,15 @@
         route = netconn.routes.get(
             resource_group_name=resource_group,
             route_table_name=route_table,
             route_name=name,
         )
 
         result = route.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_create_or_update(
@@ -2446,24 +2444,24 @@
             **kwargs
         )
     except TypeError as exc:
         result = {"error": "The object model could not be built. ({})".format(str(exc))}
         return result
 
     try:
-        route = netconn.routes.create_or_update(
+        route = netconn.routes.begin_create_or_update(
             resource_group_name=resource_group,
             route_table_name=route_table,
             route_name=name,
             route_parameters=rt_model,
         )
         route.wait()
         rt_result = route.result()
         result = rt_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -2491,15 +2489,15 @@
     try:
         routes = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.routes.list(resource_group_name=resource_group, route_table_name=route_table)
         )
 
         for route in routes:
             result[route["name"]] = route
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_table_delete(name, resource_group, **kwargs):
@@ -2524,15 +2522,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         table = netconn.route_tables.begin_delete(
             route_table_name=name, resource_group_name=resource_group, polling=True
         )
         table.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
 
     return result
 
 
 def route_table_get(name, resource_group, **kwargs):
     """
@@ -2557,15 +2555,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         table = netconn.route_tables.get(
             route_table_name=name, resource_group_name=resource_group, expand=expand
         )
         result = table.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_table_create_or_update(name, resource_group, **kwargs):
@@ -2610,15 +2608,15 @@
             route_table_name=name,
             parameters=rt_tbl_model,
             polling=True,
         )
         table.wait()
         tbl_result = table.result()
         result = tbl_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -2644,15 +2642,15 @@
     try:
         tables = saltext.azurerm.utils.azurerm.paged_object_to_list(
             netconn.route_tables.list(resource_group_name=resource_group)
         )
 
         for table in tables:
             result[table["name"]] = table
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def route_tables_list_all(**kwargs):
@@ -2671,12 +2669,12 @@
     result = {}
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
     try:
         tables = saltext.azurerm.utils.azurerm.paged_object_to_list(netconn.route_tables.list_all())
 
         for table in tables:
             result[table["name"]] = table
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
```

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/modules/azurerm_resource.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/modules/azurerm_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,15 @@
 import salt.utils.json  # pylint: disable=import-error
 import saltext.azurerm.utils.azurerm
 
 # Azure libs
 HAS_LIBS = False
 try:
     import azure.mgmt.resource.resources.models  # pylint: disable=unused-import
-    from msrest.exceptions import SerializationError
-    from msrestazure.azure_exceptions import CloudError
-    from azure.core.exceptions import ResourceNotFoundError
+    from azure.core.exceptions import ResourceNotFoundError, HttpResponseError, SerializationError
 
     HAS_LIBS = True
 except ImportError:
     pass
 
 __virtualname__ = "azurerm_resource"
 
@@ -86,15 +84,15 @@
     result = {}
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         groups = saltext.azurerm.utils.azurerm.paged_object_to_list(resconn.resource_groups.list())
 
         for group in groups:
             result[group["name"]] = group
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def resource_group_check_existence(name, **kwargs):
@@ -113,15 +111,15 @@
 
     """
     result = False
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         result = resconn.resource_groups.check_existence(name)
 
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
 
     return result
 
 
 def resource_group_get(name, **kwargs):
     """
@@ -140,15 +138,15 @@
     """
     result = {}
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         group = resconn.resource_groups.get(name)
         result = group.as_dict()
 
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def resource_group_create_or_update(name, location, **kwargs):  # pylint: disable=invalid-name
@@ -175,15 +173,15 @@
         "location": location,
         "managed_by": kwargs.get("managed_by"),
         "tags": kwargs.get("tags"),
     }
     try:
         group = resconn.resource_groups.create_or_update(name, resource_group_params)
         result = group.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def resource_group_delete(name, **kwargs):
@@ -203,15 +201,15 @@
     """
     result = False
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         group = resconn.resource_groups.begin_delete(name, polling=True)
         group.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
 
     return result
 
 
 def deployment_operation_get(operation, deployment, resource_group, **kwargs):
     """
@@ -238,15 +236,15 @@
         operation = resconn.deployment_operations.get(
             resource_group_name=resource_group,
             deployment_name=deployment,
             operation_id=operation,
         )
 
         result = operation.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def deployment_operations_list(name, resource_group, result_limit=10, **kwargs):
@@ -279,15 +277,15 @@
                 deployment_name=name,
                 top=result_limit,
             )
         )
 
         for oper in operations:
             result[oper["operation_id"]] = oper
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def deployment_delete(name, resource_group, **kwargs):
@@ -312,15 +310,15 @@
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         deploy = resconn.deployments.delete(
             deployment_name=name, resource_group_name=resource_group
         )
         deploy.wait()
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
 
     return result
 
 
 def deployment_check_existence(name, resource_group, **kwargs):
     """
@@ -342,15 +340,15 @@
     """
     result = False
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         result = resconn.deployments.check_existence(
             deployment_name=name, resource_group_name=resource_group
         )
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
 
     return result
 
 
 def deployment_create_or_update(
     name,
@@ -508,15 +506,15 @@
                 deployment_name=name,
                 resource_group_name=resource_group,
                 parameters={"properties": deploy_model},
             )
             deploy.wait()
             deploy_result = deploy.result()
             result = deploy_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -539,15 +537,15 @@
         salt-call azurerm_resource.deployment_get testdeploy testgroup
 
     """
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         deploy = resconn.deployments.get(deployment_name=name, resource_group_name=resource_group)
         result = deploy.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def deployment_cancel(name, resource_group, **kwargs):
@@ -568,15 +566,15 @@
         salt-call azurerm_resource.deployment_cancel testdeploy testgroup
 
     """
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         resconn.deployments.cancel(deployment_name=name, resource_group_name=resource_group)
         result = {"result": True}
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc), "result": False}
 
     return result
 
 
 def deployment_validate(
@@ -679,15 +677,15 @@
             deployment_name=name,
             resource_group_name=resource_group,
             parameters={"properties": deploy_model},
         )
         deploy.wait()
         deploy_result = deploy.result()
         result = deploy_result.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -712,15 +710,15 @@
     """
     resconn = saltext.azurerm.utils.azurerm.get_client("resource", **kwargs)
     try:
         deploy = resconn.deployments.export_template(
             deployment_name=name, resource_group_name=resource_group
         )
         result = deploy.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def deployments_list(resource_group, **kwargs):
@@ -741,15 +739,15 @@
     try:
         deployments = saltext.azurerm.utils.azurerm.paged_object_to_list(
             resconn.deployments.list_by_resource_group(resource_group_name=resource_group)
         )
 
         for deploy in deployments:
             result[deploy["name"]] = deploy
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def subscriptions_list_locations(subscription_id=None, **kwargs):
@@ -778,15 +776,15 @@
     try:
         locations = saltext.azurerm.utils.azurerm.paged_object_to_list(
             subconn.subscriptions.list_locations(subscription_id=kwargs["subscription_id"])
         )
 
         for loc in locations:
             result[loc["name"]] = loc
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def subscription_get(subscription_id=None, **kwargs):
@@ -812,15 +810,15 @@
         kwargs["subscription_id"] = subscription_id
 
     subconn = saltext.azurerm.utils.azurerm.get_client("subscription", **kwargs)
     try:
         subscription = subconn.subscriptions.get(subscription_id=kwargs.get("subscription_id"))
 
         result = subscription.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def subscriptions_list(**kwargs):
@@ -839,15 +837,15 @@
     result = {}
     subconn = saltext.azurerm.utils.azurerm.get_client("subscription", **kwargs)
     try:
         subs = saltext.azurerm.utils.azurerm.paged_object_to_list(subconn.subscriptions.list())
 
         for sub in subs:
             result[sub["subscription_id"]] = sub
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def tenants_list(**kwargs):
@@ -866,15 +864,15 @@
     result = {}
     subconn = saltext.azurerm.utils.azurerm.get_client("subscription", **kwargs)
     try:
         tenants = saltext.azurerm.utils.azurerm.paged_object_to_list(subconn.tenants.list())
 
         for tenant in tenants:
             result[tenant["tenant_id"]] = tenant
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def policy_assignment_delete(name, scope, **kwargs):
@@ -897,15 +895,15 @@
     """
     result = False
     polconn = saltext.azurerm.utils.azurerm.get_client("policy", **kwargs)
     try:
         # pylint: disable=unused-variable
         policy = polconn.policy_assignments.delete(policy_assignment_name=name, scope=scope)
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
 
     return result
 
 
 def policy_assignment_create(name, scope, definition_name, **kwargs):
     """
@@ -966,15 +964,15 @@
             return result
 
         try:
             policy = polconn.policy_assignments.create(
                 scope=scope, policy_assignment_name=name, parameters=policy_model
             )
             result = policy.as_dict()
-        except CloudError as exc:
+        except HttpResponseError as exc:
             saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
             result = {"error": str(exc)}
         except SerializationError as exc:
             result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
     else:
         result = {
             "error": 'The policy definition named "{}" could not be found.'.format(definition_name)
@@ -1001,15 +999,15 @@
         /subscriptions/bc75htn-a0fhsi-349b-56gh-4fghti-f84852
 
     """
     polconn = saltext.azurerm.utils.azurerm.get_client("policy", **kwargs)
     try:
         policy = polconn.policy_assignments.get(policy_assignment_name=name, scope=scope)
         result = policy.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def policy_assignments_list_for_resource_group(
@@ -1036,15 +1034,15 @@
             polconn.policy_assignments.list_for_resource_group(
                 resource_group_name=resource_group, filter=kwargs.get("filter")
             )
         )
 
         for assign in policy_assign:
             result[assign["name"]] = assign
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def policy_assignments_list(**kwargs):
@@ -1065,15 +1063,15 @@
     try:
         policy_assign = saltext.azurerm.utils.azurerm.paged_object_to_list(
             polconn.policy_assignments.list()
         )
 
         for assign in policy_assign:
             result[assign["name"]] = assign
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def policy_definition_create_or_update(name, policy_rule, **kwargs):  # pylint: disable=invalid-name
@@ -1115,15 +1113,15 @@
         return result
 
     try:
         policy = polconn.policy_definitions.create_or_update(
             policy_definition_name=name, parameters=policy_model
         )
         result = policy.as_dict()
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
         result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
 
     return result
 
@@ -1145,15 +1143,15 @@
     """
     result = False
     polconn = saltext.azurerm.utils.azurerm.get_client("policy", **kwargs)
     try:
         # pylint: disable=unused-variable
         policy = polconn.policy_definitions.delete(policy_definition_name=name)
         result = True
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
 
     return result
 
 
 def policy_definition_get(name, **kwargs):
     """
@@ -1170,15 +1168,15 @@
         salt-call azurerm_resource.policy_definition_get testpolicy
 
     """
     polconn = saltext.azurerm.utils.azurerm.get_client("policy", **kwargs)
     try:
         policy_def = polconn.policy_definitions.get(policy_definition_name=name)
         result = policy_def.as_dict()
-    except ResourceNotFoundError as exc:
+    except (ResourceNotFoundError, HttpResponseError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
 
 
 def policy_definitions_list(hide_builtin=False, **kwargs):
@@ -1202,12 +1200,12 @@
         policy_defs = saltext.azurerm.utils.azurerm.paged_object_to_list(
             polconn.policy_definitions.list()
         )
 
         for policy in policy_defs:
             if not (hide_builtin and policy["policy_type"] == "BuiltIn"):
                 result[policy["name"]] = policy
-    except CloudError as exc:
+    except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
 
     return result
```

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_compute.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_compute_availability_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-Azure Resource Manager Compute State Module
+Azure Resource Manager Compute Availability Set State Module
 
-.. versionadded:: 2019.2.0
+.. versionadded:: 2.1.0
 
 :maintainer: <devops@eitr.tech>
 :maturity: new
 :platform: linux
 
 :configuration: This module requires Azure Resource Manager credentials to be passed as a dictionary of
     keyword arguments to the ``connection_auth`` parameter in order to work properly. Since the authentication
@@ -20,95 +20,75 @@
 
     if using a service principal:
       * ``subscription_id``
       * ``tenant``
       * ``client_id``
       * ``secret``
 
+    if using managed identity:
+      * ``subscription_id``
+
     Optional provider parameters:
 
-    **cloud_environment**:
-      Used to point the cloud driver to different API endpoints, such as Azure GovCloud. Possible values:
+    **cloud_environment**: Used to point the cloud driver to different API endpoints, such as Azure GovCloud.
+
+        Possible values:
         * ``AZURE_PUBLIC_CLOUD`` (default)
         * ``AZURE_CHINA_CLOUD``
         * ``AZURE_US_GOV_CLOUD``
         * ``AZURE_GERMAN_CLOUD``
 
-    Example Pillar for Azure Resource Manager authentication:
+    Example acct setup for Azure Resource Manager authentication:
 
     .. code-block:: yaml
 
         azurerm:
-            user_pass_auth:
-                subscription_id: 3287abc8-f98a-c678-3bde-326766fd3617
-                username: fletch
-                password: 123pass
-            mysubscription:
+            default:
                 subscription_id: 3287abc8-f98a-c678-3bde-326766fd3617
                 tenant: ABCDEFAB-1234-ABCD-1234-ABCDEFABCDEF
                 client_id: ABCDEFAB-1234-ABCD-1234-ABCDEFABCDEF
                 secret: XXXXXXXXXXXXXXXXXXXXXXXX
                 cloud_environment: AZURE_PUBLIC_CLOUD
+            user_pass_auth:
+                subscription_id: 3287abc8-f98a-c678-3bde-326766fd3617
+                username: fletch
+                password: 123pass
 
-    Example states using Azure Resource Manager authentication:
-
-    .. code-block:: jinja
-
-        {% set profile = salt['pillar.get']('azurerm:mysubscription') %}
-        Ensure availability set exists:
-            azurerm_compute.availability_set_present:
-                - name: my_avail_set
-                - resource_group: my_rg
-                - virtual_machines:
-                    - my_vm1
-                    - my_vm2
-                - tags:
-                    how_awesome: very
-                    contact_name: Elmer Fudd Gantry
-                - connection_auth: {{ profile }}
-
-        Ensure availability set is absent:
-            azurerm_compute.availability_set_absent:
-                - name: other_avail_set
-                - resource_group: my_rg
-                - connection_auth: {{ profile }}
 
 """
 # Python libs
 import logging
 
 import salt.utils.dictdiffer  # pylint: disable=import-error
 
-__virtualname__ = "azurerm_compute"
-
 log = logging.getLogger(__name__)
 
 
 def __virtual__():
     """
     Only make this state available if the azurerm_compute module is available.
     """
-    if "azurerm_compute.availability_set_create_or_update" in __salt__:
-        return __virtualname__
+    if "azurerm_compute_availability_set.create_or_update" in __salt__:
+        return True
     return (False, "azurerm module could not be loaded")
 
 
-def availability_set_present(
+def present(
     name,
     resource_group,
     tags=None,
     platform_update_domain_count=None,
     platform_fault_domain_count=None,
     virtual_machines=None,
     sku=None,
     connection_auth=None,
     **kwargs
 ):
     """
-    .. versionadded:: 2019.2.0
+    .. versionadded:: 2.1.0
 
     Ensure an availability set exists.
 
     :param name:
         Name of the availability set.
 
     :param resource_group:
@@ -159,15 +139,15 @@
     if not isinstance(connection_auth, dict):
         ret["comment"] = "Connection information must be specified via connection_auth dictionary!"
         return ret
 
     if sku:
         sku = {"name": sku.capitalize()}
 
-    aset = __salt__["azurerm_compute.availability_set_get"](
+    aset = __salt__["azurerm_compute_availability_set.get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" not in aset:
         tag_changes = salt.utils.dictdiffer.deep_diff(aset.get("tags", {}), tags or {})
         if tag_changes:
             ret["changes"]["tags"] = tag_changes
@@ -233,15 +213,15 @@
         ret["comment"] = "Availability set {} would be created.".format(name)
         ret["result"] = None
         return ret
 
     aset_kwargs = kwargs.copy()
     aset_kwargs.update(connection_auth)
 
-    aset = __salt__["azurerm_compute.availability_set_create_or_update"](
+    aset = __salt__["azurerm_compute_availability_set.create_or_update"](
         name=name,
         resource_group=resource_group,
         virtual_machines=virtual_machines,
         platform_update_domain_count=platform_update_domain_count,
         platform_fault_domain_count=platform_fault_domain_count,
         sku=sku,
         tags=tags,
@@ -253,15 +233,15 @@
         ret["comment"] = "Availability set {} has been created.".format(name)
         return ret
 
     ret["comment"] = "Failed to create availability set {}! ({})".format(name, aset.get("error"))
     return ret
 
 
-def availability_set_absent(name, resource_group, connection_auth=None):
+def absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
     Ensure an availability set does not exist in a resource group.
 
     :param name:
         Name of the availability set.
@@ -275,15 +255,15 @@
     """
     ret = {"name": name, "result": False, "comment": "", "changes": {}}
 
     if not isinstance(connection_auth, dict):
         ret["comment"] = "Connection information must be specified via connection_auth dictionary!"
         return ret
 
-    aset = __salt__["azurerm_compute.availability_set_get"](
+    aset = __salt__["azurerm_compute_availability_set.get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in aset:
         ret["result"] = True
         ret["comment"] = "Availability set {} was not found.".format(name)
         return ret
@@ -293,15 +273,15 @@
         ret["result"] = None
         ret["changes"] = {
             "old": aset,
             "new": {},
         }
         return ret
 
-    deleted = __salt__["azurerm_compute.availability_set_delete"](
+    deleted = __salt__["azurerm_compute_availability_set.delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
         ret["comment"] = "Availability set {} has been deleted.".format(name)
         ret["changes"] = {"old": aset, "new": {}}
```

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_dns.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_dns.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_network.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_network.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/states/azurerm_resource.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/states/azurerm_resource.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-2.0.2/src/saltext/azurerm/utils/azurerm.py` & `saltext.azurerm-3.0.0/src/saltext/azurerm/utils/azurerm.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,30 +17,32 @@
     * `azure-storage <https://pypi.python.org/pypi/azure-storage>`_ >= 0.37.0
     * `msrestazure <https://pypi.python.org/pypi/msrestazure>`_ >= 0.6.4
 :platform: linux
 
 """
 import importlib
 import logging
+import os
 import sys
 from operator import itemgetter
 
 import salt.config  # pylint: disable=import-error
 import salt.loader  # pylint: disable=import-error
 import salt.utils.stringutils  # pylint: disable=import-error
 import salt.version  # pylint: disable=import-error
 from salt.exceptions import SaltInvocationError  # pylint: disable=import-error
 from salt.exceptions import SaltSystemExit  # pylint: disable=import-error
 
 try:
     from azure.identity import (
-        ClientSecretCredential,
-        UsernamePasswordCredential,
+        AzureAuthorityHosts,
         DefaultAzureCredential,
+        KnownAuthorities,
     )
+    from azure.core.exceptions import ClientAuthenticationError
     from msrestazure.azure_cloud import (
         MetadataEndpointError,
         get_cloud_from_metadata_endpoint,
     )
     from azure.core.pipeline.policies import UserAgentPolicy
 
     HAS_AZURE = True
@@ -60,131 +62,109 @@
         return True
 
 
 def _determine_auth(**kwargs):
     """
     Acquire Azure Resource Manager Credentials
     """
+    mrest_cloud_name = {
+        "AZURE_CHINA": "AZURE_CHINA_CLOUD",
+        "AZURE_GOVERNMENT": "AZURE_US_GOV_CLOUD",
+        "AZURE_GERMANY": "AZURE_GERMAN_CLOUD",
+    }
     if "profile" in kwargs:
         azure_credentials = __salt__["config.option"](kwargs["profile"])
         kwargs.update(azure_credentials)
 
-    service_principal_creds_kwargs = ["client_id", "secret", "tenant"]
-    user_pass_creds_kwargs = ["username", "password"]
-
     try:
-        if kwargs.get("cloud_environment") and kwargs.get("cloud_environment").startswith("http"):
+        if kwargs.get("cloud_environment", "").startswith("http"):
             cloud_env = get_cloud_from_metadata_endpoint(kwargs["cloud_environment"])
+            authority = kwargs["cloud_environment"]
         else:
             cloud_env_module = importlib.import_module("msrestazure.azure_cloud")
-            cloud_env = getattr(
-                cloud_env_module, kwargs.get("cloud_environment", "AZURE_PUBLIC_CLOUD")
-            )
-    except (AttributeError, ImportError, MetadataEndpointError):
-        raise sys.exit(  # pylint: disable=raise-missing-from
-            "The Azure cloud environment {} is not available.".format(kwargs["cloud_environment"])
-        )
 
-    if set(service_principal_creds_kwargs).issubset(kwargs):
-        if not (kwargs["client_id"] and kwargs["secret"] and kwargs["tenant"]):
-            raise SaltInvocationError(
-                "The client_id, secret, and tenant parameters must all be "
-                "populated if using service principals."
-            )
-        else:
-            credentials = ClientSecretCredential(
-                tenant_id=kwargs["tenant"],
-                client_id=kwargs["client_id"],
-                client_secret=kwargs["secret"],
-                cloud_environment=cloud_env,
+            # Map the new cloud_environment name to the corresponding old msrest name
+            old_cloud_env_name = mrest_cloud_name.get(
+                kwargs.get("cloud_environment", "AZURE_PUBLIC_CLOUD"), "AZURE_PUBLIC_CLOUD"
             )
-    elif set(user_pass_creds_kwargs).issubset(kwargs):
-        if not (kwargs["username"] and kwargs["password"]):
-            raise SaltInvocationError(
-                "The username and password parameters must both be "
-                "populated if using username/password authentication."
-            )
-        else:
-            credentials = UsernamePasswordCredential(
-                client_id=kwargs["client_id"],
-                username=kwargs["username"],
-                password=kwargs["password"],
-                cloud_environment=cloud_env,
-            )
-    elif "subscription_id" in kwargs:
-        try:
-            credentials = DefaultAzureCredential(cloud_environment=cloud_env)
-        except ImportError:
-            raise SaltSystemExit(  # pylint: disable=raise-missing-from
-                msg=("MSI authentication support not availabe (requires msrestazure >=" " 0.4.14)")
+
+            # Retrieve the cloud environment based on the old msrest name
+            cloud_env = getattr(cloud_env_module, old_cloud_env_name)
+
+            authority = getattr(
+                AzureAuthorityHosts, kwargs.get("cloud_environment", "AZURE_PUBLIC_CLOUD")
             )
+    except (AttributeError, ImportError, MetadataEndpointError):
+        raise SaltSystemExit(  # pylint: disable=raise-missing-from
+            f"The Azure cloud environment {kwargs['cloud_environment']} is not available."
+        )
 
-    else:
-        raise SaltInvocationError(
+    try:
+        credentials = DefaultAzureCredential(authority=authority, **kwargs)
+    except ClientAuthenticationError:
+        raise SaltInvocationError(  # pylint: disable=raise-missing-from
             "Unable to determine credentials. "
             "A subscription_id with username and password, "
             "or client_id, secret, and tenant or a profile with the "
             "required parameters populated"
         )
-
-    if "subscription_id" not in kwargs:
-        raise SaltInvocationError("A subscription_id must be specified")
-
-    subscription_id = salt.utils.stringutils.to_str(kwargs["subscription_id"])
+    try:
+        subscription_id = salt.utils.stringutils.to_str(kwargs["subscription_id"])
+    except KeyError:
+        raise SaltInvocationError(  # pylint: disable=raise-missing-from
+            "A subscription_id must be specified"
+        )
 
     return credentials, subscription_id, cloud_env
 
 
 def get_client(client_type, **kwargs):
     """
     Dynamically load the selected client and return a management client object
     """
     client_map = {
         "compute": "ComputeManagement",
         "authorization": "AuthorizationManagement",
         "dns": "DnsManagement",
+        "keyvault": "KeyVaultManagement",
         "storage": "StorageManagement",
         "managementlock": "ManagementLock",
         "monitor": "MonitorManagement",
         "network": "NetworkManagement",
         "policy": "Policy",
         "privatedns": "PrivateDnsManagement",
         "resource": "ResourceManagement",
         "subscription": "Subscription",
         "web": "WebSiteManagement",
     }
 
     if client_type not in client_map:
         raise SaltSystemExit(
-            msg="The Azure Resource Manager client_type {} specified can not be found.".format(
-                client_type
-            )
+            msg=f"The Azure Resource Manager client_type {client_type} specified can not be found."
         )
 
     map_value = client_map[client_type]
 
     if client_type in ["policy", "subscription"]:
         module_name = "resource"
     elif client_type in ["managementlock"]:
         module_name = "resource.locks"
     else:
         module_name = client_type
 
     try:
         client_module = importlib.import_module("azure.mgmt." + module_name)
-        # pylint: disable=invalid-name
-        Client = getattr(client_module, "{}Client".format(map_value))
+        Client = getattr(client_module, f"{map_value}Client")  # pylint: disable=invalid-name
     except ImportError:
-        raise sys.exit(  # pylint: disable=raise-missing-from
-            "The azure {} client is not available.".format(client_type)
-        )  # pylint: disable=raise-missing-from
-
+        raise SaltSystemExit(  # pylint: disable=raise-missing-from
+            f"The azure {client_type} client is not available."
+        )
     credentials, subscription_id, cloud_env = _determine_auth(**kwargs)
 
-    user_agent = UserAgentPolicy("Salt/{}".format(salt.version.__version__))
+    user_agent = UserAgentPolicy(f"Salt/{salt.version.__version__}")
     if client_type == "subscription":
         client = Client(
             credential=credentials,
             base_url=cloud_env.endpoints.resource_manager,
             user_agent_policy=user_agent,
         )
     else:
@@ -260,15 +240,15 @@
                         if items["type"][1].isupper() and isinstance(list_item, dict):
                             obj_list.append(
                                 create_object_model(
                                     module_name,
                                     items["type"][
                                         items["type"].index("[") + 1 : items["type"].rindex("]")
                                     ],
-                                    **list_item
+                                    **list_item,
                                 )
                             )
                         elif items["type"][1] == "{" and isinstance(list_item, dict):
                             obj_list.append(list_item)
                         elif not items["type"][1].isupper() and items["type"][1] != "{":
                             obj_list.append(list_item)
                     object_kwargs[attr] = obj_list
@@ -323,7 +303,48 @@
                 if isinstance(remote_val, str):
                     remote_val = remote_val.lower()
             if local_val != remote_val:
                 ret["changes"] = {"old": remote_configs, "new": local_configs}
                 return ret
 
     return ret
+
+
+def get_identity_credentials(**kwargs):
+    """
+    Acquire Azure RM Credentials from the identity provider (not for mgmt)
+
+    This is accessible on the hub so clients out in the code can use it. Non-management clients
+    can't be consolidated neatly here.
+
+    We basically set environment variables based upon incoming parameters and then pass off to
+    the DefaultAzureCredential object to correctly parse those environment variables. See the
+    `Microsoft Docs on EnvironmentCredential <https://aka.ms/azsdk-python-identity-default-cred-ref>`_
+    for more information.
+    """
+    kwarg_map = {
+        "tenant": "AZURE_TENANT_ID",
+        "client_id": "AZURE_CLIENT_ID",
+        "secret": "AZURE_CLIENT_SECRET",
+        "client_certificate_path": "AZURE_CLIENT_CERTIFICATE_PATH",
+        "username": "AZURE_USERNAME",
+        "password": "AZURE_PASSWORD",
+    }
+    for keyword, value in kwarg_map.items():
+        if kwargs.get(keyword):
+            os.environ[value] = kwargs[keyword]
+
+    try:
+        if kwargs.get("cloud_environment") and kwargs.get("cloud_environment").startswith("http"):
+            authority = kwargs["cloud_environment"]
+        else:
+            authority = getattr(
+                KnownAuthorities, kwargs.get("cloud_environment", "AZURE_PUBLIC_CLOUD")
+            )
+        log.debug("AUTHORITY: %s", authority)
+    except AttributeError as exc:
+        log.error('Unknown authority presented for "cloud_environment": %s', exc)
+        authority = KnownAuthorities.AZURE_PUBLIC_CLOUD
+
+    credential = DefaultAzureCredential(authority=authority)
+
+    return credential
```

### Comparing `saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/PKG-INFO` & `saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.azurerm
-Version: 2.0.2
+Version: 3.0.0
 Summary: Salt Extension Modules for Azure Resource Manager
 Home-page: https://github.com/salt-extensions/saltext-azurerm
 Author: EITR Technologies, LLC
 Author-email: devops@eitr.tech
 License: Apache Software License
 Project-URL: Source, https://github.com/salt-extensions/saltext-azurerm
 Project-URL: Tracker, https://github.com/salt-extensions/saltext-azurerm/issues
```

### Comparing `saltext.azurerm-2.0.2/src/saltext.azurerm.egg-info/requires.txt` & `saltext.azurerm-3.0.0/src/saltext.azurerm.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 azure-identity==1.10.0
 azure-core==1.24.2
 azure-mgmt-authorization==2.0.0
 azure-mgmt-batch==16.2.0
 azure-mgmt-compute==27.1.0
 azure-mgmt-dns==8.0.0
 azure-mgmt-privatedns==1.0.0
-azure-mgmt-keyvault==10.0.0
+azure-mgmt-keyvault==10.1.0
+azure-mgmt-monitor==6.0.1
 azure-mgmt-msi==6.0.1
 azure-mgmt-network==20.0.0
 azure-mgmt-resource==21.1.0
+azure-mgmt-storage==21.0.0
 azure-mgmt-subscription==3.0.0
 azure-mgmt-web==6.1.0
 azure-storage-blob==12.12.0
 azure-storage-common==2.1.0
 azure-storage-file==2.1.0
 azure-storage-nspkg==3.1.0
 azure-storage-queue==12.3.0
@@ -44,9 +46,10 @@
 [release]
 twine
 wheel
 
 [tests]
 mock>=3.0.5
 pytest>=7.2.0
-pytest-salt-factories>=1.0.0rc21
+pytest-salt-factories>=1.0.0rc23
+pytest-ordering
 Jinja2
```

### Comparing `saltext.azurerm-2.0.2/tests/conftest.py` & `saltext.azurerm-3.0.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @pytest.fixture(scope="session")
 def salt_factories_config():
     """
     Return a dictionary with the keyword arguments for FactoriesManager
     """
     return {
         "code_dir": str(PACKAGE_ROOT),
-        "inject_coverage": "COVERAGE_PROCESS_START" in os.environ,
         "inject_sitecustomize": "COVERAGE_PROCESS_START" in os.environ,
         "start_timeout": 120 if os.environ.get("CI") else 60,
     }
 
 
 @pytest.fixture(scope="package")
 def master(salt_factories):
```

