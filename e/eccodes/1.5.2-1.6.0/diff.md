# Comparing `tmp/eccodes-1.5.2.tar.gz` & `tmp/eccodes-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eccodes-1.5.2.tar", last modified: Tue Apr  4 13:26:27 2023, max compression
+gzip compressed data, was "eccodes-1.6.0.tar", last modified: Tue Jul 11 10:42:49 2023, max compression
```

## Comparing `eccodes-1.5.2.tar` & `eccodes-1.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.789449 eccodes-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 13:26:14.000000 eccodes-1.5.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-04 13:26:14.000000 eccodes-1.5.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-04 13:26:14.000000 eccodes-1.5.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-04 13:26:14.000000 eccodes-1.5.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-04 13:26:14.000000 eccodes-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-04 13:26:14.000000 eccodes-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-04 13:26:14.000000 eccodes-1.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-04 13:26:27.789449 eccodes-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-04 13:26:14.000000 eccodes-1.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-04 13:26:14.000000 eccodes-1.5.2/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:14.000000 eccodes-1.5.2/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-04 13:26:14.000000 eccodes-1.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-04 13:26:14.000000 eccodes-1.5.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/eccodes/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-04 13:26:14.000000 eccodes-1.5.2/eccodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-04 13:26:14.000000 eccodes-1.5.2/eccodes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-04-04 13:26:14.000000 eccodes-1.5.2/eccodes/eccodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/eccodes/highlevel/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-04 13:26:14.000000 eccodes-1.5.2/eccodes/highlevel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-04 13:26:14.000000 eccodes-1.5.2/eccodes/highlevel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-04 13:26:14.000000 eccodes-1.5.2/eccodes/highlevel/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/eccodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-04 13:26:27.000000 eccodes-1.5.2/eccodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-04 13:26:27.000000 eccodes-1.5.2/eccodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:26:27.000000 eccodes-1.5.2/eccodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-04 13:26:27.000000 eccodes-1.5.2/eccodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 13:26:27.000000 eccodes-1.5.2/eccodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:26:27.000000 eccodes-1.5.2/eccodes.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/gribapi/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-04 13:26:14.000000 eccodes-1.5.2/gribapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-04 13:26:14.000000 eccodes-1.5.2/gribapi/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-04 13:26:14.000000 eccodes-1.5.2/gribapi/eccodes.h
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-04 13:26:14.000000 eccodes-1.5.2/gribapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-04-04 13:26:14.000000 eccodes-1.5.2/gribapi/grib_api.h
--rw-r--r--   0 runner    (1001) docker     (123)    79906 2023-04-04 13:26:14.000000 eccodes-1.5.2/gribapi/gribapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-04 13:26:27.789449 eccodes-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-04 13:26:14.000000 eccodes-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.785448 eccodes-1.5.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:26:27.789449 eccodes-1.5.2/tests/sample-data/
--rw-r--r--   0 runner    (1001) docker     (123)  2361600 2023-04-04 13:26:14.000000 eccodes-1.5.2/tests/sample-data/era5-levels-members.grib
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-04 13:26:14.000000 eccodes-1.5.2/tests/sample-data/tiggelam_cnmc_sfc.grib2
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-04 13:26:14.000000 eccodes-1.5.2/tests/test_20_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-04 13:26:14.000000 eccodes-1.5.2/tests/test_20_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    31902 2023-04-04 13:26:14.000000 eccodes-1.5.2/tests/test_eccodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-04 13:26:14.000000 eccodes-1.5.2/tests/test_highlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-04 13:26:14.000000 eccodes-1.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.816256 eccodes-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 10:42:35.000000 eccodes-1.6.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-11 10:42:35.000000 eccodes-1.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-07-11 10:42:35.000000 eccodes-1.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-11 10:42:35.000000 eccodes-1.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-11 10:42:35.000000 eccodes-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-11 10:42:35.000000 eccodes-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-11 10:42:35.000000 eccodes-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-11 10:42:49.816256 eccodes-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-11 10:42:35.000000 eccodes-1.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 10:42:35.000000 eccodes-1.6.0/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.812256 eccodes-1.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.812256 eccodes-1.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:35.000000 eccodes-1.6.0/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-11 10:42:35.000000 eccodes-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-11 10:42:35.000000 eccodes-1.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.812256 eccodes-1.6.0/eccodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-11 10:42:35.000000 eccodes-1.6.0/eccodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 10:42:35.000000 eccodes-1.6.0/eccodes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-11 10:42:35.000000 eccodes-1.6.0/eccodes/eccodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.812256 eccodes-1.6.0/eccodes/highlevel/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 10:42:35.000000 eccodes-1.6.0/eccodes/highlevel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-07-11 10:42:35.000000 eccodes-1.6.0/eccodes/highlevel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-11 10:42:35.000000 eccodes-1.6.0/eccodes/highlevel/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.812256 eccodes-1.6.0/eccodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-11 10:42:49.000000 eccodes-1.6.0/eccodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-11 10:42:49.000000 eccodes-1.6.0/eccodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:42:49.000000 eccodes-1.6.0/eccodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 10:42:49.000000 eccodes-1.6.0/eccodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:42:49.000000 eccodes-1.6.0/eccodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:42:49.000000 eccodes-1.6.0/eccodes.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.812256 eccodes-1.6.0/gribapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-11 10:42:35.000000 eccodes-1.6.0/gribapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 10:42:35.000000 eccodes-1.6.0/gribapi/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 10:42:35.000000 eccodes-1.6.0/gribapi/eccodes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-11 10:42:35.000000 eccodes-1.6.0/gribapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-07-11 10:42:35.000000 eccodes-1.6.0/gribapi/grib_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)    81751 2023-07-11 10:42:35.000000 eccodes-1.6.0/gribapi/gribapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-11 10:42:49.820256 eccodes-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-11 10:42:35.000000 eccodes-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.816256 eccodes-1.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:42:49.816256 eccodes-1.6.0/tests/sample-data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2361600 2023-07-11 10:42:35.000000 eccodes-1.6.0/tests/sample-data/era5-levels-members.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-11 10:42:35.000000 eccodes-1.6.0/tests/sample-data/tiggelam_cnmc_sfc.grib2
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 10:42:35.000000 eccodes-1.6.0/tests/test_20_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-07-11 10:42:35.000000 eccodes-1.6.0/tests/test_20_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33509 2023-07-11 10:42:35.000000 eccodes-1.6.0/tests/test_eccodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-11 10:42:35.000000 eccodes-1.6.0/tests/test_highlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-11 10:42:35.000000 eccodes-1.6.0/tox.ini
```

### Comparing `eccodes-1.5.2/CHANGELOG.rst` & `eccodes-1.6.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 
 Changelog for eccodes-python
 ============================
 
