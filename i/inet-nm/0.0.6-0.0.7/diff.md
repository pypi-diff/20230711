# Comparing `tmp/inet-nm-0.0.6.tar.gz` & `tmp/inet-nm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inet-nm-0.0.6.tar", last modified: Mon Jul 10 10:27:27 2023, max compression
+gzip compressed data, was "inet-nm-0.0.7.tar", last modified: Tue Jul 11 13:25:19 2023, max compression
```

## Comparing `inet-nm-0.0.6.tar` & `inet-nm-0.0.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.465934 inet-nm-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 10:26:50.000000 inet-nm-0.0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-10 10:26:50.000000 inet-nm-0.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-07-10 10:26:50.000000 inet-nm-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 10:26:50.000000 inet-nm-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-10 10:27:27.477934 inet-nm-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-10 10:26:50.000000 inet-nm-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/cli-example.md
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 10:26:50.000000 inet-nm-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 10:26:50.000000 inet-nm-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-10 10:27:27.477934 inet-nm-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 10:26:50.000000 inet-nm-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/src/inet_nm/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_commission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_tmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_tty_from_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_update_commissioned.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_update_from_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/commissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/runner_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/src/inet_nm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_comissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_example_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.442342 inet-nm-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-11 13:24:38.000000 inet-nm-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.402342 inet-nm-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.414342 inet-nm-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-11 13:24:38.000000 inet-nm-0.0.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-11 13:24:38.000000 inet-nm-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 13:24:38.000000 inet-nm-0.0.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-11 13:24:38.000000 inet-nm-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-11 13:24:38.000000 inet-nm-0.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 13:24:38.000000 inet-nm-0.0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-11 13:24:38.000000 inet-nm-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-07-11 13:24:38.000000 inet-nm-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-11 13:24:38.000000 inet-nm-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-11 13:25:19.442342 inet-nm-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-11 13:24:38.000000 inet-nm-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.422342 inet-nm-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.422342 inet-nm-0.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/cli-example.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 13:24:38.000000 inet-nm-0.0.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 13:24:38.000000 inet-nm-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 13:24:38.000000 inet-nm-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-11 13:25:19.442342 inet-nm-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-11 13:24:38.000000 inet-nm-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.406342 inet-nm-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.430342 inet-nm-0.0.7/src/inet_nm/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_commission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_tmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_tty_from_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_update_commissioned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/cli_update_from_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/commissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-11 13:24:38.000000 inet-nm-0.0.7/src/inet_nm/runner_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.434342 inet-nm-0.0.7/src/inet_nm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 13:25:19.000000 inet-nm-0.0.7/src/inet_nm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:25:19.442342 inet-nm-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_comissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_example_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tests/test_runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-11 13:24:38.000000 inet-nm-0.0.7/tox.ini
```

### Comparing `inet-nm-0.0.6/.coveragerc` & `inet-nm-0.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/.github/workflows/ci.yml` & `inet-nm-0.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/.gitignore` & `inet-nm-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/.pre-commit-config.yaml` & `inet-nm-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/.readthedocs.yml` & `inet-nm-0.0.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/CHANGELOG.md` & `inet-nm-0.0.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/CONTRIBUTING.md` & `inet-nm-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/LICENSE.txt` & `inet-nm-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/PKG-INFO` & `inet-nm-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.6
+Version: 0.0.7
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
```

### Comparing `inet-nm-0.0.6/README.md` & `inet-nm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/docs/Makefile` & `inet-nm-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/docs/cli-example.md` & `inet-nm-0.0.7/docs/cli-example.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,62 +9,63 @@
 0. Let's just create a `board_info` list with some features...
 We can override the default args to just echo directly.
 ```bash
 $ inet-nm-update-from-os . --board-info "echo board_1 board_2" --board-features "echo feature_common feature_${BOARD}"
 Getting features_provided for board_1
 Getting features_provided for board_2
 
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/board_info.json
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/board_info.json
 ```
 
 1. Now we can add a board using the wizard. We can just add a mock device for now and for this example.
 ```bash
 $ inet-nm-commission --mock-dev
-Found 0 saved nodes in /tmp/pytest-of-weiss/pytest-93/test_cli_example0
-Enter serial number [57699532985485580169]:
+Found 0 saved nodes in /tmp/pytest-of-weiss/pytest-128/test_cli_example0
+Enter serial number [33046574371651769908]:
 Select board name for generic_vendor
 > board_1
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/nodes.json
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/nodes.json
 ```
 
 2. Let's do it again so we have 2 `board_1` boards.
 ```bash
 $ inet-nm-commission --mock-dev
-Found 1 saved nodes in /tmp/pytest-of-weiss/pytest-93/test_cli_example0
-Enter serial number [58694535556175588725]:
+Found 1 saved nodes in /tmp/pytest-of-weiss/pytest-128/test_cli_example0
+Enter serial number [48850751729363102347]:
 Select board name for generic_vendor
 > board_1
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/nodes.json
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/nodes.json
 ```
 
 3. We can also add the board with directly with the cli args.
 ```bash
 $ inet-nm-commission --mock-dev --board board_2
-Found 2 saved nodes in /tmp/pytest-of-weiss/pytest-93/test_cli_example0
-Enter serial number [69439102392297600251]:
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/nodes.json
+
+Found 2 saved nodes in /tmp/pytest-of-weiss/pytest-128/test_cli_example0
+Enter serial number [39660114694392531263]:
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/nodes.json
 ```
 
 4. If we add a board that is not in our `board_info` list, we will need to confirm it is correct.
 ```bash
 $ inet-nm-commission --mock-dev
-Found 3 saved nodes in /tmp/pytest-of-weiss/pytest-93/test_cli_example0
-Enter serial number [13602424446873101070]:
+Found 3 saved nodes in /tmp/pytest-of-weiss/pytest-128/test_cli_example0
+Enter serial number [28977745412211566911]:
 Select board name for generic_vendor
 > board_3
 Board board_3 not in board list, continue? [y/N] Y
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/nodes.json
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/nodes.json
 ```
 
 5. If we have a device showing up on the list that should not be commissioned, we can ignore it.  This will prevent accidentally commissioning it in the future and will not be selectable by this tool.
 ```bash
 $ inet-nm-commission --mock-dev --ignore
-Found 4 saved nodes in /tmp/pytest-of-weiss/pytest-93/test_cli_example0
-Enter serial number [06493041588800612712]:
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/nodes.json
+Found 4 saved nodes in /tmp/pytest-of-weiss/pytest-128/test_cli_example0
+Enter serial number [59469734794235533397]:
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/nodes.json
 ```
 
 6. Let's see what we have, since these are mocked devices we the will never be connected, so we should always check missing boards.
 ```bash
 $ inet-nm-check --missing
 {
   "board_1": 2,
@@ -134,113 +135,119 @@
 NODE:2:BOARD:board_3: 2
 ```
 
 14. There are many env vars exposed when running these scripts all starting with `NM_`. Let's check them on only one board.
 ```bash
 $ inet-nm-exec "printenv | grep NM_" --missing --boards board_2
 NODE:0:BOARD:board_2: NM_BOARD=board_2
-NODE:0:BOARD:board_2: NM_CONFIG_DIR=/tmp/pytest-of-weiss/pytest-93/test_cli_example0
-NODE:0:BOARD:board_2: NM_SERIAL=69439102392297600251
-NODE:0:BOARD:board_2: NM_UID=1e7c7ae04498e43e50b6b6b0d8e5255d
+NODE:0:BOARD:board_2: NM_CONFIG_DIR=/tmp/pytest-of-weiss/pytest-128/test_cli_example0
+NODE:0:BOARD:board_2: NM_SERIAL=39660114694392531263
+NODE:0:BOARD:board_2: NM_UID=5e1b2f6b9a3d5e956e4388a6a32de9aa
 NODE:0:BOARD:board_2: NM_PORT=Unknown
 NODE:0:BOARD:board_2: NM_IDX=0
 ```
 
