# Comparing `tmp/cru-dse-utils-0.1.3.tar.gz` & `tmp/cru-dse-utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cru-dse-utils-0.1.3.tar", last modified: Mon Jul 10 12:01:27 2023, max compression
+gzip compressed data, was "cru-dse-utils-0.1.4.tar", last modified: Tue Jul 11 12:36:39 2023, max compression
```

## Comparing `cru-dse-utils-0.1.3.tar` & `cru-dse-utils-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.107308 cru-dse-utils-0.1.3/
--rw-rw-rw-   0        0        0     1085 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3049 2023-07-10 12:01:27.106337 cru-dse-utils-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-07-08 19:47:45.000000 cru-dse-utils-0.1.3/README.md
--rw-rw-rw-   0        0        0     1040 2023-07-08 19:52:42.000000 cru-dse-utils-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 12:01:27.108307 cru-dse-utils-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 12:01:26.942391 cru-dse-utils-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.035192 cru-dse-utils-0.1.3/src/cru_dse_utils/
--rw-rw-rw-   0        0        0      493 2023-07-08 19:06:36.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/__init__.py
--rw-rw-rw-   0        0        0     4099 2023-07-07 14:40:08.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/auth.py
--rw-rw-rw-   0        0        0     9866 2023-07-08 20:13:30.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/bigquery.py
--rw-rw-rw-   0        0        0     5836 2023-07-07 16:33:53.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/dbt.py
--rw-rw-rw-   0        0        0     4540 2023-07-08 16:29:06.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/gcs.py
--rw-rw-rw-   0        0        0     4814 2023-07-07 14:39:34.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/general.py
-drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.057512 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/
--rw-rw-rw-   0        0        0     3049 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.099914 cru-dse-utils-0.1.3/tests/
--rw-rw-rw-   0        0        0     4026 2023-07-07 15:29:57.000000 cru-dse-utils-0.1.3/tests/test_auth.py
--rw-rw-rw-   0        0        0    11645 2023-07-08 20:14:13.000000 cru-dse-utils-0.1.3/tests/test_bigquery.py
--rw-rw-rw-   0        0        0     6164 2023-07-07 19:10:39.000000 cru-dse-utils-0.1.3/tests/test_dbt.py
--rw-rw-rw-   0        0        0    10458 2023-07-08 17:00:42.000000 cru-dse-utils-0.1.3/tests/test_gcs.py
--rw-rw-rw-   0        0        0     1718 2023-07-07 15:11:00.000000 cru-dse-utils-0.1.3/tests/test_general.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.319344 cru-dse-utils-0.1.4/
+-rw-rw-rw-   0        0        0     1085 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3049 2023-07-11 12:36:39.313334 cru-dse-utils-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2023-07-08 19:47:45.000000 cru-dse-utils-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1040 2023-07-11 12:32:54.000000 cru-dse-utils-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:36:39.322359 cru-dse-utils-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.144536 cru-dse-utils-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.227814 cru-dse-utils-0.1.4/src/cru_dse_utils/
+-rw-rw-rw-   0        0        0      493 2023-07-08 19:06:36.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/__init__.py
+-rw-rw-rw-   0        0        0     4099 2023-07-07 14:40:08.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/auth.py
+-rw-rw-rw-   0        0        0     9866 2023-07-08 20:13:30.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/bigquery.py
+-rw-rw-rw-   0        0        0     5836 2023-07-07 16:33:53.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/dbt.py
+-rw-rw-rw-   0        0        0     4540 2023-07-08 16:29:06.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/gcs.py
+-rw-rw-rw-   0        0        0     4785 2023-07-10 17:04:17.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/general.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.261856 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/
+-rw-rw-rw-   0        0        0     3049 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.302788 cru-dse-utils-0.1.4/tests/
+-rw-rw-rw-   0        0        0     4026 2023-07-07 15:29:57.000000 cru-dse-utils-0.1.4/tests/test_auth.py
+-rw-rw-rw-   0        0        0    11645 2023-07-08 20:14:13.000000 cru-dse-utils-0.1.4/tests/test_bigquery.py
+-rw-rw-rw-   0        0        0     6164 2023-07-07 19:10:39.000000 cru-dse-utils-0.1.4/tests/test_dbt.py
+-rw-rw-rw-   0        0        0    10458 2023-07-08 17:00:42.000000 cru-dse-utils-0.1.4/tests/test_gcs.py
+-rw-rw-rw-   0        0        0     1700 2023-07-10 19:05:56.000000 cru-dse-utils-0.1.4/tests/test_general.py
```

### Comparing `cru-dse-utils-0.1.3/LICENSE` & `cru-dse-utils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/PKG-INFO` & `cru-dse-utils-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cru-dse-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cru DSE Python Utils
 Author-email: Cru DSE Team <tony.guan@cru.org>
 License: MIT License
         
         Copyright (c) [2023] [Cru]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cru-dse-utils-0.1.3/README.md` & `cru-dse-utils-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/pyproject.toml` & `cru-dse-utils-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cru-dse-utils"
