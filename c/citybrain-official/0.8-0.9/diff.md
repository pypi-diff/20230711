# Comparing `tmp/citybrain-official-0.8.tar.gz` & `tmp/citybrain-official-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citybrain-official-0.8.tar", last modified: Wed Jul  5 02:59:46 2023, max compression
+gzip compressed data, was "citybrain-official-0.9.tar", last modified: Mon Jul 10 08:33:27 2023, max compression
```

## Comparing `citybrain-official-0.8.tar` & `citybrain-official-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-05 02:59:46.378987 citybrain-official-0.8/
--rw-r--r--   0 mabingtao   (501) staff       (20)     1060 2023-07-02 14:17:08.000000 citybrain-official-0.8/LICENSE
--rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-05 02:59:46.378797 citybrain-official-0.8/PKG-INFO
--rw-r--r--   0 mabingtao   (501) staff       (20)      802 2023-07-03 07:35:48.000000 citybrain-official-0.8/README.md
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-05 02:59:46.377430 citybrain-official-0.8/citybrain_official/
--rw-r--r--   0 mabingtao   (501) staff       (20)       88 2023-07-03 07:13:50.000000 citybrain-official-0.8/citybrain_official/__init__.py
--rw-r--r--   0 mabingtao   (501) staff       (20)     5505 2023-07-05 02:58:47.000000 citybrain-official-0.8/citybrain_official/client.py
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-05 02:59:46.378522 citybrain-official-0.8/citybrain_official.egg-info/
--rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/PKG-INFO
--rw-r--r--   0 mabingtao   (501) staff       (20)      295 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/SOURCES.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)        1 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/dependency_links.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       16 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/requires.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       19 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/top_level.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       38 2023-07-05 02:59:46.379060 citybrain-official-0.8/setup.cfg
--rw-r--r--   0 mabingtao   (501) staff       (20)      673 2023-07-05 02:59:11.000000 citybrain-official-0.8/setup.py
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-10 08:33:27.811063 citybrain-official-0.9/
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1060 2023-07-02 14:17:08.000000 citybrain-official-0.9/LICENSE
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-10 08:33:27.810212 citybrain-official-0.9/PKG-INFO
+-rw-r--r--   0 mabingtao   (501) staff       (20)      802 2023-07-03 07:35:48.000000 citybrain-official-0.9/README.md
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-10 08:33:27.808001 citybrain-official-0.9/citybrain_official/
+-rw-r--r--   0 mabingtao   (501) staff       (20)       88 2023-07-03 07:13:50.000000 citybrain-official-0.9/citybrain_official/__init__.py
+-rw-r--r--   0 mabingtao   (501) staff       (20)     6116 2023-07-10 08:32:40.000000 citybrain-official-0.9/citybrain_official/client.py
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-10 08:33:27.809183 citybrain-official-0.9/citybrain_official.egg-info/
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-10 08:33:27.000000 citybrain-official-0.9/citybrain_official.egg-info/PKG-INFO
+-rw-r--r--   0 mabingtao   (501) staff       (20)      295 2023-07-10 08:33:27.000000 citybrain-official-0.9/citybrain_official.egg-info/SOURCES.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)        1 2023-07-10 08:33:27.000000 citybrain-official-0.9/citybrain_official.egg-info/dependency_links.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       16 2023-07-10 08:33:27.000000 citybrain-official-0.9/citybrain_official.egg-info/requires.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       19 2023-07-10 08:33:27.000000 citybrain-official-0.9/citybrain_official.egg-info/top_level.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       38 2023-07-10 08:33:27.811244 citybrain-official-0.9/setup.cfg
+-rw-r--r--   0 mabingtao   (501) staff       (20)      673 2023-07-10 08:33:16.000000 citybrain-official-0.9/setup.py
```

### Comparing `citybrain-official-0.8/LICENSE` & `citybrain-official-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `citybrain-official-0.8/PKG-INFO` & `citybrain-official-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citybrain-official
-Version: 0.8
+Version: 0.9
 Summary: retrieve data from citybrain.org
 Home-page: UNKNOWN
 Author: citybrain.org
 Author-email: opensource@citybrain.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citybrain-official-0.8/README.md` & `citybrain-official-0.9/README.md`

 * *Files identical despite different names*