-15. There is also some blocking of boards if they are being used, let's try it out by blocking `board_1` for some time.
+15. Maybe we want to run a command on all boards sequentially.
+We will sleep for an inverse amount of time to show the that they are being run sequentially.
+```bash
+$ inet-nm-exec "sleep 1" --missing --skip-dups --seq --boards board_1 board_2 board_3
+```
+
+16. There is also some blocking of boards if they are being used, let's try it out by blocking `board_1` for some time.
 ```bash
 $ inet-nm-exec "sleep 0.5" --missing --skip-dups --boards board_1
 ```
 
-16. Before the command finishes, in a different terminal, we can check to see what is available to us, notice we will be missing one of the `board_1` boards.
+17. Before the command finishes, in a different terminal, we can check to see what is available to us, notice we will be missing one of the `board_1` boards.
 ```bash
 $ inet-nm-check --missing
 {
   "board_1": 1,
   "board_2": 1,
   "board_3": 1
 }
 ```
 
-17. We can see what boards are being used with the only used flag.
+18. We can see what boards are being used with the only used flag.
 ```bash
 $ inet-nm-check --missing --only-used
 {
   "board_1": 1
 }
 ```
 
-18. We can also check all used and unused boards with the include used boards flag.
+19. We can also check all used and unused boards with the include used boards flag.
 ```bash
 $ inet-nm-check --missing --used
 {
   "board_1": 2,
   "board_2": 1,
   "board_3": 1
 }
 ```
 
