# Comparing `tmp/microSWIFTtelemetry-0.2.3.tar.gz` & `tmp/microSWIFTtelemetry-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microSWIFTtelemetry-0.2.3.tar", last modified: Thu Dec 22 16:35:18 2022, max compression
+gzip compressed data, was "microSWIFTtelemetry-0.3.tar", last modified: Tue Jul 11 00:05:52 2023, max compression
```

## Comparing `microSWIFTtelemetry-0.2.3.tar` & `microSWIFTtelemetry-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-12-22 16:35:18.354751 microSWIFTtelemetry-0.2.3/
--rw-r--r--   0 jacob      (501) staff       (20)     1068 2022-11-06 06:16:28.000000 microSWIFTtelemetry-0.2.3/LICENSE
--rw-r--r--   0 jacob      (501) staff       (20)     1362 2022-12-22 16:35:18.354614 microSWIFTtelemetry-0.2.3/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     3636 2022-12-22 16:21:15.000000 microSWIFTtelemetry-0.2.3/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-12-22 16:35:18.353035 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/
--rw-r--r--   0 jacob      (501) staff       (20)      137 2022-12-04 19:59:27.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/__init__.py
--rw-r--r--   0 jacob      (501) staff       (20)     9109 2022-12-22 16:06:37.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/pull_telemetry.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-12-22 16:35:18.354418 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/
--rw-r--r--   0 jacob      (501) staff       (20)       78 2022-12-04 20:17:51.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/__init__.py
--rw-r--r--   0 jacob      (501) staff       (20)     3471 2022-12-22 16:34:32.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/compile_sbd.py
--rw-r--r--   0 jacob      (501) staff       (20)     2844 2022-12-04 23:38:04.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/definitions.py
--rw-r--r--   0 jacob      (501) staff       (20)     4082 2022-12-22 16:34:32.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/read_sbd.py
--rw-r--r--   0 jacob      (501) staff       (20)     2385 2022-12-22 16:34:24.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/version.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-12-22 16:35:18.353597 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1362 2022-12-22 16:35:18.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      506 2022-12-22 16:35:18.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2022-12-22 16:35:18.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       31 2022-12-22 16:35:18.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)       20 2022-12-22 16:35:18.000000 microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)      145 2022-11-06 01:29:54.000000 microSWIFTtelemetry-0.2.3/pyproject.toml
--rw-r--r--   0 jacob      (501) staff       (20)       38 2022-12-22 16:35:18.354791 microSWIFTtelemetry-0.2.3/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1373 2022-11-06 20:48:39.000000 microSWIFTtelemetry-0.2.3/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.420707 microSWIFTtelemetry-0.3/
+-rw-r--r--   0 jacob      (501) staff       (20)     1068 2022-11-06 06:16:28.000000 microSWIFTtelemetry-0.3/LICENSE
+-rw-r--r--   0 jacob      (501) staff       (20)     1360 2023-07-11 00:05:52.420550 microSWIFTtelemetry-0.3/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     3636 2022-12-22 16:21:15.000000 microSWIFTtelemetry-0.3/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.418555 microSWIFTtelemetry-0.3/microSWIFTtelemetry/
+-rw-r--r--   0 jacob      (501) staff       (20)      137 2022-12-04 19:59:27.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/__init__.py
+-rw-r--r--   0 jacob      (501) staff       (20)     9144 2023-07-10 23:17:39.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/pull_telemetry.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.420170 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/
+-rw-r--r--   0 jacob      (501) staff       (20)       78 2022-12-04 20:17:51.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/__init__.py
+-rw-r--r--   0 jacob      (501) staff       (20)     4301 2023-07-10 23:28:55.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/compile_sbd.py
+-rw-r--r--   0 jacob      (501) staff       (20)     3012 2023-07-08 00:22:46.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/definitions.py
+-rw-r--r--   0 jacob      (501) staff       (20)     6227 2023-07-10 22:55:49.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/read_sbd.py
+-rw-r--r--   0 jacob      (501) staff       (20)     2387 2023-07-10 23:48:51.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/version.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.419058 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1360 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      506 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       31 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       20 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)      145 2022-11-06 01:29:54.000000 microSWIFTtelemetry-0.3/pyproject.toml
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-11 00:05:52.420751 microSWIFTtelemetry-0.3/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1373 2022-11-06 20:48:39.000000 microSWIFTtelemetry-0.3/setup.py
```

### Comparing `microSWIFTtelemetry-0.2.3/LICENSE` & `microSWIFTtelemetry-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.2.3/PKG-INFO` & `microSWIFTtelemetry-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microSWIFTtelemetry
-Version: 0.2.3
+Version: 0.3
 Summary: microSWIFTtelemetry: Python-based functionality for pulling telemetry from the microSWIFT wave buoy.
 Home-page: https://github.com/SASlabgroup/microSWIFTtelemetry
 Download-URL: 
 Author: Jacob Davis
 Author-email: davisjr@uw.edu
 Maintainer: Jacob Davis
 Maintainer-email: davisjr@uw.edu
