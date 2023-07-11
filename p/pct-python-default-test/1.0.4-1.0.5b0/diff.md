# Comparing `tmp/pct_python_default_test-1.0.4.tar.gz` & `tmp/pct_python_default_test-1.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pct_python_default_test-1.0.4.tar", last modified: Mon Jun 26 21:27:53 2023, max compression
+gzip compressed data, was "pct_python_default_test-1.0.5b0.tar", last modified: Tue Jul 11 20:36:03 2023, max compression
```

## Comparing `pct_python_default_test-1.0.4.tar` & `pct_python_default_test-1.0.5b0.tar`

### file list

```diff
@@ -1,25 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/pct_python_default_test/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.362866 pct_python_default_test-1.0.5b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/lib_detect_testenv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/lib_detect_testenv/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/lib_detect_testenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/lib_detect_testenv_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/test_cli.py
```

### Comparing `pct_python_default_test-1.0.4/CHANGES.rst` & `pct_python_default_test-1.0.5b0/CHANGES.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,67 @@
 Changelog
----------
+=========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
-v1.0.4
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
+v2.0.4
 ---------
-2023-06-26:
-    - correct black settings
-    - get rid of travis
-    - do not upload .egg files to pypi.org
+2023-06-26: suppress upload of .egg files to pypi.org
 
-v1.0.3
+v2.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
     - update to pypy 3.9 tests
 
-v1.0.2
+v2.0.2.2
+---------
+2022-06-02: update to github actions checkout@v3 and setup-python@v3
+
+v2.0.2.1
 --------
-2022-05-20: update github actions test matrix to python 3.10
+2022-06-01: update github actions test matrix
 
-v1.0.1
+v2.0.2
 --------
 2022-03-29: remedy mypy Untyped decorator makes function "cli_info" untyped
 
-v1.0.0
----------
-2022-03-25: remove listdir of ./dist, moved to lib_cicd_github
+v2.0.1
+--------
+2022-03-25: fix github actions windows test
 
-v0.1.1
----------
-2020-08-01: fix pypi deploy
+v2.0.0
+-------
+2021-11-23:
+    - add "setup.py test" detection
 
-v0.1.0
---------
-2020-07-31:
-    - change1
-    - change2
-    - ...
+v1.0.2
+-------
+2021-11-22:
+    - remove second github action yml
+    - fix "setup.py test"
+
+v1.0.1
+------
+2021-11-21: implement github actions
+
+v1.0.0
+------
+2021-11-19: initial release
```

### Comparing `pct_python_default_test-1.0.4/LICENSE` & `pct_python_default_test-1.0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test_cli.py` & `pct_python_default_test-1.0.5b0/lib_detect_testenv/lib_detect_testenv_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,52 +7,52 @@
 
 # OWN
 import cli_exit_tools
 
 # PROJ
 try:
     from . import __init__conf__
-    from . import pct_python_default_test
+    from . import lib_detect_testenv
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
     # imports for doctest
     import __init__conf__  # type: ignore  # pragma: no cover
-    import pct_python_default_test  # type: ignore  # pragma: no cover
+    import lib_detect_testenv  # type: ignore  # pragma: no cover
 
 # CONSTANTS
 CLICK_CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 def info() -> None:
     """
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
-        pct_python_default_test.main()
+        # lib_detect_testenv.main()
 
 
 @cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)  # type: ignore
 def cli_info() -> None:
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

### Comparing `pct_python_default_test-1.0.4/tests/test_cli.py` & `pct_python_default_test-1.0.5b0/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # STDLIB
 import logging
+import os
 import pathlib
 import subprocess
 import sys
 
 logger = logging.getLogger()
-package_dir = "pct_python_default_test"
-cli_filename = "pct_python_default_test_cli.py"
+package_dir = "lib_detect_testenv"
+cli_filename = "lib_detect_testenv_cli.py"
+os.environ["PYTEST_IS_RUNNING"] = "True"  # to be able to detect pytest when running the cli command
 
 path_cli_command = pathlib.Path(__file__).resolve().parent.parent / package_dir / cli_filename
 
 
 def call_cli_command(commandline_args: str = "") -> bool:
     command = " ".join([sys.executable, str(path_cli_command), commandline_args])
     try:
         subprocess.run(command, shell=True, check=True)
     except subprocess.CalledProcessError:
         return False
     return True
 
 
 def test_cli_commands() -> None:
-    # due to a bug in python 3.8.1 with setup.py test we need to cancel the click tests there !
+    # due to a bug in python 3.8.1 with setup.py test on travis we need to cancel the click tests there !
     if sys.version_info < (3, 8, 1) or sys.version_info >= (3, 8, 2):
         assert not call_cli_command("--unknown_option")
         assert call_cli_command("--version")
         assert call_cli_command("-h")
         assert call_cli_command("info")
         assert call_cli_command("--traceback info")
```

