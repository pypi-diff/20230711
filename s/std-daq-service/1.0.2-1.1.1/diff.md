# Comparing `tmp/std_daq_service-1.0.2.tar.gz` & `tmp/std_daq_service-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_service-1.0.2.tar", last modified: Tue Jun 27 09:46:19 2023, max compression
+gzip compressed data, was "std_daq_service-1.1.1.tar", last modified: Tue Jul 11 12:18:39 2023, max compression
```

## Comparing `std_daq_service-1.0.2.tar` & `std_daq_service-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:46:19.574886 std_daq_service-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-06-27 09:46:19.574886 std_daq_service-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:46:19.574886 std_daq_service-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:46:19.570886 std_daq_service-1.0.2/std_daq_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/std_daq_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/std_daq_service/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/std_daq_service/start_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:46:19.570886 std_daq_service-1.0.2/std_daq_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-06-27 09:46:19.000000 std_daq_service-1.0.2/std_daq_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 09:46:19.000000 std_daq_service-1.0.2/std_daq_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:46:19.000000 std_daq_service-1.0.2/std_daq_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-27 09:46:19.000000 std_daq_service-1.0.2/std_daq_service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 09:46:19.000000 std_daq_service-1.0.2/std_daq_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:46:19.000000 std_daq_service-1.0.2/std_daq_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:46:19.570886 std_daq_service-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/tests/test_broker_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/tests/test_broker_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/tests/test_epics_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/tests/test_epics_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/tests/test_request_write_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-27 09:46:09.000000 std_daq_service-1.0.2/tests/test_status_aggregator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.992388 std_daq_service-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-11 12:18:39.992388 std_daq_service-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:18:39.992388 std_daq_service-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.988388 std_daq_service-1.1.1/std_daq_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/std_daq_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/std_daq_service/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.984388 std_daq_service-1.1.1/std_daq_service/rest_v2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.988388 std_daq_service-1.1.1/std_daq_service/rest_v2/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.988388 std_daq_service-1.1.1/std_daq_service/rest_v2/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/js/787.6a20824f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/js/787.6a20824f.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   583555 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/js/main.9c6e0ea6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/js/main.9c6e0ea6.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2414085 2023-07-11 12:18:30.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/js/main.9c6e0ea6.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 12:18:04.000000 std_daq_service-1.1.1/std_daq_service/rest_v2/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/std_daq_service/start_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.988388 std_daq_service-1.1.1/std_daq_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-11 12:18:39.000000 std_daq_service-1.1.1/std_daq_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 12:18:39.000000 std_daq_service-1.1.1/std_daq_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:18:39.000000 std_daq_service-1.1.1/std_daq_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-11 12:18:39.000000 std_daq_service-1.1.1/std_daq_service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 12:18:39.000000 std_daq_service-1.1.1/std_daq_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 12:18:39.000000 std_daq_service-1.1.1/std_daq_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:18:39.992388 std_daq_service-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/tests/test_broker_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/tests/test_broker_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/tests/test_epics_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/tests/test_epics_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/tests/test_request_write_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-11 12:17:00.000000 std_daq_service-1.1.1/tests/test_status_aggregator.py
```

### Comparing `std_daq_service-1.0.2/PKG-INFO` & `std_daq_service-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std_daq_service
-Version: 1.0.2
+Version: 1.1.1
 Description-Content-Type: text/markdown
 
 # std_daq_service
 
 This is a monorepo for standard daq services.
 
 Documentation of interfaces:
```

### Comparing `std_daq_service-1.0.2/README.md` & `std_daq_service-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/setup.py` & `std_daq_service-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 
 version = os.getenv('GITHUB_REF_NAME', '0.0.0')
 
 setup(
     name='std_daq_service',
     packages=['std_daq_service'],
     version=version,
+    include_package_data=True,
     install_requires=[
         'std-buffer',
         'pyzmq',
         'pcaspy',
         'opencv-python',
         'tifffile',
         'protobuf',
         'flask',
         'flask-cors',
         'numpy',
-        'redis'
+        'redis',
+        'fastapi',
+        'uvicorn'
     ],
     entry_points='''
         [console_scripts]
         buffer=std_daq_service.buffer.start:main
         writer=std_daq_service.writer.start:main
         validator=std_daq_service.validator.start:main
         std_daq_request=std_daq_service.tools.request:main
```

### Comparing `std_daq_service-1.0.2/std_daq_service/protocol.py` & `std_daq_service-1.1.1/std_daq_service/protocol.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/std_daq_service/start_utils.py` & `std_daq_service-1.1.1/std_daq_service/start_utils.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/std_daq_service.egg-info/PKG-INFO` & `std_daq_service-1.1.1/std_daq_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std-daq-service
-Version: 1.0.2
+Version: 1.1.1
 Description-Content-Type: text/markdown
 
 # std_daq_service
 
 This is a monorepo for standard daq services.
 
 Documentation of interfaces:
```

### Comparing `std_daq_service-1.0.2/std_daq_service.egg-info/entry_points.txt` & `std_daq_service-1.1.1/std_daq_service.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/tests/test_broker_client.py` & `std_daq_service-1.1.1/tests/test_broker_client.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/tests/test_broker_worker.py` & `std_daq_service-1.1.1/tests/test_broker_worker.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/tests/test_epics_buffer.py` & `std_daq_service-1.1.1/tests/test_epics_buffer.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/tests/test_epics_writer.py` & `std_daq_service-1.1.1/tests/test_epics_writer.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/tests/test_request_write_service.py` & `std_daq_service-1.1.1/tests/test_request_write_service.py`

 * *Files identical despite different names*

### Comparing `std_daq_service-1.0.2/tests/test_status_aggregator.py` & `std_daq_service-1.1.1/tests/test_status_aggregator.py`

 * *Files identical despite different names*

