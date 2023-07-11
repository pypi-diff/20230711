# Comparing `tmp/pynldas2-0.15.0.tar.gz` & `tmp/pynldas2-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynldas2-0.15.0.tar", last modified: Mon May  8 15:16:26 2023, max compression
+gzip compressed data, was "pynldas2-0.15.1.tar", last modified: Tue Jul 11 03:07:42 2023, max compression
```

## Comparing `pynldas2-0.15.0.tar` & `pynldas2-0.15.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-08 15:16:09.000000 pynldas2-0.15.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 15:16:09.000000 pynldas2-0.15.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-08 15:16:09.000000 pynldas2-0.15.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-08 15:16:09.000000 pynldas2-0.15.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 15:16:09.000000 pynldas2-0.15.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-08 15:16:09.000000 pynldas2-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 15:16:09.000000 pynldas2-0.15.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-05-08 15:16:26.813196 pynldas2-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-08 15:16:09.000000 pynldas2-0.15.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.809196 pynldas2-0.15.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-08 15:16:09.000000 pynldas2-0.15.0/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 15:16:09.000000 pynldas2-0.15.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 15:16:09.000000 pynldas2-0.15.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-08 15:16:09.000000 pynldas2-0.15.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/pynldas2/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/pynldas2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/pynldas2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:16:26.813196 pynldas2-0.15.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-08 15:16:09.000000 pynldas2-0.15.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 15:16:09.000000 pynldas2-0.15.0/tests/test_pynldas2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.799253 pynldas2-0.15.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.791253 pynldas2-0.15.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.795253 pynldas2-0.15.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.795253 pynldas2-0.15.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 03:07:22.000000 pynldas2-0.15.1/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 03:07:22.000000 pynldas2-0.15.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 03:07:22.000000 pynldas2-0.15.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-11 03:07:22.000000 pynldas2-0.15.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-11 03:07:22.000000 pynldas2-0.15.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-11 03:07:22.000000 pynldas2-0.15.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-11 03:07:22.000000 pynldas2-0.15.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 03:07:22.000000 pynldas2-0.15.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-11 03:07:42.795253 pynldas2-0.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-11 03:07:22.000000 pynldas2-0.15.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.787253 pynldas2-0.15.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.795253 pynldas2-0.15.1/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-11 03:07:22.000000 pynldas2-0.15.1/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 03:07:22.000000 pynldas2-0.15.1/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 03:07:22.000000 pynldas2-0.15.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-11 03:07:22.000000 pynldas2-0.15.1/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.795253 pynldas2-0.15.1/pynldas2/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 03:07:22.000000 pynldas2-0.15.1/pynldas2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-11 03:07:22.000000 pynldas2-0.15.1/pynldas2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-11 03:07:22.000000 pynldas2-0.15.1/pynldas2/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:22.000000 pynldas2-0.15.1/pynldas2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20766 2023-07-11 03:07:22.000000 pynldas2-0.15.1/pynldas2/pynldas2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.795253 pynldas2-0.15.1/pynldas2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-11 03:07:42.000000 pynldas2-0.15.1/pynldas2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-11 03:07:42.000000 pynldas2-0.15.1/pynldas2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:07:42.000000 pynldas2-0.15.1/pynldas2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:07:42.000000 pynldas2-0.15.1/pynldas2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 03:07:42.000000 pynldas2-0.15.1/pynldas2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 03:07:42.000000 pynldas2-0.15.1/pynldas2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-11 03:07:22.000000 pynldas2-0.15.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 03:07:42.799253 pynldas2-0.15.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:07:42.795253 pynldas2-0.15.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-11 03:07:22.000000 pynldas2-0.15.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-11 03:07:22.000000 pynldas2-0.15.1/tests/test_pynldas2.py
```

### Comparing `pynldas2-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml` & `pynldas2-0.15.1/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml` & `pynldas2-0.15.1/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/.github/workflows/codeql-analysis.yml` & `pynldas2-0.15.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/.github/workflows/release.yml` & `pynldas2-0.15.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/.github/workflows/test.yml` & `pynldas2-0.15.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/.gitignore` & `pynldas2-0.15.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/.pre-commit-config.yaml` & `pynldas2-0.15.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -11,27 +11,27 @@
   - id: check-toml
   - id: check-yaml
   - id: debug-statements
   - id: mixed-line-ending
     args: [--fix=lf]
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 0.11.1
+  rev: 0.10.0
   hooks:
   - id: pyproject-fmt
     name: Apply a consistent format to pyproject.toml
 
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.8.0
+  rev: v2.9.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
 
 - repo: https://github.com/hadialqattan/pycln
