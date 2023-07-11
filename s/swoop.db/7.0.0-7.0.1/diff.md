# Comparing `tmp/swoop.db-7.0.0.tar.gz` & `tmp/swoop.db-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-7.0.0.tar", last modified: Sat Jul  1 05:29:23 2023, max compression
+gzip compressed data, was "swoop.db-7.0.1.tar", last modified: Tue Jul 11 21:46:38 2023, max compression
```

## Comparing `swoop.db-7.0.0.tar` & `swoop.db-7.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-01 05:29:07.000000 swoop.db-7.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-01 05:29:07.000000 swoop.db-7.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-01 05:29:07.000000 swoop.db-7.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-01 05:29:07.000000 swoop.db-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-01 05:29:23.791331 swoop.db-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-01 05:29:07.000000 swoop.db-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-01 05:29:07.000000 swoop.db-7.0.0/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-01 05:29:07.000000 swoop.db-7.0.0/bin/get-max-migration-version.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-01 05:29:07.000000 swoop.db-7.0.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-01 05:29:07.000000 swoop.db-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-01 05:29:07.000000 swoop.db-7.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:29:23.791331 swoop.db-7.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00001_version.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00003_remove_items.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00004_update_thread.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00004_update_thread.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00005_handler_type.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00005_handler_type.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00006_workflow_constraint.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00006_workflow_constraint.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00007_change-uuid-formats.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/tests/fixtures/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/0_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/1_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/2_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/2_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/6_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/6_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/7_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/7_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_find_cached_action_for_payload.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_uuid_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.636809 swoop.db-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.628808 swoop.db-7.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.632808 swoop.db-7.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-11 21:46:19.000000 swoop.db-7.0.1/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-11 21:46:19.000000 swoop.db-7.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-11 21:46:19.000000 swoop.db-7.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-11 21:46:19.000000 swoop.db-7.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 21:46:19.000000 swoop.db-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-11 21:46:38.636809 swoop.db-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-11 21:46:19.000000 swoop.db-7.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-11 21:46:19.000000 swoop.db-7.0.1/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.632808 swoop.db-7.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-11 21:46:19.000000 swoop.db-7.0.1/bin/get-max-migration-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-11 21:46:19.000000 swoop.db-7.0.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-11 21:46:19.000000 swoop.db-7.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 21:46:19.000000 swoop.db-7.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:46:38.636809 swoop.db-7.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.628808 swoop.db-7.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.628808 swoop.db-7.0.1/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.632808 swoop.db-7.0.1/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.632808 swoop.db-7.0.1/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.636809 swoop.db-7.0.1/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00001_version.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00002_cache_func.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00002_cache_func.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00003_remove_items.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00004_update_thread.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00004_update_thread.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00005_handler_type.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00005_handler_type.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00006_workflow_constraint.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00006_workflow_constraint.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/migrations/00007_change-uuid-formats.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-11 21:46:19.000000 swoop.db-7.0.1/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.632808 swoop.db-7.0.1/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-11 21:46:38.000000 swoop.db-7.0.1/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-11 21:46:38.000000 swoop.db-7.0.1/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:46:38.000000 swoop.db-7.0.1/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 21:46:38.000000 swoop.db-7.0.1/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-11 21:46:38.000000 swoop.db-7.0.1/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 21:46:38.000000 swoop.db-7.0.1/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.636809 swoop.db-7.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.628808 swoop.db-7.0.1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.636809 swoop.db-7.0.1/tests/fixtures/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/0_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/1_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/2_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/2_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/6_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/6_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/7_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/7_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/fixtures/migrations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:46:38.636809 swoop.db-7.0.1/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/pgtap/test_find_cached_action_for_payload.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/pgtap/test_uuid_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-11 21:46:19.000000 swoop.db-7.0.1/tests/test_migrations.py
```

### Comparing `swoop.db-7.0.0/.env` & `swoop.db-7.0.1/.env`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.github/workflows/publish-image.yml` & `swoop.db-7.0.1/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.github/workflows/python-publish.yml` & `swoop.db-7.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.github/workflows/python-test.yml` & `swoop.db-7.0.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.github/workflows/snyk-scan.yml` & `swoop.db-7.0.1/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.gitignore` & `swoop.db-7.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.pre-commit-config.yaml` & `swoop.db-7.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/.snyk` & `swoop.db-7.0.1/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/CHANGELOG.md` & `swoop.db-7.0.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v7.0.1] - 2023-07-11
+
+### Changed
+
+- Use the same image version for all build stages in the Dockerfile (fixes an
+  issue with libc not found) ([#21])
+
 ## [v7.0.0] - 2023-07-01
 
 ### ⚠️ Breaking Changes
 
 The schema migration from version 6 to 7 requries truncating ALL data records
 in the database. There is no forward migration for existing data, just the
 schema.
@@ -60,18 +67,21 @@
 - `UNKNOWN` state removed from `event_state` ([#14])
 
 ## [v0.1.0] - 2023-05-31
 
 Initial release
 
 [unreleased]: https://github.com/element84/swoop-db/compare/v7.0.0...main
+[unreleased]: https://github.com/element84/swoop-db/compare/v7.0.1...main
+[v7.0.1]: https://github.com/element84/swoop-db/compare/v7.0.0...7.0.1
 [v7.0.0]: https://github.com/element84/swoop-db/compare/v2.0.0...7.0.0
 [v2.0.0]: https://github.com/element84/swoop-db/compare/v0.1.0...2.0.0
 [v0.1.0]: https://github.com/element84/swoop-db/tree/v0.1.0
 
 [#12]: https://github.com/Element84/swoop-db/pull/12
 [#14]: https://github.com/Element84/swoop-db/pull/14
 [#15]: https://github.com/Element84/swoop-db/pull/15
 [#19]: https://github.com/Element84/swoop-db/pull/19
 [#20]: https://github.com/Element84/swoop-db/pull/20
+[#21]: https://github.com/Element84/swoop-db/pull/21
 
 [dbami]: https://github.com/element84/dbami
```

