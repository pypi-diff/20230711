# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906.tar", last modified: Tue Jul 11 19:30:11 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650.tar", last modified: Tue Jul 11 20:57:50 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 19:30:11.735483 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 19:30:11.735483 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 19:30:11.735483 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 19:30:07.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 19:30:11.731483 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 19:30:11.735483 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15062 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3249 2023-07-11 19:29:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 19:30:11.735483 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 19:30:11.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 19:30:11.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 19:30:11.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 19:30:11.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 19:30:11.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 20:57:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.616138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.616138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15083 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711192906
+Version: 1.0.0.dev20230711205650
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711192906",
+  version="1.0.0.dev20230711205650",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,21 +302,22 @@
         )
 
     ############################################################################
     def __remove_existing_s3_objects(  # "delete_remote_objects"
             self,
             output_zarr_prefix
     ):
-        print(f'Removing existing s3 objects from: {self.__output_bucket}')
-        for key in self.__s3.list_objects(  # problem here
-                bucket_name=self.__output_bucket,
-                prefix=output_zarr_prefix,
-                access_key_id=self.__output_bucket_access_key,
-                secret_access_key=self.__output_bucket_secret_access_key
-        ):
+        print(f'Removing existing s3 objects from: {self.__output_bucket} with prefix {output_zarr_prefix}')
+        keys = self.__s3.list_objects(
+            bucket_name=self.__output_bucket,
+            prefix=output_zarr_prefix,
+            access_key_id=self.__output_bucket_access_key,
+            secret_access_key=self.__output_bucket_secret_access_key
+        )
+        for key in keys:
             self.__s3.delete_object(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
         # print('Removing existing s3 objects done')
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,19 @@
     table_name=table_name,
     output_bucket_access_key=output_bucket_access_key,
     output_bucket_secret_access_key=output_bucket_secret_access_key
 )
 
 
 def handler(sns_event, context):
+    print(os.environ['TABLE_NAME'])
     print(os.environ['INPUT_BUCKET'])
     print(os.environ['OUTPUT_BUCKET'])
-    print(os.environ['TABLE_NAME'])
+    print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
+    print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
     #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     # There should only ever be one message at a time.
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,20 +47,22 @@
     def list_objects(  # analog to "find_children_objects"
             self,
             bucket_name,
             prefix,
             access_key_id=None,
             secret_access_key=None
     ):
+        # Returns a list of key strings for each object in bucket defined by prefix
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
         keys = []
         for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             if 'Contents' in page.keys():
                 # keys.extend(page['Contents'])
                 keys.extend([k['Key'] for k in page['Contents']])
+        print(f'Found {len(keys)} items')
         return keys
 
     #####################################################################
     def download_file(
             self,
             bucket_name,
             key,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711192906
+Version: 1.0.0.dev20230711205650
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711192906/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

