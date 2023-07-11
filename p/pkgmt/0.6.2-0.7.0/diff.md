# Comparing `tmp/pkgmt-0.6.2.tar.gz` & `tmp/pkgmt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.6.2.tar", last modified: Fri Jun 30 15:32:14 2023, max compression
+gzip compressed data, was "pkgmt-0.7.0.tar", last modified: Tue Jul 11 18:27:35 2023, max compression
```

## Comparing `pkgmt-0.6.2.tar` & `pkgmt-0.7.0.tar`

### file list

```diff
@@ -1,63 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-06-30 15:31:57.000000 pkgmt-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 15:31:57.000000 pkgmt-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:31:57.000000 pkgmt-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 15:32:14.946761 pkgmt-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 15:31:57.000000 pkgmt-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 15:31:57.000000 pkgmt-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 15:32:14.946761 pkgmt-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-30 15:31:57.000000 pkgmt-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/src/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/src/package_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/fail_if_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/fail_if_not_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/abstractversioner.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/versionernonsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/versionersetup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-11 18:27:17.000000 pkgmt-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-11 18:27:17.000000 pkgmt-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-11 18:27:17.000000 pkgmt-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 18:27:35.757430 pkgmt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-11 18:27:17.000000 pkgmt-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 18:27:17.000000 pkgmt-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 18:27:35.757430 pkgmt-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-11 18:27:17.000000 pkgmt-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.749429 pkgmt-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/assets/template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.749429 pkgmt-0.7.0/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/assets/template/src/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/src/package_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/fail_if_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/fail_if_not_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioner/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.6.2/CHANGELOG.md` & `pkgmt-0.7.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## 0.7.0 (2023-07-11)
+
+* [API Change] Support for projects containing `version` key in `pyproject.toml`. ([#58](https://github.com/ploomber/pkgmt/issues/58))
+* [Fix] Fix bug when running git hook
+
 ## 0.6.2 (2023-06-30)
 
 * [Feature] Added file path to `pkgmt lint` ([#56](https://github.com/ploomber/pkgmt/issues/56))
 * [Feature] Clearer error when missing `pyproject.toml`
 * [Feature] Added `--exclude` option to pkgmt `lint` and pkgmt `format` ([#55](https://github.com/ploomber/pkgmt/issues/55))
 
 ## 0.6.1 (2023-06-09)
```

### Comparing `pkgmt-0.6.2/LICENSE` & `pkgmt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/README.md` & `pkgmt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/setup.py` & `pkgmt-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/.github/pull_request_template.md` & `pkgmt-0.7.0/src/pkgmt/assets/template/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.7.0/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.7.0/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/pyproject.toml` & `pkgmt-0.7.0/src/pkgmt/assets/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/setup.py` & `pkgmt-0.7.0/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.7.0/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/assets/template/tests/conftest.py` & `pkgmt-0.7.0/src/pkgmt/assets/template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/changelog.py` & `pkgmt-0.7.0/src/pkgmt/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 except ModuleNotFoundError:
     mistune = None
     MarkdownRenderer = None
     BlockState = None
     InlineParser = object
 
 from pkgmt import config
-from pkgmt.versioner.versionersetup import VersionerSetup
 from pkgmt.versioner import util
+from pkgmt.versioner.versioner import Versioner
 from pkgmt._format import pretty_iterator
 from pkgmt.exceptions import ProjectValidationError
 
 _PREFIXES = {"[API Change]", "[Feature]", "[Fix]", "[Doc]"}
 
 
 class CustomInlineParser(InlineParser):
@@ -185,15 +185,15 @@
         self.text = text
 
         markdown = mistune.Markdown(
             renderer=None, inline=CustomInlineParser(hard_wrap=False), plugins=None
         )
         self.tree = markdown(text)
 
-        versioner = VersionerSetup(project_root=project_root)
+        versioner = Versioner(project_root=project_root)
         self.current = versioner.current_version()
 
     @classmethod
     def from_path(cls, path, project_root="."):
         return cls(text=Path(path).read_text(), project_root=project_root)
 
     def sort_last_section(self):
```

### Comparing `pkgmt-0.6.2/src/pkgmt/cli.py` & `pkgmt-0.7.0/src/pkgmt/cli.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/dependencies.py` & `pkgmt-0.7.0/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/deprecation.py` & `pkgmt-0.7.0/src/pkgmt/deprecation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
 import re
 from glob import iglob
 from collections import defaultdict
 
 import click
 
-from pkgmt.versioner.versionersetup import VersionerSetup
 from pkgmt.versioner.util import complete_version_string
 from pkgmt.exceptions import ProjectValidationError
+from pkgmt.versioner.versioner import Versioner
 
 
 class Deprecations:
     def __init__(self, root_dir=None) -> None:
         self.root_dir = root_dir
 
-        versioner = VersionerSetup(project_root=root_dir)
+        versioner = Versioner(project_root=root_dir)
         self.current = complete_version_string(
             versioner.current_version().replace("dev", "")
         )
 
     def check(self):
         """Check if there are pending deprecations"""
         deprecations = find_deprecations(root_dir=self.root_dir)
```

### Comparing `pkgmt-0.6.2/src/pkgmt/dev.py` & `pkgmt-0.7.0/src/pkgmt/dev.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/fail_if_modified.py` & `pkgmt-0.7.0/src/pkgmt/fail_if_modified.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/fail_if_not_modified.py` & `pkgmt-0.7.0/src/pkgmt/fail_if_not_modified.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/formatting.py` & `pkgmt-0.7.0/src/pkgmt/formatting.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/github.py` & `pkgmt-0.7.0/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/hook.py` & `pkgmt-0.7.0/src/pkgmt/hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             return 1
         else:
             click.echo("All checks passed!")
             return 0
 
 
 def _lint(files=None, exclude=None):
+    files = files or []
+    exclude = exclude or []
+
     if len(files) == 0:
         files = ["."]
     else:
         files = list(files)
 
     exclude_str_flake8 = ",".join(exclude)
     exclude_str_black = "|".join(exclude)
```

### Comparing `pkgmt-0.6.2/src/pkgmt/links.py` & `pkgmt-0.7.0/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/new.py` & `pkgmt-0.7.0/src/pkgmt/new.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/test.py` & `pkgmt-0.7.0/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.2/src/pkgmt/versioneer.py` & `pkgmt-0.7.0/src/pkgmt/versioneer.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import sys
 import shutil
 import subprocess
 from pathlib import Path
 import click
 
 from pkgmt.changelog import expand_github_from_changelog, CHANGELOG
-from pkgmt.versioner.versionernonsetup import VersionerNonSetup
-from pkgmt.versioner.versionersetup import VersionerSetup
+from pkgmt.versioner.versioner import Versioner
 from pkgmt.versioner.util import complete_version_string, is_pre_release
 from pkgmt.deprecation import Deprecations
 
 
 def replace_in_file(path_to_file, original, replacement):
     """Replace string in file"""
     with open(path_to_file, "r+") as f:
@@ -70,18 +69,25 @@
             "(first character must be numeric)"
         )
 
     return complete_version_string(version)
 
 
 def version(
-    project_root=".", tag=True, version_package=None, yes=False, push=True, target=None
+    project_root=".",
+    tag=True,
+    yes=False,
+    push=True,
+    target=None,
 ):
     """
 
+    Function to update latest stable version in version
+    file to new development version.
+
     Parameters
     ----------
     tag : bool, default=True
         Tags the commit with the stable version
 
     yes : bool, default=False
         Skips user prompt before applying changes
@@ -90,63 +96,38 @@
         Pushes the changes to the remote repository
 
     target : {None, "stable"}, default=None
         If None, it assumes the repository is in a dev version, so it creates a
         stable version and a new dev version. If stable, it assumes the repo is in a
         dev version and creates a stable version (skipping bumping to a new dev
         version)
-
-
-    Notes
-    -----
-    Create a new version (projects with setup.py) :
-    1. version_package will be None
-    2. Set new stable version in package_name/__init__.py
-    3. Update header in CHANGELOG file, and ask to review CHANGELOG
-    4. Create commit for new version, create git tag, and push
-    5. Set new development version in package_name/__init__.py, and CHANGELOG
-    6. Commit new development version and push
-
-    Create a new version (projects without setup.py) :
-    1. These projects should contain two essential files:
-       config.yaml in root directory which should contain the repo
-       name
-       _version.py file containing __version__ in the required directory
-    2. version_package will be the directory containing _version.py file
-    3. Set new stable version in package_name/_version.py
-    4. Update header in CHANGELOG file, and ask to review CHANGELOG
-    5. Create commit for new version, create git tag, and push
-    6. Set new development version in package_name/_version.py, and CHANGELOG
-    7. Commit new development version and push
     """
+
     _git_checkout_main_branch(pull=True)
 
     pending = subprocess.check_output(["git", "status", "--short"])
 
     if pending:
         raise click.ClickException(
             "Cannot run 'pkgmt version': you have pending files to commit. "
             "Commit them or discard them and try again.\nDetected files:"
             f"\n{pending.decode()}"
         )
 
-    if version_package:
-        versioner = VersionerNonSetup(version_package, project_root=project_root)
-    else:
-        versioner = VersionerSetup(project_root=project_root)
+    versioner = Versioner(project_root)
 
     changelog_md_exists = (
         versioner.path_to_changelog and versioner.path_to_changelog.suffix == ".md"
     )
 
-    # TODO: make it compatible with VersionerNonSetup
-    if not version_package and changelog_md_exists:
+    if changelog_md_exists:
         # check changelog
         CHANGELOG.from_path(
-            path=versioner.path_to_changelog, project_root=project_root
+            path=versioner.path_to_changelog,
+            project_root=project_root,
         ).check()
 
         # look for deprecations
         Deprecations(root_dir=project_root).check()
 
     current = versioner.current_version()
     release = versioner.release_version()
@@ -173,21 +154,20 @@
                 abort=True,
             )
 
     # Expand github links and sort secions
     if changelog_md_exists:
         expand_github_from_changelog(path=versioner.path_to_changelog)
 
-        # TODO: make it compatible with VersionerNonSetup
-        if not version_package:
-            # sort changelog entries
-            changelod_sorted = CHANGELOG.from_path(
-                path=versioner.path_to_changelog, project_root=project_root
-            ).sort_last_section()
-            Path(versioner.path_to_changelog).write_text(changelod_sorted)
+        # sort changelog entries
+        changelog_sorted = CHANGELOG.from_path(
+            path=versioner.path_to_changelog,
+            project_root=project_root,
+        ).sort_last_section()
+        Path(versioner.path_to_changelog).write_text(changelog_sorted)
 
     else:
         print("Skipping CHANGELOG processing (only supported in .md files)")
 
     # Replace version number and create tag
     print("Commiting release version: {}".format(release))
     versioner.commit_version(
@@ -240,15 +220,15 @@
 def upload(tag, production, yes=False):
     """
     Check outs a tag, uploads to PyPI
     """
     print("Checking out tag {}".format(tag))
     call(["git", "checkout", tag])
 
-    versioner = VersionerSetup()
+    versioner = Versioner()
     current = versioner.current_version()
 
     if not yes:
         input_confirm(
             "Version in {} tag is {}. Do you want to continue?".format(tag, current),
             abort=True,
         )
```

### Comparing `pkgmt-0.6.2/src/pkgmt/versioner/abstractversioner.py` & `pkgmt-0.7.0/src/pkgmt/versioner/versioner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
-import abc
 import ast
 import datetime
 import subprocess
 
 from pathlib import Path
 
-from pkgmt.versioner.util import complete_version_string
+from pkgmt.versioner.util import complete_version_string, find_package_and_version_file
 
 
 def replace_in_file(path_to_file, original, replacement):
     """Replace string in file"""
     with open(path_to_file, "r+") as f:
         content = f.read()
         updated = content.replace(original, replacement)
@@ -32,25 +31,29 @@
         return f"## {content}"
     elif path.suffix == ".rst":
         return f"{content}\n" + "-" * len(content)
     else:
         raise ValueError("Unsupported format, must be .rst or .md")
 
 
-class AbstractVersioner(abc.ABC):
+class Versioner:
     def __init__(self, project_root="."):
         self.project_root = project_root or "."
-        self.package_name, self.PACKAGE = self.find_package()
+        package_name, PACKAGE, version_file_name = find_package_and_version_file(
+            self.project_root
+        )
+        self.package_name = package_name
+        self.PACKAGE = PACKAGE
         if Path(self.project_root, "CHANGELOG.rst").exists():
             self.path_to_changelog = Path(self.project_root, "CHANGELOG.rst")
         elif Path(self.project_root, "CHANGELOG.md").exists():
             self.path_to_changelog = Path(self.project_root, "CHANGELOG.md")
         else:
             self.path_to_changelog = None
-        self.version_file = self.version_file()
+        self.version_file = version_file_name
 
     def current_version(self):
         """Returns the current version in version file"""
         _version_re = re.compile(r"__version__\s+=\s+(.*)")
 
         with open(self.PACKAGE / self.version_file, "rb") as f:
             VERSION = str(
@@ -181,18 +184,7 @@
                 start_current = "# CHANGELOG"
 
             new_header = make_header(dev_version, self.path_to_changelog)
             start_new = f"{start_current}\n\n{new_header}"
             replace_in_file(self.path_to_changelog, start_current, start_new)
         else:
             print("No CHANGELOG.{rst,md} found, skipping changelog editing...")
-
-    @abc.abstractmethod
-    def find_package(self):
-        """Must return the package name and the path to the package root"""
-        pass
-
-    @abc.abstractmethod
-    def version_file(self):
-        """Must return a path to the version file, relative to the package root (as
-        returned by find_package)"""
-        pass
```

### Comparing `pkgmt-0.6.2/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.7.0/src/pkgmt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -40,11 +40,9 @@
 src/pkgmt/assets/template/tasks.py
 src/pkgmt/assets/template/.github/pull_request_template.md
 src/pkgmt/assets/template/.github/workflows/ci.yml
 src/pkgmt/assets/template/src/package_name/__init__.py
 src/pkgmt/assets/template/tests/conftest.py
 src/pkgmt/assets/template/tests/test_sample.py
 src/pkgmt/versioner/__init__.py
-src/pkgmt/versioner/abstractversioner.py
 src/pkgmt/versioner/util.py
-src/pkgmt/versioner/versionernonsetup.py
-src/pkgmt/versioner/versionersetup.py
+src/pkgmt/versioner/versioner.py
```

