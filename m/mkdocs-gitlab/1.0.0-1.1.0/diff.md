# Comparing `tmp/mkdocs_gitlab-1.0.0.tar.gz` & `tmp/mkdocs_gitlab-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_gitlab-1.0.0.tar", max compression
+gzip compressed data, was "mkdocs_gitlab-1.1.0.tar", max compression
```

## Comparing `mkdocs_gitlab-1.0.0.tar` & `mkdocs_gitlab-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-07-10 17:54:45.612761 mkdocs_gitlab-1.0.0/LICENSE
--rw-r--r--   0        0        0      786 2023-07-10 18:10:23.639650 mkdocs_gitlab-1.0.0/README.md
--rw-r--r--   0        0        0       62 2023-07-10 17:54:45.643499 mkdocs_gitlab-1.0.0/mkdocs_gitlab/__init__.py
--rw-r--r--   0        0        0       22 2023-07-10 17:54:45.641690 mkdocs_gitlab-1.0.0/mkdocs_gitlab/_version.py
--rw-r--r--   0        0        0     1268 2023-07-10 18:20:57.567797 mkdocs_gitlab-1.0.0/mkdocs_gitlab/plugin.py
--rw-r--r--   0        0        0        0 2023-07-10 17:54:45.645402 mkdocs_gitlab-1.0.0/mkdocs_gitlab/py.typed
--rw-r--r--   0        0        0     2283 2023-07-10 18:13:46.283111 mkdocs_gitlab-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/README.md
+-rw-r--r--   0        0        0       62 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/_version.py
+-rw-r--r--   0        0        0     1591 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/py.typed
+-rw-r--r--   0        0        0     2283 2023-07-11 08:55:32.930018 mkdocs_gitlab-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.1.0/PKG-INFO
```

### Comparing `mkdocs_gitlab-1.0.0/LICENSE` & `mkdocs_gitlab-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.0.0/pyproject.toml` & `mkdocs_gitlab-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.0"
+version = "1.1.0"
 tag_format = "$version"
 version_files = [
     "mkdocs_gitlab/_version.py",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "mkdocs-gitlab"
-version = "1.0.0"
+version = "1.1.0"
 description = "Use Gitlab CI variables for your docs"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/mkdocs-gitlab"
 homepage = "https://pypi.org/project/mkdocs-gitlab"
 keywords = []
```

### Comparing `mkdocs_gitlab-1.0.0/PKG-INFO` & `mkdocs_gitlab-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-gitlab
-Version: 1.0.0
+Version: 1.1.0
 Summary: Use Gitlab CI variables for your docs
 Home-page: https://pypi.org/project/mkdocs-gitlab
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,28 +20,30 @@
 # MkDocs Gitlab
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-gitlab)](https://pypi.org/project/mkdocs-gitlab/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-gitlab)](https://www.python.org/downloads/)
 [![GitHub last commit](https://img.shields.io/github/last-commit/daxartio/mkdocs-gitlab)](https://github.com/daxartio/mkdocs-gitlab)
 [![GitHub stars](https://img.shields.io/github/stars/daxartio/mkdocs-gitlab?style=social)](https://github.com/daxartio/mkdocs-gitlab)
 
+The plugin updates mkdocs config with Gitlab CI/CD variables.
+
+- CI_PROJECT_TITLE
+- CI_PROJECT_DESCRIPTION
+- CI_PAGES_URL
+- CI_PROJECT_URL
+- CI_PROJECT_PATH
+
 ## Installation
 
 ### pip
 
 ```
 pip install mkdocs-gitlab
 ```
 
-### poetry
-
-```
-poetry add mkdocs-gitlab
-```
-
 ## Usage
 
 ```yaml
 site_name: Title
 
 plugins:
 - mkdocs-gitlab
```

