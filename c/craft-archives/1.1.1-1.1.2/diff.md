# Comparing `tmp/craft-archives-1.1.1.tar.gz` & `tmp/craft-archives-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-archives-1.1.1.tar", last modified: Fri Jun 30 19:29:03 2023, max compression
+gzip compressed data, was "craft-archives-1.1.2.tar", last modified: Tue Jul 11 20:48:18 2023, max compression
```

## Comparing `craft-archives-1.1.1.tar` & `craft-archives-1.1.2.tar`

### file list

```diff
@@ -1,96 +1,101 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.694146 craft-archives-1.1.1/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       77 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.codespell_ignore_lines
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.editorconfig
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/.github/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/release-drafter.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3504 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/renovate.json5
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/.github/workflows/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/cla-check.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      822 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/docs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      586 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1448 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/release-publish.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2411 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/tests.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1961 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.gitignore
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      485 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.readthedocs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        6 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.yamlignore
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      201 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.yamllint.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3839 2023-06-30 19:19:48.000000 craft-archives-1.1.1/HACKING.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-06-30 19:19:48.000000 craft-archives-1.1.1/LICENSE
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1489 2023-06-30 19:29:03.694146 craft-archives-1.1.1/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      605 2023-06-30 19:19:48.000000 craft-archives-1.1.1/README.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/craft_archives/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1015 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      160 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives/_version.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1151 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/errors.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/craft_archives/repo/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      874 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    13124 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_key_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1985 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_ppa.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6318 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_preferences_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10621 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_sources_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_uca.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4618 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5067 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/installer.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    11312 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/package_repository.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1142 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/projects.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3439 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/utils.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/craft_archives.egg-info/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1489 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2197 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      505 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       15 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/top_level.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/docs/_static/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/_static/css/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/_static/css/custom.css
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      757 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/changelog.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1678 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/conf.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/explanation/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/explanation/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/howto/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1500 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/howto/add_repo.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       83 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/howto/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1765 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/reference/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      178 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/reference/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6034 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/reference/repo_properties.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/tutorials/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/tutorials/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8193 2023-06-30 19:19:48.000000 craft-archives-1.1.1/pyproject.toml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2023-06-30 19:29:03.694146 craft-archives-1.1.1/setup.cfg
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1375 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/integration/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/integration/repo/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/repo/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6626 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/repo/test_apt_key_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7830 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/repo/test_installer.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/test_data/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1619 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/FC42E99D.asc
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/empty.preferences
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      173 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/expected.preferences
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      127 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/many_blank_lines.preferences
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/test_data/multi-keys/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2419 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/multi-keys/0264B26D.asc
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    15720 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/multi-keys/9E61EF26.asc
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      226 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/no_header.preferences
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       35 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/only_comment.preferences
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      259 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/with_header.preferences
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/unit/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.694146 craft-archives-1.1.1/tests/unit/repo/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    17516 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_key_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1890 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_ppa.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6936 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_preferences_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8974 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_sources_manager.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1890 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_uca.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4282 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_installer.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16191 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_package_repository.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_projects.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4663 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.595326 craft-archives-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.codespell_ignore_lines
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/task.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/cla-check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/issues.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/release-drafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/release-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.yamlignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-11 20:48:02.000000 craft-archives-1.1.2/HACKING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-11 20:48:02.000000 craft-archives-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-11 20:48:18.595326 craft-archives-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 20:48:02.000000 craft-archives-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/craft_archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/craft_archives/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/craft_archives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.583326 craft-archives-1.1.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/explanation/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/howto/add_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/reference/repo_properties.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-11 20:48:02.000000 craft-archives-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:48:18.595326 craft-archives-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/integration/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/repo/test_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/FC42E99D.asc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/empty.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/expected.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/many_blank_lines.preferences
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/test_data/multi-keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/multi-keys/0264B26D.asc
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/multi-keys/9E61EF26.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/no_header.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/only_comment.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/with_header.preferences
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.595326 craft-archives-1.1.2/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tox.ini
```

### Comparing `craft-archives-1.1.1/.editorconfig` & `craft-archives-1.1.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/.github/renovate.json5` & `craft-archives-1.1.2/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/.github/workflows/docs.yaml` & `craft-archives-1.1.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/.github/workflows/release-drafter.yaml` & `craft-archives-1.1.2/.github/workflows/release-drafter.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/.github/workflows/release-publish.yaml` & `craft-archives-1.1.2/.github/workflows/release-publish.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 jobs:
   source-wheel:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
