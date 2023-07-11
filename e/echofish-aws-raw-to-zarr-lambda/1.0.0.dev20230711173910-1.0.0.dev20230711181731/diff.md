# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910.tar", last modified: Tue Jul 11 17:40:13 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731.tar", last modified: Tue Jul 11 18:18:33 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 17:40:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.567964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    14857 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 18:18:29.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.446885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.446885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15694 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4953 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711173910
+Version: 1.0.0.dev20230711181731
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711173910",
+  version="1.0.0.dev20230711181731",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         to keep the storage footprint below the 512 MB allocation.
 
         Returns
         -------
         None : None
             No return value.
         """
-        print('Deleting all local raw and zarr files')
+        print('delete_all_local_raw_and_zarr')
         for i in ['*.raw*', '*.zarr']:
             for j in glob.glob(i):
-                # print(f'Deleting {j}')
+                print(f'Deleting {j}')
                 if os.path.isdir(j):
                     shutil.rmtree(j, ignore_errors=True)
                 elif os.path.isfile(j):
                     os.remove(j)
 
     ############################################################################
     def __set_processing_status(
@@ -286,78 +286,88 @@
         #################################################################
         print('Note: Adding GeoJSON inside Zarr store')
         self.__write_geojson_to_file(store_name=store_name, data=gps_data)
         #################################################################
         self.__zarr_info_to_table(
             cruise_name=cruise_name,
             file_name=raw_file_name,
-            zarr_path=os.path.join(output_zarr_prefix, store_name),
+            zarr_path=output_zarr_prefix,
             min_echo_range=min_echo_range,
             max_echo_range=max_echo_range,
             num_ping_time_dropna=num_ping_time_dropna,
             start_time=start_time,
             end_time=end_time,
             frequencies=frequencies,
             channels=channels
         )
 
     ############################################################################
-    def __remove_existing_s3_objects(  # "delete_remote_objects"
+    # TODO: I am thinking that that this won't delete everything?
+    #  Needs batches -rk
+    #  Needs passed in list of files by prefix
+    def __remove_existing_s3_objects(
         self,
         output_zarr_prefix
     ):
-        print(f'Removing existing s3 objects from: {self.__output_bucket}')
+        print('removing existing s3 objects')
+        print('access key id')
+        print(self.__output_bucket_access_key)
+        print(self.__output_bucket_secret_access_key)
+        print('keys done')
+        self.__s3.list_objects
         for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
-            self.__s3.delete_object(
+
+            self.__s3.delete(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
-        # print('Removing existing s3 objects done')
 
     ############################################################################
     def __upload_files(
         self,
         local_directory,
         object_prefix
     ):
-        print('Uploading files')
         for subdir, dirs, files in os.walk(local_directory):
             for file in files:
                 local_path = os.path.join(subdir, file)
-                # print(local_path)
+                print(local_path)
                 s3_key = os.path.join(object_prefix, local_path)
                 self.__s3.upload_file(
                     file_name=local_path,
                     bucket_name=self.__output_bucket,
                     key=s3_key,
                     access_key_id=self.__output_bucket_access_key,
                     secret_access_key=self.__output_bucket_secret_access_key
                 )
-        # print('Done uploading files')
 
     ############################################################################
     def execute(self, message):
+        # SNS Variables passed in
         ship_name = message['ship_name']
         cruise_name = message['cruise_name']
         sensor_name = message['sensor_name']
         input_file_name = message['input_file_name']
         #
         store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
-        print(store_name)
-        output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
+        output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{store_name}/"
         bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
         print(bucket_key)
         #
+        # TODO: get processing status here and handle for idempotency
+        # print(f"Processing: {input_file_name} for {cruise_name}")
+        # processing_status = self.__get_processing_status(input_file_name, cruise_name)
+        #
         os.chdir(TEMPDIR)
         print(os.getcwd())
         #
         self.__set_processing_status(
             ship_name=ship_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
@@ -368,23 +378,31 @@
         self.__delete_all_local_raw_and_zarr_files()
         #
         self.__s3.download_file(
             bucket_name=self.__input_bucket,
             key=bucket_key,
             file_name=input_file_name
         )
+        print('s3 download file done')
         self.__create_local_zarr_store(
             raw_file_name=input_file_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             output_zarr_prefix=output_zarr_prefix,
             store_name=store_name
         )
+        print('create local zarr store done')
+        # self.__create_local_zarr_store(file_name, cruise_name, sensor_name, output_zarr_prefix, store_name)
+        # TODO: needs to (1) find all objects in s3 bucket and then (2) delete those files in batches
+        # TODO: (1) needs to search by prefix for all files
+        # TODO: (2) needs to search
         self.__remove_existing_s3_objects(output_zarr_prefix=output_zarr_prefix)
+        print('remove existing s3 objects done')
         self.__upload_files(store_name, output_zarr_prefix)
+        print('upload files done')
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
             new_status='SUCCESS'
         )
         self.__delete_all_local_raw_and_zarr_files()
         #
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import os
 import json
 from .lambda_executor import LambdaExecutor
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
-input_bucket = os.environ['INPUT_BUCKET']
+input_bucket = os.environ['INPUT_BUCKET']  # TODO: move some of these variables to be passed in from SNS
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
-
+#
 output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
 output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 
+# executor = LambdaExecutor(
+#     s3_operations=S3Operations(),
+#     dynamo_operations=DynamoOperations(),
+#     #
+#     # input_bucket=input_bucket, # TODO: remove
+#     # output_bucket=output_bucket,
+#     # table_name=table_name,
+#     #
+#     output_bucket_access_key=output_bucket_access_key,
+#     output_bucket_secret_access_key=output_bucket_secret_access_key
+# )
 executor = LambdaExecutor(
-    s3_operations=S3Operations(),
-    dynamo_operations=DynamoOperations(),
-    input_bucket=input_bucket,
-    output_bucket=output_bucket,
-    table_name=table_name,
-    output_bucket_access_key=output_bucket_access_key,
-    output_bucket_secret_access_key=output_bucket_secret_access_key
+    S3Operations(),
+    DynamoOperations(),
+    input_bucket,
+    output_bucket,
+    table_name,
+    output_bucket_access_key,
+    output_bucket_secret_access_key
 )
 
 
 def handler(sns_event, context):
-    print(os.environ['INPUT_BUCKET'])
-    print(os.environ['OUTPUT_BUCKET'])
-    print(os.environ['TABLE_NAME'])
-    #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
-    # There should only ever be one message at a time.
+    # This should only ever be one message at a time...
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
         print("Done Message : " + str(message))
     print("Done Event : " + str(sns_event))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,26 +4,77 @@
 class S3Operations:
     #####################################################################
     def __get_client(
         self,
         access_key_id=None,
         secret_access_key=None
     ):
-        session = boto3.Session()
+        # client = None
         if access_key_id:
-            client = session.client(
+            print('there is an access_key_id')
+            client = boto3.Session().client(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
         else:
-            client = session.client(service_name='s3')
+            client = boto3.Session().client('s3')
+            print('there is not an access_key_id')
+        print('testing client...')
+        client.list_objects(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow/HB0707')['Contents'][0]
         return client
 
     #####################################################################
+    def list_objects(  # analog to "find_children_objects"
+        self,
+        bucket_name,
+        prefix,
+        access_key_id=None,
+        secret_access_key=None
+    ):
+        print(access_key_id)
+        keys = []
+        s3_client = self.__get_client(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        )
+        s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds')
+        print(s3_client.meta.endpoint_url)
+        print(s3_client.meta.region_name)
+        print(s3_client.meta.config.signature_version)  # s3v4
+        print(s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds'))
+        print('listing files')
+        len(s3_client.list_objects_v2(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow')['Contents'])
+        print('other')
+        for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
+            # problem here
+            if 'Contents' in page.keys():
+                keys.extend(page['Contents'])
+        return keys
+
+    #####################################################################
+    def get_s3_files(self):
+        # gets a set of files
+        pass
+
+    #####################################################################
+    def download_file(
+        self,
+        bucket_name,
+        key,
+        file_name,
+        access_key_id=None,  # This should always be a bucket we have aws credentials for
+        secret_access_key=None
+    ):
+        self.__get_client(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        ).download_file(Bucket=bucket_name, Key=key, Filename=file_name)
+
+    #####################################################################
     def __chunked(
             self,
             ll: list,
             n: int
     ) -> Generator:
         """Yields successively n-sized chunks from ll.
 
