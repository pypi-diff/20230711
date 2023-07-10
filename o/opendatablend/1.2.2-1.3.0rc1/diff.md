# Comparing `tmp/opendatablend-1.2.2.tar.gz` & `tmp/opendatablend-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatablend-1.2.2.tar", last modified: Wed Jul  5 07:47:47 2023, max compression
+gzip compressed data, was "opendatablend-1.3.0rc1.tar", last modified: Mon Jul 10 23:45:55 2023, max compression
```

## Comparing `opendatablend-1.2.2.tar` & `opendatablend-1.3.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.866522 opendatablend-1.2.2/
--rw-rw-rw-   0        0        0     1110 2021-07-06 22:59:46.000000 opendatablend-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     8862 2023-07-05 07:47:47.868525 opendatablend-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8280 2022-04-15 16:48:40.000000 opendatablend-1.2.2/README.md
--rw-rw-rw-   0        0        0      108 2021-07-06 22:59:46.000000 opendatablend-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      861 2023-07-05 07:47:47.876170 opendatablend-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.703982 opendatablend-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.767272 opendatablend-1.2.2/src/opendatablend/
--rw-rw-rw-   0        0        0       48 2021-07-06 22:59:46.000000 opendatablend-1.2.2/src/opendatablend/__init__.py
--rw-rw-rw-   0        0        0    16623 2023-07-05 07:38:24.000000 opendatablend-1.2.2/src/opendatablend/opendatablend.py
-drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.862507 opendatablend-1.2.2/src/opendatablend.egg-info/
--rw-rw-rw-   0        0        0     8862 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 23:45:55.334466 opendatablend-1.3.0rc1/
+-rw-rw-rw-   0        0        0     1110 2021-07-06 22:59:46.000000 opendatablend-1.3.0rc1/LICENSE
+-rw-rw-rw-   0        0        0    15316 2023-07-10 23:45:55.335469 opendatablend-1.3.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0    14731 2023-07-10 23:05:48.000000 opendatablend-1.3.0rc1/README.md
+-rw-rw-rw-   0        0        0      108 2021-07-06 22:59:46.000000 opendatablend-1.3.0rc1/pyproject.toml
+-rw-rw-rw-   0        0        0      864 2023-07-10 23:45:55.339465 opendatablend-1.3.0rc1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 23:45:55.263904 opendatablend-1.3.0rc1/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 23:45:55.286901 opendatablend-1.3.0rc1/src/opendatablend/
+-rw-rw-rw-   0        0        0       64 2023-07-10 19:43:55.000000 opendatablend-1.3.0rc1/src/opendatablend/__init__.py
+-rw-rw-rw-   0        0        0    17475 2023-07-10 23:31:38.000000 opendatablend-1.3.0rc1/src/opendatablend/opendatablend.py
+drwxrwxrwx   0        0        0        0 2023-07-10 23:45:55.331465 opendatablend-1.3.0rc1/src/opendatablend.egg-info/
+-rw-rw-rw-   0        0        0    15316 2023-07-10 23:45:55.000000 opendatablend-1.3.0rc1/src/opendatablend.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-10 23:45:55.000000 opendatablend-1.3.0rc1/src/opendatablend.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 23:45:55.000000 opendatablend-1.3.0rc1/src/opendatablend.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-07-10 23:45:55.000000 opendatablend-1.3.0rc1/src/opendatablend.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 23:45:55.000000 opendatablend-1.3.0rc1/src/opendatablend.egg-info/top_level.txt
```

### Comparing `opendatablend-1.2.2/LICENSE` & `opendatablend-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatablend-1.2.2/setup.cfg` & `opendatablend-1.3.0rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 7065 6e64 6174 6162 6c65 6e64   = opendatablend
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
-00000030: 320d 0a61 7574 686f 7220 3d20 4f70 656e  2..author = Open
-00000040: 2044 6174 6120 426c 656e 640d 0a61 7574   Data Blend..aut
-00000050: 686f 725f 656d 6169 6c20 3d20 696e 666f  hor_email = info
-00000060: 406f 7065 6e64 6174 6162 6c65 6e64 2e69  @opendatablend.i
-00000070: 6f0d 0a64 6573 6372 6970 7469 6f6e 203d  o..description =
-00000080: 2054 6865 2066 6173 7465 7374 2077 6179   The fastest way
-00000090: 2074 6f20 6765 7420 6461 7461 2066 726f   to get data fro
-000000a0: 6d20 7468 6520 4f70 656e 2044 6174 6120  m the Open Data 
-000000b0: 426c 656e 6420 4461 7461 7365 7420 4150  Blend Dataset AP
-000000c0: 490d 0a6c 6f6e 675f 6465 7363 7269 7074  I..long_descript
-000000d0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000e0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-00000100: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-00000110: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
-00000130: 7065 6e64 6174 6162 6c65 6e64 2f6f 7065  pendatablend/ope
-00000140: 6e64 6174 6162 6c65 6e64 2d70 790d 0a70  ndatablend-py..p
-00000150: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000160: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-00000170: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000180: 6d2f 6f70 656e 6461 7461 626c 656e 642f  m/opendatablend/
-00000190: 6f70 656e 6461 7461 626c 656e 642d 7079  opendatablend-py
-000001a0: 2f69 7373 7565 730d 0a63 6c61 7373 6966  /issues..classif
-000001b0: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-000001e0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000001f0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000200: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-00000210: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000220: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
-00000230: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000240: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
-00000250: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000260: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000270: 7265 7320 3d20 3e3d 332e 370d 0a69 6e73  res = >=3.7..ins
-00000280: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000290: 0d0a 0961 7a75 7265 2d73 746f 7261 6765  ...azure-storage
-000002a0: 2d62 6c6f 623e 3d31 322e 3130 2e30 0d0a  -blob>=12.10.0..
-000002b0: 0962 6f74 6f33 0d0a 0962 6f74 6f63 6f72  .boto3...botocor
-000002c0: 650d 0a09 676f 6f67 6c65 2d63 6c6f 7564  e...google-cloud
-000002d0: 2d73 746f 7261 6765 3e3d 322e 332e 300d  -storage>=2.3.0.
-000002e0: 0a09 6672 6963 7469 6f6e 6c65 7373 3e3d  ..frictionless>=
-000002f0: 342e 302e 302c 3c35 2e30 2e30 0d0a 0972  4.0.0,<5.0.0...r
-00000300: 6571 7565 7374 730d 0a0d 0a5b 6f70 7469  equests....[opti
-00000310: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000320: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000330: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000340: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000350: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
+00000030: 3072 6331 0d0a 6175 7468 6f72 203d 204f  0rc1..author = O
+00000040: 7065 6e20 4461 7461 2042 6c65 6e64 0d0a  pen Data Blend..
+00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2069  author_email = i
+00000060: 6e66 6f40 6f70 656e 6461 7461 626c 656e  nfo@opendatablen
+00000070: 642e 696f 0d0a 6465 7363 7269 7074 696f  d.io..descriptio
+00000080: 6e20 3d20 5468 6520 6661 7374 6573 7420  n = The fastest 
+00000090: 7761 7920 746f 2067 6574 2064 6174 6120  way to get data 
+000000a0: 6672 6f6d 2074 6865 204f 7065 6e20 4461  from the Open Da
+000000b0: 7461 2042 6c65 6e64 2044 6174 6173 6574  ta Blend Dataset
+000000c0: 2041 5049 0d0a 6c6f 6e67 5f64 6573 6372   API..long_descr
+000000d0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000e0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+000000f0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000100: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000110: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000120: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000130: 6d2f 6f70 656e 6461 7461 626c 656e 642f  m/opendatablend/
+00000140: 6f70 656e 6461 7461 626c 656e 642d 7079  opendatablend-py
+00000150: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+00000160: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+00000170: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000180: 2e63 6f6d 2f6f 7065 6e64 6174 6162 6c65  .com/opendatable
+00000190: 6e64 2f6f 7065 6e64 6174 6162 6c65 6e64  nd/opendatablend
+000001a0: 2d70 792f 6973 7375 6573 0d0a 636c 6173  -py/issues..clas
+000001b0: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
+000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001e0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+000001f0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000200: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
+00000210: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000220: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
+00000230: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+00000240: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
+00000250: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
+00000260: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000270: 7175 6972 6573 203d 203e 3d33 2e37 0d0a  quires = >=3.7..
+00000280: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000290: 203d 200d 0a09 617a 7572 652d 7374 6f72   = ...azure-stor
+000002a0: 6167 652d 626c 6f62 3e3d 3132 2e31 302e  age-blob>=12.10.
+000002b0: 300d 0a09 626f 746f 330d 0a09 626f 746f  0...boto3...boto
+000002c0: 636f 7265 0d0a 0967 6f6f 676c 652d 636c  core...google-cl
+000002d0: 6f75 642d 7374 6f72 6167 653e 3d32 2e33  oud-storage>=2.3
+000002e0: 2e30 0d0a 0966 7269 6374 696f 6e6c 6573  .0...frictionles
+000002f0: 733e 3d34 2e30 2e30 2c3c 352e 302e 300d  s>=4.0.0,<5.0.0.
+00000300: 0a09 7265 7175 6573 7473 0d0a 0d0a 5b6f  ..requests....[o
+00000310: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000320: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+00000330: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+00000340: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000350: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `opendatablend-1.2.2/src/opendatablend/opendatablend.py` & `opendatablend-1.3.0rc1/src/opendatablend/opendatablend.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 base_url_local_substitution = 'opendatablend'
 
 class Output:
     def __init__(self, data_file_name, metadata_file_name):
         self.data_file_name = data_file_name
         self.metadata_file_name = metadata_file_name
 
+class OutputSet:
+    def __init__(self, data_file_names, metadata_file_name,):
+        self.data_file_names = data_file_names
+        self.metadata_file_name = metadata_file_name
 
 # Get and cache a data file and the dataset metadata
 def get_data(dataset_path, resource_name, base_path='/', access_key='', file_system='local', configuration={}):
-
     # Get the dataset metadata
     dataset = Package(dataset_path)
 
     # Get the data file metadata
     data_file = dataset.get_resource(resource_name)
 
     # Set the fully qualified data file name to mirror the logical folder structure at the server
@@ -40,15 +43,14 @@
     output = Output(output_data_file_name, output_metadata_file_name)
 
     # Return the output object which contains the fully qualified file names
     return output
 
 
 def cache_date_file(data_file, data_file_name, access_key, file_system, configuration):
-
     if file_system == "local":
         output_data_file_name = cache_data_file_to_local_file_system(data_file, access_key, data_file_name)
     elif file_system == "azure_blob_storage":
         output_data_file_name = cache_data_file_to_azure_blob_storage_file_system(data_file, access_key, data_file_name, configuration)
     elif file_system == "amazon_s3":
         output_data_file_name = cache_data_file_to_amazon_s3_file_system(data_file, access_key, data_file_name, configuration)
     elif file_system == "google_cloud_storage":
@@ -57,15 +59,14 @@
         print("No data file could be cached. Please specify a supported file system.")
         output_data_file_name = ''
 
     return output_data_file_name
 
 
 def cache_data_file_to_local_file_system(data_file, access_key, data_file_name):
-
     # Create the directory for the data file if it doesn't exist
     if not os.path.exists(os.path.dirname(data_file_name)):
         try:
             os.makedirs(os.path.dirname(data_file_name))
         except OSError as ex:
             if ex.errno != errno.EEXIST:
                 raise
@@ -85,15 +86,14 @@
                     local_file.write(chunk)            
 
     # Return the data file name at the relative path so it can be used
     return data_file_name
 
 
 def cache_data_file_to_azure_blob_storage_file_system(data_file, access_key, data_file_name, configuration):
-
     # Get the Azure Blob Storage configurations
     connection_string =  configuration["connection_string"]
     container_name = configuration["container_name"]
 
     # Create the blob client
     blob_service_client = BlobServiceClient.from_connection_string(connection_string)
 
@@ -213,15 +213,14 @@
               blob.upload_from_file(data)
 
     # Return the data file name at the relative path so it can be used  
     return output_data_file_name  
 
 
 def cache_dataset_metadata(dataset, base_path, file_system, configuration):
-
     metadata_data_file_snapshot_path = dataset.get('snapshot_path')
 
     # Set the fully qualified metadata file name to mirror the logical folder structure at the server
     metadata_file_name = base_path + metadata_data_file_snapshot_path.replace(base_url, base_url_local_substitution)
 
     if file_system == "local":
         output_metadata_file_name = cache_dataset_metadata_to_local_file_system(metadata_data_file_snapshot_path, metadata_file_name)
@@ -234,15 +233,14 @@
     else:
         print("No metadata file could be cached. Please specify a supported file system.")
         output_metadata_file_name = ''
     return output_metadata_file_name
 
 
 def cache_dataset_metadata_to_local_file_system(metadata_data_file_snapshot_path, metadata_file_name):
-
     # Create the directory for the dataset metadata file if it doesn't exist
     if not os.path.exists(os.path.dirname(metadata_file_name)):
         try:
             os.makedirs(os.path.dirname(metadata_file_name))
         except OSError as ex:
             if ex.errno != errno.EEXIST:
                 raise
@@ -254,15 +252,14 @@
         open(metadata_file_name, 'wb').write(data.content)
 
     # Return the metadata file name at the relative path so it can be used
     return metadata_file_name
 
 
 def cache_dataset_metadata_to_azure_blob_storage_file_system(metadata_data_file_snapshot_path, metadata_file_name, configuration):
-
     # Get the Azure Blob Storage configurations
     connection_string =  configuration["connection_string"]
     container_name = configuration["container_name"]
 
     # Create the blob client
     blob_service_client = BlobServiceClient.from_connection_string(connection_string)
 
@@ -367,7 +364,22 @@
     # Only upload the data file if it doesn't exist
     if not blob.exists():
         with BytesIO(requests.get(metadata_data_file_snapshot_path).content) as data:
               blob.upload_from_file(data)
         
     # Return the metadata file name at the relative path so it can be used
     return output_metadata_file_name
+
+
+def get_data_files(dataset_path, resource_names, access_key, file_system, configuration):
+    data_file_names = []    
+    for resource_name in resource_names:        
+        # Get data the and capture the output object
+        output = get_data(dataset_path=dataset_path, resource_name=resource_name, access_key=access_key, file_system=file_system, configuration=configuration)
+    
+        # Add data file name to the list of data file name
+        data_file_names.append(output.data_file_name)
+
+    outputSet = OutputSet(data_file_names, output.metadata_file_name)
+
+    # Return the output object which contains the fully qualified file names
+    return outputSet
```