```

### Comparing `microSWIFTtelemetry-0.2.3/README.md` & `microSWIFTtelemetry-0.3/README.md`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/pull_telemetry.py` & `microSWIFTtelemetry-0.3/microSWIFTtelemetry/pull_telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 Core module for accessing microSWIFT data from the UW-APL SWIFT server.
+#TODO:
+- needs docstr updates and flake linting
 """
 
 __all__ = [
     "create_request",
     "pull_telemetry_as_var",
     "pull_telemetry_as_zip",
     "pull_telemetry_as_json",
@@ -26,15 +28,15 @@
 
 
 def create_request(
     buoy_id: str,
     start_date: datetime,
     end_date: datetime,
     format_out: str
-)-> dict:
+) -> dict:
     """
     Create a URL-encoded request.
 
     Arguments:
         - buoy_id (str), microSWIFT ID (e.g. '043')
         - start_date (datetime), query start date in UTC
         - end_date (datetime), query end date in UTC
@@ -44,15 +46,15 @@
             * 'kml', kml of drift tracks
 
     Returns:
         - (dict), URL-enoded (utf8) request to be sent to the server
     """
 
     # Convert dates to strings:
-    start_date_str  = start_date.strftime('%Y-%m-%dT%H:%M:%S')
+    start_date_str = start_date.strftime('%Y-%m-%dT%H:%M:%S')
     end_date_str = end_date.strftime('%Y-%m-%dT%H:%M:%S')
 
     # Pack into a payload dictionary:
     payload = {
         'buoy_name' : f'microSWIFT {buoy_id}'.encode('utf8'),
         'start' : start_date_str.encode('utf8'),
         'end' : end_date_str.encode('utf8'),
@@ -63,30 +65,30 @@
 
 
 def pull_telemetry_as_var(
     buoy_id: str,
     start_date: datetime,
     end_date: datetime = datetime.utcnow(),
     var_type: str = 'dict',
-)-> Union[List[dict], DataFrame, DataArray]:
+) -> Union[List[dict], DataFrame, DataArray]:
     """
     Query the SWIFT server for microSWIFT data over a specified date
     range and return an object in memory. Note the `.zip` file of short
     burst data (SBD) messages is handled in memory and not saved to the
     local machine. Use pull_telemetry_as_zip for this purpose.
 
     Arguments:
         - buoy_id (str), microSWIFT ID (e.g. '043')
         - start_date (datetime), query start date in UTC
         - end_date (datetime, optional), query end date in UTC; defaults
                 to datetime.utcnow().
         - var_type (str, optional), variable type to return;
                 defaults to 'dict'
             Possible values include:
-            * 'dict', returns a list of dictionaries #TODO: update
+            * 'dict', returns a dictionary of lists
             * 'pandas', returns a pandas DataFrame object
             * 'xarray', returns an xarray DataArray object
 
     Returns:
         - (List[dict]), if var_type == 'dict'
         - (DataFrame), if var_type == 'pandas'
         - (DataArray), if var_type == 'xarray'
@@ -112,23 +114,23 @@
     response = urlopen(BASE_URL + request)
 
     # Read the response into memory as a virtual zip file:
     zipped_file = ZipFile(BytesIO(response.read())) # virtual zip file
     response.close()
 
     # Compile SBD messages into specified variable and return:
-    return compile_sbd(zipped_file, var_type, from_memory = True)
+    return compile_sbd(zipped_file, var_type, from_memory=True)
 
 
 def pull_telemetry_as_zip(
     buoy_id: str,
     start_date: datetime,
     end_date: datetime = datetime.utcnow(),
     local_path: str = None,
-)-> BinaryIO:
+) -> BinaryIO:
     """
     Query the SWIFT server for microSWIFT data over a specified date
     range and download a `.zip` file of individual short burst data
     (SBD) messages.
 
     Arguments:
         - buoy_id (str), microSWIFT ID (e.g. '043')
@@ -174,15 +176,15 @@
         local.close()
 
 
 def pull_telemetry_as_json(
     buoy_id: str,
     start_date: datetime,
     end_date: datetime = datetime.utcnow(),
-)-> dict:
+) -> dict:
     """
     Query the SWIFT server for microSWIFT data over a specified date
     range and download a `.zip` file of individual short burst data
     (SBD) messages.
 
     Arguments:
         - buoy_id (str), microSWIFT ID (e.g. '043')
@@ -221,20 +223,21 @@
     # Return as json
     json_data = response.read()
 
     response.close()
 
     return json.loads(json_data)
 
+
 def pull_telemetry_as_kml(
     buoy_id: str,
     start_date: datetime,
     end_date: datetime = datetime.utcnow(),
     local_path: str = None,
-)-> TextIO:
+) -> TextIO:
     """
     Query the SWIFT server for microSWIFT data over a specified date
     range and download a `.kml` file containing the buoy's coordinates.
 
     Arguments:
         - buoy_id (str), microSWIFT ID (e.g. '043')
         - start_date (datetime), query start date in UTC
@@ -267,15 +270,15 @@
     # Get the response:
     response = urlopen(BASE_URL + request)
 
     # Write the response to a local .kml geographic file:
     kml_file = response.read()
     response.close()
     if local_path is None:
-        start_date_str  = start_date.strftime('%Y-%m-%dT%H%M%S')
+        start_date_str = start_date.strftime('%Y-%m-%dT%H%M%S')
         end_date_str = end_date.strftime('%Y-%m-%dT%H%M%S')
         local_path = os.path.join(
             os.getcwd(),
             f'microSWIFT{buoy_id}_{start_date_str}_to_{end_date_str}.kml'
         )
     with open(local_path, 'wb') as local:
         local.write(kml_file)
```

