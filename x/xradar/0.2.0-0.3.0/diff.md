# Comparing `tmp/xradar-0.2.0.tar.gz` & `tmp/xradar-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xradar-0.2.0.tar", last modified: Fri Mar 24 14:55:51 2023, max compression
+gzip compressed data, was "xradar-0.3.0.tar", last modified: Tue Jul 11 08:38:03 2023, max compression
```

## Comparing `xradar-0.2.0.tar` & `xradar-0.3.0.tar`

### file list

```diff
@@ -1,107 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.740777 xradar-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-24 14:55:35.000000 xradar-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.732777 xradar-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 14:55:35.000000 xradar-0.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 14:55:35.000000 xradar-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.732777 xradar-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-03-24 14:55:35.000000 xradar-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-24 14:55:35.000000 xradar-0.2.0/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-24 14:55:35.000000 xradar-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-24 14:55:35.000000 xradar-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-24 14:55:35.000000 xradar-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 14:55:35.000000 xradar-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-24 14:55:35.000000 xradar-0.2.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-24 14:55:35.000000 xradar-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-24 14:55:35.000000 xradar-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-24 14:55:35.000000 xradar-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-24 14:55:35.000000 xradar-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-03-24 14:55:51.740777 xradar-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-03-24 14:55:35.000000 xradar-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.732777 xradar-0.2.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-24 14:55:35.000000 xradar-0.2.0/ci/unittests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.732777 xradar-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.732777 xradar-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/_static/openradar_micro.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/_static/openradar_mini.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/_static/xradar_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/authors.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/datamodel.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/exporters.md
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/importers.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/links.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-24 14:55:35.000000 xradar-0.2.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-24 14:55:35.000000 xradar-0.2.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.728777 xradar-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/examples/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/Accessors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/CfRadial1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16177 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/CfRadial1_Model_Transformation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/Furuno.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/GAMIC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/Iris.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/Multi-Volume-Concatenation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/ODIM_H5.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/Rainbow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/angle_reindexing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-03-24 14:55:35.000000 xradar-0.2.0/examples/notebooks/plot-ppi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-24 14:55:35.000000 xradar-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 14:55:35.000000 xradar-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 14:55:35.000000 xradar-0.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 14:55:51.740777 xradar-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/tests/georeference/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/georeference/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/georeference/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/io/test_furuno.py
--rw-r--r--   0 runner    (1001) docker     (123)    22257 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/io/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/io/test_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/io/test_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-24 14:55:35.000000 xradar-0.2.0/tests/test_xradar.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-24 14:55:35.000000 xradar-0.2.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/xradar/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/accessors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/xradar/georeference/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/georeference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/georeference/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/georeference/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.740777 xradar-0.2.0/xradar/io/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.740777 xradar-0.2.0/xradar/io/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/cfradial1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    24715 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/furuno.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/gamic.py
--rw-r--r--   0 runner    (1001) docker     (123)   121487 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/odim.py
--rw-r--r--   0 runner    (1001) docker     (123)    27581 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/backends/rainbow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.740777 xradar-0.2.0/xradar/io/export/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/export/cfradial2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/io/export/odim.py
--rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-24 14:55:35.000000 xradar-0.2.0/xradar/xradar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:55:51.736777 xradar-0.2.0/xradar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-24 14:55:51.000000 xradar-0.2.0/xradar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-11 08:37:48.000000 xradar-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.731847 xradar-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 08:37:48.000000 xradar-0.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 08:37:48.000000 xradar-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.731847 xradar-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-11 08:37:48.000000 xradar-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 08:37:48.000000 xradar-0.3.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-11 08:37:48.000000 xradar-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 08:37:48.000000 xradar-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 08:37:48.000000 xradar-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 08:37:48.000000 xradar-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-11 08:37:48.000000 xradar-0.3.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-11 08:37:48.000000 xradar-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-11 08:37:48.000000 xradar-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 08:37:48.000000 xradar-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-11 08:37:48.000000 xradar-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-11 08:38:03.739847 xradar-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-11 08:37:48.000000 xradar-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.731847 xradar-0.3.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-11 08:37:48.000000 xradar-0.3.0/ci/notebooktests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-11 08:37:48.000000 xradar-0.3.0/ci/unittests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.735847 xradar-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.735847 xradar-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/_static/openradar_micro.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/_static/openradar_mini.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/_static/xradar_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/authors.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/datamodel.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/exporters.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/importers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-11 08:37:48.000000 xradar-0.3.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 08:37:48.000000 xradar-0.3.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.731847 xradar-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.735847 xradar-0.3.0/examples/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/Accessors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/CfRadial1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16177 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/CfRadial1_Model_Transformation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/Furuno.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/GAMIC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/Iris.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/Multi-Volume-Concatenation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/ODIM_H5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/Rainbow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/Read-plot-Sigmet-data-from-AWS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/angle_reindexing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/multiple-sweeps-into-volume-scan.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-11 08:37:48.000000 xradar-0.3.0/examples/notebooks/plot-ppi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-11 08:37:48.000000 xradar-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 08:37:48.000000 xradar-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 08:37:48.000000 xradar-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:38:03.739847 xradar-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.735847 xradar-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.735847 xradar-0.3.0/tests/georeference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/georeference/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/georeference/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/io/test_furuno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22257 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/io/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/io/test_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/io/test_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 08:37:48.000000 xradar-0.3.0/tests/test_xradar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 08:37:48.000000 xradar-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/xradar/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/accessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/xradar/georeference/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/georeference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/georeference/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/georeference/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/xradar/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/xradar/io/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/cfradial1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/furuno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17876 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/gamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122162 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26983 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/odim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27663 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/backends/rainbow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/xradar/io/export/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/export/cfradial2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/io/export/odim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29559 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 08:37:48.000000 xradar-0.3.0/xradar/xradar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:03.739847 xradar-0.3.0/xradar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 08:38:03.000000 xradar-0.3.0/xradar.egg-info/top_level.txt
```

### Comparing `xradar-0.2.0/.github/workflows/ci.yml` & `xradar-0.3.0/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -32,56 +32,98 @@
   build_0:
     name: xradar unit tests - linux
     runs-on: ubuntu-latest
     needs: [lint]
     defaults:
       run:
         shell: bash -l {0}
