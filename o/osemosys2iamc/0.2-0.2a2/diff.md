# Comparing `tmp/osemosys2iamc-0.2.tar.gz` & `tmp/osemosys2iamc-0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osemosys2iamc-0.2.tar", last modified: Tue Jul 11 12:22:57 2023, max compression
+gzip compressed data, was "osemosys2iamc-0.2a2.tar", last modified: Tue Jul 11 10:54:24 2023, max compression
```

## Comparing `osemosys2iamc-0.2.tar` & `osemosys2iamc-0.2a2.tar`

### file list

```diff
@@ -1,46 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.477452 osemosys2iamc-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.465452 osemosys2iamc-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.473452 osemosys2iamc-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-11 12:22:57.477452 osemosys2iamc-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-11 12:22:57.481452 osemosys2iamc-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.465452 osemosys2iamc-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.473452 osemosys2iamc-0.2/src/osemosys2iamc/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/src/osemosys2iamc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/src/osemosys2iamc/resultify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.473452 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 12:22:57.000000 osemosys2iamc-0.2/src/osemosys2iamc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.477452 osemosys2iamc-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:22:57.477452 osemosys2iamc-0.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/AnnualTechnologyEmissions.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/Demand.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/ProductionByTechnologyAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/TotalCapacityAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/UseByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/config_input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/config_result.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/fixtures/config_result_capture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tests/test_resultify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-11 12:22:46.000000 osemosys2iamc-0.2/tox.ini
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.506636 osemosys2iamc-0.2a2/
+-rw-r--r--   0 wusher     (501) staff       (20)      596 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/.coveragerc
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.466470 osemosys2iamc-0.2a2/.github/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.476819 osemosys2iamc-0.2a2/.github/workflows/
+-rw-r--r--   0 wusher     (501) staff       (20)      911 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/.github/workflows/pytest.yml
+-rw-r--r--   0 wusher     (501) staff       (20)     1111 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 wusher     (501) staff       (20)      653 2022-12-14 13:36:48.000000 osemosys2iamc-0.2a2/.gitignore
+-rw-r--r--   0 wusher     (501) staff       (20)      261 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/.pre-commit-config.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)       99 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/AUTHORS.rst
+-rw-r--r--   0 wusher     (501) staff       (20)      111 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/CHANGELOG.rst
+-rw-r--r--   0 wusher     (501) staff       (20)    12790 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/CONTRIBUTING.rst
+-rwxr-xr-x   0 wusher     (501) staff       (20)     1090 2022-12-14 13:36:48.000000 osemosys2iamc-0.2a2/LICENSE.txt
+-rw-r--r--   0 wusher     (501) staff       (20)     8782 2023-07-11 10:54:24.507135 osemosys2iamc-0.2a2/PKG-INFO
+-rw-r--r--   0 wusher     (501) staff       (20)     8175 2023-07-11 10:53:16.000000 osemosys2iamc-0.2a2/README.md
+-rw-r--r--   0 wusher     (501) staff       (20)      355 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/pyproject.toml
+-rw-r--r--   0 wusher     (501) staff       (20)       99 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/requirements.txt
+-rw-r--r--   0 wusher     (501) staff       (20)     1543 2023-07-11 10:54:24.508928 osemosys2iamc-0.2a2/setup.cfg
+-rw-r--r--   0 wusher     (501) staff       (20)      710 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/setup.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.468272 osemosys2iamc-0.2a2/src/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.478378 osemosys2iamc-0.2a2/src/openentrance/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.467251 osemosys2iamc-0.2a2/src/openentrance/definitions/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.467458 osemosys2iamc-0.2a2/src/openentrance/definitions/region/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.480535 osemosys2iamc-0.2a2/src/openentrance/definitions/region/data/
+-rw-r--r--   0 wusher     (501) staff       (20)     1113 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/definitions/region/data/write-countries.py
+-rw-r--r--   0 wusher     (501) staff       (20)     2250 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/definitions/region/data/write-nuts.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.481503 osemosys2iamc-0.2a2/src/openentrance/openentrance/
+-rw-r--r--   0 wusher     (501) staff       (20)     1559 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/openentrance/__init__.py
+-rw-r--r--   0 wusher     (501) staff       (20)       58 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/setup.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.484136 osemosys2iamc-0.2a2/src/openentrance/tests/
+-rw-r--r--   0 wusher     (501) staff       (20)      414 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/tests/test_core.py
+-rw-r--r--   0 wusher     (501) staff       (20)     1801 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/tests/test_definitions.py
+-rw-r--r--   0 wusher     (501) staff       (20)     2690 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/tests/test_validate.py
+-rwxr-xr-x   0 wusher     (501) staff       (20)     3103 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/workflow.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.485928 osemosys2iamc-0.2a2/src/osemosys2iamc/
+-rw-r--r--   0 wusher     (501) staff       (20)      577 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/src/osemosys2iamc/__init__.py
+-rw-r--r--   0 wusher     (501) staff       (20)    18663 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/src/osemosys2iamc/resultify.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.491325 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/
+-rw-r--r--   0 wusher     (501) staff       (20)     8782 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/PKG-INFO
+-rw-r--r--   0 wusher     (501) staff       (20)     1329 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/SOURCES.txt
+-rw-r--r--   0 wusher     (501) staff       (20)        1 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/dependency_links.txt
+-rw-r--r--   0 wusher     (501) staff       (20)       70 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/entry_points.txt
+-rw-r--r--   0 wusher     (501) staff       (20)        1 2023-07-11 10:54:23.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/not-zip-safe
+-rw-r--r--   0 wusher     (501) staff       (20)      127 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/requires.txt
+-rw-r--r--   0 wusher     (501) staff       (20)       27 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/top_level.txt
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.495243 osemosys2iamc-0.2a2/tests/
+-rw-r--r--   0 wusher     (501) staff       (20)      281 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/tests/conftest.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.505906 osemosys2iamc-0.2a2/tests/fixtures/
+-rw-r--r--   0 wusher     (501) staff       (20)      733 2022-04-06 09:10:17.000000 osemosys2iamc-0.2a2/tests/fixtures/AnnualTechnologyEmissions.csv
+-rw-r--r--   0 wusher     (501) staff       (20)     1295 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/Demand.csv
+-rw-r--r--   0 wusher     (501) staff       (20)     1320 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/ProductionByTechnologyAnnual.csv
+-rw-r--r--   0 wusher     (501) staff       (20)      481 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/TotalCapacityAnnual.csv
+-rw-r--r--   0 wusher     (501) staff       (20)     1480 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/UseByTechnology.csv
+-rw-r--r--   0 wusher     (501) staff       (20)      453 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/VariableCost.csv
+-rw-r--r--   0 wusher     (501) staff       (20)      345 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/tests/fixtures/config_input.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)      325 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/tests/fixtures/config_result.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)      380 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/tests/fixtures/config_result_capture.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)      741 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/test_cli.py
+-rw-r--r--   0 wusher     (501) staff       (20)     3682 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/test_main.py
+-rw-r--r--   0 wusher     (501) staff       (20)    20554 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/test_resultify.py
+-rw-r--r--   0 wusher     (501) staff       (20)     2553 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tox.ini
```

### Comparing `osemosys2iamc-0.2/.coveragerc` & `osemosys2iamc-0.2a2/.coveragerc`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/.github/workflows/pytest.yml` & `osemosys2iamc-0.2a2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/.github/workflows/python-publish.yml` & `osemosys2iamc-0.2a2/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 permissions:
   contents: read
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
-    environment: release
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
```