### Comparing `microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/compile_sbd.py` & `microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/compile_sbd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,153 @@
 """
 Module for compiling microSWIFT short burst data (SBD) files.
+
+TODO:
+- support for xarray
 """
 
 __all__ = [
     "to_pandas_datetime_index",
     "sort_dict",
     "compile_sbd",
 ]
 
 import warnings
+from collections import defaultdict
 from typing import Any
 
 import numpy as np
 import pandas
 import xarray
 from pandas import DataFrame, to_datetime
 
 from microSWIFTtelemetry.sbd.read_sbd import read_sbd
 
 
 def compile_sbd(
     sbd_folder: str,
     var_type: str,
     from_memory: bool = False
-)-> Any:
+) -> Any:
     """
     Compile contents of short burst data files into the specified
     variable type or output.
 
-    Arguments:
-        - sbd_folder (str), directory containing.sbd files
-        - var_type (str), variable type to be returned
-        - from_memory (bool, optional), flag to indicate whether
+    Args:
+        sbd_folder (str): directory containing.sbd files
+        var_type (str): variable type to be returned
+        from_memory (bool, optional): flag to indicate whether
                 sbd_folder was loaded from memory (True) or a local file
                 (False); defaults to False.
 
     Raises:
-        - ValueError, var_type can only be 'dict', 'pandas', or 'xarray'
+        ValueError: var_type can only be 'dict', 'pandas', or 'xarray'
 
     Returns:
-        - (dict), if var_type == 'dict'
-        - (DataFrame), if var_type == 'pandas'
-        See pull_telemetry_as_var() for definitions
-
+        (dict): if var_type == 'dict'
+        (DataFrame): if var_type == 'pandas'
     """
     data = []
+    errors = []
 
-    if from_memory is True:
-
+    if from_memory:
         for file in sbd_folder.namelist():
-            data.append(read_sbd(sbd_folder.open(file)))
+            swift_data, error_message = read_sbd(sbd_folder.open(file))
+            if swift_data:
+                data.append(swift_data)
+            errors.append(error_message)
 
     else: #TODO: support reading from a folder of SBDs