+    env:
+      CONDA_ENV_FILE: ci/unittests.yml
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9", "3.10", "3.11"]
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Install micromamba environment
-      uses: mamba-org/provision-with-micromamba@main
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-name: xradar-tests
-        environment-file: ci/unittests.yml
-        extra-specs: |
-          python=${{ matrix.python-version }}
+          environment-name: xradar-unit-tests
+          environment-file: ${{env.CONDA_ENV_FILE}}
+          cache-environment: true
+          cache-environment-key: "${{runner.os}}-${{runner.arch}}-py${{env.PYTHON_VERSION}}-${{env.TODAY}}-${{hashFiles(env.CONDA_ENV_FILE)}}"
+          create-args: >-
+              python=${{matrix.python-version}}
+              conda
     - name: Install xradar
       run: |
         python -m pip install . --no-deps
     - name: Version Info
       run: |
         python -c "import xradar; print(xradar.version.version)"
     - name: Test with pytest
       run: |
         pytest -n auto --dist loadfile --verbose --durations=15 --cov-report xml:coverage_unit.xml --cov=xradar --pyargs tests
-        pytest -n auto --dist loadfile --verbose --durations=15 --cov-report xml:coverage_notebooks.xml --cov=xradar --pyargs examples/notebooks
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         file: ./coverage_unit.xml
         flags: unittests
         env_vars: RUNNER_OS,PYTHON_VERSION
         name: codecov-gha
         fail_ci_if_error: false
+
+  build_1:
+    name: xradar notebook tests - linux
+    runs-on: ubuntu-latest
+    needs: [lint]
+    defaults:
+      run:
+        shell: bash -l {0}
+    env:
+      CONDA_ENV_FILE: ci/notebooktests.yml
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.9", "3.10", "3.11"]
+    steps:
+    - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
+    - name: Install micromamba environment
+      uses: mamba-org/setup-micromamba@v1
+      with:
+          environment-name: xradar-notebook-tests
+          environment-file: ${{env.CONDA_ENV_FILE}}
+          cache-environment: true
+          cache-environment-key: "${{runner.os}}-${{runner.arch}}-py${{env.PYTHON_VERSION}}-${{env.TODAY}}-${{hashFiles(env.CONDA_ENV_FILE)}}"
+          create-args: >-
+              python=${{matrix.python-version}}
+              conda
+    - name: Install xradar
+      run: |
+        python -m pip install . --no-deps
+    - name: Version Info
+      run: |
+        python -c "import xradar; print(xradar.version.version)"
+    - name: Test with pytest
+      run: |
+        pytest -n auto --dist loadfile --verbose --durations=15 --cov-report xml:coverage_notebooks.xml --cov=xradar --pyargs examples/notebooks
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         file: ./coverage_notebook.xml
         flags: notebooktests
         env_vars: RUNNER_OS,PYTHON_VERSION
         name: codecov-gha
         fail_ci_if_error: false
 