### Comparing `osemosys2iamc-0.2/.gitignore` & `osemosys2iamc-0.2a2/.gitignore`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/CONTRIBUTING.rst` & `osemosys2iamc-0.2a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/LICENSE.txt` & `osemosys2iamc-0.2a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/PKG-INFO` & `osemosys2iamc-0.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osemosys2iamc
-Version: 0.2
+Version: 0.2a2
 Summary: A utility package to convert OSeMOSYS results into IAMC format
 Home-page: https://github.com/osemosys/osemosys2iamc/
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Source, https://github.com/osemosys/osemosys2iamc/
 Project-URL: Tracker, https://github.com/osemosys/osemosys2iamc/issues
```

### Comparing `osemosys2iamc-0.2/README.md` & `osemosys2iamc-0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/setup.cfg` & `osemosys2iamc-0.2a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/setup.py` & `osemosys2iamc-0.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/src/osemosys2iamc/__init__.py` & `osemosys2iamc-0.2a2/src/osemosys2iamc/__init__.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/src/osemosys2iamc/resultify.py` & `osemosys2iamc-0.2a2/src/osemosys2iamc/resultify.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/src/osemosys2iamc.egg-info/PKG-INFO` & `osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osemosys2iamc
-Version: 0.2
+Version: 0.2a2
 Summary: A utility package to convert OSeMOSYS results into IAMC format
 Home-page: https://github.com/osemosys/osemosys2iamc/
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Source, https://github.com/osemosys/osemosys2iamc/
 Project-URL: Tracker, https://github.com/osemosys/osemosys2iamc/issues
```

### Comparing `osemosys2iamc-0.2/src/osemosys2iamc.egg-info/SOURCES.txt` & `osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/pytest.yml
 .github/workflows/python-publish.yml
+src/openentrance/setup.py
+src/openentrance/workflow.py
+src/openentrance/definitions/region/data/write-countries.py
+src/openentrance/definitions/region/data/write-nuts.py
+src/openentrance/openentrance/__init__.py
+src/openentrance/tests/test_core.py
+src/openentrance/tests/test_definitions.py
+src/openentrance/tests/test_validate.py
 src/osemosys2iamc/__init__.py
 src/osemosys2iamc/resultify.py
 src/osemosys2iamc.egg-info/PKG-INFO
 src/osemosys2iamc.egg-info/SOURCES.txt
 src/osemosys2iamc.egg-info/dependency_links.txt
 src/osemosys2iamc.egg-info/entry_points.txt
 src/osemosys2iamc.egg-info/not-zip-safe
```

### Comparing `osemosys2iamc-0.2/tests/fixtures/AnnualTechnologyEmissions.csv` & `osemosys2iamc-0.2a2/tests/fixtures/AnnualTechnologyEmissions.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tests/fixtures/Demand.csv` & `osemosys2iamc-0.2a2/tests/fixtures/Demand.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tests/fixtures/ProductionByTechnologyAnnual.csv` & `osemosys2iamc-0.2a2/tests/fixtures/ProductionByTechnologyAnnual.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tests/fixtures/UseByTechnology.csv` & `osemosys2iamc-0.2a2/tests/fixtures/UseByTechnology.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tests/test_cli.py` & `osemosys2iamc-0.2a2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tests/test_main.py` & `osemosys2iamc-0.2a2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tests/test_resultify.py` & `osemosys2iamc-0.2a2/tests/test_resultify.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2/tox.ini` & `osemosys2iamc-0.2a2/tox.ini`

 * *Files identical despite different names*

