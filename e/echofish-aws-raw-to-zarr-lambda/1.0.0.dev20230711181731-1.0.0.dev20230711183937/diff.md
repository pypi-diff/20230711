# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731.tar", last modified: Tue Jul 11 18:18:33 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937.tar", last modified: Tue Jul 11 18:40:40 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 18:18:29.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.446885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.446885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15694 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4953 2023-07-11 18:17:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:18:33.450885 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 18:18:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:40:40.309588 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 18:40:40.309588 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 18:40:40.309588 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 18:40:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:40:40.305588 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:40:40.305588 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15062 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-07-11 18:39:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:40:40.309588 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 18:40:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 18:40:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 18:40:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 18:40:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 18:40:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711181731
+Version: 1.0.0.dev20230711183937
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711181731",
+  version="1.0.0.dev20230711183937",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# lambda_executor.py
 import os
 import glob
 import shutil
 import echopype as ep
 import numpy as np
 import pandas as pd
 import geopandas
@@ -10,22 +11,22 @@
 TEMPDIR = "/tmp"
 
 
 class LambdaExecutor:
 
     ############################################################################
     def __init__(
-        self,
-        s3_operations,
-        dynamo_operations,
-        input_bucket,
-        output_bucket,
-        table_name,
-        output_bucket_access_key,
-        output_bucket_secret_access_key
+            self,
+            s3_operations,
+            dynamo_operations,
+            input_bucket,
+            output_bucket,
+            table_name,
+            output_bucket_access_key,
+            output_bucket_secret_access_key
     ):
         self.__s3 = s3_operations
         self.__dynamo = dynamo_operations
         self.__input_bucket = input_bucket
         self.__output_bucket = output_bucket
         self.__table_name = table_name
         self.__output_bucket_access_key = output_bucket_access_key