+      - name: Fetch tag annotations
+        run: |
+          git fetch --force --tags --depth 1
+          git describe --dirty --long --match '[0-9]*.[0-9]*.[0-9]*' --exclude '*[^0-9.]*'
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
           check-latest: true
       - name: Build packages
         run: |
```

### Comparing `craft-archives-1.1.1/.github/workflows/tests.yaml` & `craft-archives-1.1.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/.gitignore` & `craft-archives-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/.pre-commit-config.yaml` & `craft-archives-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/HACKING.rst` & `craft-archives-1.1.2/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/LICENSE` & `craft-archives-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/PKG-INFO` & `craft-archives-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.1.1
+Version: 1.1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.1.1/README.rst` & `craft-archives-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/__init__.py` & `craft-archives-1.1.2/craft_archives/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/errors.py` & `craft-archives-1.1.2/craft_archives/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/__init__.py` & `craft-archives-1.1.2/craft_archives/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/apt_key_manager.py` & `craft-archives-1.1.2/craft_archives/repo/apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/apt_ppa.py` & `craft-archives-1.1.2/craft_archives/repo/apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/apt_preferences_manager.py` & `craft-archives-1.1.2/craft_archives/repo/apt_preferences_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/apt_sources_manager.py` & `craft-archives-1.1.2/craft_archives/repo/apt_sources_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/apt_uca.py` & `craft-archives-1.1.2/craft_archives/repo/apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/errors.py` & `craft-archives-1.1.2/craft_archives/repo/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/installer.py` & `craft-archives-1.1.2/craft_archives/repo/installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/repo/package_repository.py` & `craft-archives-1.1.2/craft_archives/repo/package_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from urllib.parse import urlparse
 
 import pydantic
 from overrides import overrides  # pyright: ignore[reportUnknownVariableType]
 from pydantic import (
     AnyUrl,
     ConstrainedStr,
+    FileUrl,
     root_validator,  # pyright: ignore[reportUnknownVariableType]
     validator,  # pyright: ignore[reportUnknownVariableType]
 )
 
 # NOTE: using this instead of typing.Literal because of this bad typing_extensions
 # interaction: https://github.com/pydantic/pydantic/issues/5821#issuecomment-1559196859
 # We can revisit this when typing_extensions >4.6.0 is released, and/or we no longer
@@ -216,15 +217,15 @@
         """The pin string for this repository if needed."""
         return f'origin "{UCA_NETLOC}"'
 
 
 class PackageRepositoryApt(PackageRepository):
     """An APT package repository."""
 
-    url: AnyUrl
+    url: Union[AnyUrl, FileUrl]
     key_id: KeyIdStr = pydantic.Field(alias="key-id")
     architectures: Optional[List[str]]
     formats: Optional[List[Literal["deb", "deb-src"]]]
     path: Optional[str]
     components: Optional[List[str]]
     key_server: Optional[str] = pydantic.Field(alias="key-server")
     suites: Optional[List[str]]
```

### Comparing `craft-archives-1.1.1/craft_archives/repo/projects.py` & `craft-archives-1.1.2/craft_archives/repo/projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives/utils.py` & `craft-archives-1.1.2/craft_archives/utils.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/craft_archives.egg-info/PKG-INFO` & `craft-archives-1.1.2/craft_archives.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.1.1
+Version: 1.1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.1.1/craft_archives.egg-info/SOURCES.txt` & `craft-archives-1.1.2/craft_archives.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 LICENSE
 README.rst
 pyproject.toml
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/renovate.json5
+.github/ISSUE_TEMPLATE/bug.yaml
+.github/ISSUE_TEMPLATE/config.yml
+.github/ISSUE_TEMPLATE/task.yaml
 .github/workflows/cla-check.yaml
 .github/workflows/docs.yaml