### Comparing `swoop.db-7.0.0/CONTRIBUTING.md` & `swoop.db-7.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/Dockerfile` & `swoop.db-7.0.1/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 WORKDIR /opt/swoop/db
 RUN python3 -m venv --copies swoop-db-venv
 COPY requirements.txt .
 RUN ./swoop-db-venv/bin/pip install -r requirements.txt
 RUN --mount=source=.git,target=.git,type=bind git clone . clone
 RUN ./swoop-db-venv/bin/pip install ./clone
 
-FROM postgres:15-bullseye
+FROM postgres:15
 # install build deps and pg_partman
 RUN set -x && \
     apt-get update && \
     apt-get install -y postgresql-15-partman curl make patch && \
     apt-get clean -y && \
     rm -r /var/lib/apt/lists/*
```

### Comparing `swoop.db-7.0.0/LICENSE` & `swoop.db-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/PKG-INFO` & `swoop.db-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 7.0.0
+Version: 7.0.1
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-7.0.0/README.md` & `swoop.db-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/RELEASE.md` & `swoop.db-7.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/docker-compose.yml` & `swoop.db-7.0.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/pyproject.toml` & `swoop.db-7.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/cli.py` & `swoop.db-7.0.1/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/fixtures/base_01.sql` & `swoop.db-7.0.1/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-7.0.1/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.down.sql` & `swoop.db-7.0.1/src/swoop/db/migrations/00002_cache_func.down.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.up.sql` & `swoop.db-7.0.1/src/swoop/db/migrations/00002_cache_func.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/migrations/00004_update_thread.down.sql` & `swoop.db-7.0.1/src/swoop/db/migrations/00004_update_thread.down.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/migrations/00004_update_thread.up.sql` & `swoop.db-7.0.1/src/swoop/db/migrations/00004_update_thread.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/migrations/00007_change-uuid-formats.up.sql` & `swoop.db-7.0.1/src/swoop/db/migrations/00007_change-uuid-formats.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop/db/schema.sql` & `swoop.db-7.0.1/src/swoop/db/schema.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-7.0.1/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 7.0.0
+Version: 7.0.1
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-7.0.0/src/swoop.db.egg-info/SOURCES.txt` & `swoop.db-7.0.1/src/swoop.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/conftest.py` & `swoop.db-7.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/0_base_01.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/0_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/1_result.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/1_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/2_base_01.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/2_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/2_result.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/2_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/6_base_01.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/6_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/6_result.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/6_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/7_base_01.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/7_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/7_result.sql` & `swoop.db-7.0.1/tests/fixtures/migrations/7_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/fixtures/migrations/README.md` & `swoop.db-7.0.1/tests/fixtures/migrations/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/pgtap/test_action.sql` & `swoop.db-7.0.1/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/pgtap/test_find_cached_action_for_payload.sql` & `swoop.db-7.0.1/tests/pgtap/test_find_cached_action_for_payload.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/pgtap/test_limit-locking.sql` & `swoop.db-7.0.1/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/pgtap/test_uuid_v7.sql` & `swoop.db-7.0.1/tests/pgtap/test_uuid_v7.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/test_database.py` & `swoop.db-7.0.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.0/tests/test_migrations.py` & `swoop.db-7.0.1/tests/test_migrations.py`

 * *Files identical despite different names*

