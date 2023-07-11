# Comparing `tmp/influxdb3-python-0.1.7.tar.gz` & `tmp/influxdb3-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.7.tar", last modified: Mon Jul 10 15:29:01 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.8.tar", last modified: Tue Jul 11 13:07:29 2023, max compression
```

## Comparing `influxdb3-python-0.1.7.tar` & `influxdb3-python-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:01.121914 influxdb3-python-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 15:28:49.000000 influxdb3-python-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-10 15:29:01.121914 influxdb3-python-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-10 15:28:49.000000 influxdb3-python-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:01.121914 influxdb3-python-0.1.7/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-10 15:29:01.000000 influxdb3-python-0.1.7/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 15:29:01.000000 influxdb3-python-0.1.7/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:29:01.000000 influxdb3-python-0.1.7/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 15:29:01.000000 influxdb3-python-0.1.7/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 15:29:01.000000 influxdb3-python-0.1.7/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:01.121914 influxdb3-python-0.1.7/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-07-10 15:28:49.000000 influxdb3-python-0.1.7/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-10 15:28:49.000000 influxdb3-python-0.1.7/influxdb_client_3/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:29:01.121914 influxdb3-python-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-10 15:28:49.000000 influxdb3-python-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:01.121914 influxdb3-python-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-10 15:28:49.000000 influxdb3-python-0.1.7/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.7/LICENSE` & `influxdb3-python-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.7/PKG-INFO` & `influxdb3-python-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.7/README.md` & `influxdb3-python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.7/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.8/influxdb3_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.7/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.8/influxdb_client_3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
 from influxdb_client_3.read_file import upload_file
 
 
 def write_client_options(**kwargs):
     return kwargs
 
+def default_client_options(**kwargs):
+    return kwargs
 
 def flight_client_options(**kwargs):
     return kwargs  # You can replace this with a specific data structure if needed
 
 class InfluxDBClient3:
     def __init__(
             self,
@@ -41,15 +43,15 @@
         :type write_client_options: dict
         :param flight_client_options: Options for the FlightClient.
         :type flight_client_options: dict
         :param kwargs: Additional arguments for the InfluxDB Client.
         """
         self._org = org
         self._database = database
-        self._write_client_options = write_client_options or write_client_options(write_options=SYNCHRONOUS)
+        self._write_client_options = write_client_options if write_client_options is not None else default_client_options(write_options=SYNCHRONOUS)
 
         # Extracting the hostname from URL if provided
         parsed_url = urllib.parse.urlparse(host)
         host = parsed_url.hostname or host
 
         self._client = _InfluxDBClient(
             url=f"https://{host}",
```

### Comparing `influxdb3-python-0.1.7/influxdb_client_3/read_file.py` & `influxdb3-python-0.1.8/influxdb_client_3/read_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from pyarrow import json as pa_json
 import pyarrow.csv as csv
 import pyarrow.feather as feather
 import pyarrow.parquet as parquet
-import pyarrow.orc as orc
+import os
+
+# Check if the OS is not Windows
+if os.name != 'nt':
+    import pyarrow.orc as orc
+
 import pandas as pd
 
 class upload_file:
     def __init__(self, file, **kwargs):
         self._file = file
         self._kwargs = kwargs
 
@@ -16,27 +21,31 @@
             elif self._file.endswith(".parquet"):
                 return self.load_parquet(self._file)
             elif self._file.endswith(".csv"):
                 return self.load_csv(self._file)
             elif self._file.endswith(".json"):
                 return self.load_json(self._file)
             elif self._file.endswith(".orc"):
+
                 return self.load_orc(self._file)
             else:
                 raise ValueError("Unsupported file type")
 
     def load_feather(self, file):
         return feather.read_table(file, **self._kwargs)
         
     def load_parquet(self, file):
         return parquet.read_table(file, **self._kwargs)
         
     def load_csv(self, file):
         return csv.read_csv(file, **self._kwargs)
     
     def load_orc(self, file):
-        return orc.read_table(file, **self._kwargs)
+        if os.name == 'nt':
+            raise ValueError("Unsupported file type for this OS")
+        else:
+            return orc.read_table(file, **self._kwargs)
     
     #TODO: Use pyarrow.json.read_json() instead of pandas.read_json()
     def load_json(self, file):
         return pd.read_json(file, **self._kwargs)
```

### Comparing `influxdb3-python-0.1.7/setup.py` & `influxdb3-python-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.7/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.8/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

