# Comparing `tmp/akari-proto-0.3.2.tar.gz` & `tmp/akari-proto-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-proto-0.3.2.tar", last modified: Mon May 22 00:35:59 2023, max compression
+gzip compressed data, was "akari-proto-0.3.3.tar", last modified: Tue Jul 11 07:57:10 2023, max compression
```

## Comparing `akari-proto-0.3.2.tar` & `akari-proto-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 00:35:59.392185 akari-proto-0.3.2/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1021 2023-05-22 00:35:59.392185 akari-proto-0.3.2/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      285 2023-05-22 00:31:41.000000 akari-proto-0.3.2/README.md
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 00:35:59.392185 akari-proto-0.3.2/akari_proto/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-proto-0.3.2/akari_proto/__init__.py
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 00:35:59.392185 akari-proto-0.3.2/akari_proto/grpc/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-proto-0.3.2/akari_proto/grpc/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3936 2023-01-29 18:11:01.000000 akari-proto-0.3.2/akari_proto/grpc/error.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    10094 2023-01-29 18:11:01.000000 akari-proto-0.3.2/akari_proto/joints_controller_pb2.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    20455 2023-01-29 18:11:01.000000 akari-proto-0.3.2/akari_proto/joints_controller_pb2_grpc.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     8086 2023-05-22 00:31:41.000000 akari-proto-0.3.2/akari_proto/m5stack_pb2.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    13951 2023-05-22 00:31:41.000000 akari-proto-0.3.2/akari_proto/m5stack_pb2_grpc.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-proto-0.3.2/akari_proto/py.typed
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 00:35:59.392185 akari-proto-0.3.2/akari_proto.egg-info/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1021 2023-05-22 00:35:59.000000 akari-proto-0.3.2/akari_proto.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      430 2023-05-22 00:35:59.000000 akari-proto-0.3.2/akari_proto.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        1 2023-05-22 00:35:59.000000 akari-proto-0.3.2/akari_proto.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       32 2023-05-22 00:35:59.000000 akari-proto-0.3.2/akari_proto.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       12 2023-05-22 00:35:59.000000 akari-proto-0.3.2/akari_proto.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       38 2023-05-22 00:35:59.392185 akari-proto-0.3.2/setup.cfg
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1060 2023-05-22 00:31:41.000000 akari-proto-0.3.2/setup.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:57:10.041796 akari-proto-0.3.3/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1092 2023-07-11 07:57:10.041796 akari-proto-0.3.3/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      285 2023-07-11 07:38:40.000000 akari-proto-0.3.3/README.md
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:57:10.041796 akari-proto-0.3.3/akari_proto/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-01-09 03:09:57.000000 akari-proto-0.3.3/akari_proto/__init__.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:57:10.041796 akari-proto-0.3.3/akari_proto/grpc/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-01-09 03:09:57.000000 akari-proto-0.3.3/akari_proto/grpc/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3936 2022-08-13 07:11:41.000000 akari-proto-0.3.3/akari_proto/grpc/error.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10094 2022-11-07 07:21:30.000000 akari-proto-0.3.3/akari_proto/joints_controller_pb2.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    20455 2022-11-07 07:21:30.000000 akari-proto-0.3.3/akari_proto/joints_controller_pb2_grpc.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8086 2023-02-08 15:51:00.000000 akari-proto-0.3.3/akari_proto/m5stack_pb2.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    13951 2023-02-08 15:51:00.000000 akari-proto-0.3.3/akari_proto/m5stack_pb2_grpc.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-01-09 03:09:57.000000 akari-proto-0.3.3/akari_proto/py.typed
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:57:10.041796 akari-proto-0.3.3/akari_proto.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1092 2023-07-11 07:57:09.000000 akari-proto-0.3.3/akari_proto.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      430 2023-07-11 07:57:10.000000 akari-proto-0.3.3/akari_proto.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-07-11 07:57:09.000000 akari-proto-0.3.3/akari_proto.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       32 2023-07-11 07:57:09.000000 akari-proto-0.3.3/akari_proto.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       12 2023-07-11 07:57:09.000000 akari-proto-0.3.3/akari_proto.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-07-11 07:57:10.041796 akari-proto-0.3.3/setup.cfg
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1060 2023-07-11 07:38:40.000000 akari-proto-0.3.3/setup.py
```

### Comparing `akari-proto-0.3.2/PKG-INFO` & `akari-proto-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: akari-proto
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package of akari protobuf definitions and utility functions
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
+Description: # akari\_proto
+        
+        [AKARI](https://github.com/AkariGroup/) を gRPC 経由で使うための protobuf 定義
+        
+        詳細は[オンラインドキュメント](https://AkariGroup.github.io/docs)、および [akari_client](https://pypi.org/project/akari-client/) を参照してください。
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
-
-# akari\_proto
-
-[AKARI](https://github.com/AkariGroup/) を gRPC 経由で使うための protobuf 定義
-
-詳細は[オンラインドキュメント](https://AkariGroup.github.io/docs)、および [akari_client](https://pypi.org/project/akari-client/) を参照してください。
```

### Comparing `akari-proto-0.3.2/akari_proto/grpc/error.py` & `akari-proto-0.3.3/akari_proto/grpc/error.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.2/akari_proto/joints_controller_pb2.py` & `akari-proto-0.3.3/akari_proto/joints_controller_pb2.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.2/akari_proto/joints_controller_pb2_grpc.py` & `akari-proto-0.3.3/akari_proto/joints_controller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.2/akari_proto/m5stack_pb2.py` & `akari-proto-0.3.3/akari_proto/m5stack_pb2.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.2/akari_proto/m5stack_pb2_grpc.py` & `akari-proto-0.3.3/akari_proto/m5stack_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.2/akari_proto.egg-info/PKG-INFO` & `akari-proto-0.3.3/akari_proto.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: akari-proto
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package of akari protobuf definitions and utility functions
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
+Description: # akari\_proto
+        
+        [AKARI](https://github.com/AkariGroup/) を gRPC 経由で使うための protobuf 定義
+        
+        詳細は[オンラインドキュメント](https://AkariGroup.github.io/docs)、および [akari_client](https://pypi.org/project/akari-client/) を参照してください。
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
-
-# akari\_proto
-
-[AKARI](https://github.com/AkariGroup/) を gRPC 経由で使うための protobuf 定義
-
-詳細は[オンラインドキュメント](https://AkariGroup.github.io/docs)、および [akari_client](https://pypi.org/project/akari-client/) を参照してください。
```

### Comparing `akari-proto-0.3.2/setup.py` & `akari-proto-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="akari-proto",
-    version="0.3.2",
+    version="0.3.3",
     description="Python package of akari protobuf definitions and utility functions",
     packages=find_packages(exclude=["tests"]),
     author="akari",
     author_email="akari.tmc@gmail.com",
     package_data={"akari_proto": ["py.typed"]},
     license="Apache License 2.0",
     long_description=open("README.md").read(),
```