-  rev: v2.1.3
+  rev: v2.1.5
   hooks:
   - id: pycln
     name: Find and remove unused import statements with pycln
     args: [--config=pyproject.toml]
 
 - repo: https://github.com/bwhmather/ssort
   rev: v0.11.6
@@ -54,23 +54,23 @@
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
     name: Autoformat with black
 
 - repo: https://github.com/asottile/blacken-docs
-  rev: 1.13.0
+  rev: 1.15.0
   hooks:
   - id: blacken-docs
     name: Autoformat codes in docstrings with blacken-docs
     additional_dependencies: [black]
     args: [-t, py38, -l, '100']
 
 - repo: https://github.com/guilatrova/tryceratops
-  rev: v2.0.0
+  rev: v2.3.2
   hooks:
   - id: tryceratops
     name: Check try-exceptions blocks with tryceratops
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
@@ -83,23 +83,23 @@
   rev: v1.1.1
   hooks:
   - id: doc8
     name: Check documentation formats with doc8
     args: [--max-line-length, '100']
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.5
   hooks:
   - id: codespell
     name: Check common misspellings in text files with codespell.
     additional_dependencies:
     - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.2
+  rev: v3.9.0
   hooks:
   - id: pyupgrade
     name: Upgrade sytnax to python 3.8+ with pyupgrade
     args: [--py38-plus]
 
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
@@ -115,15 +115,15 @@
     - flake8-docstrings
     - flake8-type-checking
     - flake8-simplify
     - flake8-print
     - pep8-naming
 
 - repo: https://github.com/dosisod/refurb
-  rev: v1.16.0
+  rev: v1.17.0
   hooks:
   - id: refurb
     name: Modernizing Python codebases using Refurb
     additional_dependencies:
     - numpy
 
 - repo: https://github.com/PyCQA/bandit
```

### Comparing `pynldas2-0.15.0/CITATION.cff` & `pynldas2-0.15.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/CODE_OF_CONDUCT.rst` & `pynldas2-0.15.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/CONTRIBUTING.rst` & `pynldas2-0.15.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/HISTORY.rst` & `pynldas2-0.15.1/HISTORY.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 =======
 History
 =======
 
+0.15.1 (2023-07-10)
+-------------------
+
+Bug Fixes
+~~~~~~~~~
+- Fix a bug in computing snow where the ``t_snow`` argument was not
+  being converted to Kelvin.
+
+New Features
+~~~~~~~~~~~~
+- If ``snow=True`` is passed to both ``get_bygeom`` and ``get_bycoords``
+  functions, the ``variables`` argument will be checked to see if it
+  contains ``prcp`` and ``temp``, if not, they will be added to the
+  list of variables to be retrieved. This is to ensure that the
+  ``snow`` argument works as expected.
+
 0.15.0 (2023-05-07)
 -------------------
 From release 0.15 onward, all minor versions of HyRiver packages
 will be pinned. This ensures that previous minor versions of HyRiver
 packages cannot be installed with later minor releases. For example,
 if you have ``py3dep==0.14.x`` installed, you cannot install
 ``pydaymet==0.15.x``. This is to ensure that the API is
@@ -17,17 +33,15 @@
   Valid values for source are ``grib`` (default) and ``netcdf``.
   Both return the same values, the latter also offers additional variable ``psurf``
   for surface pressure.
   Valid variable names for ``netcdf`` are:
   ``prcp``, ``pet``, ``wind_u``, ``wind_v``, ``humidity``,
   ``temp``, ``rsds``, ``rlds``, ``psurf``
   Valid variable names for ``grib`` source are unchanged as to not
