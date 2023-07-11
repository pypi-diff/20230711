# Comparing `tmp/iotcore_api-1.1.41.tar.gz` & `tmp/iotcore_api-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.1.41.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.5.tar", max compression
```

## Comparing `iotcore_api-1.1.41.tar` & `iotcore_api-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.41/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.41/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    56452 2023-05-30 15:26:21.704664 iotcore_api-1.1.41/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.41/iotcoreapi/nan_treatment.py
--rw-r--r--   0        0        0      744 2023-05-30 15:42:45.508297 iotcore_api-1.1.41/pyproject.toml
--rw-r--r--   0        0        0    34548 2023-05-30 15:40:36.063059 iotcore_api-1.1.41/README.md
--rw-r--r--   0        0        0    34051 1970-01-01 00:00:00.000000 iotcore_api-1.1.41/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.5/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.5/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    57644 2023-07-11 14:53:11.875194 iotcore_api-1.1.5/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.5/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      743 2023-07-11 14:55:54.845157 iotcore_api-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    33781 2023-07-11 14:57:06.239918 iotcore_api-1.1.5/README.md
+-rw-r--r--   0        0        0    34163 1970-01-01 00:00:00.000000 iotcore_api-1.1.5/PKG-INFO
```

### Comparing `iotcore_api-1.1.41/iotcoreapi/exceptions.py` & `iotcore_api-1.1.5/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.41/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.5/iotcoreapi/iotcoreapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,16 @@
         return response
 
     return wrapper
 
 
 class IoTCoreAPI:
 
-    def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "", version: str = "3.0",
+    def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "",
+                 version: typing.Union[str, int] = "3.0",
                  logger: logging.Logger = None):
         """
         Init method for iotcoreapi. Needs API configuration parameters
 
         Args:
             ip: IoT Core base endpoint
             port: API Port. Defaults to 56000
@@ -79,44 +80,52 @@
         # Check verson number
         version_regex = r'^\d+\.\d+$'
         if not bool(re.match(version_regex, version)):
             raise ValueError('Version number does not match correct format. Should be "1.0", "2.0"...')
         self.version = version
         self._version_number = float(version)
         self._time_formats = ['datetime', 'unix']
-        self._output_formats = ['dataframe', 'json']
-        self.url_NX = ip + ":" + str(port)
+        self._output_formats = ['dataframe', 'json', 'dataframe_table']
+        self.url_NX = "http://" + ip + ":" + str(port)
         self.header = {
             "nexustoken": self.token,
             "nexusapiversion": self.version,
             "Content-Type": "application/json",
         }
         self.logger = logger
         self._log_print("Created new instance of IoTCoreAPI")
 
     def _convert_response(self, response: typing.Union[dict, typing.List[dict]], output_format: str,
-                          time_format: str = None, nan_method: str = None) -> typing.Union[pd.DataFrame, dict, typing.List[dict]]:
+                          time_format: str = None, nan_method: str = None) -> typing.Union[
+        pd.DataFrame, dict, typing.List[dict]]:
         """
         Auxiliary function to transform response in json format to dataframe if indicated in output_format arg.
         Args:
             response: json
-            output_format: 'dataframe' or 'json'
+            output_format: 'dataframe' or 'json' or dataframe_table
             time_format: 'datetime' or 'unix'
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response: json or dataframe
         """
-        if output_format == 'dataframe':
+        if output_format == 'dataframe' or output_format == 'dataframe_table':
             if response:
                 response = self._json_normalize_check(response)
                 if time_format == 'datetime':
                     response['timeStamp'] = pd.to_datetime(response.timeStamp, unit='s', utc=True)
                 if nan_method is not None:
                     response = nan_treatment(response, nan_method)
+                if output_format == 'dataframe_table':
+                    try:
+                        response = pd.pivot_table(response, values='value', index='timeStamp', columns=['uid'],
+                                                  aggfunc='sum')
+                    except:
+                        raise IotCoreAPIException('Could not convert data to dataframe_table format. Please provide another format')
+
             else:
                 response = pd.DataFrame(columns=['timeStamp', 'uid', 'name', 'value'])
         return response
 
     def _log_print(self, message, severity='info'):
         if self.logger is not None:
             if severity == 'info':
@@ -159,41 +168,42 @@
 
     def catalogue_tags(self, include_attributes: bool = True, output_format: str = 'dataframe') -> typing.Union[
         dict, pd.DataFrame]:
         """Return all tags available for the token
 
         Args:
             include_attributes (optional): if version >3.0, bool to return attributes or not
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format: Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         url = self.url_NX + "/api/Tags"
         if self._version_number >= 3.0:
             params = {"IncludeAttributes": include_attributes}
         else:
             params = None
         return self._convert_response(self._getResponse(url, params), output_format)
 