### Comparing `citybrain-official-0.8/citybrain_official/client.py` & `citybrain-official-0.9/citybrain_official/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import requests
 import json
 import os
 import csv
 import time
+import tempfile
 from io import StringIO
 import pandas
 
 __DEFAULT_ENDPOINT = "https://dev.citybrain.org/api/getData"
 __DEFAULT_ODPS_DATA_ADDRESS = "170DD61338021000"
 
 endpoint: str = ""
 
+def __get_download_endpoint() -> str:
+    return __get_endpoint().replace("getData", "download")
+
 def __get_endpoint() -> str:
     if endpoint != '':
         return endpoint
     envEndpoint = os.getenv('CITYBRAIN_DATA_ENDPOINT')
     if envEndpoint is not None and envEndpoint != '':
         return envEndpoint
     return __DEFAULT_ENDPOINT
@@ -24,19 +28,23 @@
     if dataAddress != '':
         return dataAddress
     envODPSDataAddress = os.getenv('CITYBRAIN_ODPS_DATA_ADDRESS')
     if envODPSDataAddress is not None and envODPSDataAddress != '':
         return envODPSDataAddress
     return __DEFAULT_ODPS_DATA_ADDRESS
 
+def retrieve_file(dataAddress: str) -> str:
+    return __download_file(dataAddress=dataAddress)
+
+
 def retrieve_raw(dataAddress: str = '', sql: str = '') -> any:
     if sql == '':
         if dataAddress == '':
             raise Exception('must specify data address')
-        content = __download_file(dataAddress=dataAddress)
+        content = __get_content(dataAddress=dataAddress)
         return content.replace('\ufeff', '', 1)
     else:
         # create odps sql task
         taskID = __create_sql_task(dataAddress=dataAddress, sql=sql)
 
         # query task status until terminated
         status = __query_task_status(dataAddress=dataAddress, taskID=taskID)
@@ -48,15 +56,15 @@
         return __download_task_result(dataAddress=dataAddress, taskID=taskID)
 
 def retrieve_df(dataAddress: str = '', sql: str = '') -> pandas.DataFrame:
     if sql == '': # file data
         if dataAddress == '':
             raise Exception('must specify data address')
         # download file content
-        content = __download_file(dataAddress=dataAddress)
+        content = __get_content(dataAddress=dataAddress)
         content = content.replace('\ufeff', '', 1)
 
         # convert to dataframe
         src = []
         tmp = StringIO(content)
         csvReader = csv.reader(tmp, delimiter=',')
         for row in csvReader:
@@ -81,14 +89,27 @@
             return pandas.DataFrame([])
         src = []
         for row in result[1:]:
             src.append(row.split(';'))
         return pandas.DataFrame(src, columns=result[0].split(';'))
     
 def __download_file(dataAddress: str) -> str:
+    endpoint = __get_download_endpoint()
+    with requests.get(endpoint+'?dpaddress='+dataAddress, stream=True) as r:
+        r.raise_for_status()
+        
+        fd, filename = tempfile.mkstemp()
+        with open(filename, 'wb') as tmp:
+            for chunk in r.iter_content(chunk_size=4096): 
+                tmp.write(chunk)
+
+    return filename
+
+    
+def __get_content(dataAddress: str) -> str:
     endpoint = __get_endpoint()
     reqBody = {'dpAddress': dataAddress, 'payload': ''}
     resp = requests.post(url=endpoint, headers={'content-type': 'application/json'}, json=reqBody, timeout=None)
     if resp.status_code != 200:
         raise Exception('request failed, status code is: ' + str(resp.status_code))
     result = resp.json()
     if result['code'] != 200:
```

### Comparing `citybrain-official-0.8/citybrain_official.egg-info/PKG-INFO` & `citybrain-official-0.9/citybrain_official.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citybrain-official
-Version: 0.8
+Version: 0.9
 Summary: retrieve data from citybrain.org
 Home-page: UNKNOWN
 Author: citybrain.org
 Author-email: opensource@citybrain.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