-19. Once the process finished the used board should be freed.
+20. Once the process finished the used board should be freed.
 ```bash
 $ inet-nm-check --missing --only-used
 {}
 ```
 
-20. If something terrible and somebody locks all the board.
+21. If something terrible and somebody locks all the board.
 ```bash
 $ inet-nm-exec "sleep 2" --missing
 ```
 
-21. In a different terminal, we can see all our boards are used.
+22. In a different terminal, we can see all our boards are used.
 ```bash
 $ inet-nm-check --missing --only-used
 {
   "board_1": 2,
   "board_2": 1,
   "board_3": 1
 }
 ```
 
-22. We can force them to be freed with the free command, this will not cancel ongoing processes so be careful as flashing or board output might conflict.
+23. We can force them to be freed with the free command, this will not cancel ongoing processes so be careful as flashing or board output might conflict.
 ```bash
 $ inet-nm-free
 Releasing all locks
-Removing lock file /tmp/inet_nm/locks/12858d000ee97feb73f6ef2346d70058.lock
-Removing lock file /tmp/inet_nm/locks/1e7c7ae04498e43e50b6b6b0d8e5255d.lock
-Removing lock file /tmp/inet_nm/locks/b8389e9d64f7868aff48073c2eaf1130.lock
-Removing lock file /tmp/inet_nm/locks/9c142c38b67bf8b231eeaa8c9643828a.lock
+Removing lock file /tmp/inet_nm/locks/1b1766d0ba2e659aadade393718d27cc.lock
+Removing lock file /tmp/inet_nm/locks/5e1b2f6b9a3d5e956e4388a6a32de9aa.lock
+Removing lock file /tmp/inet_nm/locks/1c3a3933105da429ec8cec5513b09176.lock
+Removing lock file /tmp/inet_nm/locks/524d1fcaf596d7a04adceabf2d0cdf49.lock
 All locks released
 ```
 
-23. Now we can see they are free again.
+24. Now we can see they are free again.
 ```bash
 $ inet-nm-check --missing
 {
   "board_1": 2,
   "board_2": 1,
   "board_3": 1
 }
 ```
 
-24. What happens if we now add `board_3` to the board info cache?
+25. What happens if we now add `board_3` to the board info cache?
 ```bash
 $ inet-nm-update-from-os . --board-info "echo board_1 board_2 board_3" --board-features "echo feature_common feature_${BOARD}"
 Getting features_provided for board_1
 Getting features_provided for board_2
 Getting features_provided for board_3
 
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/board_info.json
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/board_info.json
 ```
 
-25. Well we can updated the nodes cache in a separate step, no need to re-commission.
+26. Well we can updated the nodes cache in a separate step, no need to re-commission.
 ```bash
 $ inet-nm-update-commissioned
-Updated /tmp/pytest-of-weiss/pytest-93/test_cli_example0/nodes.json
+Updated /tmp/pytest-of-weiss/pytest-128/test_cli_example0/nodes.json
 ```
 
-26. Now we can see the new feature and board is available.
+27. Now we can see the new feature and board is available.
 ```bash
 $ inet-nm-check --missing --feat-filter feature_board_3
 {
   "board_3": 1
 }
 ```
```

### Comparing `inet-nm-0.0.6/docs/conf.py` & `inet-nm-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/docs/index.md` & `inet-nm-0.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/setup.cfg` & `inet-nm-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/setup.py` & `inet-nm-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/_helpers.py` & `inet-nm-0.0.7/src/inet_nm/_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/check.py` & `inet-nm-0.0.7/src/inet_nm/check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_check.py` & `inet-nm-0.0.7/src/inet_nm/cli_check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_commission.py` & `inet-nm-0.0.7/src/inet_nm/cli_commission.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,19 @@
         nm_nodes.append(cmr.mock_device())
 
     try:
         selected_node = cmr.select_available_node(nm_nodes)
     except ValueError:
         print("No available nodes found")
         sys.exit(1)
