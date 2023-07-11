# Comparing `tmp/types-flake8-bugbear-23.6.5.0.tar.gz` & `tmp/types-flake8-bugbear-23.7.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-bugbear-23.6.5.0.tar", last modified: Tue Jun  6 01:37:57 2023, max compression
+gzip compressed data, was "types-flake8-bugbear-23.7.10.0.tar", last modified: Tue Jul 11 09:16:17 2023, max compression
```

## Comparing `types-flake8-bugbear-23.6.5.0.tar` & `types-flake8-bugbear-23.7.10.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/bugbear-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/bugbear-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/bugbear-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/bugbear-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/bugbear-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/bugbear-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/top_level.txt
```

### Comparing `types-flake8-bugbear-23.6.5.0/CHANGELOG.md` & `types-flake8-bugbear-23.7.10.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 23.7.10.0 (2023-07-11)
+
+[stubsabot] Bump flake8-bugbear to 23.7.10 (#10434)
+
+Release: https://pypi.org/pypi/flake8-bugbear/23.7.10
+Homepage: https://github.com/PyCQA/flake8-bugbear
+Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
+Diff: https://github.com/PyCQA/flake8-bugbear/compare/23.6.5...23.7.10
+
+Stubsabot analysis of the diff between the two releases:
+ - 1 public Python file has been added: `tests/b034.py`.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 1 file included in typeshed's stubs has been modified or renamed: `bugbear.py`.
+ - Total lines of Python code added: 230.
+ - Total lines of Python code deleted: 91.
+
 ## 23.6.5.0 (2023-06-06)
 
 [stubsabot] Bump flake8-bugbear to 23.6.5 (#10265)
 
 Release: https://pypi.org/pypi/flake8-bugbear/23.6.5
 Homepage: https://github.com/PyCQA/flake8-bugbear
 Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
```

### Comparing `types-flake8-bugbear-23.6.5.0/PKG-INFO` & `types-flake8-bugbear-23.7.10.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.6.5.0
+Version: 23.7.10.0
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,8 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9d6e3564bb00e87304c93cacd3d365a908fe9fd5`.
+This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

### Comparing `types-flake8-bugbear-23.6.5.0/bugbear-stubs/__init__.pyi` & `types-flake8-bugbear-23.7.10.0/bugbear-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-bugbear-23.6.5.0/setup.py` & `types-flake8-bugbear-23.7.10.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9d6e3564bb00e87304c93cacd3d365a908fe9fd5`.
+This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="23.6.5.0",
+      version="23.7.10.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md",
```

### Comparing `types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/PKG-INFO` & `types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.6.5.0
+Version: 23.7.10.0
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,8 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9d6e3564bb00e87304c93cacd3d365a908fe9fd5`.
+This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