@@ -37,31 +38,31 @@
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
-        self,
-        ship_name: str,
-        cruise_name: str,
-        sensor_name: str,
-        file_name: str,
-        new_status: str
+            self,
+            ship_name: str,
+            cruise_name: str,
+            sensor_name: str,
+            file_name: str,
+            new_status: str
     ):
         # Updates PIPELINE_STATUS via new_status value
         # HASH: FILE_NAME, RANGE: SENSOR_NAME
         self.__dynamo.put_item(
             table_name=self.__table_name,
             item={
                 'FILE_NAME': {'S': file_name},  # HASH
@@ -71,18 +72,18 @@
                 'PIPELINE_TIME': {'S': datetime.now().isoformat(timespec="seconds") + "Z"},
                 'PIPELINE_STATUS': {'S': new_status},
             }
         )
 
     ############################################################################
     def __update_processing_status(
-        self,
-        cruise_name,
-        file_name,
-        new_status
+            self,
+            cruise_name,
+            file_name,
+            new_status
     ):
         self.__dynamo.update_item(
             table_name=self.__table_name,
             key={
                 'FILE_NAME': {'S': file_name},  # Partition Key
                 'CRUISE_NAME': {'S': cruise_name},  # Sort Key
             },
@@ -95,42 +96,42 @@
                     'S': new_status
                 }
             }
         )
 
     ############################################################################
     def __get_processing_status(
-        self,
-        file_name,
-        cruise_name
+            self,
+            file_name,
+            cruise_name
     ):
         # HASH: FILE_NAME, RANGE: SENSOR_NAME
         item = self.__dynamo.get_item(
             TableName=self.__table_name,
             Key={
                 'FILE_NAME': {'S': file_name},  # Partition Key
                 'CRUISE_NAME': {'S': cruise_name},  # Sort Key
             })
         if item is None:
             return 'NONE'
         return item['PIPELINE_STATUS']['S']
 
     ############################################################################
     def __zarr_info_to_table(
-        self,
-        cruise_name,
-        file_name,
-        zarr_path,
-        min_echo_range,
-        max_echo_range,
-        num_ping_time_dropna,
-        start_time,
-        end_time,
-        frequencies,
-        channels
+            self,
+            cruise_name,
+            file_name,
+            zarr_path,
+            min_echo_range,
+            max_echo_range,
+            num_ping_time_dropna,
+            start_time,
+            end_time,
+            frequencies,
+            channels
     ):
         self.__dynamo.update_item(
             table_name=self.__table_name,
             key={
                 'FILE_NAME': {'S': file_name},  # Partition Key
                 'CRUISE_NAME': {'S': cruise_name},  # Sort Key # TODO: should be FILE_NAME & SENSOR_NAME so they are truely unique for when two sensors are processed within one cruise
             },
@@ -181,21 +182,21 @@
 
     ############################################################################
     def __get_gps_data(
             self,
             echodata: ep.echodata.echodata.EchoData
     ) -> tuple:
         assert(
-            'latitude' in echodata.platform.variables and 'longitude' in echodata.platform.variables
+                'latitude' in echodata.platform.variables and 'longitude' in echodata.platform.variables
         ), "Problem: GPS coordinates not found in echodata."
         latitude = echodata.platform.latitude.values
         longitude = echodata.platform.longitude.values  # len(longitude) == 14691
         # RE: time coordinates: https://github.com/OSOceanAcoustics/echopype/issues/656#issue-1219104771
         assert(
-            'time1' in echodata.platform.variables and 'time1' in echodata.environment.variables
+                'time1' in echodata.platform.variables and 'time1' in echodata.environment.variables
         ), "Problem: Time coordinate not found in echodata."
         # 'nmea_times' are times from the nmea datalogger associated with GPS
         nmea_times = echodata.platform.time1.values
         # 'time1' are times from the echosounder associated with transducer measurement
         time1 = echodata.environment.time1.values
         # Align 'sv_times' to 'nmea_times'
         assert(
@@ -205,15 +206,15 @@
         indices = np.searchsorted(a=nmea_times, v=time1, side="right") - 1
         #
         lat = latitude[indices]
         lat[indices < 0] = np.nan  # values recorded before indexing are set to nan
         lon = longitude[indices]
         lon[indices < 0] = np.nan
         assert(
-            np.all(lat[~np.isnan(lat)] >= -90.) and np.all(lat[~np.isnan(lat)] <= 90.)
+                np.all(lat[~np.isnan(lat)] >= -90.) and np.all(lat[~np.isnan(lat)] <= 90.)
         ), "Problem: Data falls outside GPS bounds!"
         # https://osoceanacoustics.github.io/echopype-examples/echopype_tour.html
         gps_df = pd.DataFrame({
             'latitude': lat,
             'longitude': lon,
             'time1': time1
         }).set_index(['time1'])
@@ -249,20 +250,20 @@
             No return value.
         """
         with open(os.path.join(store_name, 'geo.json'), "w") as outfile:
             outfile.write(data)
 
     ############################################################################
     def __create_local_zarr_store(
-        self,
-        raw_file_name,
-        cruise_name,
-        sensor_name,
-        output_zarr_prefix,
-        store_name
+            self,
+            raw_file_name,
+            cruise_name,
+            sensor_name,
+            output_zarr_prefix,
+            store_name
     ):
         print(f'Opening raw: {raw_file_name}')
         # TODO: surround with try-catch
         echodata = ep.open_raw(raw_file_name, sonar_model=sensor_name)
         print('Compute volume backscattering strength (Sv) from raw data.')
         ds_sv = ep.calibrate.compute_Sv(echodata)
         frequencies = echodata.environment.frequency_nominal.values
@@ -286,88 +287,78 @@
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
-    def __remove_existing_s3_objects(
-        self,
-        output_zarr_prefix
+    def __remove_existing_s3_objects(  # "delete_remote_objects"
+            self,
+            output_zarr_prefix
     ):
-        print('removing existing s3 objects')
-        print('access key id')
-        print(self.__output_bucket_access_key)
-        print(self.__output_bucket_secret_access_key)
-        print('keys done')
-        self.__s3.list_objects
+        print(f'Removing existing s3 objects from: {self.__output_bucket}')
         for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
-
-            self.__s3.delete(
+            self.__s3.delete_object(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
+        # print('Removing existing s3 objects done')
 
     ############################################################################
     def __upload_files(
-        self,
-        local_directory,
-        object_prefix
+            self,
+            local_directory,
+            object_prefix
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
@@ -378,31 +369,23 @@
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

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,39 @@
+# lambda_handler.py
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
+    print(os.environ['INPUT_BUCKET'])
+    print(os.environ['OUTPUT_BUCKET'])
+    print(os.environ['TABLE_NAME'])
+    #
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

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711181731
+Version: 1.0.0.dev20230711183937
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711181731/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711183937/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