-  introduce breaking changes.
-
-By `Luc Rébillout <https://github.com/LucRSquared>`__.
+  introduce breaking changes. By `Luc Rébillout <https://github.com/LucRSquared>`__.
 - For now, retain compatibility with ``shapely<2`` while supporting
   ``shapley>=2``.
 
 0.14.0 (2023-03-05)
 -------------------
 
 New Features
```

### Comparing `pynldas2-0.15.0/LICENSE` & `pynldas2-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/PKG-INFO` & `pynldas2-0.15.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynldas2
-Version: 0.15.0
+Version: 0.15.1
 Summary: Get NLDAS2 forcing data.
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pynldas2/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pynldas2.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pynldas2.html
 Project-URL: Issues, https://github.com/hyriver/pynldas2/issues
```

### Comparing `pynldas2-0.15.0/README.rst` & `pynldas2-0.15.1/README.rst`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/ci/requirements/environment-dev.yml` & `pynldas2-0.15.1/ci/requirements/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/ci/requirements/environment.yml` & `pynldas2-0.15.1/ci/requirements/environment.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/noxfile.py` & `pynldas2-0.15.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/pynldas2/__init__.py` & `pynldas2-0.15.1/pynldas2/__init__.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/pynldas2/exceptions.py` & `pynldas2-0.15.1/pynldas2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/pynldas2/print_versions.py` & `pynldas2-0.15.1/pynldas2/print_versions.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/pynldas2/pynldas2.py` & `pynldas2-0.15.1/pynldas2/pynldas2.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import functools
 import itertools
 import re
 import warnings
 from io import BytesIO, StringIO
-from typing import TYPE_CHECKING, Sequence, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Sequence, TypeVar, Union
 
 import async_retriever as ar
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pygeoutils as hgu
 import pyproj
@@ -21,15 +21,15 @@
 from pynldas2.exceptions import InputRangeError, InputTypeError, InputValueError, NLDASServiceError
 
 try:
     from numba import config as numba_config
     from numba import njit, prange
 
     ngjit = functools.partial(njit, cache=True, nogil=True)
-    numba_config.THREADING_LAYER = "workqueue"
+    numba_config.THREADING_LAYER = "workqueue"  # pyright: ignore[reportGeneralTypeIssues]
     has_numba = True
 except ImportError:
     has_numba = False
     prange = range
     numba_config = None
     njit = None
 
@@ -199,17 +199,17 @@
     """Separate snow based on :footcite:t:`Martinez_2010`.
 
     Parameters
     ----------
     clm : pandas.DataFrame or xarray.Dataset
         Climate data that should include ``prcp`` and ``temp``.
     t_rain : float, optional
-        Threshold for temperature for considering rain, defaults to 2.5 degrees C.
+        Threshold for temperature in deg C for considering rain, defaults to 2.5 degrees C.
     t_snow : float, optional
-        Threshold for temperature for considering snow, defaults to 0.6 degrees C.
+        Threshold for temperature in deg C for considering snow, defaults to 0.6 degrees C.
 
     Returns
     -------
     pandas.DataFrame or xarray.Dataset
         Input data with ``snow`` column if input is a ``pandas.DataFrame``,
         or ``snow`` variable if input is an ``xarray.Dataset``.
 
@@ -222,16 +222,16 @@
             "Numba not installed. Using slow pure python version.", UserWarning, stacklevel=2
         )
 
     if not isinstance(clm, (pd.DataFrame, xr.Dataset)):
         raise InputTypeError("clm", "pandas.DataFrame or xarray.Dataset")
 
     if isinstance(clm, xr.Dataset):
-        return _snow_gridded(clm, t_rain + 273.15, t_snow)  # type: ignore
-    return _snow_point(clm, t_rain + 273.15, t_snow)
+        return _snow_gridded(clm, t_rain + 273.15, t_snow + 273.15)  # type: ignore
+    return _snow_point(clm, t_rain + 273.15, t_snow + 273.15)
 
 
 def _txt2df(
     txt: str,
     resp_id: int,
     kwds: list[dict[str, dict[str, str]]],
     source: str = "grib",
@@ -284,15 +284,18 @@
     else:
         raise InputValueError("source", ["grib", "netcdf"])
 
     if variables is None:
         clm_vars = [f"{source_tag}:{d['nldas_name']}" for d in nldas_vars.values()]
     else:
         clm_vars = [variables] if isinstance(variables, str) else list(variables)
-        clm_vars = clm_vars + ["temp"] if snow and "temp" not in clm_vars else clm_vars
+        if snow:
+            required_vars = ["temp", "prcp"]
+            if not all(v in clm_vars for v in required_vars):
+                clm_vars = list(set(clm_vars).union(required_vars))
         if any(v not in nldas_vars for v in clm_vars):
             raise InputValueError("variables", list(nldas_vars))
         clm_vars = [f"{source_tag}:{nldas_vars[v]['nldas_name']}" for v in clm_vars]
 
     return dates, clm_vars, nldas_vars
 
 
@@ -444,17 +447,17 @@
         for v in clm_ds.data_vars:
             clm_ds[v].attrs = nldas_vars[str(v)]
         return clm_ds
 
     if n_pts == 1:
         clm = next(iter(clm_list), pd.DataFrame())
     else:
-        clm = cast("pd.DataFrame", pd.concat(clm_list, keys=idx, axis=1))
+        clm = pd.concat(clm_list, keys=idx, axis=1)
         clm.columns = clm.columns.set_names(["id", "variable"])
-    clm.index = clm.index.tz_localize("UTC")
+    clm.index = pd.DatetimeIndex(clm.index, tz="UTC")
     clm.index.name = "time"
     return clm
 
 
 def get_grid_mask():
     """Get the NLDAS2 grid that contains the land/water/soil/vegetation mask.
```