-        raise Exception(('Reading from a folder on the local machine is not'
-                         'supported yet.'))
-        # for SBDfile in sbd_folder:
-        #     with open(SBDfile, mode='rb') as file: # b is important -> binary
-        #         # fileContent = file.read()
-        #         data.append(read_sbd(file))
+        raise NotImplementedError('Reading from a folder on the local '
+                                  'machine is not supported yet.')
+
+    errors = _combine_dict_list(errors)
 
     if var_type == 'dict':
-        d = {k: [d.get(k) for d in data] for k in set().union(*data)}
+        d = _combine_dict_list(data)
         if d:
             d = sort_dict(d)
         else:
-            warnings.warn("empty dict")
-        return d
+            warnings.warn("Empty dictionary; if you expected data, make sure "
+                          "the `buoy_id` is a valid microSWIFT ID and that "
+                          "`start_date` and `end_date` are correct.")
+        return d, errors
 
-    elif var_type == 'pandas':
+    if var_type == 'pandas':
         df = pandas.DataFrame(data)
+        errors = pandas.DataFrame(errors)
         if not df.empty:
             to_pandas_datetime_index(df)
         else:
-            warnings.warn("empty DataFrame")
-        return df
+            warnings.warn("Empty DataFrame; if you expected data, make sure "
+                          "the `buoy_id` is a valid microSWIFT ID and that "
+                          "`start_date` and `end_date` are correct.")
+        return df, errors
 
-    elif var_type == 'xarray': #TODO: support for xarray
-        raise Exception('xarray is not supported yet')
+    if var_type == 'xarray':  # TODO: support for xarray
+        raise NotImplementedError('xarray is not supported yet')
 
-    else:
-        raise ValueError("var_type can only be 'dict', 'pandas', or 'xarray'")
+    raise ValueError("var_type can only be 'dict', 'pandas', or 'xarray'")
 
 
 def to_pandas_datetime_index(
     df: DataFrame,
     datetime_column: str = 'datetime',
-)-> DataFrame:
+) -> DataFrame:
     """
     Convert a pandas.DataFrame integer index to a pandas.DatetimeIndex
     in place.
 
-    Arguments:
-        - df (DataFrame), DataFrame with integer index
-        - datetime_column (str, optional), column name containing
+    Args:
+        df (DataFrame): DataFrame with integer index
+        datetime_column (str, optional): column name containing
                 datetime objects to be converted to datetime index;
                 defaults to 'datetime'.
 
     Returns:
-        - (DataFrame), DataFrame with datetime index
+        (DataFrame): DataFrame with datetime index
     """
     df[datetime_column] = to_datetime(df['datetime'], utc=True)
     df.set_index('datetime', inplace=True)
     df.sort_index(inplace=True)
     # df.drop(['datetime'], axis=1, inplace=True)
 
 
+def _combine_dict_list(dict_list):
+    """Helper function to combine a list of dictionaries with equivalent keys.
+
+    Args:
+        dict_list (list): list containing dictonaries
+
+    Returns:
+        dict: unified dictionary
+    """
+    combined_dict = defaultdict(list)
+    for d in dict_list:
+        for key, value in d.items():
+            combined_dict[key].append(value)
+
+    return combined_dict
+    # return {k: [d.get(k) for d in dict_list] for k in set().union(*dict_list)}
+
+
 def sort_dict(
     d: dict,
-)-> dict:
+) -> dict:
     """
     Sort each key of a dictionary containing microSWIFT data based on
     the key containing datetime information.
 
-    Arguments:
-        - d (dict), unsorted dictionary
+    Args:
+        d (dict): unsorted dictionary
             * Must contain a 'datetime' key with a list of datetimes
 
     Returns:
-        - (dict), sorted dictionary
+        (dict): sorted dictionary
     """
     sort_index = np.argsort(d['datetime'])
     d_sorted = {}
     for key, val in d.items():
         d_sorted[key] = np.array(val)[sort_index]
 
     return d_sorted
+
```

### Comparing `microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/sbd/definitions.py` & `microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 __all__ = [
     "get_sensor_type_definition",
     "get_variable_definitions",
 ]
 
 from typing import List, Tuple
 