+.github/workflows/issues.yaml
 .github/workflows/release-drafter.yaml
 .github/workflows/release-publish.yaml
 .github/workflows/tests.yaml
 craft_archives/__init__.py
 craft_archives/_version.py
 craft_archives/errors.py
 craft_archives/utils.py
```

### Comparing `craft-archives-1.1.1/docs/changelog.rst` & `craft-archives-1.1.2/docs/changelog.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 *********
 Changelog
 *********
 
 See the `Releases page`_ on Github for a complete list of commits that are
 included in each version.
 
+1.1.2 (2023-07-12)
+------------------
+
+This release addresses a regression where local filepaths were no longer
+accepted for the ``url`` property of an deb-type repository.
+
 1.1.1 (2023-06-30)
 ------------------
 
 This release addresses a regression where asset files with multiple
 fingerprints (either from multiple keys or subkeys) were no longer accepted.
 
 1.1.0 (2023-05-30)
```

### Comparing `craft-archives-1.1.1/docs/conf.py` & `craft-archives-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/docs/howto/add_repo.rst` & `craft-archives-1.1.2/docs/howto/add_repo.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/docs/index.rst` & `craft-archives-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/docs/reference/repo_properties.rst` & `craft-archives-1.1.2/docs/reference/repo_properties.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/pyproject.toml` & `craft-archives-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/conftest.py` & `craft-archives-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/integration/repo/test_apt_key_manager.py` & `craft-archives-1.1.2/tests/integration/repo/test_apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/integration/repo/test_installer.py` & `craft-archives-1.1.2/tests/integration/repo/test_installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/test_data/FC42E99D.asc` & `craft-archives-1.1.2/tests/test_data/FC42E99D.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/test_data/multi-keys/0264B26D.asc` & `craft-archives-1.1.2/tests/test_data/multi-keys/0264B26D.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/test_data/multi-keys/9E61EF26.asc` & `craft-archives-1.1.2/tests/test_data/multi-keys/9E61EF26.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_apt_key_manager.py` & `craft-archives-1.1.2/tests/unit/repo/test_apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_apt_ppa.py` & `craft-archives-1.1.2/tests/unit/repo/test_apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_apt_preferences_manager.py` & `craft-archives-1.1.2/tests/unit/repo/test_apt_preferences_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_apt_sources_manager.py` & `craft-archives-1.1.2/tests/unit/repo/test_apt_sources_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_apt_uca.py` & `craft-archives-1.1.2/tests/unit/repo/test_apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_installer.py` & `craft-archives-1.1.2/tests/unit/repo/test_installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_package_repository.py` & `craft-archives-1.1.2/tests/unit/repo/test_package_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,22 +93,28 @@
             "url": "https://some/url",
             "key-id": "BCDEF12345" * 4,
             "formats": ["deb"],
             "components": ["some", "components"],
             "key-server": "my-key-server",
             "suites": ["some", "suites"],
         },
+        {  # File URLs. See: https://github.com/canonical/craft-archives/issues/92
+            "type": "apt",
+            "url": "file:///tmp/apt-repo",
+            "path": "my/path",
+            "key-id": "BCDEF12345" * 4,
+        },
     ],
 )
 def test_apt_valid(repo, priority):
     if priority is not None:
         repo["priority"] = priority
     apt_deb = PackageRepositoryApt.unmarshal(repo)
     assert apt_deb.type == "apt"
-    assert apt_deb.url == "https://some/url"
+    assert apt_deb.url == repo["url"]
     assert apt_deb.key_id == "BCDEF12345" * 4
     assert apt_deb.formats == (["deb"] if "formats" in repo else None)
     assert apt_deb.components == (
         ["some", "components"] if "components" in repo else None
     )
     assert apt_deb.key_server == ("my-key-server" if "key-server" in repo else None)
     assert apt_deb.path == ("my/path" if "path" in repo else None)
```

### Comparing `craft-archives-1.1.1/tests/unit/repo/test_projects.py` & `craft-archives-1.1.2/tests/unit/repo/test_projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.1/tox.ini` & `craft-archives-1.1.2/tox.ini`

 * *Files identical despite different names*