+
+1.6.0 (2023-07-11)
+--------------------
+
+- ECC-1630: Get API version as an integer
+- ECC-1622: Drop Python version 3.7
+- ECC-1601: GRIB: Support data values array decoded in single-precision
+- ECC-1611: Add function to determine if a BUFR key is a coordinate descriptor
+
 1.5.2 (2023-04-04)
 --------------------
 
 - Add support for Python versions 3.10 and 3.11
 - ECC-1555: 2D numpy array incorrectly handled
 - ECC-1539: Use the 'warnings' library for selfcheck
 - ECC-1538: Add support for CODES_TYPE_BYTES
```

### Comparing `eccodes-1.5.2/CONTRIBUTING.rst` & `eccodes-1.6.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 1. The pull request should include tests.
 
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 
-3. The pull request should work for Python 3.7, 3.8, 3.9, 3.10, 3.11 and for PyPy2 and PyPy3.
+3. The pull request should work for Python 3.8, 3.9, 3.10, 3.11 and for PyPy2 and PyPy3.
    Check the tox results and make sure that the tests pass for all supported Python versions.
 
 
 Testing CDS data
 ----------------
 
 You can test the CF-GRIB driver on a set of products downloaded from the Climate Data Store
```

### Comparing `eccodes-1.5.2/Dockerfile` & `eccodes-1.6.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/LICENSE` & `eccodes-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/Makefile` & `eccodes-1.6.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 PACKAGE := eccodes-python
 IMAGE := $(PACKAGE)-image
 MODULE := eccodes
-PYTHONS := python3.9 python3.8 python3.7 pypy3
+PYTHONS := python3.9 python3.8 pypy3
 PYTHON := python
 
 PYTESTFLAGS_TEST := -v --flakes --doctest-glob '*.rst' --cov=$(MODULE) --cov-report=html --cache-clear
 PYTESTFLAGS_QC := --pep8 --mccabe $(PYTESTFLAGS_TEST)
 
 export WHEELHOUSE := ~/.wheelhouse
 export PIP_FIND_LINKS := $(WHEELHOUSE)
```

### Comparing `eccodes-1.5.2/PKG-INFO` & `eccodes-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: eccodes
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python interface to the ecCodes GRIB and BUFR decoder/encoder
 Home-page: https://github.com/ecmwf/eccodes-python
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: ecCodes GRIB BUFR
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
@@ -26,15 +25,15 @@
 Python 3 interface to decode and encode GRIB and BUFR files via the
 `ECMWF ecCodes library <https://confluence.ecmwf.int/display/ECC/>`_.
 
 Features:
 
 - reads and writes GRIB 1 and 2 files,
 - reads and writes BUFR 3 and 4 files,
-- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8, 3.7 and PyPy3,
+- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8 and PyPy3,
 - works on most *Linux* distributions and *MacOS*, the *ecCodes* C-library
   is the only system dependency,
 - PyPI package can be installed without compiling,
   at the cost of being twice as slow as the original *ecCodes* module,
 - an optional compile step makes the code as fast as the original module
   but it needs the recommended (the most up-to-date) version of *ecCodes*.
 
@@ -148,14 +147,23 @@
 In applying this licence, ECMWF does not waive the privileges and immunities
 granted to it by virtue of its status as an intergovernmental organisation nor
 does it submit to any jurisdiction.
 
 Changelog for eccodes-python
 ============================
 
+
+1.6.0 (2023-07-11)
+--------------------
+
+- ECC-1630: Get API version as an integer
+- ECC-1622: Drop Python version 3.7
+- ECC-1601: GRIB: Support data values array decoded in single-precision
+- ECC-1611: Add function to determine if a BUFR key is a coordinate descriptor
+
 1.5.2 (2023-04-04)
 --------------------
 
 - Add support for Python versions 3.10 and 3.11
 - ECC-1555: 2D numpy array incorrectly handled
 - ECC-1539: Use the 'warnings' library for selfcheck
 - ECC-1538: Add support for CODES_TYPE_BYTES
```

### Comparing `eccodes-1.5.2/README.rst` & `eccodes-1.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Python 3 interface to decode and encode GRIB and BUFR files via the
 `ECMWF ecCodes library <https://confluence.ecmwf.int/display/ECC/>`_.
 
 Features:
 
 - reads and writes GRIB 1 and 2 files,
 - reads and writes BUFR 3 and 4 files,
-- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8, 3.7 and PyPy3,
+- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8 and PyPy3,
 - works on most *Linux* distributions and *MacOS*, the *ecCodes* C-library
   is the only system dependency,
 - PyPI package can be installed without compiling,
   at the cost of being twice as slow as the original *ecCodes* module,
 - an optional compile step makes the code as fast as the original module
   but it needs the recommended (the most up-to-date) version of *ecCodes*.
```

### Comparing `eccodes-1.5.2/docs/conf.py` & `eccodes-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/docs/index.rst` & `eccodes-1.6.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Python 3 interface to encode and decode GRIB and BUFR files via the
 `ECMWF ecCodes library <https://confluence.ecmwf.int/display/ECC/>`_.
 
 Features:
 
 - reads and writes GRIB 1 and 2 files,
 - reads and writes BUFR 3 and 4 files,
-- supports all modern versions of Python 3.9, 3.8, 3.7 and PyPy3,
+- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8 and PyPy3,
 - works on most *Linux* distributions and *MacOS*, the *ecCodes* C-library is the only system dependency,
 - PyPI package can be installed without compiling,
   at the cost of being twice as slow as the original *ecCodes* module,
 - an optional compile step makes the code as fast as the original module
   but it needs the recommended (the most up-to-date) version of *ecCodes*.
 
 Limitations:
```

### Comparing `eccodes-1.5.2/eccodes/__main__.py` & `eccodes-1.6.0/eccodes/__main__.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/eccodes/eccodes.py` & `eccodes-1.6.0/eccodes/eccodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from gribapi import any_new_from_file as codes_any_new_from_file
 from gribapi import bindings_version
 from gribapi import bufr_new_from_file as codes_bufr_new_from_file
 from gribapi import (
     codes_any_new_from_samples,
     codes_bufr_copy_data,
     codes_bufr_extract_headers,
+    codes_bufr_key_is_coordinate,
     codes_bufr_key_is_header,
     codes_bufr_keys_iterator_delete,
     codes_bufr_keys_iterator_get_name,
     codes_bufr_keys_iterator_new,
     codes_bufr_keys_iterator_next,
     codes_bufr_keys_iterator_rewind,
     codes_bufr_multi_element_constant_arrays_off,
@@ -60,14 +61,15 @@
 from gribapi import grib_get_array as codes_get_array
 from gribapi import grib_get_data as codes_grib_get_data
 from gribapi import grib_get_double as codes_get_double
 from gribapi import grib_get_double_array as codes_get_double_array
 from gribapi import grib_get_double_element as codes_get_double_element
 from gribapi import grib_get_double_elements as codes_get_double_elements
 from gribapi import grib_get_elements as codes_get_elements
+from gribapi import grib_get_float_array as codes_get_float_array
 from gribapi import grib_get_long as codes_get_long
 from gribapi import grib_get_long_array as codes_get_long_array
 from gribapi import grib_get_message as codes_get_message
 from gribapi import grib_get_message_offset as codes_get_message_offset
 from gribapi import grib_get_message_size as codes_get_message_size
 from gribapi import grib_get_native_type as codes_get_native_type
 from gribapi import grib_get_size as codes_get_size
@@ -222,14 +224,15 @@
     "bindings_version",
     "BufferTooSmallError",
     "CodeNotFoundInTableError",
     "codes_any_new_from_file",
     "codes_bufr_copy_data",
     "codes_bufr_extract_headers",
     "codes_bufr_key_is_header",
+    "codes_bufr_key_is_coordinate",
     "codes_bufr_keys_iterator_delete",
     "codes_bufr_keys_iterator_get_name",
     "codes_bufr_keys_iterator_new",
     "codes_bufr_keys_iterator_next",
     "codes_bufr_keys_iterator_rewind",
     "codes_bufr_multi_element_constant_arrays_off",
     "codes_bufr_multi_element_constant_arrays_on",
@@ -245,14 +248,15 @@
     "codes_get_api_version",
     "codes_get_array",
     "codes_get_double_array",
     "codes_get_double_element",
     "codes_get_double_elements",
     "codes_get_double",
     "codes_get_elements",
+    "codes_get_float_array",
     "codes_get_gaussian_latitudes",
     "codes_get_library_path",
     "codes_get_long_array",
     "codes_get_long",
     "codes_get_message_offset",
     "codes_get_message_size",
     "codes_get_message",
```

### Comparing `eccodes-1.5.2/eccodes/highlevel/message.py` & `eccodes-1.6.0/eccodes/highlevel/message.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/eccodes/highlevel/reader.py` & `eccodes-1.6.0/eccodes/highlevel/reader.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/eccodes.egg-info/PKG-INFO` & `eccodes-1.6.0/eccodes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: eccodes
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python interface to the ecCodes GRIB and BUFR decoder/encoder
 Home-page: https://github.com/ecmwf/eccodes-python
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: ecCodes GRIB BUFR
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
@@ -26,15 +25,15 @@
 Python 3 interface to decode and encode GRIB and BUFR files via the
 `ECMWF ecCodes library <https://confluence.ecmwf.int/display/ECC/>`_.
 
 Features:
 
 - reads and writes GRIB 1 and 2 files,
 - reads and writes BUFR 3 and 4 files,
-- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8, 3.7 and PyPy3,
+- supports all modern versions of Python 3.11, 3.10, 3.9, 3.8 and PyPy3,
 - works on most *Linux* distributions and *MacOS*, the *ecCodes* C-library
   is the only system dependency,
 - PyPI package can be installed without compiling,
   at the cost of being twice as slow as the original *ecCodes* module,
 - an optional compile step makes the code as fast as the original module
   but it needs the recommended (the most up-to-date) version of *ecCodes*.
 
@@ -148,14 +147,23 @@
 In applying this licence, ECMWF does not waive the privileges and immunities
 granted to it by virtue of its status as an intergovernmental organisation nor
 does it submit to any jurisdiction.
 
 Changelog for eccodes-python
 ============================
 
+
+1.6.0 (2023-07-11)
+--------------------
+
+- ECC-1630: Get API version as an integer
+- ECC-1622: Drop Python version 3.7
+- ECC-1601: GRIB: Support data values array decoded in single-precision
+- ECC-1611: Add function to determine if a BUFR key is a coordinate descriptor
+
 1.5.2 (2023-04-04)
 --------------------
 
 - Add support for Python versions 3.10 and 3.11
 - ECC-1555: 2D numpy array incorrectly handled
 - ECC-1539: Use the 'warnings' library for selfcheck
 - ECC-1538: Add support for CODES_TYPE_BYTES
```

### Comparing `eccodes-1.5.2/eccodes.egg-info/SOURCES.txt` & `eccodes-1.6.0/eccodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/gribapi/__init__.py` & `eccodes-1.6.0/gribapi/__init__.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/gribapi/bindings.py` & `eccodes-1.6.0/gribapi/bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import logging
 import pkgutil
 
 import cffi
 
-__version__ = "1.5.2"
+__version__ = "1.6.0"
 
 LOG = logging.getLogger(__name__)
 
 try:
     import ecmwflibs as findlibs
 except ImportError:
     import findlibs
```

### Comparing `eccodes-1.5.2/gribapi/eccodes.h` & `eccodes-1.6.0/gribapi/eccodes.h`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,26 @@
  * This software is licensed under the terms of the Apache Licence Version 2.0
  * which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
  *
  * In applying this licence, ECMWF does not waive the privileges and immunities granted to it by
  * virtue of its status as an intergovernmental organisation nor does it submit to any jurisdiction.
  */
 
-typedef struct grib_handle            codes_handle;
-typedef struct grib_context           codes_context;
+typedef struct grib_handle    codes_handle;
+typedef struct grib_context   codes_context;
 
 grib_handle* codes_handle_new_from_file(codes_context* c, FILE* f, ProductKind product, int* error);
 
 codes_handle* codes_bufr_handle_new_from_samples(codes_context* c, const char* sample_name);
 codes_handle* codes_handle_new_from_samples(codes_context* c, const char* sample_name);
 
 int codes_bufr_copy_data(grib_handle* hin, grib_handle* hout);
 
 void codes_bufr_multi_element_constant_arrays_on(codes_context* c);
 void codes_bufr_multi_element_constant_arrays_off(codes_context* c);
 int codes_bufr_extract_headers_malloc(codes_context* c, const char* filename, codes_bufr_header** result, int* num_messages, int strict_mode);
-int codes_extract_offsets_malloc(grib_context* c, const char* filename, ProductKind product, long int** offsets, int* num_messages, int strict_mode);
+int codes_extract_offsets_malloc(codes_context* c, const char* filename, ProductKind product, long int** offsets, int* num_messages, int strict_mode);
 int codes_bufr_key_is_header(const codes_handle* h, const char* key, int* err);
+int codes_bufr_key_is_coordinate(const codes_handle* h, const char* key, int* err);
 
 char* codes_samples_path(const codes_context *c);
 char* codes_definition_path(const codes_context *c);
```

### Comparing `eccodes-1.5.2/gribapi/errors.py` & `eccodes-1.6.0/gribapi/errors.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/gribapi/grib_api.h` & `eccodes-1.6.0/gribapi/grib_api.h`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 int grib_get_long(const grib_handle* h, const char* key, long* value);
 int grib_get_double(const grib_handle* h, const char* key, double* value);
 int grib_get_double_element(const grib_handle* h, const char* key, int i, double* value);
 int grib_get_double_elements(const grib_handle* h, const char* key, const int* index_array, long size, double* value);
 int grib_get_string(const grib_handle* h, const char* key, char* mesg, size_t *length);
 int grib_get_string_array(const grib_handle* h, const char* key, char** vals, size_t *length);
 int grib_get_double_array(const grib_handle* h, const char* key, double* vals, size_t *length);
+int grib_get_float_array(const grib_handle* h, const char* key, float* vals, size_t *length);
 int grib_get_long_array(const grib_handle* h, const char* key, long* vals, size_t *length);
 
 int grib_copy_namespace(grib_handle* dest, const char* name, grib_handle* src);
 int grib_set_long(grib_handle* h, const char* key, long val);
 int grib_set_double(grib_handle* h, const char* key, double val);
 int grib_set_string(grib_handle* h, const char* key, const char* mesg, size_t *length);
 int grib_set_double_array(grib_handle* h, const char*  key , const double*        vals   , size_t length);
```

### Comparing `eccodes-1.5.2/gribapi/gribapi.py` & `eccodes-1.6.0/gribapi/gribapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 The Python 3 interface to ecCodes uses the <a href="http://numpy.scipy.org/"><b>NumPy</b></a> package
 as the container of choice for the possible arrays of values that can be encoded/decoded in and from a message.
 Numpy is a package used for scientific computing in Python and an efficient container for generic data.
 
 @em Requirements:
 
-    - Python 3.7 or higher
+    - Python 3.8 or higher
     - NumPy
 
 """
 
 import os
 import sys
 from functools import wraps
@@ -1191,14 +1191,34 @@
     arr = np.empty((nval,), dtype="float64")
     vals_p = ffi.cast("double *", arr.ctypes.data)
     err = lib.grib_get_double_array(h, key.encode(ENC), vals_p, length_p)
     GRIB_CHECK(err)
     return arr
 
 
+@require(msgid=int, key=str)
+def grib_get_float_array(msgid, key):
+    """
+    @brief Get the value of the key as a NumPy array of floats.
+
+    @param msgid   id of the message loaded in memory
+    @param key     key name
+    @return        numpy.ndarray
+    @exception CodesInternalError
+    """
+    h = get_handle(msgid)
+    nval = grib_get_size(msgid, key)
+    length_p = ffi.new("size_t*", nval)
+    arr = np.empty((nval,), dtype="float32")
+    vals_p = ffi.cast("float *", arr.ctypes.data)
+    err = lib.grib_get_float_array(h, key.encode(ENC), vals_p, length_p)
+    GRIB_CHECK(err)
+    return arr
+
+
 # See ECC-1246
 def _decode_bytes(binput, maxlen=None):
     if maxlen:
         a_str = ffi.string(binput, maxlen)
     else:
         a_str = ffi.string(binput)
     # Check for a MISSING value i.e., each character has all its bits=1
@@ -1943,25 +1963,25 @@
 @require(msgid=int, key=str)
 def grib_get(msgid, key, ktype=None):
     r"""
     @brief Get the value of a key in a message.
 
     The type of value returned depends on the native type of the requested key.
     The type of value returned can be forced by using the type argument of the
-    function. The type argument can be int, float or str.
+    function. The ktype argument can be int, float, str or bytes.
 
     The \em msgid references a message loaded in memory.
 
     \b Examples: \ref grib_get_keys.py "grib_get_keys.py", \ref grib_print_data.py "grib_print_data.py"
 
     @see grib_new_from_file, grib_release, grib_set
 
     @param msgid      id of the message loaded in memory
     @param key        key name
-    @param ktype      the type we want the output in (int, float or str), native type if not specified
+    @param ktype      the type we want the output in, native type if not specified
     @return           scalar value of key as int, float or str
     @exception CodesInternalError
     """
     if not key:
         raise ValueError("Invalid key name")
 
     if ktype is None:
@@ -1983,53 +2003,67 @@
 @require(msgid=int, key=str)
 def grib_get_array(msgid, key, ktype=None):
     """
     @brief Get the contents of an array key.
 
     The type of the array returned depends on the native type of the requested key.
     For numeric data, the output array will be stored in a NumPy ndarray.
-    The type of value returned can be forced by using the type argument of the function.
-    The type argument can be int, float or string.
+    The type of value returned can be forced by using the ktype argument of the function.
+    The ktype argument can be int, float, float32, float64, str or bytes.
 
-    @param msgid      id of the message loaded in memory
-    @param key        the key to get the value for
-    @param ktype      the type we want the output in (can be int, float or string), native type if not specified
-    @return           numpy.ndarray
+    @param msgid  id of the message loaded in memory
+    @param key    the key to get the value for
+    @param ktype  the type we want the output in, native type if not specified
+    @return       numpy.ndarray or None
     @exception CodesInternalError
     """
     if ktype is None:
         ktype = grib_get_native_type(msgid, key)
 
     result = None
     if ktype is int:
         result = grib_get_long_array(msgid, key)
-    elif ktype is float:
+    elif ktype is float or ktype is np.float64:
         result = grib_get_double_array(msgid, key)
+    elif ktype is np.float32:
+        result = grib_get_float_array(msgid, key)
     elif ktype is str:
         result = grib_get_string_array(msgid, key)
     elif ktype is bytes:
         result = grib_get_string_array(msgid, key)
 
     return result
 
 
 @require(gribid=int)
-def grib_get_values(gribid):
+def grib_get_values(gribid, ktype=float):
     """
     @brief Retrieve the contents of the 'values' key for a GRIB message.
 
     A NumPy ndarray containing the values in the GRIB message is returned.
 
     \b Examples: \ref grib_print_data.py "grib_print_data.py", \ref grib_samples.py "grib_samples.py"
 
-    @param gribid   id of the GRIB loaded in memory
-    @return         numpy.ndarray
+    @param gribid    id of the GRIB loaded in memory
+    @param ktype     data type of the result: numpy.float32 or numpy.float64
+    @return          numpy.ndarray
     @exception CodesInternalError
     """
-    return grib_get_double_array(gribid, "values")
+    result = None
+
+    if ktype is np.float32:
+        result = grib_get_float_array(gribid, "values")
+    elif ktype is np.float64 or ktype is float:
+        result = grib_get_double_array(gribid, "values")
+    else:
+        raise TypeError(
+            f"Unsupported data type {ktype}. Supported data types are numpy.float32 and numpy.float64"
+        )
+
+    return result
 
 
 @require(gribid=int)
 def grib_get_data(gribid):
     """
     @brief Get array containing latitude/longitude and data values.
 
@@ -2245,33 +2279,37 @@
     context = lib.grib_context_get_default()
     if flag:
         lib.grib_gts_header_on(context)
     else:
         lib.grib_gts_header_off(context)
 
 
-def grib_get_api_version():
+def grib_get_api_version(vformat=str):
     """
     @brief Get the API version.
 
-    Returns the version of the API as a string in the format "major.minor.revision".
+    Returns the version of the API as a string in the format "major.minor.revision"
+    or as an integer (10000*major + 100*minor + revision)
     """
 
     def div(v, d):
         return (v / d, v % d)
 
     if not lib:
         raise RuntimeError("Could not load the ecCodes library!")
 
     v = lib.grib_get_api_version()
-    v, revision = div(v, 100)
-    v, minor = div(v, 100)
-    major = v
 
-    return "%d.%d.%d" % (major, minor, revision)
+    if vformat is str:
+        v, revision = div(v, 100)
+        v, minor = div(v, 100)
+        major = v
+        return "%d.%d.%d" % (major, minor, revision)
+    else:
+        return v
 
 
 __version__ = grib_get_api_version()
 
 
 def codes_get_version_info():
     """
@@ -2490,14 +2528,33 @@
     """
     h = get_handle(msgid)
     err, value = err_last(lib.codes_bufr_key_is_header)(h, key.encode(ENC))
     GRIB_CHECK(err)
     return value
 
 
+@require(msgid=int)
+def codes_bufr_key_is_coordinate(msgid, key):
+    """
+    @brief Check if the BUFR key corresponds to a coordinate descriptor.
+
+    If the data section has not been unpacked, then passing in a key from
+    the data section will throw KeyValueNotFoundError.
+
+    @param msgid      id of the BUFR message loaded in memory
+    @param key        key name
+    @return           1->coordinate, 0->not coordinate
+    @exception CodesInternalError
+    """
+    h = get_handle(msgid)
+    err, value = err_last(lib.codes_bufr_key_is_coordinate)(h, key.encode(ENC))
+    GRIB_CHECK(err)
+    return value
+
+
 def codes_extract_offsets(filepath, product_kind, is_strict=True):
     """
     @brief Message offset extraction
 
     @param filepath   path of input file
     @product_kind     one of CODES_PRODUCT_GRIB, CODES_PRODUCT_BUFR, CODES_PRODUCT_ANY or CODES_PRODUCT_GTS
     @param is_strict  if True, fail as soon as any invalid message is encountered
```

### Comparing `eccodes-1.5.2/setup.cfg` & `eccodes-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/setup.py` & `eccodes-1.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 
 install_requires = ["numpy"]
 if sys.version_info < (3, 7):
     install_requires = ["numpy<1.20"]
 elif sys.version_info < (3, 8):
     install_requires = ["numpy<1.22"]
+elif sys.version_info < (3, 9):
+    install_requires = ["numpy<1.25"]
 
 install_requires += ["attrs", "cffi", "findlibs"]
 
 setuptools.setup(
     name="eccodes",
     version=parse_version_from("gribapi/bindings.py"),
     description="Python interface to the ecCodes GRIB and BUFR decoder/encoder",
@@ -64,15 +66,14 @@
     test_suite="tests",
     zip_safe=True,
     keywords="ecCodes GRIB BUFR",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent",
```

### Comparing `eccodes-1.5.2/tests/sample-data/era5-levels-members.grib` & `eccodes-1.6.0/tests/sample-data/era5-levels-members.grib`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/tests/sample-data/tiggelam_cnmc_sfc.grib2` & `eccodes-1.6.0/tests/sample-data/tiggelam_cnmc_sfc.grib2`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/tests/test_20_messages.py` & `eccodes-1.6.0/tests/test_20_messages.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/tests/test_eccodes.py` & `eccodes-1.6.0/tests/test_eccodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,29 @@
     eccodes.eccodes.codes_set_definitions_path(eccodes.codes_definition_path())
 
 
 def test_codes_set_samples_path():
     eccodes.codes_set_samples_path(eccodes.codes_samples_path())
 
 
+def test_api_version():
+    vs = eccodes.codes_get_api_version()
+    assert type(vs) == str
+    assert len(vs) > 0
+    assert vs == eccodes.codes_get_api_version(str)
+    vi = eccodes.codes_get_api_version(int)
+    assert type(vi) == int
+    assert vi > 20000
+    print(vi)
+
+
 def test_version_info():
     vinfo = eccodes.codes_get_version_info()
     assert len(vinfo) == 2
+    print(vinfo)
 
 
 def test_codes_is_defined():
     gid = eccodes.codes_grib_new_from_samples("sh_sfc_grib1")
     assert eccodes.codes_is_defined(gid, "JS")
 
 
@@ -258,14 +270,34 @@
     gid = eccodes.codes_grib_new_from_samples("reduced_gg_pl_160_grib2")
     pl = eccodes.codes_get_array(gid, "pl")
     assert pl[0] == 18
     pli = eccodes.codes_get_array(gid, "pl", int)
     assert np.array_equal(pl, pli)
     pls = eccodes.codes_get_array(gid, "centre", str)
     assert pls == ["ecmf"]
+    dvals = eccodes.codes_get_array(gid, "values")
+    assert len(dvals) == 138346
+    assert type(dvals[0]) == np.float64
+    eccodes.codes_release(gid)
+
+
+def _test_grib_get_array_single_precision():
+    gid = eccodes.codes_grib_new_from_samples("reduced_gg_pl_160_grib2")
+
+    dvals = eccodes.codes_get_array(gid, "values", ktype=float)
+    assert type(dvals[0]) == np.float64
+    fvals = eccodes.codes_get_array(gid, "values", ktype=np.float32)
+    assert type(fvals[0]) == np.float32
+    fvals = eccodes.codes_get_float_array(gid, "values")
+    assert type(fvals[0]) == np.float32
+    dvals = eccodes.codes_get_values(gid)
+    assert type(dvals[0]) == np.float64
+    fvals = eccodes.codes_get_values(gid, np.float32)
+    assert type(fvals[0]) == np.float32
+
     eccodes.codes_release(gid)
 
 
 def test_grib_gaussian_latitudes():
     orders = [256, 1280]
     # Latitude of the first element (nearest the north pole)
     expected_lats = [89.731148, 89.946187]
@@ -545,15 +577,15 @@
 def test_gribex_mode():
     eccodes.codes_gribex_mode_on()
     eccodes.codes_gribex_mode_off()
 
 
 def test_grib_new_from_samples_error():
     with pytest.raises(eccodes.FileNotFoundError):
-        eccodes.codes_new_from_samples("poopoo", eccodes.CODES_PRODUCT_GRIB)
+        eccodes.codes_new_from_samples("nonExistentSample", eccodes.CODES_PRODUCT_GRIB)
 
 
 def test_grib_new_from_file_error(tmp_path):
     # Note: AssertionError can be raised when type checks are enabled
     with pytest.raises((TypeError, AssertionError)):
         eccodes.codes_grib_new_from_file(None)
     p = tmp_path / "afile.txt"
@@ -813,19 +845,31 @@
     assert eccodes.codes_bufr_key_is_header(bid, "satelliteID")
     assert eccodes.codes_bufr_key_is_header(bid, "unexpandedDescriptors")
 
     with pytest.raises(eccodes.KeyValueNotFoundError):
         eccodes.codes_bufr_key_is_header(bid, "satelliteSensorIndicator")
 
     eccodes.codes_set(bid, "unpack", 1)
-
     assert not eccodes.codes_bufr_key_is_header(bid, "satelliteSensorIndicator")
     assert not eccodes.codes_bufr_key_is_header(bid, "#6#brightnessTemperature")
 
 
+def _test_codes_bufr_key_is_coordinate():
+    bid = eccodes.codes_bufr_new_from_samples("BUFR4")
+    assert not eccodes.codes_bufr_key_is_coordinate(bid, "edition")
+
+    with pytest.raises(eccodes.KeyValueNotFoundError):
+        eccodes.codes_bufr_key_is_coordinate(bid, "latitude")
+
+    eccodes.codes_set(bid, "unpack", 1)
+    assert eccodes.codes_bufr_key_is_coordinate(bid, "latitude")
+    assert eccodes.codes_bufr_key_is_coordinate(bid, "#14#timePeriod")
+    assert not eccodes.codes_bufr_key_is_coordinate(bid, "dewpointTemperature")
+
+
 def test_bufr_extract_headers():
     fpath = get_sample_fullpath("BUFR4_local.tmpl")
     if fpath is None:
         return
     headers = list(eccodes.codes_bufr_extract_headers(fpath))
     # Sample file contains just one message
     assert len(headers) == 1
```

### Comparing `eccodes-1.5.2/tests/test_highlevel.py` & `eccodes-1.6.0/tests/test_highlevel.py`

 * *Files identical despite different names*

### Comparing `eccodes-1.5.2/tox.ini` & `eccodes-1.6.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 commands = pytest -v --flakes --cache-clear --basetemp={envtmpdir} {posargs}
 
 [testenv:docs]
 deps = -r{toxinidir}/ci/requirements-docs.txt
 commands = sphinx-build -W -b html docs build/sphinx/html
 
 [testenv:qc]
-basepython = python3.7
+basepython = python3.8
 # needed for pytest-cov
 usedevelop = true
 commands = pytest -v --flakes --pep8 --mccabe --cov=eccodes --doctest-glob="*.rst" --cov-report=html --cache-clear --basetemp={envtmpdir} {posargs}
 
 [testenv:deps]
 deps =
 commands = python setup.py test
```

