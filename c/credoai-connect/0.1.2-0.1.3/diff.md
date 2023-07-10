# Comparing `tmp/credoai-connect-0.1.2.tar.gz` & `tmp/credoai-connect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credoai-connect-0.1.2.tar", last modified: Tue May  2 23:05:30 2023, max compression
+gzip compressed data, was "credoai-connect-0.1.3.tar", last modified: Mon Jul 10 22:16:27 2023, max compression
```

## Comparing `credoai-connect-0.1.2.tar` & `credoai-connect-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.514306 credoai-connect-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/adapters/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/evidence/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4700 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/evidence_requirement.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/evidence/lens_evidence/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/governance/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/credo_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     5695 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/credo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    19128 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/governance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/data_scrubbing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/version_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/credoai_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 23:05:30.514306 credoai-connect-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.868889 credoai-connect-0.1.3/connect/
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.868889 credoai-connect-0.1.3/connect/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/adapters/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.868889 credoai-connect-0.1.3/connect/evidence/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4700 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.868889 credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/evidence_requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.868889 credoai-connect-0.1.3/connect/evidence/lens_evidence/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/lens_evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/lens_evidence/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/lens_evidence/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/evidence/lens_evidence/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.868889 credoai-connect-0.1.3/connect/governance/
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/governance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/governance/credo_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5695 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/governance/credo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19128 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/governance/governance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/connect/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/utils/data_scrubbing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/connect/utils/version_check.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/credoai_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-07-10 22:16:27.000000 credoai-connect-0.1.3/credoai_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-07-10 22:16:27.000000 credoai-connect-0.1.3/credoai_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 22:16:27.000000 credoai-connect-0.1.3/credoai_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-10 22:16:27.000000 credoai-connect-0.1.3/credoai_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-10 22:16:27.000000 credoai-connect-0.1.3/credoai_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:27.872889 credoai-connect-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 22:16:19.000000 credoai-connect-0.1.3/tests/__init__.py
```

### Comparing `credoai-connect-0.1.2/LICENSE` & `credoai-connect-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/PKG-INFO` & `credoai-connect-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credoai-connect
-Version: 0.1.2
+Version: 0.1.3
 Summary: Credo AI Connect: Integration point for Credo AI Governance Platform
 Home-page: 
 Download-URL: https://github.com/credo-ai/credoai_connect
 Author: Ian Eisenberg
 Author-email: ian@credo.ai
 Maintainer: Ian Eisenberg
 Maintainer-email: ian@credo.ai
@@ -45,7 +45,18 @@
 ```
 pip install credoai-connect
 ```
 
 ## Documentation
 
 Documentation is hosted by [readthedocs](https://credoai-connect.readthedocs.io/en/stable/).
+
+
+## Logging
+Logging defaults to stdout. In order to collect all logging information into a specific file,
+set the desired location to the environment variable `CREDO_CONNECT_LOG_PATH`. 
+
+
+
+> **Warning**
+> Make sure the destination has write permissions, otherwise you will get a `PermissionError` at the moment you
+> attempt library import.
```

### Comparing `credoai-connect-0.1.2/connect/adapters/adapters.py` & `credoai-connect-0.1.3/connect/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/containers.py` & `credoai-connect-0.1.3/connect/evidence/containers.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/containers.py` & `credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/containers.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/evidence.py` & `credoai-connect-0.1.3/connect/evidence/deepchecks_evidence/evidence.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/evidence.py` & `credoai-connect-0.1.3/connect/evidence/evidence.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/evidence_requirement.py` & `credoai-connect-0.1.3/connect/evidence/evidence_requirement.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/lens_evidence/containers.py` & `credoai-connect-0.1.3/connect/evidence/lens_evidence/containers.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/evidence/lens_evidence/evidence.py` & `credoai-connect-0.1.3/connect/evidence/lens_evidence/evidence.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/governance/credo_api.py` & `credoai-connect-0.1.3/connect/governance/credo_api.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/governance/credo_api_client.py` & `credoai-connect-0.1.3/connect/governance/credo_api_client.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/governance/governance.py` & `credoai-connect-0.1.3/connect/governance/governance.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/utils/common.py` & `credoai-connect-0.1.3/connect/utils/common.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/utils/data_scrubbing.py` & `credoai-connect-0.1.3/connect/utils/data_scrubbing.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/connect/utils/logging.py` & `credoai-connect-0.1.3/connect/utils/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import deque
 from io import StringIO
 from logging import FileHandler, Formatter, Handler, StreamHandler, getLogger
 from os.path import join
+from os import getenv
 from sys import stdout
 
 
 class TailLogHandler(Handler):
     def __init__(self, log_queue):
         Handler.__init__(self)
         self.log_queue = log_queue
@@ -63,13 +64,14 @@
 
     def setup_file(self):
         file_handler = FileHandler(self.file_path)
         file_handler.setFormatter(self.formatter)
         self.logger.addHandler(file_handler)
 
 
-def setup_logger(name="connect", path=None, record_stream=False, logging_level="INFO"):
+def setup_logger(name="connect", record_stream=False, logging_level="INFO"):
+    path = getenv("CREDO_CONNECT_LOG_PATH")
     tmp = Logger(name, path, record_stream, logging_level)
     return tmp.logger, tmp.stream
 
 
-global_logger, global_tail = setup_logger(path=".")
+global_logger, global_tail = setup_logger()
```

### Comparing `credoai-connect-0.1.2/connect/utils/version_check.py` & `credoai-connect-0.1.3/connect/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/credoai_connect.egg-info/PKG-INFO` & `credoai-connect-0.1.3/credoai_connect.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credoai-connect
-Version: 0.1.2
+Version: 0.1.3
 Summary: Credo AI Connect: Integration point for Credo AI Governance Platform
 Home-page: 
 Download-URL: https://github.com/credo-ai/credoai_connect
 Author: Ian Eisenberg
 Author-email: ian@credo.ai
 Maintainer: Ian Eisenberg
 Maintainer-email: ian@credo.ai
@@ -45,7 +45,18 @@
 ```
 pip install credoai-connect
 ```
 
 ## Documentation
 
 Documentation is hosted by [readthedocs](https://credoai-connect.readthedocs.io/en/stable/).
+
+
+## Logging
+Logging defaults to stdout. In order to collect all logging information into a specific file,
+set the desired location to the environment variable `CREDO_CONNECT_LOG_PATH`. 
+
+
+
+> **Warning**
+> Make sure the destination has write permissions, otherwise you will get a `PermissionError` at the moment you
+> attempt library import.
```

### Comparing `credoai-connect-0.1.2/credoai_connect.egg-info/SOURCES.txt` & `credoai-connect-0.1.3/credoai_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.2/setup.py` & `credoai-connect-0.1.3/setup.py`

 * *Files identical despite different names*

