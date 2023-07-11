# Comparing `tmp/copernicus_marine_client-0.8.2.tar.gz` & `tmp/copernicus_marine_client-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.8.2.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.3.tar", max compression
```

## Comparing `copernicus_marine_client-0.8.2.tar` & `copernicus_marine_client-0.8.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     9103 2023-07-05 07:04:24.236147 copernicus_marine_client-0.8.2/README.md
--rw-r--r--   0        0        0     3171 2023-07-06 10:59:48.043538 copernicus_marine_client-0.8.2/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544268 copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22216 2023-07-04 12:57:10.517378 copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6086 2023-07-06 15:00:15.185228 copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544602 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      994 2023-07-06 10:59:48.043727 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3773 2023-07-04 07:33:17.711168 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4811 2023-07-05 07:04:24.237360 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_login.py
--rw-r--r--   0        0        0     7914 2023-07-05 07:04:24.237641 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    16597 2023-07-06 15:00:15.185721 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     5504 2023-07-05 07:04:24.238384 copernicus_marine_client-0.8.2/copernicus_marine_client/configuration_files_creator.py
--rw-r--r--   0        0        0     7410 2023-07-06 14:15:57.965380 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     4542 2023-07-03 12:00:07.546849 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0     8265 2023-07-06 14:10:45.282837 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     6561 2023-07-06 06:34:51.194727 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     3964 2023-07-06 15:00:15.186118 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0     4387 2023-07-06 14:10:45.283346 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/subset_xarray.py
--rw-r--r--   0        0        0      768 2023-07-04 13:23:10.163027 copernicus_marine_client-0.8.2/copernicus_marine_client/logging_conf.json
--rw-r--r--   0        0        0      888 2023-07-06 15:00:49.565238 copernicus_marine_client-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    10635 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.2/setup.py
--rw-r--r--   0        0        0    10042 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     9103 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/README.md
+-rw-r--r--   0        0        0     3171 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22196 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6086 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3797 2023-07-11 08:16:13.394928 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4811 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     7976 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    16597 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     5504 2023-07-04 16:10:02.508215 copernicus_marine_client-0.8.3/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7410 2023-07-03 13:46:52.425573 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4542 2023-07-03 13:46:52.425573 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     8265 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     8203 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     3964 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.3/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      887 2023-07-11 15:22:50.028698 copernicus_marine_client-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    10631 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.3/setup.py
+-rw-r--r--   0        0        0    10038 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.3/PKG-INFO
```

### Comparing `copernicus_marine_client-0.8.2/README.md` & `copernicus_marine_client-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,16 +454,16 @@
         for protocol in protocol_key_order
     )
     try:
         dataset_url = next(filter(lambda dataset: dataset, dataset_urls))
         protocol = get_protocol_from_url(dataset_url)
     except StopIteration as exception:
         error = KeyError(
-            f"Dataset {dataset_id} does not have a valid protocol "
-            f"for subset function. Available protocols: {protocol_key_order}"
+            f"Dataset {dataset_id} does not have a valid protocol."
+            f" Available protocols: {protocol_key_order}"
         )
         logging.error(error)
         raise error from exception
     return protocol, dataset_url
 
 
 def get_dataset_from_id(
```

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,17 +125,19 @@
         if not include_datasets:
             attributes.pop("datasets", None)
         if not include_keywords:
             attributes.pop("keywords", None)
         return obj.__dict__
 
     json_dump = (
-        dumps(catalogue, default=default_filter, sort_keys=True)
+        dumps(catalogue, default=default_filter, sort_keys=False)
         if one_line
-        else dumps(catalogue, default=default_filter, sort_keys=True, indent=2)
+        else dumps(
+            catalogue, default=default_filter, sort_keys=False, indent=2
+        )
     )
     logger = logging.getLogger("blank_logger")
     logger.warn(json_dump)
 
 
 if __name__ == "__main__":
     cli_group_describe()
```

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_login.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
             raise value_error
     username, password = get_username_password(
         username,
         password,
         config_file_directory,
     )
     # --- Download redirection by protocol
+    logging.info(f"Downloading using protocol {protocol}...")
     if protocol == FTP_KEY:
         download_summary = download_ftp(
             username,
             password,
             native_request,
         )
         logging.info(download_summary)
```

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/configuration_files_creator.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/configuration_files_creator.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_motu.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/subset_xarray.py` & `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/subset_xarray.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/copernicus_marine_client/logging_conf.json` & `copernicus_marine_client-0.8.3/copernicus_marine_client/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.2/pyproject.toml` & `copernicus_marine_client-0.8.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.8.2"
+version = "0.8.3"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
@@ -19,15 +19,15 @@
 pystac = ">=1.7.2"
 xarray = ">=2023.3.0"
 tqdm = ">=4.65.0"
 zarr = ">=2.13.3"
 pydap = ">=3.2.2"
 dask = ">=2022.1.1"
 netCDF4 = ">=1.6.3"
-s3fs = "^2023.6.0"
+boto3 = "^1.28.2"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.20.0"
 types-requests = "2.27.11"
 ipython="^8.14.0"
 
 [tool.poetry.scripts]
```

### Comparing `copernicus_marine_client-0.8.2/setup.py` & `copernicus_marine_client-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,37 +8,37 @@
  'copernicus_marine_client.download_functions']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3',
+ 'boto3>=1.28.2,<2.0.0',
  'cachier>=2.0.2',
  'click>=8.0.4',
  'dask>=2022.1.1',
  'motuclient==1.8.4',
  'netCDF4>=1.6.3',
  'numpy>=1.0',
  'owslib>=0.27.2',
  'pydap>=3.2.2',
  'pystac>=1.7.2',
  'requests>=2.27.1',
- 's3fs>=2023.6.0,<2024.0.0',
  'setuptools>=62.0.0',
  'tqdm>=4.65.0',
  'xarray>=2023.3.0',
  'zarr>=2.13.3']
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.8.2',
+    'version': '0.8.3',
     'description': '',
     'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n**Be aware that the regular expression must match the full absolute path of the files to filter.**\n\nExample:\n```\n> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to continue? [y/N]:\n```\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    assume_yes=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `copernicus_marine_client-0.8.2/PKG-INFO` & `copernicus_marine_client-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3)
+Requires-Dist: boto3 (>=1.28.2,<2.0.0)
 Requires-Dist: cachier (>=2.0.2)
 Requires-Dist: click (>=8.0.4)
 Requires-Dist: dask (>=2022.1.1)
 Requires-Dist: motuclient (==1.8.4)
 Requires-Dist: netCDF4 (>=1.6.3)
 Requires-Dist: numpy (>=1.0)
 Requires-Dist: owslib (>=0.27.2)
 Requires-Dist: pydap (>=3.2.2)
 Requires-Dist: pystac (>=1.7.2)
 Requires-Dist: requests (>=2.27.1)
-Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: setuptools (>=62.0.0)
 Requires-Dist: tqdm (>=4.65.0)
 Requires-Dist: xarray (>=2023.3.0)
 Requires-Dist: zarr (>=2.13.3)
 Description-Content-Type: text/markdown
 
 # Copernicus Marine Service client
```

