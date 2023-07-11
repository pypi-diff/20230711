# Comparing `tmp/taichu-storage-0.0.1.tar.gz` & `tmp/taichu-storage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-storage-0.0.1.tar", last modified: Mon Jul 10 10:59:30 2023, max compression
+gzip compressed data, was "taichu-storage-0.0.2.tar", last modified: Tue Jul 11 02:00:49 2023, max compression
```

## Comparing `taichu-storage-0.0.1.tar` & `taichu-storage-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-10 10:59:30.154480 taichu-storage-0.0.1/
--rw-r--r--   0 wangkun    (501) staff       (20)      256 2023-07-10 10:59:30.154201 taichu-storage-0.0.1/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-10 10:59:30.154578 taichu-storage-0.0.1/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      742 2023-07-10 10:59:21.000000 taichu-storage-0.0.1/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-10 10:59:30.151793 taichu-storage-0.0.1/storage/
--rw-r--r--   0 wangkun    (501) staff       (20)     2538 2023-07-10 09:47:34.000000 taichu-storage-0.0.1/storage/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2099 2023-07-04 08:28:17.000000 taichu-storage-0.0.1/storage/b1.py
--rw-r--r--   0 wangkun    (501) staff       (20)     4703 2023-07-10 06:30:55.000000 taichu-storage-0.0.1/storage/b3.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.1/storage/env.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2633 2023-07-10 10:54:39.000000 taichu-storage-0.0.1/storage/minio_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1308 2023-07-05 03:26:07.000000 taichu-storage-0.0.1/storage/obs.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-10 10:59:30.153821 taichu-storage-0.0.1/taichu_storage.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      256 2023-07-10 10:59:30.000000 taichu-storage-0.0.1/taichu_storage.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      299 2023-07-10 10:59:30.000000 taichu-storage-0.0.1/taichu_storage.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-10 10:59:30.000000 taichu-storage-0.0.1/taichu_storage.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       37 2023-07-10 10:59:30.000000 taichu-storage-0.0.1/taichu_storage.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        8 2023-07-10 10:59:30.000000 taichu-storage-0.0.1/taichu_storage.egg-info/top_level.txt
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:00:49.770481 taichu-storage-0.0.2/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:00:49.770224 taichu-storage-0.0.2/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 02:00:49.770574 taichu-storage-0.0.2/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      730 2023-07-10 11:04:28.000000 taichu-storage-0.0.2/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:00:49.768615 taichu-storage-0.0.2/taichu_storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)     2559 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2171 2023-07-11 02:00:34.000000 taichu-storage-0.0.2/taichu_storage/b1.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     4717 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/b3.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.2/taichu_storage/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/minio_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1322 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/obs.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:00:49.769914 taichu-storage-0.0.2/taichu_storage.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      341 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       37 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/top_level.txt
```

### Comparing `taichu-storage-0.0.1/setup.py` & `taichu-storage-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
     long_description = 'storage sdks aggregation'
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='0.0.1',
-        description='taichu storage is a tool for storage',
+        version='0.0.2',
+        description='storage sdks aggregation',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
         install_requires=requirements,
```

### Comparing `taichu-storage-0.0.1/storage/__init__.py` & `taichu-storage-0.0.2/taichu_storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     #     raise Exception("Not Implemented: list")
 
 
 def create_storage(protocol: Protocol, cfgs=None):
     if cfgs is None:
         cfgs = {}
     if protocol == Protocol.OBS:
-        from storage.obs import StorageObs
+        from taichu_storage.obs import StorageObs
         return StorageObs(cfgs)
     if protocol == Protocol.BOTO3:
-        from storage.b3 import StorageBoto3
+        from taichu_storage.b3 import StorageBoto3
         return StorageBoto3(cfgs)
     else:
-        from storage.b1 import StorageAlluxio
+        from taichu_storage.b1 import StorageAlluxio
         return StorageAlluxio()
```

### Comparing `taichu-storage-0.0.1/storage/b1.py` & `taichu-storage-0.0.2/taichu_storage/b1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 
-from storage import StorageInterface
+from taichu_storage import StorageInterface
 import boto.s3.connection
-from storage.env import *
+from taichu_storage.env import *
 import boto.exception
 
 
 class StorageAlluxio(StorageInterface):
-    def __init__(self):
+    def __init__(self, cfgs=None):
+        if cfgs is None:
+            cfgs = {}
         self._client = boto.connect_s3(
             aws_access_key_id=S3_ACCESS_KEY_ID,
             aws_secret_access_key=S3_SECRET_ACCESS_KEY,
             host=ALLUXIO_HOST,
             port=ALLUXIO_PORT,
             path=ALLUXIO_PATH,
             is_secure=False,
```

### Comparing `taichu-storage-0.0.1/storage/b3.py` & `taichu-storage-0.0.2/taichu_storage/b3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 import boto3
 import botocore.exceptions
 from botocore.config import Config
 
-from storage import StorageInterface
-from storage.env import *
+from taichu_storage import StorageInterface
+from taichu_storage.env import *
 
 
 class StorageBoto3(StorageInterface):
     def __init__(self, cfgs=None):
         if cfgs is None:
             cfgs = {}
```

### Comparing `taichu-storage-0.0.1/storage/env.py` & `taichu-storage-0.0.2/taichu_storage/env.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.1/storage/minio_client.py` & `taichu-storage-0.0.2/taichu_storage/minio_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import logging
 
-from storage import StorageInterface
+from taichu_storage import StorageInterface
 from minio import Minio
 from io import BytesIO
 
 
 class StorageMinio(StorageInterface):
     _use_alluxio_path = True
```

### Comparing `taichu-storage-0.0.1/storage/obs.py` & `taichu-storage-0.0.2/taichu_storage/obs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
-from storage import StorageInterface
-from storage.env import *
+from taichu_storage import StorageInterface
+from taichu_storage.env import *
 from obs import ObsClient, PutObjectHeader
 
 
 class StorageObs(StorageInterface):
 
     def download_file(self, file_path, key):
         pass
```

