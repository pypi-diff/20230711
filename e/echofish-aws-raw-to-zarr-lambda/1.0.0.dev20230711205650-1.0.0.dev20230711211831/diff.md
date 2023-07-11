# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650.tar", last modified: Tue Jul 11 20:57:50 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831.tar", last modified: Tue Jul 11 21:19:31 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 20:57:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.616138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.616138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15083 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-07-11 20:56:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:57:50.620138 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 20:57:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 21:19:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.587630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.587630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15083 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711205650
+Version: 1.0.0.dev20230711211831
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711205650",
+  version="1.0.0.dev20230711211831",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,34 +5,39 @@
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
 input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
 
-output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
-output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
+if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
+    output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
+
+if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
+    output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     dynamo_operations=DynamoOperations(),
     input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
-    output_bucket_access_key=output_bucket_access_key,
-    output_bucket_secret_access_key=output_bucket_secret_access_key
+    output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
+    output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY')
 )
 
 
 def handler(sns_event, context):
     print(os.environ['TABLE_NAME'])
     print(os.environ['INPUT_BUCKET'])
     print(os.environ['OUTPUT_BUCKET'])
-    print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
-    print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
+    if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
+        print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
+    if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
+        print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
     #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     # There should only ever be one message at a time.
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711205650
+Version: 1.0.0.dev20230711211831
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711205650/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

