# Comparing `tmp/pytest-nhsd-apim-3.3.5.tar.gz` & `tmp/pytest-nhsd-apim-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-nhsd-apim-3.3.5.tar", last modified: Mon Jul 10 14:19:19 2023, max compression
+gzip compressed data, was "pytest-nhsd-apim-3.3.6.tar", last modified: Tue Jul 11 13:03:57 2023, max compression
```

## Comparing `pytest-nhsd-apim-3.3.5.tar` & `pytest-nhsd-apim-3.3.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:19:19.837460 pytest-nhsd-apim-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-10 14:19:19.837460 pytest-nhsd-apim-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 14:19:19.837460 pytest-nhsd-apim-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:19:19.833460 pytest-nhsd-apim-3.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:19:19.837460 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57430 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/apigee_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/auth_journey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/identity_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/nhsd_apim_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/pytest_nhsd_apim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:19:19.837460 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-10 14:19:19.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 14:19:19.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:19:19.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 14:19:19.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 14:19:19.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 14:19:19.000000 pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:19:19.837460 pytest-nhsd-apim-3.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/tests/test_apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-10 14:18:45.000000 pytest-nhsd-apim-3.3.5/tests/test_nhsd_apim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:57.817585 pytest-nhsd-apim-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-11 13:03:57.817585 pytest-nhsd-apim-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 13:03:57.817585 pytest-nhsd-apim-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:57.813585 pytest-nhsd-apim-3.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:57.817585 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57430 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/apigee_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/auth_journey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/identity_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/nhsd_apim_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/pytest_nhsd_apim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:57.817585 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-11 13:03:57.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-11 13:03:57.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:03:57.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 13:03:57.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 13:03:57.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 13:03:57.000000 pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:57.817585 pytest-nhsd-apim-3.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/tests/test_apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-11 13:03:10.000000 pytest-nhsd-apim-3.3.6/tests/test_nhsd_apim.py
```

### Comparing `pytest-nhsd-apim-3.3.5/PKG-INFO` & `pytest-nhsd-apim-3.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.5
+Version: 3.3.6
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
 Author: Adrian Ciobanita
 Author-email: adrian.ciobanita1@nhs.net
 Maintainer: Alex Carrie
 Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
```

### Comparing `pytest-nhsd-apim-3.3.5/README.md` & `pytest-nhsd-apim-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/pyproject.toml` & `pytest-nhsd-apim-3.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pytest-nhsd-apim"
-version = "3.3.5"
+version = "3.3.6"
 description = "Pytest plugin accessing NHSDigital's APIM proxies"
 authors = ["Adrian Ciobanita <adrian.ciobanita1@nhs.net>", "Alex Carrie <alexander.carrie1@nhs.net>", "Lucas Fantini <lucas.fantini@nhs.net>"]
 maintainers = ["Alex Carrie <alexander.carrie1@nhs.net>", "Alex Hawdon <alex.hawdon1@nhs.net"]
 readme = "README.md"
 repository = "https://github.com/NHSDigital/pytest-nhsd-apim"
 classifiers = ["Framework :: Pytest"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 Authlib = "^0.15.5"
 cryptography = ">=36.0.1,<42.0.0"
-lxml = "^4.7.1"
+lxml = "^4.9.1"
 python = "^3.8"
 pycryptodome = "^3.13.0"
 PyJWT = "^2.3.0"
 pyotp = "^2.6.0"
 pytest = "^6.2.5"
 requests = "^2.27.1"
 toml = "^0.10.2"
```

### Comparing `pytest-nhsd-apim-3.3.5/setup.py` & `pytest-nhsd-apim-3.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/apigee_apis.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/apigee_edge.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/apigee_edge.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/auth_journey.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/auth_journey.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/config.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/config.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/identity_service.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/identity_service.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/log.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/log.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/nhsd_apim_authorization.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/nhsd_apim_authorization.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/pytest_nhsd_apim.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/pytest_nhsd_apim.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/secrets.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/secrets.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim/token_cache.py` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim/token_cache.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/PKG-INFO` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.5
+Version: 3.3.6
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
 Author: Adrian Ciobanita
 Author-email: adrian.ciobanita1@nhs.net
 Maintainer: Alex Carrie
 Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
```

### Comparing `pytest-nhsd-apim-3.3.5/src/pytest_nhsd_apim.egg-info/SOURCES.txt` & `pytest-nhsd-apim-3.3.6/src/pytest_nhsd_apim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/tests/test_apigee_apis.py` & `pytest-nhsd-apim-3.3.6/tests/test_apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/tests/test_examples.py` & `pytest-nhsd-apim-3.3.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.5/tests/test_nhsd_apim.py` & `pytest-nhsd-apim-3.3.6/tests/test_nhsd_apim.py`

 * *Files identical despite different names*

