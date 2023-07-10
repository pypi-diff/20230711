# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510.tar", last modified: Mon Jul 10 20:46:16 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951.tar", last modified: Mon Jul 10 21:40:54 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:46:16.172060 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 20:46:16.172060 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:46:16.172060 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-10 20:46:11.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:46:16.168060 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:46:16.172060 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15503 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     5652 2023-07-10 20:45:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:46:16.172060 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 20:46:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-10 20:46:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:46:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 20:46:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 20:46:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:40:54.191064 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 21:40:54.191064 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:40:54.191064 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-10 21:40:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:40:54.187063 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:40:54.187063 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15590 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-07-10 21:39:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:40:54.191064 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 21:40:54.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-10 21:40:54.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:40:54.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 21:40:54.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 21:40:54.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230710204510
+Version: 1.0.0.dev20230710213951
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230710204510",
+  version="1.0.0.dev20230710213951",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
     # TODO: I am thinking that that this won't delete everything?
     #  Needs batches -rk
     #  Needs passed in list of files by prefix
     def __remove_existing_s3_objects(
         self,
         output_zarr_prefix
     ):
-        print('removing existing s3 objects')
+        print(f'removing existing s3 objects from: {self.__output_bucket}')
         for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
             self.__s3.delete(
@@ -385,14 +385,15 @@
             store_name=store_name
         )
         print('create local zarr store done')
         # self.__create_local_zarr_store(file_name, cruise_name, sensor_name, output_zarr_prefix, store_name)
         # TODO: needs to (1) find all objects in s3 bucket and then (2) delete those files in batches
         # TODO: (1) needs to search by prefix for all files
         # TODO: (2) needs to search
+        print(f"output bucket = {self.__output_bucket}")
         self.__remove_existing_s3_objects(output_zarr_prefix=output_zarr_prefix)
         print('remove existing s3 objects done')
         self.__upload_files(store_name, output_zarr_prefix)
         print('upload files done')
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     table_name,
     output_bucket_access_key,
     output_bucket_secret_access_key
 )
 
 
 def handler(sns_event, context):
+    print(os.environ['INPUT_BUCKET'])
+    print(os.environ['OUTPUT_BUCKET'])
+    print(os.environ['TABLE_NAME'])
+    #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     # This should only ever be one message at a time...
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230710204510
+Version: 1.0.0.dev20230710213951
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710204510/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710213951/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

