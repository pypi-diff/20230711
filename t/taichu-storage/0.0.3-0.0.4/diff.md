# Comparing `tmp/taichu-storage-0.0.3.tar.gz` & `tmp/taichu-storage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-storage-0.0.3.tar", last modified: Tue Jul 11 02:44:38 2023, max compression
+gzip compressed data, was "taichu-storage-0.0.4.tar", last modified: Tue Jul 11 09:19:04 2023, max compression
```

## Comparing `taichu-storage-0.0.3.tar` & `taichu-storage-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:44:38.655778 taichu-storage-0.0.3/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:44:38.655528 taichu-storage-0.0.3/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 02:44:38.655872 taichu-storage-0.0.3/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-11 02:43:30.000000 taichu-storage-0.0.3/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:44:38.653362 taichu-storage-0.0.3/taichu_storage/
--rw-r--r--   0 wangkun    (501) staff       (20)     2559 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2171 2023-07-11 02:00:34.000000 taichu-storage-0.0.3/taichu_storage/b1.py
--rw-r--r--   0 wangkun    (501) staff       (20)     4717 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/b3.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.3/taichu_storage/env.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/minio_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1322 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/obs.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:44:38.655178 taichu-storage-0.0.3/taichu_storage.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      341 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)      104 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/top_level.txt
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 09:19:04.893113 taichu-storage-0.0.4/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 09:19:04.892744 taichu-storage-0.0.4/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 09:19:04.893369 taichu-storage-0.0.4/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 09:19:04.890443 taichu-storage-0.0.4/taichu_storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)     2597 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     4717 2023-07-11 01:58:58.000000 taichu-storage-0.0.4/taichu_storage/b3.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     3167 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage/boto_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.4/taichu_storage/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.4/taichu_storage/minio_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1643 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage/obs.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 09:19:04.892100 taichu-storage-0.0.4/taichu_storage.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      350 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)      104 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 09:19:04.000000 taichu-storage-0.0.4/taichu_storage.egg-info/top_level.txt
```

### Comparing `taichu-storage-0.0.3/setup.py` & `taichu-storage-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     long_description = 'storage sdks aggregation'
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='0.0.3',
+        version='0.0.4',
         description='storage sdks aggregation',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-storage-0.0.3/taichu_storage/__init__.py` & `taichu-storage-0.0.4/taichu_storage/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from enum import Enum
 
 
 class Protocol(Enum):
     BOTO = 1
     OBS = 2
     BOTO3 = 3
+    MINIO = 4
 
 
 class StorageInterface:
     _client = None
     _bucket = None
 
     def client(self):
@@ -51,15 +52,15 @@
         raise Exception("Not Implemented: download_file")
 
     @abstractmethod
     def download_directory(self, key, local_target_directory):
         raise Exception("Not Implemented: download_directory")
 
     @abstractmethod
-    def generate_signed_url(self, key, expiration=600):
+    def generate_signed_url(self, key, expiration=600, host_url=None):
         raise Exception("Not Implemented: generate_signed_url")
 
     @abstractmethod
     def generate_upload_credentials(self, key, expiration=3600):
         raise Exception("Not Implemented: generate_upload_credentials")
 
     # @abstractmethod
@@ -81,9 +82,9 @@
     if protocol == Protocol.OBS:
         from taichu_storage.obs import StorageObs
         return StorageObs(cfgs)
     if protocol == Protocol.BOTO3:
         from taichu_storage.b3 import StorageBoto3
         return StorageBoto3(cfgs)
     else:
-        from taichu_storage.b1 import StorageAlluxio
+        from taichu_storage.boto_client import StorageAlluxio
         return StorageAlluxio()
```

### Comparing `taichu-storage-0.0.3/taichu_storage/b1.py` & `taichu-storage-0.0.4/taichu_storage/obs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,55 @@
 import logging
 
 from taichu_storage import StorageInterface
-import boto.s3.connection
 from taichu_storage.env import *
-import boto.exception
+from obs import ObsClient, PutObjectHeader
 
 
-class StorageAlluxio(StorageInterface):
+class StorageObs(StorageInterface):
+
     def __init__(self, cfgs=None):
         if cfgs is None:
             cfgs = {}
-        self._client = boto.connect_s3(
-            aws_access_key_id=S3_ACCESS_KEY_ID,
-            aws_secret_access_key=S3_SECRET_ACCESS_KEY,
-            host=ALLUXIO_HOST,
-            port=ALLUXIO_PORT,
-            path=ALLUXIO_PATH,
-            is_secure=False,
-            calling_format=boto.s3.connection.OrdinaryCallingFormat(),
+
+        self._bucket = cfgs.get('obs_bucket')
+        obs_ak = cfgs.get('obs_ak')
+        obs_sk = cfgs.get('obs_sk')
+        obs_server = cfgs.get('obs_server')
+
+        self._client = ObsClient(
+            access_key_id=obs_ak,
+            secret_access_key=obs_sk,
+            server=obs_server
         )
-        self._bucket = self._client.get_bucket(STORAGE_BUCKET)
 
-    def write_bytes(self, content_bytes, key):
+    def download_file(self, file_path, key):
+        pass
+
+    def download_directory(self, key, local_target_directory):
+        pass
+
+    def generate_signed_url(self, key, expiration=600, host_url=None):
         try:
-            s3_key = self._bucket.new_key(key)
-            s3_key.set_contents_from_file(content_bytes)
-        except boto.exception.BotoClientError:
-            pass
+            rps = self._client.createSignedUrl("GET", self._bucket, key, "", 6000, {}, {})
+            return rps.signedUrl
         except Exception as e:
-            logging.info("key: " + key)
-            logging.error("TaichuStorageError", e)
+            logging.error(e)
+            return ''
+
+    def generate_upload_credentials(self, key, expiration=3600):
+        pass
+
+    def write_bytes(self, content_bytes, key):
+        self.write_string(content_bytes, key)
 
     def write_string(self, content_string, key):
         try:
-            s3_key = self._bucket.new_key(key)
-            s3_key.set_contents_from_string(content_string)
-        except boto.exception.BotoClientError:
-            pass
+            self._client.putContent(self._bucket, key, content=content_string)
         except Exception as e:
             logging.info("key: " + key)
             logging.error("TaichuStorageError", e)
 
     def upload_file(self, file_path, key):
-        s3_key = self._bucket.new_key(key)
-        with open(file_path, "rb") as f:
-            try:
-                s3_key.set_contents_from_file(f)
-            except:
-                return
-
-    def download_dir(self, src, dest):
-        rps = self._bucket.list(prefix=src)
-        for r in rps:
-            os.makedirs(dest, exist_ok=True)
-            local_file = f'{dest}{r.name.replace(src, "")}'
-            try:
-                key = self._bucket.get_key(r.name)
-                with open(local_file, 'wb') as f:
-                    key.get_contents_to_file(f)
-            except Exception as e:
-                if 'SAXParseException' in str(type(e)):
-                    pass
-                else:
-                    logging.error(e)
+        headers = PutObjectHeader()
+        headers.contentType = 'text/plain'
+        self._client.putFile(self._bucket, key, file_path, metadata={}, headers=headers)
```

### Comparing `taichu-storage-0.0.3/taichu_storage/b3.py` & `taichu-storage-0.0.4/taichu_storage/b3.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.3/taichu_storage/env.py` & `taichu-storage-0.0.4/taichu_storage/env.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.3/taichu_storage/minio_client.py` & `taichu-storage-0.0.4/taichu_storage/minio_client.py`

 * *Files identical despite different names*