### Comparing `pynldas2-0.15.0/pynldas2.egg-info/PKG-INFO` & `pynldas2-0.15.1/pynldas2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynldas2
-Version: 0.15.0
+Version: 0.15.1
 Summary: Get NLDAS2 forcing data.
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pynldas2/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pynldas2.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pynldas2.html
 Project-URL: Issues, https://github.com/hyriver/pynldas2/issues
```

### Comparing `pynldas2-0.15.0/pynldas2.egg-info/SOURCES.txt` & `pynldas2-0.15.1/pynldas2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/pyproject.toml` & `pynldas2-0.15.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
   "Topic :: Scientific/Engineering :: Hydrology",
   "Typing :: Typed",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "async-retriever==0.15",
+  "async-retriever<0.16,>=0.15",
   "h5netcdf",
   "numpy>=1.21",
   "pandas>=1",
-  "pygeoutils==0.15",
+  "pygeoutils<0.16,>=0.15",
   "pyproj>=3.0.1",
   "rioxarray>=0.11",
   "xarray>=2022.03",
 ]
 [project.optional-dependencies]
 speedup = [
   "numba",
```

### Comparing `pynldas2-0.15.0/tests/test_exceptions.py` & `pynldas2-0.15.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.15.0/tests/test_pynldas2.py` & `pynldas2-0.15.1/tests/test_pynldas2.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,23 +67,23 @@
 
 
 @pytest.mark.speedup
 def test_snow():
     clm = nldas.get_bycoords(
         (-89.6, 48.3), "2000-01-01", "2000-01-02", crs=DEF_CRS, variables="prcp", snow=True
     )
-    assert_close(clm.snow.mean(), 0.0017)
+    assert_close(clm.snow.mean(), 0.0458)
     clm = nldas.get_bygeom(
         Point(-89.6, 48.3).buffer(0.05),
         "2000-01-01",
         "2000-01-02",
         DEF_CRS,
         "prcp",
         snow=True,
     )
-    assert_close(clm.snow.mean().compute().item(), 0.00163)
+    assert_close(clm.snow.mean().compute().item(), 0.04287)
 
 
 def test_show_versions():
     f = io.StringIO()
     nldas.show_versions(file=f)
     assert "SYS INFO" in f.getvalue()
```

