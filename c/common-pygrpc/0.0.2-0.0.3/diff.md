# Comparing `tmp/common_pygrpc-0.0.2-py3-none-any.whl.zip` & `tmp/common_pygrpc-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 18028 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     5476 b- defN 23-Jun-25 02:14 common_pb2.py
--rw-rw-rw-  2.0 fat     2360 b- defN 23-Jun-25 02:14 common_pb2_grpc.py
--rw-rw-rw-  2.0 fat     7981 b- defN 23-Mar-08 05:43 grpclib.py
--rw-rw-rw-  2.0 fat    34507 b- defN 23-Jun-25 02:14 common_pygrpc-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      771 b- defN 23-Jun-25 02:14 common_pygrpc-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 02:14 common_pygrpc-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       35 b- defN 23-Jun-25 02:14 common_pygrpc-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      628 b- defN 23-Jun-25 02:14 common_pygrpc-0.0.2.dist-info/RECORD
-8 files, 51850 bytes uncompressed, 16938 bytes compressed:  67.3%
+Zip file size: 18033 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     5476 b- defN 23-Jul-11 01:41 common_pb2.py
+-rw-rw-rw-  2.0 fat     2360 b- defN 23-Jul-11 01:41 common_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     8014 b- defN 23-Jul-11 01:38 grpclib.py
+-rw-rw-rw-  2.0 fat    34507 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      771 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      628 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/RECORD
+8 files, 51883 bytes uncompressed, 16943 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: common_pb2_grpc.py
 Comment: 
 
 Filename: grpclib.py
 Comment: 
 
-Filename: common_pygrpc-0.0.2.dist-info/LICENSE
+Filename: common_pygrpc-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: common_pygrpc-0.0.2.dist-info/METADATA
+Filename: common_pygrpc-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: common_pygrpc-0.0.2.dist-info/WHEEL
+Filename: common_pygrpc-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: common_pygrpc-0.0.2.dist-info/top_level.txt
+Filename: common_pygrpc-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: common_pygrpc-0.0.2.dist-info/RECORD
+Filename: common_pygrpc-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grpclib.py

```diff
@@ -121,17 +121,15 @@
     def load(self, servers):
         """
         load grpc server list
         :param servers: Server
         :return:
         """
         for server in servers:
-            channel = grpc.insecure_channel(server.addr)
-            stub = common_pb2_grpc.CommonServiceStub(channel)
-            self.stubs[server.server] = stub
+            self.stubs[server.server] = server.addr
 
     def __init__(self):
         self.stubs = {}
 
 
 class GrpcServer:
     def __init__(self, host='0.0.0.0', port=6565, max_workers=10):
@@ -182,24 +180,24 @@
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             sig = inspect.signature(func)
             bind = sig.bind(*args, **kwargs).arguments
             if sig.parameters.get("cls"):
                 cls = bind.get("cls")
                 bind.pop("cls")
-            rpc_client = grpc_client.connect(server)
-            response_json = GrpcHelper.call_rpc_result(
-                rpc_client,
-                clazz=func.__module__,
-                method=func.__qualname__,
-                args=(),
-                kwargs={k: v for k, v in bind.items()},
-            )
-
-            return response_json
+            rpc_client_addr = grpc_client.connect(server)
+            with grpc.insecure_channel(rpc_client_addr) as channel:
+                response_json = GrpcHelper.call_rpc_result(
+                    rpc_client=common_pb2_grpc.CommonServiceStub(channel),
+                    clazz=func.__module__,
+                    method=func.__qualname__,
+                    args=(),
+                    kwargs={k: v for k, v in bind.items()},
+                )
+                return response_json
 
         return wrapper
 
     return decorator
 
 
 class GrpcHelper:
```

## Comparing `common_pygrpc-0.0.2.dist-info/LICENSE` & `common_pygrpc-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `common_pygrpc-0.0.2.dist-info/METADATA` & `common_pygrpc-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-pygrpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: common python grpc service
 Home-page: https://github.com/reggiepy/common_pygrpc
 Author: reggiepy
 Author-email: reggiepy@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `common_pygrpc-0.0.2.dist-info/RECORD` & `common_pygrpc-0.0.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 common_pb2.py,sha256=mLfibqIqoX1sCFx9qZ3Bdhhw6EZzX3UKTUvj44Jnhug,5476
 common_pb2_grpc.py,sha256=AfjdBnKtDdEB69MJNNwx85HsliQ6C1mtE8874IJQi7M,2360
-grpclib.py,sha256=Hveo7dTtAgjn7mkxmv73w6uPAcjQowRZg4uIk0UeH9c,7981
-common_pygrpc-0.0.2.dist-info/LICENSE,sha256=tFOSjGfy514BlNS7Y7olIRUtzFj0jweWohgjuwlmfkQ,34507
-common_pygrpc-0.0.2.dist-info/METADATA,sha256=E8p5hKw6rNIy64Zd-sCeEg0II4N5KRlq63ajeap3QII,771
-common_pygrpc-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-common_pygrpc-0.0.2.dist-info/top_level.txt,sha256=xfw2Lc6jQADxWVtkofKQ507frTm0AHt-pK3HWu4Qj_Q,35
-common_pygrpc-0.0.2.dist-info/RECORD,,
+grpclib.py,sha256=rh56e5ekTIqAsN9irzJ645tXOuSAiZtWz25aO5nHlfw,8014
+common_pygrpc-0.0.3.dist-info/LICENSE,sha256=tFOSjGfy514BlNS7Y7olIRUtzFj0jweWohgjuwlmfkQ,34507
+common_pygrpc-0.0.3.dist-info/METADATA,sha256=fpihLQ982yj55QFy0b5dQdjz6l__ND_juNUoE_MsFZo,771
+common_pygrpc-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+common_pygrpc-0.0.3.dist-info/top_level.txt,sha256=xfw2Lc6jQADxWVtkofKQ507frTm0AHt-pK3HWu4Qj_Q,35
+common_pygrpc-0.0.3.dist-info/RECORD,,
```

