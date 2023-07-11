# Comparing `tmp/pytest_resilient_circuits-49.0.4423.tar.gz` & `tmp/pytest_resilient_circuits-49.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_resilient_circuits-49.0.4423.tar", last modified: Thu Jun  1 15:59:04 2023, max compression
+gzip compressed data, was "pytest_resilient_circuits-49.1.51.tar", last modified: Tue Jul 11 16:15:02 2023, max compression
```

## Comparing `pytest_resilient_circuits-49.0.4423.tar` & `pytest_resilient_circuits-49.1.51.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:04.057552 pytest_resilient_circuits-49.0.4423/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10989 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2023-06-01 15:59:04.057552 pytest_resilient_circuits-49.0.4423/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:04.057552 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      370 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/circuits_fixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:04.057552 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__actions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__attachments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__const.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__functions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__message_destinations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__task.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__wikis.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_POST__attachment.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_POST__table_data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18019 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/mocks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1954 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22326 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/resilient_circuits_fixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:04.057552 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/shared_mock_data/mock_constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:04.057552 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2023-06-01 15:59:03.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2023-06-01 15:59:04.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:59:03.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2023-06-01 15:59:03.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2023-06-01 15:59:03.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2023-06-01 15:59:03.000000 pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2023-06-01 15:59:04.061552 pytest_resilient_circuits-49.0.4423/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2023-06-01 15:57:43.000000 pytest_resilient_circuits-49.0.4423/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:02.845332 pytest_resilient_circuits-49.1.51/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11088 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2023-07-11 16:15:02.845332 pytest_resilient_circuits-49.1.51/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:02.845332 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      370 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/circuits_fixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:02.845332 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__actions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__attachments.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__const.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__functions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__message_destinations.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__task.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      501 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__wikis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_POST__attachment.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_POST__table_data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      542 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18019 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/mocks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1954 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/plugin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22326 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/resilient_circuits_fixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:02.845332 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/shared_mock_data/mock_constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:02.845332 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2023-07-11 16:15:02.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2023-07-11 16:15:02.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:15:02.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2023-07-11 16:15:02.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2023-07-11 16:15:02.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2023-07-11 16:15:02.000000 pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2023-07-11 16:15:02.849332 pytest_resilient_circuits-49.1.51/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      196 2023-07-11 16:13:50.000000 pytest_resilient_circuits-49.1.51/setup.py
```

### Comparing `pytest_resilient_circuits-49.0.4423/CHANGES` & `pytest_resilient_circuits-49.1.51/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07: version 49.1
+* No major changes. Just bumping build number to coincide with other builds
+
 2023-05: version 49.0
 * No major changes. Just bumping build number to coincide with other builds.
 
 2023-02: version 48.0
 * Updated project to use ``pyproject.toml`` and ``setup.cfg`` metadata files. Build backend continues to use ``setuptools``.
   Instead of directly invoking setup.py to get a sdist or wheel, use ``build`` as a build frontend:
```

### Comparing `pytest_resilient_circuits-49.0.4423/PKG-INFO` & `pytest_resilient_circuits-49.1.51/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_resilient_circuits
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Resilient Circuits fixtures for PyTest
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `pytest_resilient_circuits-49.0.4423/README.md` & `pytest_resilient_circuits-49.1.51/README.md`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/LICENSE` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/circuits_fixtures.py` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/circuits_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__actions.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__actions.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__attachments.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__attachments.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__const.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__const.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__functions.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__functions.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__task.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__task.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/misc.py` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/misc.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/mocks.py` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/mocks.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/plugin.py` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits/resilient_circuits_fixtures.py` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits/resilient_circuits_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/PKG-INFO` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-resilient-circuits
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Resilient Circuits fixtures for PyTest
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `pytest_resilient_circuits-49.0.4423/pytest_resilient_circuits.egg-info/SOURCES.txt` & `pytest_resilient_circuits-49.1.51/pytest_resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-49.0.4423/setup.cfg` & `pytest_resilient_circuits-49.1.51/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient-circuits >= 49.0
+	resilient-circuits >= 49.1
 	
 	requests-mock      ~= 1.9
 	
 	ConfigParser       ~= 5.2; python_version >= "3.6"
 	pytest             ~= 7.0; python_version >= "3.6"
 	
 	ConfigParser       ~= 4.0; python_version == "2.7"
```