+
   test_build_distribution_testpypi:
     name: test build distribution for testpypi
     needs: [lint, build_0]
     runs-on: ubuntu-latest
     defaults:
       run:
         shell: bash -l {0}
```

### Comparing `xradar-0.2.0/.github/workflows/upload_pypi.yml` & `xradar-0.3.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/.gitignore` & `xradar-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/.pre-commit-config.yaml` & `xradar-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/CITATION.cff` & `xradar-0.3.0/CITATION.cff`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # YAML 1.2
 # Metadata for citation of this software according to the CFF format (https://citation-file-format.github.io/)
 cff-version: 1.0.3
 message: If you use this software, please cite it using these metadata.
 # FIXME title as repository name might not be the best name, please make human readable
-title: 'openradar/xradar: xradar v0.2.0'
+title: 'openradar/xradar: xradar v0.3.0'
 doi: 10.5281/zenodo.7091737
 # FIXME splitting of full names is error prone, please check if given/family name are correct
 authors:
 - given-names: Max
   family-names: Grover
   affiliation: Argonne National Laboratory
   orcid: https://orcid.org/0000-0002-0370-8974
@@ -15,11 +15,11 @@
   family-names: Mühlbauer
   affiliation: University Bonn
   orcid: https://orcid.org/0000-0001-6599-1034
 - given-names: Edouard
   family-names: Goudenhoofdt
   affiliation: Royal Meteorological Institute of Belgium
   orcid: https://orcid.org/0000-0002-6376-1515
-version: 0.2.0
-date-released: 2023-03-24
+version: 0.3.0
+date-released: 2023-07-11
 repository-code: https://github.com/openradar/xradar
 license: MIT
```