-version = "0.1.3"
+version = "0.1.4"
 description = "Cru DSE Python Utils"
 readme = "README.md"
 authors = [{ name = "Cru DSE Team", email = "tony.guan@cru.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `cru-dse-utils-0.1.3/src/cru_dse_utils/auth.py` & `cru-dse-utils-0.1.4/src/cru_dse_utils/auth.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/src/cru_dse_utils/bigquery.py` & `cru-dse-utils-0.1.4/src/cru_dse_utils/bigquery.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/src/cru_dse_utils/dbt.py` & `cru-dse-utils-0.1.4/src/cru_dse_utils/dbt.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/src/cru_dse_utils/gcs.py` & `cru-dse-utils-0.1.4/src/cru_dse_utils/gcs.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/src/cru_dse_utils/general.py` & `cru-dse-utils-0.1.4/src/cru_dse_utils/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import logging
 
 
 def get_request(
     url: str,
     headers: Dict[str, str],
     params: Dict[Any, Any],
-    logger: logging.Logger,
     max_retries: int = 5,
 ) -> Union[requests.Response, None]:
     """
     Sends an HTTP GET request to the specified URL with the specified headers.
 
     This function sends an HTTP GET request to the specified URL with the
     specified headers. If the response is not a valid JSON object, the
```

### Comparing `cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/PKG-INFO` & `cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cru-dse-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cru DSE Python Utils
 Author-email: Cru DSE Team <tony.guan@cru.org>
 License: MIT License
         
         Copyright (c) [2023] [Cru]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cru-dse-utils-0.1.3/tests/test_auth.py` & `cru-dse-utils-0.1.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/tests/test_bigquery.py` & `cru-dse-utils-0.1.4/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/tests/test_dbt.py` & `cru-dse-utils-0.1.4/tests/test_dbt.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/tests/test_gcs.py` & `cru-dse-utils-0.1.4/tests/test_gcs.py`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.3/tests/test_general.py` & `cru-dse-utils-0.1.4/tests/test_general.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import logging
 import requests
 from requests.models import Response
 from unittest.mock import Mock, patch
 from cru_dse_utils import get_request
 
+
 # Test get_request for a successful request where everything works as expected.
 def test_get_request():
     mock_response = Mock(spec=Response)
     mock_response.status_code = 200
     mock_response.json.return_value = {"key": "value"}
 
     logger = logging.getLogger("test")
     url = "https://test.com"
     headers = {"Header": "test"}
     params = {"Param": "test"}
 
     with patch("requests.get", return_value=mock_response) as mock_get:
-        result = get_request(url, headers, params, logger)
+        result = get_request(url, headers, params)
 
     assert result == mock_response
     mock_get.assert_called_once_with(url, headers=headers, params=params, timeout=60)
 
+
 # Test get_request for timeout error.
 def test_get_request_timeout_error():
     logger = logging.getLogger("test")
     url = "https://test.com"
     headers = {"Header": "test"}
     params = {"Param": "test"}
 
     with patch("requests.get", side_effect=requests.exceptions.Timeout()), patch(
         "time.sleep"
     ):
-        assert get_request(url, headers, params, logger) is None
+        assert get_request(url, headers, params) is None
+
 
 # Test get_request for connection error.
 def test_get_request_json_error():
     mock_response = Mock(spec=Response)
     mock_response.status_code = 200
     mock_response.json.side_effect = ValueError()
 
@@ -43,8 +46,8 @@
     url = "https://test.com"
     headers = {"Header": "test"}
     params = {"Param": "test"}
 
     with patch("requests.get", return_value=mock_response), patch(
         "time.sleep", return_value=None
     ):
-        assert get_request(url, headers, params, logger) is None
+        assert get_request(url, headers, params) is None
```

