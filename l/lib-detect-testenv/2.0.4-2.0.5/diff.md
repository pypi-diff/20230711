# Comparing `tmp/lib_detect_testenv-2.0.4.tar.gz` & `tmp/lib_detect_testenv-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_detect_testenv-2.0.4.tar", last modified: Mon Jun 26 20:04:01 2023, max compression
+gzip compressed data, was "lib_detect_testenv-2.0.5.tar", last modified: Tue Jul 11 20:56:14 2023, max compression
```

## Comparing `lib_detect_testenv-2.0.4.tar` & `lib_detect_testenv-2.0.5.tar`

### file list

```diff
@@ -1,25 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.439535 lib_detect_testenv-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-26 20:04:01.439535 lib_detect_testenv-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.435535 lib_detect_testenv-2.0.4/lib_detect_testenv/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.435535 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 20:04:01.439535 lib_detect_testenv-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.435535 lib_detect_testenv-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.980442 lib_detect_testenv-2.0.5/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.976442 lib_detect_testenv-2.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.980442 lib_detect_testenv-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.980442 lib_detect_testenv-2.0.5/lib_detect_testenv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/lib_detect_testenv/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/test_cli.py
```

### Comparing `lib_detect_testenv-2.0.4/CHANGES.rst` & `lib_detect_testenv-2.0.5/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-11:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
 2023-01-13:
```

### Comparing `lib_detect_testenv-2.0.4/LICENSE` & `lib_detect_testenv-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.4/PKG-INFO` & `lib_detect_testenv-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: lib_detect_testenv
-Version: 2.0.4
+Version: 2.0.5
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
-Home-page: https://github.com/bitranox/lib_detect_testenv
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_detect_testenv
+Project-URL: Documentation, https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_detect_testenv.git
+Project-URL: Changelog, https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.4 as of 2023-06-26 see `Changelog`_
+Version v2.0.5 as of 2023-07-11 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -53,36 +57,36 @@
    :target: https://codeclimate.com/github/bitranox/lib_detect_testenv/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_detect_testenv?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_detect_testenv
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_detect_testenv/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_detect_testenv
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-detect-testenv
    :target: https://pypi.org/project/lib-detect-testenv/
    :alt: PyPI - Downloads
 
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
 tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_detect_testenv>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -312,14 +316,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_detect_testenv
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_detect_testenv[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_detect_testenv.git
 
@@ -335,22 +346,22 @@
     # for the latest development version :
     lib_detect_testenv @ git+https://github.com/bitranox/lib_detect_testenv.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_detect_testenv.git
     $ cd lib_detect_testenv
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -401,14 +412,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-11:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
 2023-01-13:
```

### Comparing `lib_detect_testenv-2.0.4/README.rst` & `lib_detect_testenv-2.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_detect_testenv
 ==================
 
 
-Version v2.0.4 as of 2023-06-26 see `Changelog`_
+Version v2.0.5 as of 2023-07-11 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -35,36 +35,36 @@
    :target: https://codeclimate.com/github/bitranox/lib_detect_testenv/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_detect_testenv?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_detect_testenv
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_detect_testenv/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_detect_testenv
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-detect-testenv
    :target: https://pypi.org/project/lib-detect-testenv/
    :alt: PyPI - Downloads
 
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
 tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_detect_testenv>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -294,14 +294,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_detect_testenv
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_detect_testenv[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_detect_testenv.git
 
@@ -317,22 +324,22 @@
     # for the latest development version :
     lib_detect_testenv @ git+https://github.com/bitranox/lib_detect_testenv.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_detect_testenv.git
     $ cd lib_detect_testenv
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -383,14 +390,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-11:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
 2023-01-13:
```

### Comparing `lib_detect_testenv-2.0.4/lib_detect_testenv/__init__.py` & `lib_detect_testenv-2.0.5/lib_detect_testenv/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv.py` & `lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv_cli.py` & `lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)  # type: ignore
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
@@ -46,13 +46,13 @@
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()  # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/PKG-INFO` & `lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: lib-detect-testenv
-Version: 2.0.4
+Version: 2.0.5
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
-Home-page: https://github.com/bitranox/lib_detect_testenv
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_detect_testenv
+Project-URL: Documentation, https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_detect_testenv.git
+Project-URL: Changelog, https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.4 as of 2023-06-26 see `Changelog`_
+Version v2.0.5 as of 2023-07-11 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -53,36 +57,36 @@
    :target: https://codeclimate.com/github/bitranox/lib_detect_testenv/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_detect_testenv?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_detect_testenv
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_detect_testenv/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_detect_testenv
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-detect-testenv
    :target: https://pypi.org/project/lib-detect-testenv/
    :alt: PyPI - Downloads
 
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
 tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_detect_testenv>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -312,14 +316,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_detect_testenv
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_detect_testenv[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_detect_testenv.git
 
@@ -335,22 +346,22 @@
     # for the latest development version :
     lib_detect_testenv @ git+https://github.com/bitranox/lib_detect_testenv.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_detect_testenv.git
     $ cd lib_detect_testenv
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -401,14 +412,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-11:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
 2023-01-13:
```

### Comparing `lib_detect_testenv-2.0.4/tests/test_cli.py` & `lib_detect_testenv-2.0.5/tests/test_cli.py`

 * *Files identical despite different names*