+    except cmr.TtyNotPresent as exc:
+        if args.mock_dev:
+            selected_node = nm_nodes[-1]
+        else:
+            raise exc
     if args.ignore:
         selected_node.ignore = True
     else:
         binfo = bi_cfg.load()
         selected_node.board = args.board or cmr.select_board(
             list(binfo.keys()), selected_node
         )
```

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_exec.py` & `inet-nm-0.0.7/src/inet_nm/cli_exec.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,32 @@
     parser.add_argument(
         "-t",
         "--timeout",
         type=float,
         default=None,
         help="Wait until node available in seconds.",
     )
+    parser.add_argument(
+        "--seq",
+        action="store_true",
+        help="Run commands sequentially instead of concurrently",
+    )
 
     cfg.config_arg(parser)
     chk.check_args(parser)
     args = parser.parse_args()
     kwargs = vars(args)
     timeout = kwargs.pop("timeout")
     cmd = kwargs.pop("cmd")
+    seq = kwargs.pop("seq")
     nodes = nodes = rh.sanity_check("/bin/bash", **kwargs)
     # Somehow allows cleanup to happen...
     signal.signal(signal.SIGHUP, rh.do_nothing)
     try:
-        with apps.NmShellRunner(nodes, default_timeout=timeout) as runner:
+        with apps.NmShellRunner(nodes, default_timeout=timeout, seq=seq) as runner:
             runner.cmd = cmd
             runner.run()
     except KeyboardInterrupt:
         print()
         print("User aborted!")
         sys.exit(1)
     sys.exit(0)
```

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_free.py` & `inet-nm-0.0.7/src/inet_nm/cli_free.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_tmux.py` & `inet-nm-0.0.7/src/inet_nm/cli_tmux.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_tty_from_uid.py` & `inet-nm-0.0.7/src/inet_nm/cli_tty_from_uid.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_update_commissioned.py` & `inet-nm-0.0.7/src/inet_nm/cli_update_commissioned.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/cli_update_from_os.py` & `inet-nm-0.0.7/src/inet_nm/cli_update_from_os.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/commissioner.py` & `inet-nm-0.0.7/src/inet_nm/commissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/config.py` & `inet-nm-0.0.7/src/inet_nm/config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/data_types.py` & `inet-nm-0.0.7/src/inet_nm/data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/filelock.py` & `inet-nm-0.0.7/src/inet_nm/filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/locking.py` & `inet-nm-0.0.7/src/inet_nm/locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm/runner_apps.py` & `inet-nm-0.0.7/src/inet_nm/runner_apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,34 @@
     """
 
     cmd = "echo $NM_IDX"
     SETUP_WAIT = 0.1
 
     @staticmethod
     def _run_command(cmd, prefix, env):
-        process = subprocess.Popen(
-            cmd, env=env, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
-        )
-        while True:
+        def get_output(process):
             output = process.stdout.readline()
 
             if output:
                 nm_print(f"{prefix}{output.decode().strip()}")
             else:
                 # Have a small sleep so we are not burning CPU waiting for output.
-                time.sleep(0.2)
+                time.sleep(0.1)
+            return output
+
+        process = subprocess.Popen(
+            cmd, env=env, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
+        )
+        while True:
+            output = get_output(process)
             poll = process.poll()
             if poll is not None:
+                output = True
+                while output:
+                    output = get_output(process)
                 break
         rc = process.returncode
 
         return rc
 
     def func(self, node: NmNode, idx: int, env: Dict[str, str]):
         """Execute shell commands on nodes.
```

### Comparing `inet-nm-0.0.6/src/inet_nm/runner_base.py` & `inet-nm-0.0.7/src/inet_nm/runner_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,27 @@
     concurrently in separate threads, and handles cleanup after operations
     have completed.
 
     The operations to be run are defined by a method `func` which is to
     be implemented in the subclass.
     """
 
-    def __init__(self, nodes: List[NmNode], default_timeout: int = None):
+    def __init__(self, nodes: List[NmNode], default_timeout: int = None, seq=False):
         """
         Initialize a new instance of NmNodesRunner.
 
         Args:
             nodes: A list of NmNode instances to be managed.
             default_timeout: Default timeout value for file lock acquisition.
