# Comparing `tmp/stcal-1.4.1.tar.gz` & `tmp/stcal-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stcal-1.4.1.tar", last modified: Thu Jun 29 13:33:24 2023, max compression
+gzip compressed data, was "stcal-1.4.2.tar", last modified: Tue Jul 11 12:40:09 2023, max compression
```

## Comparing `stcal-1.4.1.tar` & `stcal-1.4.2.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.789134 stcal-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.709134 stcal-1.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.709134 stcal-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-29 13:33:12.000000 stcal-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-29 13:33:12.000000 stcal-1.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-06-29 13:33:12.000000 stcal-1.4.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-29 13:33:12.000000 stcal-1.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-29 13:33:12.000000 stcal-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-29 13:33:12.000000 stcal-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-29 13:33:24.785134 stcal-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-29 13:33:12.000000 stcal-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 13:33:12.000000 stcal-1.4.1/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/stcal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-29 13:33:12.000000 stcal-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:33:24.789134 stcal-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.709134 stcal-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dark_current/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dark_current/dark_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dark_current/dark_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dynamicdq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    36437 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/twopoint_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/linearity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/linearity/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.717134 stcal-1.4.1/src/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)   127963 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/ols_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    56323 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.717134 stcal-1.4.1/src/stcal/saturation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/saturation/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:33:23.000000 stcal-1.4.1/src/stcal.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.753134 stcal-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/current_gdqfits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.785134 stcal-1.4.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/data/input_gdq_flarge.fits
--rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/data/large_event_input_dq_cube2.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/data/snowball1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    53011 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_ramp_fitting_gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_twopoint_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-29 13:33:12.000000 stcal-1.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.933833 stcal-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.889833 stcal-1.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.889833 stcal-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 12:39:59.000000 stcal-1.4.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-11 12:39:59.000000 stcal-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-11 12:39:59.000000 stcal-1.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-07-11 12:39:59.000000 stcal-1.4.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-11 12:39:59.000000 stcal-1.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 12:39:59.000000 stcal-1.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-11 12:39:59.000000 stcal-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-11 12:40:09.933833 stcal-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-11 12:39:59.000000 stcal-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-11 12:39:59.000000 stcal-1.4.2/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.889833 stcal-1.4.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:39:59.000000 stcal-1.4.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-11 12:39:59.000000 stcal-1.4.2/benchmarks/dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/benchmarks/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-11 12:39:59.000000 stcal-1.4.2/benchmarks/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-11 12:39:59.000000 stcal-1.4.2/benchmarks/ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-11 12:39:59.000000 stcal-1.4.2/benchmarks/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/docs/stcal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/docs/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/stcal/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/stcal/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/stcal/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/docs/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/stcal/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-11 12:39:59.000000 stcal-1.4.2/docs/stcal/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-11 12:39:59.000000 stcal-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:40:09.933833 stcal-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.885833 stcal-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/src/stcal/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/src/stcal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/dark_current/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/dark_current/dark_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/dark_current/dark_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/dynamicdq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/src/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/jump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/jump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36676 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/jump/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/jump/twopoint_difference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/src/stcal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/linearity/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.897833 stcal-1.4.2/src/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/ramp_fitting/gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127963 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/ramp_fitting/ols_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/ramp_fitting/ramp_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/ramp_fitting/ramp_fit_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56323 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/ramp_fitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.897833 stcal-1.4.2/src/stcal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-11 12:39:59.000000 stcal-1.4.2/src/stcal/saturation/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.893833 stcal-1.4.2/src/stcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:40:09.000000 stcal-1.4.2/src/stcal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.897833 stcal-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:40:09.929833 stcal-1.4.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/data/input_gdq_flarge.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/data/large_event_input_dq_cube2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/data/snowball1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53011 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_ramp_fitting_gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-07-11 12:39:59.000000 stcal-1.4.2/tests/test_twopoint_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-11 12:39:59.000000 stcal-1.4.2/tox.ini
```

### Comparing `stcal-1.4.1/.github/labeler.yml` & `stcal-1.4.2/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/.github/pull_request_template.md` & `stcal-1.4.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/.github/workflows/ci.yml` & `stcal-1.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/.github/workflows/publish-to-pypi.yml` & `stcal-1.4.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/.gitignore` & `stcal-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/.readthedocs.yaml` & `stcal-1.4.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/CHANGES.rst` & `stcal-1.4.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+1.4.3 (unreleased)
+==================
+
+Bug Fixes
+---------
+
+jump
+~~~~
+
+- 
+
+1.4.2 (2023-07-11)
+==================
+
+Bug Fixes
+---------
+
+jump
+~~~~
+
+- Added setting of number_extended_events for non-multiprocessing
+  mode. This is the value that is put into the header keyword EXTNCRS. [#178]
+
 1.4.1 (2023-06-29)
 ==================
 
 Bug Fixes
 ---------
 
 jump
```

### Comparing `stcal-1.4.1/CODE_OF_CONDUCT.md` & `stcal-1.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/CONTRIBUTING.md` & `stcal-1.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/LICENSE` & `stcal-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/PKG-INFO` & `stcal-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.4.1
+Version: 1.4.2
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.4.1/README.md` & `stcal-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/benchmarks/dark_current.py` & `stcal-1.4.2/benchmarks/dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/benchmarks/linearity.py` & `stcal-1.4.2/benchmarks/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/benchmarks/ramp_fitting.py` & `stcal-1.4.2/benchmarks/ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/benchmarks/saturation.py` & `stcal-1.4.2/benchmarks/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/docs/Makefile` & `stcal-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/docs/conf.py` & `stcal-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/docs/stcal/jump/description.rst` & `stcal-1.4.2/docs/stcal/jump/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/docs/stcal/ramp_fitting/description.rst` & `stcal-1.4.2/docs/stcal/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/pyproject.toml` & `stcal-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/dark_current/dark_class.py` & `stcal-1.4.2/src/stcal/dark_current/dark_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/dark_current/dark_sub.py` & `stcal-1.4.2/src/stcal/dark_current/dark_sub.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/dqflags.py` & `stcal-1.4.2/src/stcal/dqflags.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/jump/jump.py` & `stcal-1.4.2/src/stcal/jump/jump.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,32 +258,36 @@
                            after_jump_flag_n1=after_jump_flag_n1,
                            after_jump_flag_e2=after_jump_flag_e2,
                            after_jump_flag_n2=after_jump_flag_n2, copy_arrs=False,
                            minimum_groups=3, minimum_sigclip_groups=minimum_sigclip_groups,
                            only_use_ints=only_use_ints)
         #  This is the flag that controls the flagging of either snowballs.
         if expand_large_events:
-            flag_large_events(gdq, jump_flag, sat_flag, min_sat_area=min_sat_area,
+            total_snowballs = flag_large_events(gdq, jump_flag, sat_flag, min_sat_area=min_sat_area,
                               min_jump_area=min_jump_area,
                               expand_factor=expand_factor,
                               sat_required_snowball=sat_required_snowball,
                               min_sat_radius_extend=min_sat_radius_extend,
                               edge_size=edge_size, sat_expand=sat_expand,
                               max_extended_radius=max_extended_radius)
+            log.info('Total snowballs = %i' % total_snowballs)
+            number_extended_events = total_snowballs
         if find_showers:
             gdq, num_showers = find_faint_extended(data, gdq, readnoise_2d,
                                                    frames_per_group, minimum_sigclip_groups,
                                                    snr_threshold=extend_snr_threshold,
                                                    min_shower_area=extend_min_area,
                                                    inner=extend_inner_radius,
                                                    outer=extend_outer_radius,
                                                    sat_flag=sat_flag, jump_flag=jump_flag,
                                                    ellipse_expand=extend_ellipse_expand_ratio,
                                                    num_grps_masked=grps_masked_after_shower,
                                                    max_extended_radius=max_extended_radius)
+            log.info('Total showers= %i' % num_showers)
+            number_extended_events = num_showers
     else:
         yinc = int(n_rows / n_slices)
         slices = []
         # Slice up data, gdq, readnoise_2d into slices
         # Each element of slices is a tuple of
         # (data, gdq, readnoise_2d, rejection_thresh, three_grp_thresh,
         #  four_grp_thresh, nframes)
```

### Comparing `stcal-1.4.1/src/stcal/jump/twopoint_difference.py` & `stcal-1.4.2/src/stcal/jump/twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/linearity/linearity.py` & `stcal-1.4.2/src/stcal/linearity/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/ramp_fitting/gls_fit.py` & `stcal-1.4.2/src/stcal/ramp_fitting/gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/ramp_fitting/ols_fit.py` & `stcal-1.4.2/src/stcal/ramp_fitting/ols_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit.py` & `stcal-1.4.2/src/stcal/ramp_fitting/ramp_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit_class.py` & `stcal-1.4.2/src/stcal/ramp_fitting/ramp_fit_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/ramp_fitting/utils.py` & `stcal-1.4.2/src/stcal/ramp_fitting/utils.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal/saturation/saturation.py` & `stcal-1.4.2/src/stcal/saturation/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/src/stcal.egg-info/PKG-INFO` & `stcal-1.4.2/src/stcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.4.1
+Version: 1.4.2
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.4.1/src/stcal.egg-info/SOURCES.txt` & `stcal-1.4.2/src/stcal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 src/stcal/ramp_fitting/ols_fit.py
 src/stcal/ramp_fitting/ramp_fit.py
 src/stcal/ramp_fitting/ramp_fit_class.py
 src/stcal/ramp_fitting/utils.py
 src/stcal/saturation/__init__.py
 src/stcal/saturation/saturation.py
 tests/__init__.py
-tests/current_gdqfits
 tests/test_dark_current.py
 tests/test_dq.py
 tests/test_jump.py
 tests/test_linearity.py
 tests/test_ramp_fitting.py
 tests/test_ramp_fitting_gls_fit.py
 tests/test_saturation.py
```

### Comparing `stcal-1.4.1/tests/data/input_gdq_flarge.fits` & `stcal-1.4.2/tests/data/input_gdq_flarge.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/data/large_event_input_dq_cube2.fits` & `stcal-1.4.2/tests/data/large_event_input_dq_cube2.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/data/snowball1.fits` & `stcal-1.4.2/tests/data/snowball1.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_dark_current.py` & `stcal-1.4.2/tests/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_dq.py` & `stcal-1.4.2/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_jump.py` & `stcal-1.4.2/tests/test_jump.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
     gdq, num_showers = find_faint_extended(data, gdq, readnoise, 1, 100,
                                            snr_threshold=1.3,
                                            min_shower_area=20, inner=1,
                                            outer=2, sat_flag=2, jump_flag=4,
                                            ellipse_expand=1.1, num_grps_masked=3)
     #  Check that all the expected samples in group 2 are flagged as jump and
     #  that they are not flagged outside
+    assert (num_showers == 3)
     assert (np.all(gdq[0, 1, 22, 14:23] == 0))
     assert (np.all(gdq[0, 1, 21, 16:20] == DQFLAGS['JUMP_DET']))
     assert (np.all(gdq[0, 1, 20, 15:22] == DQFLAGS['JUMP_DET']))
     assert (np.all(gdq[0, 1, 19, 15:23] == DQFLAGS['JUMP_DET']))
     assert (np.all(gdq[0, 1, 18, 14:23] == DQFLAGS['JUMP_DET']))
     assert (np.all(gdq[0, 1, 17, 14:23] == DQFLAGS['JUMP_DET']))
     assert (np.all(gdq[0, 1, 16, 14:23] == DQFLAGS['JUMP_DET']))
@@ -206,14 +207,15 @@
     gdq, num_showers = find_faint_extended(data, gdq, readnoise, 1, 100,
                                            snr_threshold=1.3,
                                            min_shower_area=20, inner=1,
                                            outer=2, sat_flag=2, jump_flag=4,
                                            ellipse_expand=1.1, num_grps_masked=3)
     #  Check that all the expected samples in group 2 are flagged as jump and
     #  that they are not flagged outside
+    assert(num_showers == 0)
     assert (np.all(gdq[0, 1, 22, 14:23] == 0))
     assert (np.all(gdq[0, 1, 21, 16:20] == 0))
     assert (np.all(gdq[0, 1, 20, 15:22] == 0))
     assert (np.all(gdq[0, 1, 19, 15:23] == 0))
     assert (np.all(gdq[0, 1, 18, 14:23] == 0))
     assert (np.all(gdq[0, 1, 17, 14:23] == 0))
     assert (np.all(gdq[0, 1, 16, 14:23] == 0))
@@ -261,18 +263,22 @@
     snowball_diff = snowball_1 - correct_snowball_1
     assert (np.all(snowball_diff == 0))
 
 
 @pytest.mark.skip("Used for local testing")
 def test_inputjump_sat_star():
     testcube = fits.getdata('data/input_gdq_flarge.fits')
-    flag_large_events(testcube, DQFLAGS['JUMP_DET'], DQFLAGS['SATURATED'], min_sat_area=1,
-                      min_jump_area=6,
-                      expand_factor=2.0, use_ellipses=False,
-                      sat_required_snowball=True, min_sat_radius_extend=2.5, sat_expand=2)
+    num_extended_events = flag_large_events(testcube, DQFLAGS['JUMP_DET'], DQFLAGS['SATURATED'],
+                                            min_sat_area=1,
+                                            min_jump_area=6,
+                                            expand_factor=2.0,
+                                            sat_required_snowball=True,
+                                            min_sat_radius_extend=2.5,
+                                            sat_expand=2)
+    assert(num_extended_events == 312)
     fits.writeto("outgdq2.fits", testcube, overwrite=True)
 
 
 @pytest.mark.skip("Used for local testing")
 def test_inputjump_sat_star2():
     testcube = fits.getdata('input_gdq_satstar.fits')
     flag_large_events(testcube, DQFLAGS['JUMP_DET'], DQFLAGS['SATURATED'], min_sat_area=1,
```

### Comparing `stcal-1.4.1/tests/test_linearity.py` & `stcal-1.4.2/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_ramp_fitting.py` & `stcal-1.4.2/tests/test_ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_ramp_fitting_gls_fit.py` & `stcal-1.4.2/tests/test_ramp_fitting_gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_saturation.py` & `stcal-1.4.2/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tests/test_twopoint_difference.py` & `stcal-1.4.2/tests/test_twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.1/tox.ini` & `stcal-1.4.2/tox.ini`

 * *Files identical despite different names*

