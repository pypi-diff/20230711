# Comparing `tmp/speechmatics-python-1.8.4.tar.gz` & `tmp/speechmatics-python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechmatics-python-1.8.4.tar", last modified: Wed Jul  5 09:06:20 2023, max compression
+gzip compressed data, was "speechmatics-python-1.9.0.tar", last modified: Tue Jul 11 17:04:45 2023, max compression
```

## Comparing `speechmatics-python-1.8.4.tar` & `speechmatics-python-1.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/speechmatics/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/batch_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28496 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/speechmatics_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/mock_rt_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    25863 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_cli_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:04:45.572542 speechmatics-python-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-11 17:04:45.572542 speechmatics-python-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 17:04:45.572542 speechmatics-python-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:04:45.572542 speechmatics-python-1.9.0/speechmatics/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/batch_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28496 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/speechmatics/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:04:45.572542 speechmatics-python-1.9.0/speechmatics_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-11 17:04:45.000000 speechmatics-python-1.9.0/speechmatics_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-11 17:04:45.000000 speechmatics-python-1.9.0/speechmatics_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:04:45.000000 speechmatics-python-1.9.0/speechmatics_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:04:45.000000 speechmatics-python-1.9.0/speechmatics_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 17:04:45.000000 speechmatics-python-1.9.0/speechmatics_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:04:45.000000 speechmatics-python-1.9.0/speechmatics_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:04:45.572542 speechmatics-python-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/mock_rt_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25863 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/test_cli_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-11 17:04:36.000000 speechmatics-python-1.9.0/tests/utils.py
```

### Comparing `speechmatics-python-1.8.4/CHANGELOG.md` & `speechmatics-python-1.9.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/LICENSE.txt` & `speechmatics-python-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/PKG-INFO` & `speechmatics-python-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmatics-python
-Version: 1.8.4
+Version: 1.9.0
 Summary: Python library and CLI for Speechmatics
 Home-page: https://github.com/speechmatics/speechmatics-python/
 Author: Speechmatics
 Author-email: support@speechmatics.com
 License: MIT
 Project-URL: Documentation, https://speechmatics.github.io/speechmatics-python/
 Project-URL: Source Code, https://github.com/speechmatics/speechmatics-python/
```

### Comparing `speechmatics-python-1.8.4/README.md` & `speechmatics-python-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/setup.py` & `speechmatics-python-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/adapters.py` & `speechmatics-python-1.9.0/speechmatics/adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/batch_client.py` & `speechmatics-python-1.9.0/speechmatics/batch_client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/cli.py` & `speechmatics-python-1.9.0/speechmatics/cli.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/cli_parser.py` & `speechmatics-python-1.9.0/speechmatics/cli_parser.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/client.py` & `speechmatics-python-1.9.0/speechmatics/client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/config.py` & `speechmatics-python-1.9.0/speechmatics/config.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/exceptions.py` & `speechmatics-python-1.9.0/speechmatics/exceptions.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/helpers.py` & `speechmatics-python-1.9.0/speechmatics/helpers.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics/models.py` & `speechmatics-python-1.9.0/speechmatics/models.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/speechmatics_python.egg-info/PKG-INFO` & `speechmatics-python-1.9.0/speechmatics_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmatics-python
-Version: 1.8.4
+Version: 1.9.0
 Summary: Python library and CLI for Speechmatics
 Home-page: https://github.com/speechmatics/speechmatics-python/
 Author: Speechmatics
 Author-email: support@speechmatics.com
 License: MIT
 Project-URL: Documentation, https://speechmatics.github.io/speechmatics-python/
 Project-URL: Source Code, https://github.com/speechmatics/speechmatics-python/
```

### Comparing `speechmatics-python-1.8.4/speechmatics_python.egg-info/SOURCES.txt` & `speechmatics-python-1.9.0/speechmatics_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/conftest.py` & `speechmatics-python-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/mock_rt_server.py` & `speechmatics-python-1.9.0/tests/mock_rt_server.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/test_adapters.py` & `speechmatics-python-1.9.0/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/test_cli.py` & `speechmatics-python-1.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/test_cli_handlers.py` & `speechmatics-python-1.9.0/tests/test_cli_handlers.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/test_client.py` & `speechmatics-python-1.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/test_models.py` & `speechmatics-python-1.9.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.4/tests/utils.py` & `speechmatics-python-1.9.0/tests/utils.py`

 * *Files identical despite different names*

