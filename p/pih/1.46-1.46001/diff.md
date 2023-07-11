# Comparing `tmp/pih-1.46.tar.gz` & `tmp/pih-1.46001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.46.tar", last modified: Tue Jul 11 06:54:38 2023, max compression
+gzip compressed data, was "pih-1.46001.tar", last modified: Tue Jul 11 06:56:24 2023, max compression
```

## Comparing `pih-1.46.tar` & `pih-1.46001.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 06:54:36.599122 pih-1.46/
--rw-rw-rw-   0        0        0      258 2023-07-11 06:54:38.192847 pih-1.46/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 06:54:37.849102 pih-1.46/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.46/pih/__init__.py
--rw-rw-rw-   0        0        0    19633 2023-07-11 03:15:46.000000 pih-1.46/pih/collection.py
--rw-rw-rw-   0        0        0    55119 2023-07-11 04:21:24.000000 pih-1.46/pih/console_api.py
--rw-rw-rw-   0        0        0   106061 2023-07-11 03:57:38.000000 pih-1.46/pih/const.py
--rw-rw-rw-   0        0        0   299532 2023-07-11 06:54:01.000000 pih-1.46/pih/pih.py
--rw-rw-rw-   0        0        0    24689 2023-07-09 01:49:27.000000 pih-1.46/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.46/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.46/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.46/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6368 2023-07-11 03:24:37.000000 pih-1.46/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.46/pih/service_example.py
--rw-rw-rw-   0        0        0    37450 2023-07-11 02:24:33.000000 pih-1.46/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.46/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-11 06:54:38.130358 pih-1.46/pih.egg-info/
--rw-rw-rw-   0        0        0      258 2023-07-11 06:54:35.000000 pih-1.46/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-11 06:54:36.000000 pih-1.46/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 06:54:35.000000 pih-1.46/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-11 06:54:35.000000 pih-1.46/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 06:54:35.000000 pih-1.46/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2014 2023-06-27 04:00:23.000000 pih-1.46/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-11 06:54:38.224097 pih-1.46/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 06:56:23.072092 pih-1.46001/
+-rw-rw-rw-   0        0        0      261 2023-07-11 06:56:24.712780 pih-1.46001/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 06:56:24.275210 pih-1.46001/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.46001/pih/__init__.py
+-rw-rw-rw-   0        0        0    19633 2023-07-11 03:15:46.000000 pih-1.46001/pih/collection.py
+-rw-rw-rw-   0        0        0    55119 2023-07-11 04:21:24.000000 pih-1.46001/pih/console_api.py
+-rw-rw-rw-   0        0        0   106061 2023-07-11 03:57:38.000000 pih-1.46001/pih/const.py
+-rw-rw-rw-   0        0        0   299535 2023-07-11 06:56:13.000000 pih-1.46001/pih/pih.py
+-rw-rw-rw-   0        0        0    24689 2023-07-09 01:49:27.000000 pih-1.46001/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.46001/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.46001/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.46001/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6368 2023-07-11 03:24:37.000000 pih-1.46001/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.46001/pih/service_example.py
+-rw-rw-rw-   0        0        0    37450 2023-07-11 02:24:33.000000 pih-1.46001/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.46001/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:56:24.634563 pih-1.46001/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-11 06:56:21.000000 pih-1.46001/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2014 2023-06-27 04:00:23.000000 pih-1.46001/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 06:56:24.744140 pih-1.46001/setup.cfg
```

### Comparing `pih-1.46/pih/collection.py` & `pih-1.46001/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/console_api.py` & `pih-1.46001/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/const.py` & `pih-1.46001/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/pih.py` & `pih-1.46001/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1625,15 +1625,15 @@
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.46"
+            return "1.46001"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.46/pih/rpc.py` & `pih-1.46001/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/rpcCommandCall_pb2.py` & `pih-1.46001/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.46001/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/rpc_collection.py` & `pih-1.46001/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/rpc_const.py` & `pih-1.46001/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/service_example.py` & `pih-1.46001/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/tools.py` & `pih-1.46001/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih/widgets.py` & `pih-1.46001/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.46/pih_setup.py` & `pih-1.46001/pih_setup.py`

 * *Files identical despite different names*