+
 def get_sensor_type_definition(sensor_type: int) -> str:
     """
     Dictionary of microSWIFT sensor type definitions;
     see https://github.com/alexdeklerk/microSWIFT.
 
     Arguments:
         - sensor_type (int), sensor type defintion to return
@@ -25,25 +26,26 @@
     Returns:
         - (str), sensor type defintion in Python's struct module format
             * See: https://docs.python.org/3/library/struct.html
     """
 
     # Define the sensor type using Python's struct module format
     PAYLOAD_DEFINITIONS = {
-        50 : '<sbbhfff42f42f42f42f42f42f42ffffffffiiiiii',
-        51 : '<sbbhfff42fffffffffffiiiiii',
-        52 : '<sbbheee42eee42b42b42b42b42Bffeeef',
+        50: '<sbbhfff42f42f42f42f42f42f42ffffffffiiiiii',
+        51: '<sbbhfff42fffffffffffiiiiii',
+        52: '<sbBheee42eee42b42b42b42b42Bffeeef',  # original v1 has `b` in third pos
     }
 
     if sensor_type not in PAYLOAD_DEFINITIONS.keys():
         raise ValueError((f'sensor_type not defined - can only be value in:'
                           f'{list(PAYLOAD_DEFINITIONS.keys())}'))
 
     return PAYLOAD_DEFINITIONS[sensor_type]
 
+
 def get_variable_definitions() -> List[Tuple]:
     """
     microSWIFT variable definitions.
 
     Returns:
         - (List[Tuple]), microSWIFT variable definitions with format:
             [
@@ -52,15 +54,15 @@
             ]
     """
     VARIABLE_DEFINITIONS = [
         ('datetime', "native Python datetime.datetime", "(datetime)"),
         ('significant_height', "significant wave height", "(m)"),
         ('peak_period', "peak period", "(s) "),
         ('peak_direction', "peak ave direction", "(deg)"),
-        ('energy_density' , "energy density", "(m^2/Hz)"),
+        ('energy_density', "energy density", "(m^2/Hz)"),
         ('frequency' , "frequency", "(Hz)"),
         ('a1', "first directional moment, positive E", "(-)"),
         ('b1', "second directional moment, positive N", "(-)"),
         ('a2', "third directional moment, positive E-W", "(-)"),
         ('b2', "fourth directional moment, positive NE-SW", "(-)"),
         ('check', "check factor", "(-)"),
         ('u_mean', "mean GPS E-W velocity, positive E", "(m/s)"),
@@ -68,10 +70,12 @@
         ('z_mean', "mean GPS altitude, positive up", "(m)"),
         ('latitude', "mean GPS latitude", "(decimal degrees)"),
         ('longitude', "mean GPS longitude", "(decimal degrees)"),
         ('temperature', "mean temperature", "(C)"),
         ('salinity', "mean salinity", "(psu)"),
         ('voltage', "mean battery voltage", "(V)"),
         ('sensor_type', "Iridium sensor type definition", "(-)"),
+        ('com_port', "Iridium com port or # of replaced values", "(-)"),
+        ('payload_size', "Iridium message size", "(bytes)"),
     ]
 
     return VARIABLE_DEFINITIONS
```

### Comparing `microSWIFTtelemetry-0.2.3/microSWIFTtelemetry/version.py` & `microSWIFTtelemetry-0.3/microSWIFTtelemetry/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import, division, print_function
 from os.path import join as pjoin
 
 # Format expected by setup.py and doc/source/conf.py: string of form "X.Y.Z"
 _version_major = 0
-_version_minor = 2
-_version_micro = 3  # use '' for first of series, number for 1 and above
+_version_minor = 3
+_version_micro = ''  # use '' for first of series, number for 1 and above
 # _version_extra = 'dev'
-_version_extra = ''  #TODO: Uncomment this for full releases
+_version_extra = ''  # TODO: Uncomment this for full releases
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor]
 if _version_micro:
     _ver.append(_version_micro)
 if _version_extra:
     _ver.append(_version_extra)
```

### Comparing `microSWIFTtelemetry-0.2.3/microSWIFTtelemetry.egg-info/PKG-INFO` & `microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microSWIFTtelemetry
-Version: 0.2.3
+Version: 0.3
 Summary: microSWIFTtelemetry: Python-based functionality for pulling telemetry from the microSWIFT wave buoy.
 Home-page: https://github.com/SASlabgroup/microSWIFTtelemetry
 Download-URL: 
 Author: Jacob Davis
 Author-email: davisjr@uw.edu
 Maintainer: Jacob Davis
 Maintainer-email: davisjr@uw.edu
```

### Comparing `microSWIFTtelemetry-0.2.3/setup.py` & `microSWIFTtelemetry-0.3/setup.py`

 * *Files identical despite different names*