+            seq: If True, operations are run sequentially instead of concurrently.
+
         """
         self.nodes = nodes
         self.default_timeout = default_timeout
+        self.seq = seq
         self.lockable_nodes = [
             (node, FileLock(lk.get_lock_path(node), timeout=default_timeout))
             for node in nodes
         ]
         self.locks = [lock for _, lock in self.lockable_nodes]
         self._acquired = False
 
@@ -114,15 +117,18 @@
                 NM_SERIAL=node.serial,
                 NM_BOARD=node.board,
                 NM_PORT=nm_port,
             ).to_dict()
 
             thread = Thread(target=self.func, args=(node, idx, node_env))
             thread.start()
-            self.threads.append(thread)
+            if self.seq:
+                thread.join()
+            else:
+                self.threads.append(thread)
 
         for thread in self.threads:
             thread.join()
 
         self.post()
         self.release()
```

### Comparing `inet-nm-0.0.6/src/inet_nm/runner_helper.py` & `inet-nm-0.0.7/src/inet_nm/runner_helper.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/src/inet_nm.egg-info/PKG-INFO` & `inet-nm-0.0.7/src/inet_nm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.6
+Version: 0.0.7
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
```

### Comparing `inet-nm-0.0.6/src/inet_nm.egg-info/SOURCES.txt` & `inet-nm-0.0.7/src/inet_nm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_check.py` & `inet-nm-0.0.7/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_comissioner.py` & `inet-nm-0.0.7/tests/test_comissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_config.py` & `inet-nm-0.0.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_data_types.py` & `inet-nm-0.0.7/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_example_usage.py` & `inet-nm-0.0.7/tests/test_example_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pexpect
 import pytest
 from flaky import flaky
 
 
 class CliTester:
     DEFAULT_START_WAIT_TIME = 0.2
-    DEFAULT_PROCESS_TIMEOUT = 1
+    DEFAULT_PROCESS_TIMEOUT = 2
     title = None
     footer = None
     description = None
 
     def __init__(self, cfg_dir):
         os.environ["NM_CONFIG_DIR"] = str(cfg_dir)
         os.environ["COVERAGE_PROCESS_START"] = ".coveragerc"
@@ -45,15 +45,15 @@
             child.sendline(line)
         if skip_read:
             self._async_procs.append(child)
             self._step_results.append(
                 (description, f"{cmd} {' '.join(args or [])}", "")
             )
             return ""
-        output = child.read().decode()
+        output = child.read().decode().replace("\r\n", "\n")
         self._step_results.append(
             (description, f"{cmd} {' '.join(args or [])}", output)
         )
         return output
 
     def format_md(self):
         out = ""
@@ -234,14 +234,35 @@
         description="There are many env vars exposed when running these scripts "
         "all starting with `NM_`. Let's check them on only one board.",
         cmd="inet-nm-exec",
         args=['"printenv | grep NM_"', "--missing", "--boards", "board_2"],
     )
     assert "NM_BOARD=board_2" in ret
 
+    start_time = time.time()
+    ret = ct.run_step(
+        description="Maybe we want to run a command on all boards sequentially.\n"
+        "We will sleep for an inverse amount of time to show the that they are "
+        "being run sequentially.",
+        cmd="inet-nm-exec",
+        args=[
+            '"sleep 1"',
+            "--missing",
+            "--skip-dups",
+            "--seq",
+            "--boards",
+            "board_1",
+            "board_2",
+            "board_3",
+        ],
+        timeout=5,
+    )
+    end_time = time.time()
+    assert end_time - start_time >= 3
+
     ret = ct.run_step(
         description="There is also some blocking of boards if they are being used, "
         "let's try it out by blocking `board_1` for some time.",
         cmd="inet-nm-exec",
         args=['"sleep 0.5"', "--missing", "--skip-dups", "--boards", "board_1"],
         timeout=2,
         skip_read=True,
```

### Comparing `inet-nm-0.0.6/tests/test_filelock.py` & `inet-nm-0.0.7/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_helpers.py` & `inet-nm-0.0.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_locking.py` & `inet-nm-0.0.7/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_runner_apps.py` & `inet-nm-0.0.7/tests/test_runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tests/test_runner_base.py` & `inet-nm-0.0.7/tests/test_runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.6/tox.ini` & `inet-nm-0.0.7/tox.ini`

 * *Files identical despite different names*

