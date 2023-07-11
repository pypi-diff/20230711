# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049.tar", last modified: Tue Jul 11 16:41:53 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910.tar", last modified: Tue Jul 11 17:40:13 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:41:53.380297 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 16:41:53.380297 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 16:41:53.380297 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 16:41:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:41:53.376297 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:41:53.376297 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15811 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-07-11 16:40:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:41:53.380297 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 16:41:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 16:41:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:41:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 16:41:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 16:41:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 17:40:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.567964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    14857 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-07-11 17:39:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:40:13.571964 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 17:40:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711164049
+Version: 1.0.0.dev20230711173910
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711164049",
+  version="1.0.0.dev20230711173910",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         to keep the storage footprint below the 512 MB allocation.
 
         Returns
         -------
         None : None
             No return value.
         """
-        print('delete_all_local_raw_and_zarr')
+        print('Deleting all local raw and zarr files')
         for i in ['*.raw*', '*.zarr']:
             for j in glob.glob(i):
-                print(f'Deleting {j}')
+                # print(f'Deleting {j}')
                 if os.path.isdir(j):
                     shutil.rmtree(j, ignore_errors=True)
                 elif os.path.isfile(j):
                     os.remove(j)
 
     ############################################################################
     def __set_processing_status(
@@ -286,86 +286,78 @@
         #################################################################
         print('Note: Adding GeoJSON inside Zarr store')
         self.__write_geojson_to_file(store_name=store_name, data=gps_data)
         #################################################################
         self.__zarr_info_to_table(
             cruise_name=cruise_name,
             file_name=raw_file_name,
-            zarr_path=output_zarr_prefix,
+            zarr_path=os.path.join(output_zarr_prefix, store_name),
             min_echo_range=min_echo_range,
             max_echo_range=max_echo_range,
             num_ping_time_dropna=num_ping_time_dropna,
             start_time=start_time,
             end_time=end_time,
             frequencies=frequencies,
             channels=channels
         )
 
     ############################################################################
-    # TODO: I am thinking that that this won't delete everything?
-    #  Needs batches -rk
-    #  Needs passed in list of files by prefix
     def __remove_existing_s3_objects(  # "delete_remote_objects"
         self,
         output_zarr_prefix
     ):
-        # s3_client = self.s3__get_client(
-        #     access_key_id=self.__output_bucket_access_key,
-        #     secret_access_key=self.__output_bucket_secret_access_key
-        # )
-        print(f'removing existing s3 objects from: {self.__output_bucket}')
+        print(f'Removing existing s3 objects from: {self.__output_bucket}')
         for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
             self.__s3.delete_object(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
+        # print('Removing existing s3 objects done')
 
     ############################################################################
     def __upload_files(
         self,
         local_directory,
         object_prefix
     ):
+        print('Uploading files')
         for subdir, dirs, files in os.walk(local_directory):
             for file in files:
                 local_path = os.path.join(subdir, file)
-                print(local_path)
+                # print(local_path)
                 s3_key = os.path.join(object_prefix, local_path)
                 self.__s3.upload_file(
                     file_name=local_path,
                     bucket_name=self.__output_bucket,
                     key=s3_key,
                     access_key_id=self.__output_bucket_access_key,
                     secret_access_key=self.__output_bucket_secret_access_key
                 )
+        # print('Done uploading files')
 
     ############################################################################
     def execute(self, message):
-        # SNS Variables passed in
         ship_name = message['ship_name']
         cruise_name = message['cruise_name']
         sensor_name = message['sensor_name']
         input_file_name = message['input_file_name']
         #
         store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
-        output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{store_name}/"
+        print(store_name)
+        output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
         bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
         print(bucket_key)
         #
-        # TODO: get processing status here and handle for idempotency
-        # print(f"Processing: {input_file_name} for {cruise_name}")
-        # processing_status = self.__get_processing_status(input_file_name, cruise_name)
-        #
         os.chdir(TEMPDIR)
         print(os.getcwd())
         #
         self.__set_processing_status(
             ship_name=ship_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
@@ -376,32 +368,23 @@
         self.__delete_all_local_raw_and_zarr_files()
         #
         self.__s3.download_file(
             bucket_name=self.__input_bucket,
             key=bucket_key,
             file_name=input_file_name
         )
-        print('s3 download file done')
         self.__create_local_zarr_store(
             raw_file_name=input_file_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             output_zarr_prefix=output_zarr_prefix,
             store_name=store_name
         )
-        print('create local zarr store done')
-        # self.__create_local_zarr_store(file_name, cruise_name, sensor_name, output_zarr_prefix, store_name)
-        # TODO: needs to (1) find all objects in s3 bucket and then (2) delete those files in batches
-        # TODO: (1) needs to search by prefix for all files
-        # TODO: (2) needs to search
-        print(f"output bucket = {self.__output_bucket}")
         self.__remove_existing_s3_objects(output_zarr_prefix=output_zarr_prefix)
-        print('remove existing s3 objects done')
         self.__upload_files(store_name, output_zarr_prefix)
-        print('upload files done')
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
             new_status='SUCCESS'
         )
         self.__delete_all_local_raw_and_zarr_files()
         #
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 import os
 import json
 from .lambda_executor import LambdaExecutor
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
-input_bucket = os.environ['INPUT_BUCKET']  # TODO: move some of these variables to be passed in from SNS
+input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
-#
+
 output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
 output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 
-# executor = LambdaExecutor(
-#     s3_operations=S3Operations(),
-#     dynamo_operations=DynamoOperations(),
-#     #
-#     # input_bucket=input_bucket, # TODO: remove
-#     # output_bucket=output_bucket,
-#     # table_name=table_name,
-#     #
-#     output_bucket_access_key=output_bucket_access_key,
-#     output_bucket_secret_access_key=output_bucket_secret_access_key
-# )
 executor = LambdaExecutor(
-    S3Operations(),
-    DynamoOperations(),
-    input_bucket,
-    output_bucket,
-    table_name,
-    output_bucket_access_key,
-    output_bucket_secret_access_key
+    s3_operations=S3Operations(),
+    dynamo_operations=DynamoOperations(),
+    input_bucket=input_bucket,
+    output_bucket=output_bucket,
+    table_name=table_name,
+    output_bucket_access_key=output_bucket_access_key,
+    output_bucket_secret_access_key=output_bucket_secret_access_key
 )
 
 
 def handler(sns_event, context):
     print(os.environ['INPUT_BUCKET'])
     print(os.environ['OUTPUT_BUCKET'])
     print(os.environ['TABLE_NAME'])
     #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
-    # This should only ever be one message at a time...
+    # There should only ever be one message at a time.
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
         print("Done Message : " + str(message))
     print("Done Event : " + str(sns_event))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,48 +74,45 @@
         self,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        s3_client.delete_object(
-            Bucket=bucket_name,
-            Key=key,
-        )
+        s3_client.delete_object(Bucket=bucket_name, Key=key)
 
     #####################################################################
-    def delete_children_files(
-        self,
-        raw_zarr_files: list,
-        output_bucket: str,
-        access_key_id: str = None,
-        secret_access_key: str = None,
-    ):
-        s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        # deletes all given keys in s3 bucket
-        objects_to_delete = []
-        for raw_zarr_file in raw_zarr_files:
-            objects_to_delete.append({'Key': raw_zarr_file['Key']})
-        # Delete in groups of 100 — Boto3 constraint
-        for batch in self.__chunked(ll=objects_to_delete, n=100):
-            deleted = s3_client.delete_objects(
-                Bucket=output_bucket,
-                Delete={
-                    "Objects": batch
-                }
-            )
-            print(f"Deleted {len(deleted['Deleted'])} files")
+    # def delete_children_files(
+    #     self,
+    #     raw_zarr_files: list,
+    #     output_bucket: str,
+    #     access_key_id: str = None,
+    #     secret_access_key: str = None,
+    # ):
+    #     s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
+    #     # deletes all given keys in s3 bucket
+    #     objects_to_delete = []
+    #     for raw_zarr_file in raw_zarr_files:
+    #         objects_to_delete.append({'Key': raw_zarr_file['Key']})
+    #     # Delete in groups of 100 — Boto3 constraint
+    #     for batch in self.__chunked(ll=objects_to_delete, n=100):
+    #         deleted = s3_client.delete_objects(
+    #             Bucket=output_bucket,
+    #             Delete={
+    #                 "Objects": batch
+    #             }
+    #         )
+    #         print(f"Deleted {len(deleted['Deleted'])} files")
 
     #####################################################################
     def upload_file(
         self,
         file_name,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        s3_client.upload_file(file_name, bucket_name, key)
+        s3_client.upload_file(Filename=file_name, Bucket=bucket_name, Key=key)
 
     #####################################################################
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711164049
+Version: 1.0.0.dev20230711173910
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711164049/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711173910/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