### Comparing `xradar-0.2.0/CONTRIBUTING.md` & `xradar-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/LICENSE` & `xradar-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/Makefile` & `xradar-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/PKG-INFO` & `xradar-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xradar
-Version: 0.2.0
+Version: 0.3.0
 Summary: Xradar includes all the tools to get your weather radar into the xarray data model.
 Author-email: Maxwell Grover <mgrover@anl.gov>, Kai Mühlbauer <kai.muehlbauer@uni-bonn.de>, Zachary Sherman <zsherman@anl.gov>
 License: MIT License
         
         Copyright (c) 2022-2023, Open Radar Community Developers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # xradar
 
 [![PyPI Version](https://img.shields.io/pypi/v/xradar.svg)](https://pypi.python.org/pypi/xradar)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/xradar.svg)](https://anaconda.org/conda-forge/xradar)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7091737.svg)](https://doi.org/10.5281/zenodo.7091737)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7767521.svg)](https://doi.org/10.5281/zenodo.7767521)
 
 [![CI](https://github.com/openradar/xradar/actions/workflows/ci.yml/badge.svg)](https://github.com/openradar/xradar/actions/workflows/ci.yml)
 [![Build distribution](https://github.com/openradar/xradar/actions/workflows/upload_pypi.yml/badge.svg)](https://github.com/openradar/xradar/actions/workflows/upload_pypi.yml)
 [![RTD Version](https://readthedocs.org/projects/xradar/badge/?version=latest)](https://xradar.readthedocs.io/en/latest/?version=latest)
 
 Xradar includes all the tools to get your weather radar into the xarray data model.
 
@@ -88,14 +88,23 @@
 * Import Iris/Sigmet
 * Import Furuno SCN/SCNX
 * Georeferencing (AEQD)
 * Angle Reindexing
 
 # History
 
+## 0.3.0 (2023-07-11)
+* ENH: Add new examples using radar data on AWS s3 bucket ({pull}`102`) by [@aladinor](https://github.com/aladinor)
+* FIX: Correct DB_DBTE8/DB_DBZE8 and DB_DBTE16/DB_DBZE16 decoding for iris-backend ({pull}`110`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: Cast boolean string to int in rainbow dictionary ({pull}`113`) by [@egouden](https://github.com/egouden)
+* MNT: switch to mamba-org/setup-micromamba, split CI tests ({issue}`115`), ({pull}`116`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: time interpolation ({pull}`117`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: robust ``angle_res`` retrieval in ``extract_angle_parameters`` ({issue}`112`), ({pull}`118`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: robust radar identifier in ``to_odim()`` ({pull}`120`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+
 ## 0.2.0 (2023-03-24)
 
 * ENH: switch to add optional how attributes in ODIM format writer ({pull}`97`) by [@egouden](https://github.com/egouden)
 * FIX: add keyword argument for mandatory source attribute in ODIM format writer ({pull}`96`) by [@egouden](https://github.com/egouden)
 * FIX: check for dim0 if not given, only swap_dims if needed ({issue}`92`), ({pull}`94`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
 * FIX+ENH: need array copy before overwriting and make compression available in to_odim ({pull}`95`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
```

### Comparing `xradar-0.2.0/README.md` & `xradar-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # xradar
 
 [![PyPI Version](https://img.shields.io/pypi/v/xradar.svg)](https://pypi.python.org/pypi/xradar)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/xradar.svg)](https://anaconda.org/conda-forge/xradar)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7091737.svg)](https://doi.org/10.5281/zenodo.7091737)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7767521.svg)](https://doi.org/10.5281/zenodo.7767521)
 
 [![CI](https://github.com/openradar/xradar/actions/workflows/ci.yml/badge.svg)](https://github.com/openradar/xradar/actions/workflows/ci.yml)
 [![Build distribution](https://github.com/openradar/xradar/actions/workflows/upload_pypi.yml/badge.svg)](https://github.com/openradar/xradar/actions/workflows/upload_pypi.yml)
 [![RTD Version](https://readthedocs.org/projects/xradar/badge/?version=latest)](https://xradar.readthedocs.io/en/latest/?version=latest)
 
 Xradar includes all the tools to get your weather radar into the xarray data model.
```

### Comparing `xradar-0.2.0/docs/Makefile` & `xradar-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/_static/openradar_micro.svg` & `xradar-0.3.0/docs/_static/openradar_micro.svg`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/_static/openradar_mini.svg` & `xradar-0.3.0/docs/_static/openradar_mini.svg`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/_static/xradar_logo.svg` & `xradar-0.3.0/docs/_static/xradar_logo.svg`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/conf.py` & `xradar-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/datamodel.md` & `xradar-0.3.0/docs/datamodel.md`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/history.md` & `xradar-0.3.0/docs/history.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # History
 
+## 0.3.0 (2023-07-11)
+* ENH: Add new examples using radar data on AWS s3 bucket ({pull}`102`) by [@aladinor](https://github.com/aladinor)
+* FIX: Correct DB_DBTE8/DB_DBZE8 and DB_DBTE16/DB_DBZE16 decoding for iris-backend ({pull}`110`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: Cast boolean string to int in rainbow dictionary ({pull}`113`) by [@egouden](https://github.com/egouden)
+* MNT: switch to mamba-org/setup-micromamba, split CI tests ({issue}`115`), ({pull}`116`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: time interpolation ({pull}`117`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: robust ``angle_res`` retrieval in ``extract_angle_parameters`` ({issue}`112`), ({pull}`118`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: robust radar identifier in ``to_odim()`` ({pull}`120`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+
 ## 0.2.0 (2023-03-24)
 
 * ENH: switch to add optional how attributes in ODIM format writer ({pull}`97`) by [@egouden](https://github.com/egouden)
 * FIX: add keyword argument for mandatory source attribute in ODIM format writer ({pull}`96`) by [@egouden](https://github.com/egouden)
 * FIX: check for dim0 if not given, only swap_dims if needed ({issue}`92`), ({pull}`94`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
 * FIX+ENH: need array copy before overwriting and make compression available in to_odim ({pull}`95`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
```

### Comparing `xradar-0.2.0/docs/importers.md` & `xradar-0.3.0/docs/importers.md`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/installation.md` & `xradar-0.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/make.bat` & `xradar-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/docs/usage.md` & `xradar-0.3.0/docs/usage.md`

 * *Files 20% similar despite different names*

```diff
@@ -27,11 +27,12 @@
 notebooks/CfRadial1_Model_Transformation
 notebooks/CfRadial1
 notebooks/ODIM_H5
 notebooks/GAMIC
 notebooks/Furuno
 notebooks/Rainbow
 notebooks/Iris
+notebooks/Read-plot-Sigmet-data-from-AWS
 notebooks/plot-ppi
 notebooks/angle_reindexing
 notebooks/Multi-Volume-Concatenation.ipynb
 ```
```

### Comparing `xradar-0.2.0/examples/notebooks/Accessors.ipynb` & `xradar-0.3.0/examples/notebooks/Accessors.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/CfRadial1.ipynb` & `xradar-0.3.0/examples/notebooks/CfRadial1.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/CfRadial1_Model_Transformation.ipynb` & `xradar-0.3.0/examples/notebooks/CfRadial1_Model_Transformation.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/Furuno.ipynb` & `xradar-0.3.0/examples/notebooks/Furuno.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/GAMIC.ipynb` & `xradar-0.3.0/examples/notebooks/GAMIC.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/Iris.ipynb` & `xradar-0.3.0/examples/notebooks/Iris.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/Multi-Volume-Concatenation.ipynb` & `xradar-0.3.0/examples/notebooks/Multi-Volume-Concatenation.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/ODIM_H5.ipynb` & `xradar-0.3.0/examples/notebooks/ODIM_H5.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/Rainbow.ipynb` & `xradar-0.3.0/examples/notebooks/Rainbow.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/angle_reindexing.ipynb` & `xradar-0.3.0/examples/notebooks/angle_reindexing.ipynb`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/conftest.py` & `xradar-0.3.0/examples/notebooks/conftest.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/examples/notebooks/plot-ppi.ipynb` & `xradar-0.3.0/examples/notebooks/plot-ppi.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9352678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.9.16'}, 'kernelspec': "*

 * *               "OrderedDict([('display_name', 'Python 3 (ipykernel)'), ('language', 'python'), "*

 * *               "('name', 'python3')])}"}*

```diff
@@ -216,23 +216,28 @@
                 ")\n",
                 "ax.coastlines()\n",
                 "ax.gridlines(draw_labels=True)"
             ]
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "Python 3 (ipykernel)",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xradar-0.2.0/pyproject.toml` & `xradar-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/conftest.py` & `xradar-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/georeference/test_projection.py` & `xradar-0.3.0/tests/georeference/test_projection.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/georeference/test_transforms.py` & `xradar-0.3.0/tests/georeference/test_transforms.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/io/test_furuno.py` & `xradar-0.3.0/tests/io/test_furuno.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/io/test_io.py` & `xradar-0.3.0/tests/io/test_io.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/io/test_iris.py` & `xradar-0.3.0/tests/io/test_iris.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/io/test_rainbow.py` & `xradar-0.3.0/tests/io/test_rainbow.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/test_accessors.py` & `xradar-0.3.0/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/test_model.py` & `xradar-0.3.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/tests/test_xradar.py` & `xradar-0.3.0/tests/test_xradar.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/__init__.py` & `xradar-0.3.0/xradar/__init__.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/accessors.py` & `xradar-0.3.0/xradar/accessors.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/georeference/projection.py` & `xradar-0.3.0/xradar/georeference/projection.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/georeference/transforms.py` & `xradar-0.3.0/xradar/georeference/transforms.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/io/backends/__init__.py` & `xradar-0.3.0/xradar/io/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/io/backends/cfradial1.py` & `xradar-0.3.0/xradar/io/backends/cfradial1.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,10 +435,10 @@
         )
         if ds is None:
             raise ValueError(f"Group `{group}` missing from file `{filename_or_obj}`.")
 
         if decode_coords and reindex_angle is not False:
             ds = ds.pipe(util.remove_duplicate_rays)
             ds = ds.pipe(util.reindex_angle, **reindex_angle)
-            ds = ds.pipe(util.ipol_time)
+            ds = ds.pipe(util.ipol_time, **reindex_angle)
 
         return ds
```

### Comparing `xradar-0.2.0/xradar/io/backends/common.py` & `xradar-0.3.0/xradar/io/backends/common.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/io/backends/furuno.py` & `xradar-0.3.0/xradar/io/backends/furuno.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,15 @@
 
         ds.encoding["engine"] = "furuno"
 
         # handle duplicates and reindex
         if decode_coords and reindex_angle is not False:
             ds = ds.pipe(util.remove_duplicate_rays)
             ds = ds.pipe(util.reindex_angle, **reindex_angle)
-            ds = ds.pipe(util.ipol_time)
+            ds = ds.pipe(util.ipol_time, **reindex_angle)
 
         # handling first dimension
         dim0 = "elevation" if ds.sweep_mode.load() == "rhi" else "azimuth"
         if first_dim == "auto":
             if "time" in ds.dims:
                 ds = ds.swap_dims({"time": dim0})
             ds = ds.sortby(dim0)
```

### Comparing `xradar-0.2.0/xradar/io/backends/gamic.py` & `xradar-0.3.0/xradar/io/backends/gamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,15 @@
 
         ds.encoding["engine"] = "gamic"
 
         # handle duplicates and reindex
         if decode_coords and reindex_angle is not False:
             ds = ds.pipe(util.remove_duplicate_rays)
             ds = ds.pipe(util.reindex_angle, **reindex_angle)
-            ds = ds.pipe(util.ipol_time)
+            ds = ds.pipe(util.ipol_time, **reindex_angle)
 
         # handling first dimension
         dim0 = "elevation" if ds.sweep_mode.load() == "rhi" else "azimuth"
 
         if first_dim == "auto":
             if "time" in ds.dims:
                 ds = ds.swap_dims({"time": dim0})
```

### Comparing `xradar-0.2.0/xradar/io/backends/iris.py` & `xradar-0.3.0/xradar/io/backends/iris.py`

 * *Files 0% similar despite different names*

```diff
@@ -2278,21 +2278,53 @@
         # Albedo (2 byte)
         (68, {"name": "DB_ALBEDO16", "dtype": "uint16", "func": None}),
         # VIL Density (2 byte)
         (69, {"name": "DB_VILD16", "dtype": "uint16", "func": None}),
         # Turbulence (2 byte)
         (70, {"name": "DB_TURB16", "dtype": "uint16", "func": None}),
         # Total Power Enhanced (via H+V or HV) (1 byte)
-        (71, {"name": "DB_DBTE8", "dtype": "uint8", "func": None}),
+        (
+            71,
+            {
+                "name": "DB_DBTE8",
+                "dtype": "uint8",
+                "func": decode_array,
+                "fkw": {"scale": 2.0, "offset": -64.0},
+            },
+        ),
         # Total Power Enhanced (via H+V or HV) (2 byte)
-        (72, {"name": "DB_DBTE16", "dtype": "uint16", "func": None}),
+        (
+            72,
+            {
+                "name": "DB_DBTE16",
+                "dtype": "uint16",
+                "func": decode_array,
+                "fkw": {"scale": 100.0, "offset": -32768.0},
+            },
+        ),
         # Clutter Corrected Reflectivity Enhanced (1 byte)
-        (73, {"name": "DB_DBZE8", "dtype": "uint8", "func": None}),
+        (
+            73,
+            {
+                "name": "DB_DBZE8",
+                "dtype": "uint8",
+                "func": decode_array,
+                "fkw": {"scale": 2.0, "offset": -64.0},
+            },
+        ),
         # Clutter Corrected Reflectivity Enhanced (2 byte)
-        (74, {"name": "DB_DBZE16", "dtype": "uint16", "func": None}),
+        (
+            74,
+            {
+                "name": "DB_DBZE16",
+                "dtype": "uint16",
+                "func": decode_array,
+                "fkw": {"scale": 100.0, "offset": -32768.0},
+            },
+        ),
         # Polarimetric meteo index (1 byte)
         (
             75,
             {
                 "name": "DB_PMI8",
                 "dtype": "uint8",
                 "func": decode_sqi,
@@ -3970,15 +4002,15 @@
 
         ds.encoding["engine"] = "iris"
 
         # handle duplicates and reindex
         if decode_coords and reindex_angle is not False:
             ds = ds.pipe(util.remove_duplicate_rays)
             ds = ds.pipe(util.reindex_angle, **reindex_angle)
-            ds = ds.pipe(util.ipol_time)
+            ds = ds.pipe(util.ipol_time, **reindex_angle)
 
         ds.attrs.pop("elevation_lower_limit", None)
         ds.attrs.pop("elevation_upper_limit", None)
 
         # handling first dimension
         dim0 = "elevation" if ds.sweep_mode.load() == "rhi" else "azimuth"
```

### Comparing `xradar-0.2.0/xradar/io/backends/odim.py` & `xradar-0.3.0/xradar/io/backends/odim.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,15 +744,15 @@
 
         ds.encoding["engine"] = "odim"
 
         # handle duplicates and reindex
         if decode_coords and reindex_angle is not False:
             ds = ds.pipe(util.remove_duplicate_rays)
             ds = ds.pipe(util.reindex_angle, **reindex_angle)
-            ds = ds.pipe(util.ipol_time)
+            ds = ds.pipe(util.ipol_time, **reindex_angle)
 
         # handling first dimension
         dim0 = "elevation" if ds.sweep_mode.load() == "rhi" else "azimuth"
         if first_dim == "auto":
             if "time" in ds.dims:
                 ds = ds.swap_dims({"time": dim0})
             ds = ds.sortby(dim0)
```

### Comparing `xradar-0.2.0/xradar/io/backends/rainbow.py` & `xradar-0.3.0/xradar/io/backends/rainbow.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,14 +515,16 @@
         )
 
     def _get_rbdict_value(self, rbdict, name, dtype=None, default=None):
         value = rbdict.get(name, None)
         if value is None:
             value = self.pargroup.get(name, default)
         if dtype is not None:
+            if dtype == bool:
+                value = int(value)
             value = dtype(value)
         return value
 
     def _update_volume_slices(self):
         if isinstance(self._header["scan"]["slice"], list):
             slice0 = self._header["scan"]["slice"][0]
             for i, slice in enumerate(self._header["scan"]["slice"][1:]):
@@ -832,15 +834,15 @@
 
         ds.encoding["engine"] = "rainbow"
 
         # handle duplicates and reindex
         if decode_coords and reindex_angle is not False:
             ds = ds.pipe(util.remove_duplicate_rays)
             ds = ds.pipe(util.reindex_angle, **reindex_angle)
-            ds = ds.pipe(util.ipol_time)
+            ds = ds.pipe(util.ipol_time, **reindex_angle)
 
         # handling first dimension
         dim0 = "elevation" if ds.sweep_mode.load() == "rhi" else "azimuth"
         if first_dim == "auto":
             if "time" in ds.dims:
                 ds = ds.swap_dims({"time": dim0})
             ds = ds.sortby(dim0)
```

### Comparing `xradar-0.2.0/xradar/io/export/cfradial2.py` & `xradar-0.3.0/xradar/io/export/cfradial2.py`

 * *Files identical despite different names*

### Comparing `xradar-0.2.0/xradar/io/export/odim.py` & `xradar-0.3.0/xradar/io/export/odim.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,18 +157,18 @@
     optional_how : boolean
         True to include optional how attributes, defaults to False
     compression : str
         Compression filter name, defaults to "gzip".
     compression_opts : compression strategy
         options as needed by above filter, defaults to 6
     """
-    nod = "NOD" in source
-    wmo = "WMO" in source
-    rad = "RAD" in source
-    if not nod and not rad and not wmo:
+    has_identifier = False
+    if source is not None:
+        has_identifier = any(key in source for key in ["NOD", "WMO", "RAD"])
+    if not has_identifier:
         raise ValueError(
             "Please provide the source parameter with at least one"
             "of the mandatory radar identifier (NOD, RAD, WMO)"
         )
 
     root = dtree["/"]
```

### Comparing `xradar-0.2.0/xradar/model.py` & `xradar-0.3.0/xradar/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,14 +883,16 @@
         time resolution or array with time values ('seconds since'-notation).
     date_str : str
         String with the form 'YYYY-mm-ddTHH:MM:SS' depicting the reference time.
     rng : float or :class:`numpy:numpy.ndarray`
         range resolution or array with range values.
     azimuth : float or :class:`numpy:numpy.ndarray`
         azimuth resolution or array with azimuth values.
+    direction : int
+        1 - CW/UP, -1 CCW/DOWN
     a1gate : int
         First measured ray. Defaults to 0. Only used for PPI.
     elevation : float or :class:`numpy:numpy.ndarray`
         elevation resolution or array with elevation values.
     sweep : str
         "PPI" or "RHI".
 
@@ -933,18 +935,19 @@
                 raise ValueError("given elevation value will be ignored for RHI sweep")
             elevation = 90 / shape[0]
 
     a1gate = kwargs.pop("a1gate", 0)
     time = kwargs.pop("time", 0.25)
     date_str = kwargs.pop("date_str", "2022-08-27T10:00:00")
     rng = kwargs.pop("rng", 100)
+    direction = kwargs.pop("direction", 1)
 
     # calculate according to PPI/RHI
     if sweep == "PPI":
-        azimuth = get_azimuth_dataarray(azimuth, nrays=None, a1gate=a1gate)
+        azimuth = get_azimuth_dataarray(azimuth, nrays=None, a1gate=a1gate)[::direction]
         nrays = azimuth.shape[0]
         elevation = get_elevation_dataarray(elevation, nrays=nrays)
     else:
         elevation = get_elevation_dataarray(elevation, nrays=None)
         nrays = elevation.shape[0]
         azimuth = get_azimuth_dataarray(azimuth, nrays=nrays, a1gate=a1gate)
```

### Comparing `xradar-0.2.0/xradar.egg-info/PKG-INFO` & `xradar-0.3.0/xradar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xradar
-Version: 0.2.0
+Version: 0.3.0
 Summary: Xradar includes all the tools to get your weather radar into the xarray data model.
 Author-email: Maxwell Grover <mgrover@anl.gov>, Kai Mühlbauer <kai.muehlbauer@uni-bonn.de>, Zachary Sherman <zsherman@anl.gov>
 License: MIT License
         
         Copyright (c) 2022-2023, Open Radar Community Developers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # xradar
 
 [![PyPI Version](https://img.shields.io/pypi/v/xradar.svg)](https://pypi.python.org/pypi/xradar)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/xradar.svg)](https://anaconda.org/conda-forge/xradar)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7091737.svg)](https://doi.org/10.5281/zenodo.7091737)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7767521.svg)](https://doi.org/10.5281/zenodo.7767521)
 
 [![CI](https://github.com/openradar/xradar/actions/workflows/ci.yml/badge.svg)](https://github.com/openradar/xradar/actions/workflows/ci.yml)
 [![Build distribution](https://github.com/openradar/xradar/actions/workflows/upload_pypi.yml/badge.svg)](https://github.com/openradar/xradar/actions/workflows/upload_pypi.yml)
 [![RTD Version](https://readthedocs.org/projects/xradar/badge/?version=latest)](https://xradar.readthedocs.io/en/latest/?version=latest)
 
 Xradar includes all the tools to get your weather radar into the xarray data model.
 
@@ -88,14 +88,23 @@
 * Import Iris/Sigmet
 * Import Furuno SCN/SCNX
 * Georeferencing (AEQD)
 * Angle Reindexing
 
 # History
 
+## 0.3.0 (2023-07-11)
+* ENH: Add new examples using radar data on AWS s3 bucket ({pull}`102`) by [@aladinor](https://github.com/aladinor)
+* FIX: Correct DB_DBTE8/DB_DBZE8 and DB_DBTE16/DB_DBZE16 decoding for iris-backend ({pull}`110`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: Cast boolean string to int in rainbow dictionary ({pull}`113`) by [@egouden](https://github.com/egouden)
+* MNT: switch to mamba-org/setup-micromamba, split CI tests ({issue}`115`), ({pull}`116`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: time interpolation ({pull}`117`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: robust ``angle_res`` retrieval in ``extract_angle_parameters`` ({issue}`112`), ({pull}`118`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+* FIX: robust radar identifier in ``to_odim()`` ({pull}`120`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
+
 ## 0.2.0 (2023-03-24)
 
 * ENH: switch to add optional how attributes in ODIM format writer ({pull}`97`) by [@egouden](https://github.com/egouden)
 * FIX: add keyword argument for mandatory source attribute in ODIM format writer ({pull}`96`) by [@egouden](https://github.com/egouden)
 * FIX: check for dim0 if not given, only swap_dims if needed ({issue}`92`), ({pull}`94`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
 * FIX+ENH: need array copy before overwriting and make compression available in to_odim ({pull}`95`) by [@kmuehlbauer](https://github.com/kmuehlbauer)
```

### Comparing `xradar-0.2.0/xradar.egg-info/SOURCES.txt` & `xradar-0.3.0/xradar.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 requirements.txt
 requirements_dev.txt
 tox.ini
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/ci.yml
 .github/workflows/upload_pypi.yml
+ci/notebooktests.yml
 ci/unittests.yml
 docs/Makefile
 docs/authors.md
 docs/conf.py
 docs/contributing.md
 docs/datamodel.md
 docs/exporters.md
@@ -40,16 +41,18 @@
 examples/notebooks/CfRadial1_Model_Transformation.ipynb
 examples/notebooks/Furuno.ipynb
 examples/notebooks/GAMIC.ipynb
 examples/notebooks/Iris.ipynb
 examples/notebooks/Multi-Volume-Concatenation.ipynb
 examples/notebooks/ODIM_H5.ipynb
 examples/notebooks/Rainbow.ipynb
+examples/notebooks/Read-plot-Sigmet-data-from-AWS.ipynb
 examples/notebooks/angle_reindexing.ipynb
 examples/notebooks/conftest.py
+examples/notebooks/multiple-sweeps-into-volume-scan.ipynb
 examples/notebooks/plot-ppi.ipynb
 tests/__init__.py
 tests/conftest.py
 tests/test_accessors.py
 tests/test_model.py
 tests/test_util.py
 tests/test_xradar.py
```