-    def catalogue_tags_filtered(self, installations: typing.Union[list, str] = None, drivers: typing.Union[list, str] = None,
+    def catalogue_tags_filtered(self, installations: typing.Union[list, str] = None,
+                                drivers: typing.Union[list, str] = None,
                                 tags: typing.Union[list, str] = None,
                                 attributes: typing.Union[list, str] = None,
                                 output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Searching for tags that comply with a certain criteria can be achieved with the filtered route. If fields are empty, all tags are returned.
 
         Args:
             installations: name of the installations
             drivers: name of drivers
             tags: name of tags
             attributes: not implemented yet
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format: Result given in 'dataframe' or 'json' or 'dataframe_table'. Defaults to 'dataframe'
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -216,15 +226,15 @@
         response = self._postResponse(url, body)
         return self._convert_response(response, output_format)
 
     def catalogue_tags_attributes(self, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
         Args:
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format: Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -250,15 +260,15 @@
         response = self._getResponse(url)
         return self._convert_response(response, output_format)
 
     def catalogue_documents(self, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Returns all tagviews shared in the token
 
         Args:
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format: Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -267,15 +277,15 @@
         return self._convert_response(response, output_format)
 
     def catalogue_tagview_detail(self, uid: str, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Return all variables from a given tagview
 
         Args:
             uid: uid of the tagview
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format: Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -287,16 +297,16 @@
         return response
 
     def catalogue_alarms(self, group_uid: str = None, output_format: str = 'dataframe') -> typing.Union[
         typing.List[dict], pd.DataFrame]:
         """Returns information of the alarms in the token
 
         Args:
-            group_uid: Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
+            output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
         Returns:
             response in json or dataframe
             """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -307,15 +317,15 @@
         response = self._getResponse(url_completa, params)
         return self._convert_response(response, output_format)
 
     def catalogue_alarm_groups(self, output_format: str = 'dataframe') -> typing.Union[typing.List[dict], pd.DataFrame]:
         """Returns information of the alarm groups in the token
 
         Args:
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -324,21 +334,22 @@
         url_completa = self.url_NX + "/api/Alarms/Groups"
         response = self._getResponse(url_completa)
         return self._convert_response(response, output_format)
 
     # -------- READING OPERATIONS --------
 
     def read_tags_realtime(self, tags_uids: typing.List[str], output_format: str = 'dataframe',
-                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                           time_format='datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[dict]]:
         """Reads real time value of the tags provided in the array tags_uids
 
         Args:
-            tags_uids: list with uids of the tags
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            tags_uids : list with uids of the tags
+            output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -349,22 +360,23 @@
         url = self.url_NX + "/api/Tags/realtime"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_realtime(self, uid: str, uids_tags: typing.List[str] = None,
                               output_format: str = 'dataframe',
-                              time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                              time_format='datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[dict]]:
         """Returns real time value for the uids variables provided in a given tagview
 
         Args:
-            uid: uid of the tagview
-            uids_tags: list of uids
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            uid : uid of the tagview
+            uids_tags : list of uids
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -375,29 +387,32 @@
             uids_tags = []
         body = json.dumps(uids_tags)
         url = self.url_NX + "/api/Documents/tagviews/" + uid + "/realtime"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tags_historic(self, uids: typing.List[str], start_ts: typing.Union[int, float], end_ts: typing.Union[int, float],
-                           data_source: typing.Union[str, int] = 'RAW', resolution: typing.Union[str, int] = 'RES_1_HOUR',
+    def read_tags_historic(self, uids: typing.List[str], start_ts: typing.Union[int, float],
+                           end_ts: typing.Union[int, float],
+                           data_source: typing.Union[str, int] = 'RAW',
+                           resolution: typing.Union[str, int] = 'RES_1_HOUR',
                            agg_operation: typing.Union[str, int] = "LAST_VALUE", output_format: str = 'dataframe',
-                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                           time_format='datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[dict]]:
         """Obtain historic data of the specified tags
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix time or datetime
             end_ts: end time in unix time or datetime
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             agg_operation: MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -418,23 +433,24 @@
              "aggOperation": agg_operation})
         url = self.url_NX + "/api/Tags/historic"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_rawhistoric(self, uids, start_ts, end_ts, output_format: str = 'dataframe',
-                              time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                              time_format='datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[dict]]:
         """To obtain raw data with no aggregation or normalization applied
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix time or datetime
             end_ts: end time in unix time or datetime
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -450,33 +466,35 @@
             end_ts = end_ts.timestamp()
         body = json.dumps({"uids": uids, "startTs": start_ts, "endTs": end_ts})
         url = self.url_NX + "/api/Tags/rawhistoric"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tags_transient(self, uids: typing.List[str], start_ts: typing.Union[int, float], end_ts: typing.Union[int, float],
+    def read_tags_transient(self, uids: typing.List[str], start_ts: typing.Union[int, float],
+                            end_ts: typing.Union[int, float],
                             data_source: typing.Union[str, int] = None,
                             resolution: typing.Union[str, int] = 'RES_1_SEC',
                             output_format: str = 'dataframe',
-                            time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                            time_format='datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[dict]]:
         """
         This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
         aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
         please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
         for historic.
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained. start_ts:
             start_ts: time in unix time or datetime
             end_ts: end time in unix time or datetime. Timespan must be smaller than 15 mins
             data_source: Can be set to null or empty. Not needed
             resolution: RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -499,26 +517,27 @@
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_historic(self, uid: str, start_ts: typing.Union[datetime.datetime, float, int],
                               end_ts: typing.Union[datetime.datetime, float, int], tags_uids: typing.List[str] = None,
                               data_source='RAW',
                               resolution='RES_1_HOUR', output_format: str = 'dataframe',
-                              time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                              time_format='datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[dict]]:
         """Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
         Args:
             uid: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             tags_uids (optional): list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
             """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -536,32 +555,35 @@
             {"uids": tags_uids, "startTs": start_ts, "endTs": end_ts, "dataSource": data_source,
              "resolution": resolution})
         url = self.url_NX + "/api/Documents/tagviews/" + uid + "/historic"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tagview_historic_text_filters(self, uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int],
+    def read_tagview_historic_text_filters(self, uid_tagview: str,
+                                           start_ts: typing.Union[datetime.datetime, float, int],
                                            end_ts: typing.Union[datetime.datetime, float, int],
-                                           filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW',
+                                           filter_txt: typing.Union[str, typing.List[str]] = None,
+                                           data_source: str = 'RAW',
                                            resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe',
-                                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, \
-                                                                                                     typing.List[dict]]:
+                                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, \
+                typing.List[dict]]:
         """
         Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             filtered_hist (dataframe):
                 columns:
                     name: name of tag
                     value: value of tag
@@ -605,16 +627,16 @@
                                            nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             filtered_hist (dataframe):
                 columns:
                     name: name of tag
                     value: value of tag
@@ -641,33 +663,37 @@
         if isinstance(filtered_hist, pd.DataFrame):
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
-    def read_tags_historic_text_filters(self, uids: typing.List[str], start_ts: typing.Union[datetime.datetime, int, float],
+    def read_tags_historic_text_filters(self, uids: typing.List[str],
+                                        start_ts: typing.Union[datetime.datetime, int, float],
                                         end_ts: typing.Union[datetime.datetime, int, float],
-                                        filter_txt: typing.Union[str, typing.List[str]] = None, data_source: typing.Union[str, int] = 'RAW',
+                                        filter_txt: typing.Union[str, typing.List[str]] = None,
+                                        data_source: typing.Union[str, int] = 'RAW',
                                         resolution: typing.Union[str, int] = 'RES_1_HOUR',
-                                        agg_operation: typing.Union[str, int] = "LAST_VALUE", output_format: str = 'dataframe',
-                                        time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[
-        dict]]:
+                                        agg_operation: typing.Union[str, int] = "LAST_VALUE",
+                                        output_format: str = 'dataframe',
+                                        time_format: str = 'datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, typing.List[
+            dict]]:
         """Obtain historic data of the specified tags by name
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             agg_operation: MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -708,16 +734,16 @@
                                         time_format: str = 'datetime',
                                         nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
-            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             dataframe or json:
                 columns:
                     name: name of tag
                     value: value of tag
@@ -749,15 +775,15 @@
         return filtered_hist
 
     def read_alarm_status(self, alarm_guid: str) -> dict:
         """
         Reads alarm status for a given alarm
 
         Args:
-            alarm_guid: guid of the alarm
+            alarm_guid : guid of the alarm
 
         Returns:
             Dictionary with following data:
             {
                 "name": "BasicAlarm1",
                 "uid": "b926bfb0-3f2f-49df-a2eb-138452296903",
                 "status": "ARE",
@@ -788,18 +814,18 @@
         Args:
             tags: tags name or names to be created
 
         Returns:
             response object in json format:
                 [
                    {
-                     "Uid": "unique tag identifier",
-                     "Name": "name of the tag",
-                     "Installation": "name of the installation",
-                     "Driver": "name of the driver",
+                     "Uid" : "unique tag identifier",
+                     "Name" : "name of the tag",
+                     "Installation" : "name of the installation",
+                     "Driver" : "name of the driver",
                      "Attributes": [
                        {
                          "AttributeName":"name of the attribute",
                          "Value":"value of the attribute for this tag"
                        },
                        ...
                      ]
@@ -812,15 +838,15 @@
         if isinstance(tags, str):
             tags = [tags]
         body = json.dumps(tags)
         self._log_print(f'Tags to be created: {body}')
         url_post = self.url_NX + "/api/Tags/Insert"
         return self._postResponse(url_post, body)
 
-    def write_tag_insert_or_update(self, tagname: str, **attributes) -> typing.List[dict]:
+    def write_tag_insert_or_update(self, tagname, **attributes) -> typing.List[dict]:
         """This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
         Args:
             tagname: name of the new tag
             **attributes: dictionary of attributes and their values
 
         Returns:
@@ -869,15 +895,15 @@
     def write_tags_historic_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> typing.List[dict]:
         """Update historical data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
-                    value: value of the tag
+                    value : value of the tag
                     timeStamp: timeStamp in unix
             skip_errors: True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response in json format
         """
         # la funcion mira cuantas variables diferentes contiene el dataframe y comprueba si todas ellas existen
@@ -915,15 +941,15 @@
     def write_tags_realtime_insert(self, df: pd.DataFrame, skip_errors: bool = True):
         """Update realtime data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
-                    value: value of the tag
+                    value : value of the tag
                     timeStamp (optional): timeStamp in unix. If not provided, will take current time
             skip_errors: True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response text (None if OK)
         """
         vbles = list(df.name.unique())
@@ -1007,15 +1033,15 @@
     def write_tags_transient_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> typing.List[dict]:
         """Update transient data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
-                    value: value of the tag
+                    value : value of the tag
                     timeStamp: timeStamp in unix
             skip_errors  = True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response in json format
         """
         # la funcion mira cuantas variables diferentes contiene el dataframe y comprueba si todas ellas existen
```

### Comparing `iotcore_api-1.1.41/iotcoreapi/nan_treatment.py` & `iotcore_api-1.1.5/iotcoreapi/nan_treatment.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.41/pyproject.toml` & `iotcore_api-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iotcore-api"
-version = "1.1.41"
+version = "1.1.5"
 description ="IoT core connection methods and utilities"
 readme = "README.md"
 packages = [
     {include = 'iotcoreapi/*.py'}
 ]
 authors = ["Idrica"]
 keywords = ["iotcoreapi", "goaigua"]
```

### Comparing `iotcore_api-1.1.41/README.md` & `iotcore_api-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -163,887 +163,887 @@
 tags = iot_api.catalogue_tags(include_attributes=True)
 ```
 
 See [Reference](#reference) for more information about covered endpoints.
 
 # Reference
 
-# Table of Contents
-
-* [iotcoreapi](#iotcoreapi)
-  * [IoTCoreAPI](#iotcoreapi.IoTCoreAPI)
-    * [\_\_init\_\_](#iotcoreapi.IoTCoreAPI.__init__)
-    * [catalogue\_tags](#iotcoreapi.IoTCoreAPI.catalogue_tags)
-    * [catalogue\_tags\_filtered](#iotcoreapi.IoTCoreAPI.catalogue_tags_filtered)
-    * [catalogue\_tags\_attributes](#iotcoreapi.IoTCoreAPI.catalogue_tags_attributes)
-    * [catalogue\_tags\_writable](#iotcoreapi.IoTCoreAPI.catalogue_tags_writable)
-    * [catalogue\_documents](#iotcoreapi.IoTCoreAPI.catalogue_documents)
-    * [catalogue\_tagview\_detail](#iotcoreapi.IoTCoreAPI.catalogue_tagview_detail)
-    * [catalogue\_alarms](#iotcoreapi.IoTCoreAPI.catalogue_alarms)
-    * [catalogue\_alarm\_groups](#iotcoreapi.IoTCoreAPI.catalogue_alarm_groups)
-    * [read\_tags\_realtime](#iotcoreapi.IoTCoreAPI.read_tags_realtime)
-    * [read\_tagview\_realtime](#iotcoreapi.IoTCoreAPI.read_tagview_realtime)
-    * [read\_tags\_historic](#iotcoreapi.IoTCoreAPI.read_tags_historic)
-    * [read\_tags\_rawhistoric](#iotcoreapi.IoTCoreAPI.read_tags_rawhistoric)
-    * [read\_tags\_transient](#iotcoreapi.IoTCoreAPI.read_tags_transient)
-    * [read\_tagview\_historic](#iotcoreapi.IoTCoreAPI.read_tagview_historic)
-    * [read\_tagview\_historic\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters)
-    * [read\_tagview\_realtime\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tagview_realtime_text_filters)
-    * [read\_tags\_historic\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tags_historic_text_filters)
-    * [read\_tags\_realtime\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters)
-    * [read\_alarm\_status](#iotcoreapi.IoTCoreAPI.read_alarm_status)
-    * [write\_tags\_insert](#iotcoreapi.IoTCoreAPI.write_tags_insert)
-    * [write\_tag\_insert\_or\_update](#iotcoreapi.IoTCoreAPI.write_tag_insert_or_update)
-    * [write\_tags\_insert\_or\_update\_by\_json](#iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json)
-    * [write\_tags\_historic\_insert](#iotcoreapi.IoTCoreAPI.write_tags_historic_insert)
-    * [write\_tags\_realtime\_insert](#iotcoreapi.IoTCoreAPI.write_tags_realtime_insert)
-    * [write\_tag\_realtime\_insert](#iotcoreapi.IoTCoreAPI.write_tag_realtime_insert)
-    * [write\_tags\_transient\_insert](#iotcoreapi.IoTCoreAPI.write_tags_transient_insert)
-    * [write\_alarm\_acknowledge](#iotcoreapi.IoTCoreAPI.write_alarm_acknowledge)
-    * [write\_alarm\_event](#iotcoreapi.IoTCoreAPI.write_alarm_event)
-    * [operate\_tags](#iotcoreapi.IoTCoreAPI.operate_tags)
-    * [operate\_tag\_single](#iotcoreapi.IoTCoreAPI.operate_tag_single)
-
-<a id="iotcoreapi"></a>
-
-# iotcoreapi
-
-iotcoreapi
-Class definition
-
-<a id="iotcoreapi.IoTCoreAPI"></a>
-
-## IoTCoreAPI Objects
-
-```python
-class IoTCoreAPI()
-```
-
-<a id="iotcoreapi.IoTCoreAPI.__init__"></a>
-
-#### \_\_init\_\_
-
-```python
-def __init__(ip: str = "localhost",
-             port: int = 56000,
-             token: str = "",
-             version: str = "3.0",
-             logger: logging.Logger = None)
-```
-
-Init method for iotcoreapi. Needs API configuration parameters
-
-**Arguments**:
-
-- `ip` - IoT Core base endpoint
-- `port` - API Port. Defaults to 56000
-- `token` - API token
-- `version` - 1.0, 2.0 or 3.0. Defaults to 3.0
-- `logger` - Optional. Logger object to output log messages. If not provided, logger messages will be printed to console
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_tags"></a>
-
-#### catalogue\_tags
-
-```python
-def catalogue_tags(
-        include_attributes: bool = True,
-        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
-```
-
-Return all tags available for the token
-
-**Arguments**:
-
-- `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
-
-#### catalogue\_tags\_filtered
-
-```python
-def catalogue_tags_filtered(
-        installations: typing.Union[list, str] = None,
-        drivers: typing.Union[list, str] = None,
-        tags: typing.Union[list, str] = None,
-        attributes: typing.Union[list, str] = None,
-        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
-```
-
-Searching for tags that comply with a certain criteria can be achieved with the filtered route. If fields are empty, all tags are returned.
-
-**Arguments**:
-
-- `installations` - name of the installations
-- `drivers` - name of drivers
-- `tags` - name of tags
-- `attributes` - not implemented yet
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
-
-#### catalogue\_tags\_attributes
-
-```python
-def catalogue_tags_attributes(
-        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
-```
-
-Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
-
-**Arguments**:
-
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
-
-#### catalogue\_tags\_writable
-
-```python
-def catalogue_tags_writable(
-        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
-```
-
-Return tags available for writing. If version is under 3.0, returned array does not have attribute information
-
-**Arguments**:
-
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_documents"></a>
-
-#### catalogue\_documents
-
-```python
-def catalogue_documents(
-        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
-```
-
-Returns all tagviews shared in the token
-
-**Arguments**:
-
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
-
-#### catalogue\_tagview\_detail
-
-```python
-def catalogue_tagview_detail(
-        uid: str,
-        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
-```
-
-Return all variables from a given tagview
-
-**Arguments**:
-
-- `uid` - uid of the tagview
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
-
-#### catalogue\_alarms
-
-```python
-def catalogue_alarms(
-    group_uid: str = None,
-    output_format: str = 'dataframe'
-) -> typing.Union[typing.List[dict], pd.DataFrame]
-```
-
-Returns information of the alarms in the token
-
-**Arguments**:
-
-- `group_uid` - Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
-
-#### catalogue\_alarm\_groups
-
-```python
-def catalogue_alarm_groups(
-    output_format: str = 'dataframe'
-) -> typing.Union[typing.List[dict], pd.DataFrame]
-```
-
-Returns information of the alarm groups in the token
-
-**Arguments**:
-
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-
-
-**Returns**:
-
-  response in json
-
-<a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
-
-#### read\_tags\_realtime
-
-```python
-def read_tags_realtime(
-        tags_uids: typing.List[str],
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Reads real time value of the tags provided in the array tags_uids
-
-**Arguments**:
-
-- `tags_uids` - list with uids of the tags
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime"></a>
-
-#### read\_tagview\_realtime
-
-```python
-def read_tagview_realtime(
-        uid: str,
-        uids_tags: typing.List[str] = None,
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Returns real time value for the uids variables provided in a given tagview
-
-**Arguments**:
-
-- `uid` - uid of the tagview
-- `uids_tags` - list of uids
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.read_tags_historic"></a>
-
-#### read\_tags\_historic
-
-```python
-def read_tags_historic(
-        uids: typing.List[str],
-        start_ts: typing.Union[int, float],
-        end_ts: typing.Union[int, float],
-        data_source: typing.Union[str, int] = 'RAW',
-        resolution: typing.Union[str, int] = 'RES_1_HOUR',
-        agg_operation: typing.Union[str, int] = "LAST_VALUE",
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Obtain historic data of the specified tags
-
-**Arguments**:
-
-- `uids` - list of unique identifiers of the tags whose values must be obtained.
-- `start_ts` - start time in unix time or datetime
-- `end_ts` - end time in unix time or datetime
-- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
-- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-- `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.read_tags_rawhistoric"></a>
-
-#### read\_tags\_rawhistoric
-
-```python
-def read_tags_rawhistoric(
-        uids,
-        start_ts,
-        end_ts,
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-To obtain raw data with no aggregation or normalization applied
-
-**Arguments**:
-
-- `uids` - list of unique identifiers of the tags whose values must be obtained.
-- `start_ts` - start time in unix time or datetime
-- `end_ts` - end time in unix time or datetime
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.read_tags_transient"></a>
-
-#### read\_tags\_transient
-
-```python
-def read_tags_transient(
-        uids: typing.List[str],
-        start_ts: typing.Union[int, float],
-        end_ts: typing.Union[int, float],
-        data_source: typing.Union[str, int] = None,
-        resolution: typing.Union[str, int] = 'RES_1_SEC',
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
-aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
-please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
-for historic.
-
-**Arguments**:
-
-- `uids` - list of unique identifiers of the tags whose values must be obtained. start_ts:
-- `start_ts` - time in unix time or datetime
-- `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
-- `data_source` - Can be set to null or empty. Not needed
-- `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  response in json or dataframe
-
-<a id="iotcoreapi.IoTCoreAPI.read_tagview_historic"></a>
-
-#### read\_tagview\_historic
-
-```python
-def read_tagview_historic(
-        uid: str,
-        start_ts: typing.Union[datetime.datetime, float, int],
-        end_ts: typing.Union[datetime.datetime, float, int],
-        tags_uids: typing.List[str] = None,
-        data_source='RAW',
-        resolution='RES_1_HOUR',
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
-
-**Arguments**:
-
-- `uid` - uid of the tagview
-- `start_ts` - start time in unix or datetime
-- `end_ts` - end time in unix or datetime
-- `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
-- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
-- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
-
-<a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
-
-#### read\_tagview\_historic\_text\_filters
-
-```python
-def read_tagview_historic_text_filters(uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int], end_ts: typing.Union[datetime.datetime, float, int], filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW', resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe', time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, \
-                                                                                                     typing.List[dict]]
-```
-
-Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
-
-**Arguments**:
-
-- `uid_tagview` - uid of the tagview
-- `start_ts` - start time in unix or datetime
-- `end_ts` - end time in unix or datetime
-- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
-- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  filtered_hist (dataframe):
-  columns:
-- `name` - name of tag
-- `value` - value of tag
-- `timeStamp` - timeStamp in datatetime or unix time
-
-<a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime_text_filters"></a>
-
-#### read\_tagview\_realtime\_text\_filters
-
-```python
-def read_tagview_realtime_text_filters(
-        uid_tagview: str,
-        filter_txt: typing.Union[str, typing.List[str]] = None,
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
-
-**Arguments**:
-
-- `uid_tagview` - uid of the tagview
-- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  filtered_hist (dataframe):
-  columns:
-- `name` - name of tag
-- `value` - value of tag
-- `timeStamp` - timeStamp in datatetime or unix time
-
-<a id="iotcoreapi.IoTCoreAPI.read_tags_historic_text_filters"></a>
-
-#### read\_tags\_historic\_text\_filters
-
-```python
-def read_tags_historic_text_filters(
-        uids: typing.List[str],
-        start_ts: typing.Union[datetime.datetime, int, float],
-        end_ts: typing.Union[datetime.datetime, int, float],
-        filter_txt: typing.Union[str, typing.List[str]] = None,
-        data_source: typing.Union[str, int] = 'RAW',
-        resolution: typing.Union[str, int] = 'RES_1_HOUR',
-        agg_operation: typing.Union[str, int] = "LAST_VALUE",
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Obtain historic data of the specified tags by name
-
-**Arguments**:
-
-- `uids` - list of unique identifiers of the tags whose values must be obtained.
-- `start_ts` - start time in unix or datetime
-- `end_ts` - end time in unix or datetime
-- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
-- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-- `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  response in json
-
-<a id="iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters"></a>
-
-#### read\_tags\_realtime\_text\_filters
-
-```python
-def read_tags_realtime_text_filters(
-        filter_txt: typing.Union[str, typing.List[str]] = None,
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None
-) -> typing.Union[pd.DataFrame, typing.List[dict]]
-```
-
-Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
-
-**Arguments**:
-
-- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
-- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-
-
-**Returns**:
-
-  dataframe or json:
-  columns:
-- `name` - name of tag
-- `value` - value of tag
-- `timeStamp` - timeStamp in datatetime or unix time
-
-<a id="iotcoreapi.IoTCoreAPI.read_alarm_status"></a>
-
-#### read\_alarm\_status
-
-```python
-def read_alarm_status(alarm_guid: str) -> dict
-```
-
-Reads alarm status for a given alarm
-
-**Arguments**:
-
-- `alarm_guid` - guid of the alarm
-
-
-**Returns**:
-
-  Dictionary with following data:
-  {
-- `"name"` - "BasicAlarm1",
-- `"uid"` - "b926bfb0-3f2f-49df-a2eb-138452296903",
-- `"status"` - "ARE",
-- `"alarmAREDate"` - "2022-07-12T12:55:28.9274145+02:00",
-- `"alarmLastUpdate"` - "2022-07-12T09:58:39.3102729+02:00",
-- `"alarmCurrentValue"` - true,
-- `"resultTimestampActivation"` - "2022-07-12T09:58:42.3931339+02:00",
-- `"resultTimestampDeactivation"` - "2022-07-12T09:55:34.6931883+02:00",
-- `"lastNotificationTS"` - "1900-01-01T00:00:00",
-- `"signalValue"` - 95.84623491198114,
-- `"dataComparisonType"` - ">",
-- `"dataComparisonValue"` - 0,
-- `"signalValueOnLastHisteresis"` - 80.27092576039533,
-- `"lastEvent"` - "New Event: Alarm supervised by the API"
-  }
-
-<a id="iotcoreapi.IoTCoreAPI.write_tags_insert"></a>
-
-#### write\_tags\_insert
-
-```python
-def write_tags_insert(
-        tags: typing.Union[str, typing.List[str]]) -> typing.List[dict]
-```
-
-Check if provided tag names exist, then create them if not
-
-**Arguments**:
-
-- `tags` - tags name or names to be created
-
-
-**Returns**:
-
-  response object in json format:
-  [
-  {
-- `"Uid"` - "unique tag identifier",
-- `"Name"` - "name of the tag",
-- `"Installation"` - "name of the installation",
-- `"Driver"` - "name of the driver",
-- `"Attributes"` - [
-  {
-  "AttributeName":"name of the attribute",
-  "Value":"value of the attribute for this tag"
-  },
-  ...
-  ]
-  },
-  ...
-  ]
-
-<a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
-
-#### write\_tag\_insert\_or\_update
-
-```python
-def write_tag_insert_or_update(tagname: str,
-                               **attributes) -> typing.List[dict]
-```
-
-This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
-
-**Arguments**:
-
-- `tagname` - name of the new tag
-- `**attributes` - dictionary of attributes and their values
-
-
-**Returns**:
-
-  response in json format
-
-
-**Examples**:
-
-  Call the function with a tag name and any number of attributes
-  response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
-
-<a id="iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json"></a>
-
-#### write\_tags\_insert\_or\_update\_by\_json
-
-```python
-def write_tags_insert_or_update_by_json(
-        tags_and_attributes: typing.List[dict])
-```
-
-This method creates the tags with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
-
-**Arguments**:
-
-- `tags_and_attributes` - json list containing info for each tag:
-  [
-  {
-- `"Name"` - "name of the new tag",
-  "Attributes":
-  [
-  {
-- `"AttributeName"` - "NameOfAttribute1",
-- `"Value"` - "ValueOfAttribute1"
-  }
-  ]
-  }
-  ],
-  ...
-
-
-**Returns**:
-
-  response in json format
-
-<a id="iotcoreapi.IoTCoreAPI.write_tags_historic_insert"></a>
-
-#### write\_tags\_historic\_insert
-
-```python
-@_no_row_limit_decorator
-def write_tags_historic_insert(df: pd.DataFrame,
-                               skip_errors: bool = True) -> typing.List[dict]
-```
-
-Update historical data for tags. Tags need to be created with write_tags_insert first.
-
-**Arguments**:
-
-- `df` - dataframe
-  columns:
-- `name` - name of the tag
-- `value` - value of the tag
-- `timeStamp` - timeStamp in unix
-- `skip_errors` - True: If true, not created tags will be dropped from dataframe
-
-
-**Returns**:
-
-  response in json format
-
-<a id="iotcoreapi.IoTCoreAPI.write_tags_realtime_insert"></a>
-
-#### write\_tags\_realtime\_insert
-
-```python
-@_no_row_limit_decorator
-def write_tags_realtime_insert(df: pd.DataFrame, skip_errors: bool = True)
-```
-
-Update realtime data for tags. Tags need to be created with write_tags_insert first.
-
-**Arguments**:
-
-- `df` - dataframe
-  columns:
-- `name` - name of the tag
-- `value` - value of the tag
-- `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
-- `skip_errors` - True: If true, not created tags will be dropped from dataframe
-
-
-**Returns**:
-
-  response text (None if OK)
-
-<a id="iotcoreapi.IoTCoreAPI.write_tag_realtime_insert"></a>
-
-#### write\_tag\_realtime\_insert
-
-```python
-def write_tag_realtime_insert(name: str,
-                              value: typing.Union[float, int],
-                              timeStamp=None)
-```
-
-Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
-
-**Arguments**:
-
-- `name` - tag name
-- `value` - value of the tag
-- `timeStamp` _optional_ - time in unix time. If None, will take current time
-
-
-**Returns**:
-
-  response text (None if OK)
-
-<a id="iotcoreapi.IoTCoreAPI.write_tags_transient_insert"></a>
-
-#### write\_tags\_transient\_insert
-
-```python
-@_no_row_limit_decorator
-def write_tags_transient_insert(df: pd.DataFrame,
-                                skip_errors: bool = True) -> typing.List[dict]
-```
-
-Update transient data for tags. Tags need to be created with write_tags_insert first.
-
-**Arguments**:
-
-- `df` - dataframe
-  columns:
-- `name` - name of the tag
-- `value` - value of the tag
-- `timeStamp` - timeStamp in unix
-  skip_errors  = True: If true, not created tags will be dropped from dataframe
-
-
-**Returns**:
-
-  response in json format
-
-<a id="iotcoreapi.IoTCoreAPI.write_alarm_acknowledge"></a>
-
-#### write\_alarm\_acknowledge
-
-```python
-def write_alarm_acknowledge(guid: str, status: str) -> str
-```
-
-Used to change the status of an alarm from ANR or ENR to ARE o EXR.
-
-**Arguments**:
-
-- `guid` - guid of the alarm
-- `status` - 'ARE' or 'EXR', 'ANR' or 'ENR'
-
-
-**Returns**:
-
-  response text (None if OK)
-
-<a id="iotcoreapi.IoTCoreAPI.write_alarm_event"></a>
-
-#### write\_alarm\_event
-
-```python
-def write_alarm_event(guid: str, msg: str) -> str
-```
-
-Used to insert an event with a message in the history of the alarm. The alarma must be active and enabled.
-
-**Arguments**:
-
-- `guid` - guid of the alarm
-- `msg` - text of the message
-
-<a id="iotcoreapi.IoTCoreAPI.operate_tags"></a>
-
-#### operate\_tags
-
-```python
-def operate_tags(df: pd.DataFrame)
-```
-
-If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
-
-**Arguments**:
-
-- `df` - dataframe
-  columns:
-- `uid` - tag uid
-- `value` - value to write
-
-<a id="iotcoreapi.IoTCoreAPI.operate_tag_single"></a>
-
-#### operate\_tag\_single
-
-```python
-def operate_tag_single(tag_uid: str, value: typing.Union[int, float])
-```
-
-If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
-
-**Arguments**:
-
-- `tag_uid` - nombre de la variable a escribir en el PLC
-- `value` - valor de la variable a escribir
+# Table of Contents
+
+* [iotcoreapi](#iotcoreapi)
+  * [IoTCoreAPI](#iotcoreapi.IoTCoreAPI)
+    * [\_\_init\_\_](#iotcoreapi.IoTCoreAPI.__init__)
+    * [catalogue\_tags](#iotcoreapi.IoTCoreAPI.catalogue_tags)
+    * [catalogue\_tags\_filtered](#iotcoreapi.IoTCoreAPI.catalogue_tags_filtered)
+    * [catalogue\_tags\_attributes](#iotcoreapi.IoTCoreAPI.catalogue_tags_attributes)
+    * [catalogue\_tags\_writable](#iotcoreapi.IoTCoreAPI.catalogue_tags_writable)
+    * [catalogue\_documents](#iotcoreapi.IoTCoreAPI.catalogue_documents)
+    * [catalogue\_tagview\_detail](#iotcoreapi.IoTCoreAPI.catalogue_tagview_detail)
+    * [catalogue\_alarms](#iotcoreapi.IoTCoreAPI.catalogue_alarms)
+    * [catalogue\_alarm\_groups](#iotcoreapi.IoTCoreAPI.catalogue_alarm_groups)
+    * [read\_tags\_realtime](#iotcoreapi.IoTCoreAPI.read_tags_realtime)
+    * [read\_tagview\_realtime](#iotcoreapi.IoTCoreAPI.read_tagview_realtime)
+    * [read\_tags\_historic](#iotcoreapi.IoTCoreAPI.read_tags_historic)
+    * [read\_tags\_rawhistoric](#iotcoreapi.IoTCoreAPI.read_tags_rawhistoric)
+    * [read\_tags\_transient](#iotcoreapi.IoTCoreAPI.read_tags_transient)
+    * [read\_tagview\_historic](#iotcoreapi.IoTCoreAPI.read_tagview_historic)
+    * [read\_tagview\_historic\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters)
+    * [read\_tagview\_realtime\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tagview_realtime_text_filters)
+    * [read\_tags\_historic\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tags_historic_text_filters)
+    * [read\_tags\_realtime\_text\_filters](#iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters)
+    * [read\_alarm\_status](#iotcoreapi.IoTCoreAPI.read_alarm_status)
+    * [write\_tags\_insert](#iotcoreapi.IoTCoreAPI.write_tags_insert)
+    * [write\_tag\_insert\_or\_update](#iotcoreapi.IoTCoreAPI.write_tag_insert_or_update)
+    * [write\_tags\_insert\_or\_update\_by\_json](#iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json)
+    * [write\_tags\_historic\_insert](#iotcoreapi.IoTCoreAPI.write_tags_historic_insert)
+    * [write\_tags\_realtime\_insert](#iotcoreapi.IoTCoreAPI.write_tags_realtime_insert)
+    * [write\_tag\_realtime\_insert](#iotcoreapi.IoTCoreAPI.write_tag_realtime_insert)
+    * [write\_tags\_transient\_insert](#iotcoreapi.IoTCoreAPI.write_tags_transient_insert)
+    * [write\_alarm\_acknowledge](#iotcoreapi.IoTCoreAPI.write_alarm_acknowledge)
+    * [write\_alarm\_event](#iotcoreapi.IoTCoreAPI.write_alarm_event)
+    * [operate\_tags](#iotcoreapi.IoTCoreAPI.operate_tags)
+    * [operate\_tag\_single](#iotcoreapi.IoTCoreAPI.operate_tag_single)
+
+<a id="iotcoreapi"></a>
+
+# iotcoreapi
+
+iotcoreapi
+Class definition
+
+<a id="iotcoreapi.IoTCoreAPI"></a>
+
+## IoTCoreAPI Objects
+
+```python
+class IoTCoreAPI()
+```
+
+<a id="iotcoreapi.IoTCoreAPI.__init__"></a>
+
+#### \_\_init\_\_
+
+```python
+def __init__(ip: str = "localhost",
+             port: int = 56000,
+             token: str = "",
+             version: typing.Union[str, int] = "3.0",
+             logger: logging.Logger = None)
+```
+
+Init method for iotcoreapi. Needs API configuration parameters
+
+**Arguments**:
+
+- `ip` - IoT Core base endpoint
+- `port` - API Port. Defaults to 56000
+- `token` - API token
+- `version` - 1.0, 2.0 or 3.0. Defaults to 3.0
+- `logger` - Optional. Logger object to output log messages. If not provided, logger messages will be printed to console
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_tags"></a>
+
+#### catalogue\_tags
+
+```python
+def catalogue_tags(
+        include_attributes: bool = True,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
+```
+
+Return all tags available for the token
+
+**Arguments**:
+
+- `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
+- `output_format` - Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
+
+#### catalogue\_tags\_filtered
+
+```python
+def catalogue_tags_filtered(
+        installations: typing.Union[list, str] = None,
+        drivers: typing.Union[list, str] = None,
+        tags: typing.Union[list, str] = None,
+        attributes: typing.Union[list, str] = None,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
+```
+
+Searching for tags that comply with a certain criteria can be achieved with the filtered route. If fields are empty, all tags are returned.
+
+**Arguments**:
+
+- `installations` - name of the installations
+- `drivers` - name of drivers
+- `tags` - name of tags
+- `attributes` - not implemented yet
+- `output_format` - Result given in 'dataframe' or 'json' or 'dataframe_table'. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
+
+#### catalogue\_tags\_attributes
+
+```python
+def catalogue_tags_attributes(
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
+```
+
+Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
+
+**Arguments**:
+
+- `output_format` - Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
+
+#### catalogue\_tags\_writable
+
+```python
+def catalogue_tags_writable(
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
+```
+
+Return tags available for writing. If version is under 3.0, returned array does not have attribute information
+
+**Arguments**:
+
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_documents"></a>
+
+#### catalogue\_documents
+
+```python
+def catalogue_documents(
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
+```
+
+Returns all tagviews shared in the token
+
+**Arguments**:
+
+- `output_format` - Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
+
+#### catalogue\_tagview\_detail
+
+```python
+def catalogue_tagview_detail(
+        uid: str,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
+```
+
+Return all variables from a given tagview
+
+**Arguments**:
+
+- `uid` - uid of the tagview
+- `output_format` - Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
+
+#### catalogue\_alarms
+
+```python
+def catalogue_alarms(
+    group_uid: str = None,
+    output_format: str = 'dataframe'
+) -> typing.Union[typing.List[dict], pd.DataFrame]
+```
+
+Returns information of the alarms in the token
+
+**Arguments**:
+
+  group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
+
+#### catalogue\_alarm\_groups
+
+```python
+def catalogue_alarm_groups(
+    output_format: str = 'dataframe'
+) -> typing.Union[typing.List[dict], pd.DataFrame]
+```
+
+Returns information of the alarm groups in the token
+
+**Arguments**:
+
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+
+
+**Returns**:
+
+  response in json
+
+<a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
+
+#### read\_tags\_realtime
+
+```python
+def read_tags_realtime(
+        tags_uids: typing.List[str],
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Reads real time value of the tags provided in the array tags_uids
+
+**Arguments**:
+
+  tags_uids : list with uids of the tags
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime"></a>
+
+#### read\_tagview\_realtime
+
+```python
+def read_tagview_realtime(
+        uid: str,
+        uids_tags: typing.List[str] = None,
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Returns real time value for the uids variables provided in a given tagview
+
+**Arguments**:
+
+  uid : uid of the tagview
+  uids_tags : list of uids
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.read_tags_historic"></a>
+
+#### read\_tags\_historic
+
+```python
+def read_tags_historic(
+        uids: typing.List[str],
+        start_ts: typing.Union[int, float],
+        end_ts: typing.Union[int, float],
+        data_source: typing.Union[str, int] = 'RAW',
+        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+        agg_operation: typing.Union[str, int] = "LAST_VALUE",
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Obtain historic data of the specified tags
+
+**Arguments**:
+
+- `uids` - list of unique identifiers of the tags whose values must be obtained.
+- `start_ts` - start time in unix time or datetime
+- `end_ts` - end time in unix time or datetime
+- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
+- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
+- `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.read_tags_rawhistoric"></a>
+
+#### read\_tags\_rawhistoric
+
+```python
+def read_tags_rawhistoric(
+        uids,
+        start_ts,
+        end_ts,
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+To obtain raw data with no aggregation or normalization applied
+
+**Arguments**:
+
+- `uids` - list of unique identifiers of the tags whose values must be obtained.
+- `start_ts` - start time in unix time or datetime
+- `end_ts` - end time in unix time or datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.read_tags_transient"></a>
+
+#### read\_tags\_transient
+
+```python
+def read_tags_transient(
+        uids: typing.List[str],
+        start_ts: typing.Union[int, float],
+        end_ts: typing.Union[int, float],
+        data_source: typing.Union[str, int] = None,
+        resolution: typing.Union[str, int] = 'RES_1_SEC',
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
+aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
+please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
+for historic.
+
+**Arguments**:
+
+- `uids` - list of unique identifiers of the tags whose values must be obtained. start_ts:
+- `start_ts` - time in unix time or datetime
+- `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
+- `data_source` - Can be set to null or empty. Not needed
+- `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  response in json or dataframe
+
+<a id="iotcoreapi.IoTCoreAPI.read_tagview_historic"></a>
+
+#### read\_tagview\_historic
+
+```python
+def read_tagview_historic(
+        uid: str,
+        start_ts: typing.Union[datetime.datetime, float, int],
+        end_ts: typing.Union[datetime.datetime, float, int],
+        tags_uids: typing.List[str] = None,
+        data_source='RAW',
+        resolution='RES_1_HOUR',
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
+
+**Arguments**:
+
+- `uid` - uid of the tagview
+- `start_ts` - start time in unix or datetime
+- `end_ts` - end time in unix or datetime
+- `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
+- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
+- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
+
+<a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
+
+#### read\_tagview\_historic\_text\_filters
+
+```python
+def read_tagview_historic_text_filters(uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int], end_ts: typing.Union[datetime.datetime, float, int], filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW', resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe', time_format: str = 'datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, \
+                typing.List[dict]]
+```
+
+Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
+
+**Arguments**:
+
+- `uid_tagview` - uid of the tagview
+- `start_ts` - start time in unix or datetime
+- `end_ts` - end time in unix or datetime
+- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
+- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
+- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  filtered_hist (dataframe):
+  columns:
+- `name` - name of tag
+- `value` - value of tag
+- `timeStamp` - timeStamp in datatetime or unix time
+
+<a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime_text_filters"></a>
+
+#### read\_tagview\_realtime\_text\_filters
+
+```python
+def read_tagview_realtime_text_filters(
+        uid_tagview: str,
+        filter_txt: typing.Union[str, typing.List[str]] = None,
+        output_format: str = 'dataframe',
+        time_format: str = 'datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
+
+**Arguments**:
+
+- `uid_tagview` - uid of the tagview
+- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  filtered_hist (dataframe):
+  columns:
+- `name` - name of tag
+- `value` - value of tag
+- `timeStamp` - timeStamp in datatetime or unix time
+
+<a id="iotcoreapi.IoTCoreAPI.read_tags_historic_text_filters"></a>
+
+#### read\_tags\_historic\_text\_filters
+
+```python
+def read_tags_historic_text_filters(
+        uids: typing.List[str],
+        start_ts: typing.Union[datetime.datetime, int, float],
+        end_ts: typing.Union[datetime.datetime, int, float],
+        filter_txt: typing.Union[str, typing.List[str]] = None,
+        data_source: typing.Union[str, int] = 'RAW',
+        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+        agg_operation: typing.Union[str, int] = "LAST_VALUE",
+        output_format: str = 'dataframe',
+        time_format: str = 'datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Obtain historic data of the specified tags by name
+
+**Arguments**:
+
+- `uids` - list of unique identifiers of the tags whose values must be obtained.
+- `start_ts` - start time in unix or datetime
+- `end_ts` - end time in unix or datetime
+- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
+- `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
+- `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
+- `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  response in json
+
+<a id="iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters"></a>
+
+#### read\_tags\_realtime\_text\_filters
+
+```python
+def read_tags_realtime_text_filters(
+        filter_txt: typing.Union[str, typing.List[str]] = None,
+        output_format: str = 'dataframe',
+        time_format: str = 'datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
+```
+
+Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
+
+**Arguments**:
+
+- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+
+**Returns**:
+
+  dataframe or json:
+  columns:
+- `name` - name of tag
+- `value` - value of tag
+- `timeStamp` - timeStamp in datatetime or unix time
+
+<a id="iotcoreapi.IoTCoreAPI.read_alarm_status"></a>
+
+#### read\_alarm\_status
+
+```python
+def read_alarm_status(alarm_guid: str) -> dict
+```
+
+Reads alarm status for a given alarm
+
+**Arguments**:
+
+  alarm_guid : guid of the alarm
+
+
+**Returns**:
+
+  Dictionary with following data:
+  {
+- `"name"` - "BasicAlarm1",
+- `"uid"` - "b926bfb0-3f2f-49df-a2eb-138452296903",
+- `"status"` - "ARE",
+- `"alarmAREDate"` - "2022-07-12T12:55:28.9274145+02:00",
+- `"alarmLastUpdate"` - "2022-07-12T09:58:39.3102729+02:00",
+- `"alarmCurrentValue"` - true,
+- `"resultTimestampActivation"` - "2022-07-12T09:58:42.3931339+02:00",
+- `"resultTimestampDeactivation"` - "2022-07-12T09:55:34.6931883+02:00",
+- `"lastNotificationTS"` - "1900-01-01T00:00:00",
+- `"signalValue"` - 95.84623491198114,
+- `"dataComparisonType"` - ">",
+- `"dataComparisonValue"` - 0,
+- `"signalValueOnLastHisteresis"` - 80.27092576039533,
+- `"lastEvent"` - "New Event: Alarm supervised by the API"
+  }
+
+<a id="iotcoreapi.IoTCoreAPI.write_tags_insert"></a>
+
+#### write\_tags\_insert
+
+```python
+def write_tags_insert(
+        tags: typing.Union[str, typing.List[str]]) -> typing.List[dict]
+```
+
+Check if provided tag names exist, then create them if not
+
+**Arguments**:
+
+- `tags` - tags name or names to be created
+
+
+**Returns**:
+
+  response object in json format:
+  [
+  {
+  "Uid" : "unique tag identifier",
+  "Name" : "name of the tag",
+  "Installation" : "name of the installation",
+  "Driver" : "name of the driver",
+- `"Attributes"` - [
+  {
+  "AttributeName":"name of the attribute",
+  "Value":"value of the attribute for this tag"
+  },
+  ...
+  ]
+  },
+  ...
+  ]
+
+<a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
+
+#### write\_tag\_insert\_or\_update
+
+```python
+def write_tag_insert_or_update(tagname, **attributes) -> typing.List[dict]
+```
+
+This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
+
+**Arguments**:
+
+- `tagname` - name of the new tag
+- `**attributes` - dictionary of attributes and their values
+
+
+**Returns**:
+
+  response in json format
+
+
+**Examples**:
+
+  Call the function with a tag name and any number of attributes
+  response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
+
+<a id="iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json"></a>
+
+#### write\_tags\_insert\_or\_update\_by\_json
+
+```python
+def write_tags_insert_or_update_by_json(
+        tags_and_attributes: typing.List[dict])
+```
+
+This method creates the tags with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
+
+**Arguments**:
+
+- `tags_and_attributes` - json list containing info for each tag:
+  [
+  {
+- `"Name"` - "name of the new tag",
+  "Attributes":
+  [
+  {
+- `"AttributeName"` - "NameOfAttribute1",
+- `"Value"` - "ValueOfAttribute1"
+  }
+  ]
+  }
+  ],
+  ...
+
+
+**Returns**:
+
+  response in json format
+
+<a id="iotcoreapi.IoTCoreAPI.write_tags_historic_insert"></a>
+
+#### write\_tags\_historic\_insert
+
+```python
+@_no_row_limit_decorator
+def write_tags_historic_insert(df: pd.DataFrame,
+                               skip_errors: bool = True) -> typing.List[dict]
+```
+
+Update historical data for tags. Tags need to be created with write_tags_insert first.
+
+**Arguments**:
+
+- `df` - dataframe
+  columns:
+- `name` - name of the tag
+  value : value of the tag
+- `timeStamp` - timeStamp in unix
+- `skip_errors` - True: If true, not created tags will be dropped from dataframe
+
+
+**Returns**:
+
+  response in json format
+
+<a id="iotcoreapi.IoTCoreAPI.write_tags_realtime_insert"></a>
+
+#### write\_tags\_realtime\_insert
+
+```python
+@_no_row_limit_decorator
+def write_tags_realtime_insert(df: pd.DataFrame, skip_errors: bool = True)
+```
+
+Update realtime data for tags. Tags need to be created with write_tags_insert first.
+
+**Arguments**:
+
+- `df` - dataframe
+  columns:
+- `name` - name of the tag
+  value : value of the tag
+- `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
+- `skip_errors` - True: If true, not created tags will be dropped from dataframe
+
+
+**Returns**:
+
+  response text (None if OK)
+
+<a id="iotcoreapi.IoTCoreAPI.write_tag_realtime_insert"></a>
+
+#### write\_tag\_realtime\_insert
+
+```python
+def write_tag_realtime_insert(name: str,
+                              value: typing.Union[float, int],
+                              timeStamp=None)
+```
+
+Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
+
+**Arguments**:
+
+- `name` - tag name
+- `value` - value of the tag
+- `timeStamp` _optional_ - time in unix time. If None, will take current time
+
+
+**Returns**:
+
+  response text (None if OK)
+
+<a id="iotcoreapi.IoTCoreAPI.write_tags_transient_insert"></a>
+
+#### write\_tags\_transient\_insert
+
+```python
+@_no_row_limit_decorator
+def write_tags_transient_insert(df: pd.DataFrame,
+                                skip_errors: bool = True) -> typing.List[dict]
+```
+
+Update transient data for tags. Tags need to be created with write_tags_insert first.
+
+**Arguments**:
+
+- `df` - dataframe
+  columns:
+- `name` - name of the tag
+  value : value of the tag
+- `timeStamp` - timeStamp in unix
+  skip_errors  = True: If true, not created tags will be dropped from dataframe
+
+
+**Returns**:
+
+  response in json format
+
+<a id="iotcoreapi.IoTCoreAPI.write_alarm_acknowledge"></a>
+
+#### write\_alarm\_acknowledge
+
+```python
+def write_alarm_acknowledge(guid: str, status: str) -> str
+```
+
+Used to change the status of an alarm from ANR or ENR to ARE o EXR.
+
+**Arguments**:
+
+- `guid` - guid of the alarm
+- `status` - 'ARE' or 'EXR', 'ANR' or 'ENR'
+
+
+**Returns**:
+
+  response text (None if OK)
+
+<a id="iotcoreapi.IoTCoreAPI.write_alarm_event"></a>
+
+#### write\_alarm\_event
+
+```python
+def write_alarm_event(guid: str, msg: str) -> str
+```
+
+Used to insert an event with a message in the history of the alarm. The alarma must be active and enabled.
+
+**Arguments**:
+
+- `guid` - guid of the alarm
+- `msg` - text of the message
+
+<a id="iotcoreapi.IoTCoreAPI.operate_tags"></a>
+
+#### operate\_tags
+
+```python
+def operate_tags(df: pd.DataFrame)
+```
+
+If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
+
+**Arguments**:
+
+- `df` - dataframe
+  columns:
+- `uid` - tag uid
+- `value` - value to write
+
+<a id="iotcoreapi.IoTCoreAPI.operate_tag_single"></a>
+
+#### operate\_tag\_single
+
+```python
+def operate_tag_single(tag_uid: str, value: typing.Union[int, float])
+```
+
+If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
+
+**Arguments**:
+
+- `tag_uid` - nombre de la variable a escribir en el PLC
+- `value` - valor de la variable a escribir
```

### Comparing `iotcore_api-1.1.41/PKG-INFO` & `iotcore_api-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.1.41
+Version: 1.1.5
 Summary: IoT core connection methods and utilities
 Keywords: iotcoreapi,goaigua
 Author: Idrica
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -238,15 +238,15 @@
 
 #### \_\_init\_\_
 
 ```python
 def __init__(ip: str = "localhost",
              port: int = 56000,
              token: str = "",
-             version: str = "3.0",
+             version: typing.Union[str, int] = "3.0",
              logger: logging.Logger = None)
 ```
 
 Init method for iotcoreapi. Needs API configuration parameters
 
 **Arguments**:
 
@@ -267,15 +267,15 @@
 ```
 
 Return all tags available for the token
 
 **Arguments**:
 
 - `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
@@ -295,15 +295,15 @@
 
 **Arguments**:
 
 - `installations` - name of the installations
 - `drivers` - name of drivers
 - `tags` - name of tags
 - `attributes` - not implemented yet
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json' or 'dataframe_table'. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
@@ -315,15 +315,15 @@
         output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
 **Arguments**:
 
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
@@ -355,15 +355,15 @@
         output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Returns all tagviews shared in the token
 
 **Arguments**:
 
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
@@ -377,15 +377,15 @@
 ```
 
 Return all variables from a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
@@ -399,16 +399,16 @@
 ) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
-- `group_uid` - Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+  group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
@@ -421,41 +421,41 @@
 ) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
 
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
 
 #### read\_tags\_realtime
 
 ```python
 def read_tags_realtime(
         tags_uids: typing.List[str],
         output_format: str = 'dataframe',
-        time_format: str = 'datetime',
+        time_format='datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
-- `tags_uids` - list with uids of the tags
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+  tags_uids : list with uids of the tags
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   response in json or dataframe
 
@@ -464,27 +464,27 @@
 #### read\_tagview\_realtime
 
 ```python
 def read_tagview_realtime(
         uid: str,
         uids_tags: typing.List[str] = None,
         output_format: str = 'dataframe',
-        time_format: str = 'datetime',
+        time_format='datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
-- `uid` - uid of the tagview
-- `uids_tags` - list of uids
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+  uid : uid of the tagview
+  uids_tags : list of uids
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   response in json or dataframe
 
@@ -497,31 +497,31 @@
         uids: typing.List[str],
         start_ts: typing.Union[int, float],
         end_ts: typing.Union[int, float],
         data_source: typing.Union[str, int] = 'RAW',
         resolution: typing.Union[str, int] = 'RES_1_HOUR',
         agg_operation: typing.Union[str, int] = "LAST_VALUE",
         output_format: str = 'dataframe',
-        time_format: str = 'datetime',
+        time_format='datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json' or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   response in json or dataframe
 
@@ -531,28 +531,28 @@
 
 ```python
 def read_tags_rawhistoric(
         uids,
         start_ts,
         end_ts,
         output_format: str = 'dataframe',
-        time_format: str = 'datetime',
+        time_format='datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   response in json or dataframe
 
@@ -564,15 +564,15 @@
 def read_tags_transient(
         uids: typing.List[str],
         start_ts: typing.Union[int, float],
         end_ts: typing.Union[int, float],
         data_source: typing.Union[str, int] = None,
         resolution: typing.Union[str, int] = 'RES_1_SEC',
         output_format: str = 'dataframe',
-        time_format: str = 'datetime',
+        time_format='datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
 aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
 please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
@@ -581,16 +581,16 @@
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained. start_ts:
 - `start_ts` - time in unix time or datetime
 - `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
 - `data_source` - Can be set to null or empty. Not needed
 - `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   response in json or dataframe
 
@@ -603,59 +603,60 @@
         uid: str,
         start_ts: typing.Union[datetime.datetime, float, int],
         end_ts: typing.Union[datetime.datetime, float, int],
         tags_uids: typing.List[str] = None,
         data_source='RAW',
         resolution='RES_1_HOUR',
         output_format: str = 'dataframe',
-        time_format: str = 'datetime',
+        time_format='datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
 **Arguments**:
 
 - `uid` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
 
 #### read\_tagview\_historic\_text\_filters
 
 ```python
-def read_tagview_historic_text_filters(uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int], end_ts: typing.Union[datetime.datetime, float, int], filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW', resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe', time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, \
-                                                                                                     typing.List[dict]]
+def read_tagview_historic_text_filters(uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int], end_ts: typing.Union[datetime.datetime, float, int], filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW', resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe', time_format: str = 'datetime', nan_method: str = None) -> typing.Union[
+        pd.DataFrame, \
+                typing.List[dict]]
 ```
 
 Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
@@ -679,16 +680,16 @@
 
 Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
@@ -722,16 +723,16 @@
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   response in json
 
@@ -749,16 +750,16 @@
 ```
 
 Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
+  output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
+  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
 
 **Returns**:
 
   dataframe or json:
   columns:
@@ -774,15 +775,15 @@
 def read_alarm_status(alarm_guid: str) -> dict
 ```
 
 Reads alarm status for a given alarm
 
 **Arguments**:
 
-- `alarm_guid` - guid of the alarm
+  alarm_guid : guid of the alarm
 
 
 **Returns**:
 
   Dictionary with following data:
   {
 - `"name"` - "BasicAlarm1",
@@ -818,18 +819,18 @@
 
 
 **Returns**:
 
   response object in json format:
   [
   {
-- `"Uid"` - "unique tag identifier",
-- `"Name"` - "name of the tag",
-- `"Installation"` - "name of the installation",
-- `"Driver"` - "name of the driver",
+  "Uid" : "unique tag identifier",
+  "Name" : "name of the tag",
+  "Installation" : "name of the installation",
+  "Driver" : "name of the driver",
 - `"Attributes"` - [
   {
   "AttributeName":"name of the attribute",
   "Value":"value of the attribute for this tag"
   },
   ...
   ]
@@ -838,16 +839,15 @@
   ]
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
 
 #### write\_tag\_insert\_or\_update
 
 ```python
-def write_tag_insert_or_update(tagname: str,
-                               **attributes) -> typing.List[dict]
+def write_tag_insert_or_update(tagname, **attributes) -> typing.List[dict]
 ```
 
 This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tagname` - name of the new tag
@@ -910,15 +910,15 @@
 Update historical data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-- `value` - value of the tag
+  value : value of the tag
 - `timeStamp` - timeStamp in unix
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
 
 
 **Returns**:
 
   response in json format
@@ -935,15 +935,15 @@
 Update realtime data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-- `value` - value of the tag
+  value : value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
 
 
 **Returns**:
 
   response text (None if OK)
@@ -984,15 +984,15 @@
 Update transient data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-- `value` - value of the tag
+  value : value of the tag
 - `timeStamp` - timeStamp in unix
   skip_errors  = True: If true, not created tags will be dropped from dataframe
 
 
 **Returns**:
 
   response in json format
```