@@ -39,80 +90,60 @@
         Batches : Generator
             Breaks the data into smaller chunks for processing
         """
         for i in range(0, len(ll), n):
             yield ll[i:i + n]
 
     #####################################################################
-    def list_objects(  # analog to "find_children_objects"
-        self,
-        bucket_name,
-        prefix,
-        access_key_id=None,
-        secret_access_key=None
-    ):
-        s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        keys = []
-        for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
-            if 'Contents' in page.keys():
-                keys.extend(page['Contents'])
-        return keys
-
-    #####################################################################
-    def download_file(
+    def delete(
         self,
         bucket_name,
         key,
-        file_name,
         access_key_id=None,
         secret_access_key=None
     ):
-        s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        s3_client.download_file(Bucket=bucket_name, Key=key, Filename=file_name)
+        self.__get_client(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        ).delete_object(
+            Bucket=bucket_name,
+            Key=key,
+        )
 
     #####################################################################
-    def delete_object(
+    def delete_children_files(  # was "delete_remote_objects"
         self,
-        bucket_name,
-        key,
-        access_key_id=None,
-        secret_access_key=None
+        raw_zarr_files: list,
+        output_bucket: str,
+        access_key_id: str = None,
+        secret_access_key: str = None,
     ):
-        s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        s3_client.delete_object(Bucket=bucket_name, Key=key)
-
-    #####################################################################
-    # def delete_children_files(
-    #     self,
-    #     raw_zarr_files: list,
-    #     output_bucket: str,
-    #     access_key_id: str = None,
-    #     secret_access_key: str = None,
-    # ):
-    #     s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-    #     # deletes all given keys in s3 bucket
-    #     objects_to_delete = []
-    #     for raw_zarr_file in raw_zarr_files:
-    #         objects_to_delete.append({'Key': raw_zarr_file['Key']})
-    #     # Delete in groups of 100 — Boto3 constraint
-    #     for batch in self.__chunked(ll=objects_to_delete, n=100):
-    #         deleted = s3_client.delete_objects(
-    #             Bucket=output_bucket,
-    #             Delete={
-    #                 "Objects": batch
-    #             }
-    #         )
-    #         print(f"Deleted {len(deleted['Deleted'])} files")
+        # deletes all given keys in s3 bucket
+        objects_to_delete = []
+        for raw_zarr_file in raw_zarr_files:
+            objects_to_delete.append({'Key': raw_zarr_file['Key']})
+        # Delete in groups of 100 — Boto3 constraint
+        for batch in self.__chunked(ll=objects_to_delete, n=100):
+            deleted = self.__get_client(
+                access_key_id=access_key_id,
+                secret_access_key=secret_access_key
+            ).delete_objects(
+                Bucket=output_bucket,
+                Delete={
+                    "Objects": batch
+                }
+            )
+            print(f"Deleted {len(deleted['Deleted'])} files")
 
     #####################################################################
     def upload_file(
         self,
         file_name,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
-        s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        s3_client.upload_file(Filename=file_name, Bucket=bucket_name, Key=key)
-
-    #####################################################################
+        self.__get_client(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        ).upload_file(file_name, bucket_name, key)
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711173910
+Version: 1.0.0.dev20230711181731
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

