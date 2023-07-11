# Comparing `tmp/aishield-0.1.4.tar.gz` & `tmp/aishield-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishield-0.1.4.tar", last modified: Thu Jun 15 13:54:43 2023, max compression
+gzip compressed data, was "aishield-0.1.5.tar", last modified: Mon Jul 10 11:27:35 2023, max compression
```

## Comparing `aishield-0.1.4.tar` & `aishield-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.755033 aishield-0.1.4/
--rw-rw-rw-   0        0        0     3541 2023-06-15 13:54:43.754056 aishield-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2866 2023-06-15 13:50:40.000000 aishield-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.555311 aishield-0.1.4/aishield/
--rw-rw-rw-   0        0        0     1780 2022-12-14 06:23:58.000000 aishield-0.1.4/aishield/__init__.py
--rw-rw-rw-   0        0        0    15410 2023-05-24 06:52:11.000000 aishield-0.1.4/aishield/aishield_api.py
--rw-rw-rw-   0        0        0     5070 2023-01-17 09:49:00.000000 aishield-0.1.4/aishield/configs.py
--rw-rw-rw-   0        0        0    12777 2023-03-29 12:12:00.000000 aishield-0.1.4/aishield/connection.py
--rw-rw-rw-   0        0        0     1463 2023-05-24 12:22:21.000000 aishield-0.1.4/aishield/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.636320 aishield-0.1.4/aishield/image_classification/
--rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.4/aishield/image_classification/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-03-29 13:26:08.000000 aishield-0.1.4/aishield/image_classification/base_ic.py
--rw-rw-rw-   0        0        0     1305 2023-03-29 13:27:06.000000 aishield-0.1.4/aishield/image_classification/evasion.py
--rw-rw-rw-   0        0        0     1988 2023-03-29 13:38:09.000000 aishield-0.1.4/aishield/image_classification/extraction.py
--rw-rw-rw-   0        0        0      720 2023-03-29 13:36:39.000000 aishield-0.1.4/aishield/image_classification/poision.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.670479 aishield-0.1.4/aishield/tabular_classification/
--rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.4/aishield/tabular_classification/__init__.py
--rw-rw-rw-   0        0        0     4344 2023-03-24 12:45:35.000000 aishield-0.1.4/aishield/tabular_classification/base_tc.py
--rw-rw-rw-   0        0        0      539 2023-03-24 12:45:52.000000 aishield-0.1.4/aishield/tabular_classification/evasion.py
--rw-rw-rw-   0        0        0     1195 2023-03-24 12:46:00.000000 aishield-0.1.4/aishield/tabular_classification/extraction.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.698818 aishield-0.1.4/aishield/timeseries_forecasting/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:03:16.000000 aishield-0.1.4/aishield/timeseries_forecasting/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-05-26 09:44:19.000000 aishield-0.1.4/aishield/timeseries_forecasting/base_tsf.py
--rw-rw-rw-   0        0        0     1198 2023-05-24 06:49:21.000000 aishield-0.1.4/aishield/timeseries_forecasting/extraction.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.733920 aishield-0.1.4/aishield/utils/
--rw-rw-rw-   0        0        0        0 2022-10-17 19:21:54.000000 aishield-0.1.4/aishield/utils/__init__.py
--rw-rw-rw-   0        0        0      816 2022-10-25 15:02:47.000000 aishield-0.1.4/aishield/utils/exceptions.py
--rw-rw-rw-   0        0        0      559 2022-11-29 05:18:14.000000 aishield-0.1.4/aishield/utils/logger.py
--rw-rw-rw-   0        0        0     3318 2023-01-13 09:56:26.000000 aishield-0.1.4/aishield/utils/util.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.572880 aishield-0.1.4/aishield.egg-info/
--rw-rw-rw-   0        0        0     3541 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2022-11-18 10:08:05.000000 aishield-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 13:54:43.756009 aishield-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1296 2023-05-26 10:54:48.000000 aishield-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.750151 aishield-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2022-10-23 18:04:29.000000 aishield-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0      931 2022-11-29 05:22:31.000000 aishield-0.1.4/tests/test_aishield_api.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.167168 aishield-0.1.5/
+-rw-rw-rw-   0        0        0     3850 2023-07-10 11:27:35.165208 aishield-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-07-07 05:37:06.000000 aishield-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:34.982476 aishield-0.1.5/aishield/
+-rw-rw-rw-   0        0        0     1780 2022-12-14 06:23:58.000000 aishield-0.1.5/aishield/__init__.py
+-rw-rw-rw-   0        0        0    18322 2023-07-10 11:24:06.000000 aishield-0.1.5/aishield/aishield_api.py
+-rw-rw-rw-   0        0        0     5909 2023-07-06 07:36:46.000000 aishield-0.1.5/aishield/configs.py
+-rw-rw-rw-   0        0        0    14240 2023-07-05 09:46:54.000000 aishield-0.1.5/aishield/connection.py
+-rw-rw-rw-   0        0        0     1506 2023-07-10 11:19:10.000000 aishield-0.1.5/aishield/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.037484 aishield-0.1.5/aishield/image_classification/
+-rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.5/aishield/image_classification/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-03-29 13:26:08.000000 aishield-0.1.5/aishield/image_classification/base_ic.py
+-rw-rw-rw-   0        0        0     1305 2023-03-29 13:27:06.000000 aishield-0.1.5/aishield/image_classification/evasion.py
+-rw-rw-rw-   0        0        0     1988 2023-03-29 13:38:09.000000 aishield-0.1.5/aishield/image_classification/extraction.py
+-rw-rw-rw-   0        0        0      720 2023-03-29 13:36:39.000000 aishield-0.1.5/aishield/image_classification/poision.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.059974 aishield-0.1.5/aishield/image_segmentation/
+-rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.5/aishield/image_segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2911 2023-06-30 10:55:04.000000 aishield-0.1.5/aishield/image_segmentation/base_is.py
+-rw-rw-rw-   0        0        0     1986 2023-06-30 10:54:18.000000 aishield-0.1.5/aishield/image_segmentation/extraction.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.091365 aishield-0.1.5/aishield/tabular_classification/
+-rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.5/aishield/tabular_classification/__init__.py
+-rw-rw-rw-   0        0        0     4344 2023-03-24 12:45:35.000000 aishield-0.1.5/aishield/tabular_classification/base_tc.py
+-rw-rw-rw-   0        0        0      539 2023-03-24 12:45:52.000000 aishield-0.1.5/aishield/tabular_classification/evasion.py
+-rw-rw-rw-   0        0        0     1195 2023-03-24 12:46:00.000000 aishield-0.1.5/aishield/tabular_classification/extraction.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.114863 aishield-0.1.5/aishield/timeseries_forecasting/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:03:16.000000 aishield-0.1.5/aishield/timeseries_forecasting/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-05-26 09:44:19.000000 aishield-0.1.5/aishield/timeseries_forecasting/base_tsf.py
+-rw-rw-rw-   0        0        0     1198 2023-05-24 06:49:21.000000 aishield-0.1.5/aishield/timeseries_forecasting/extraction.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.146018 aishield-0.1.5/aishield/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-17 19:21:54.000000 aishield-0.1.5/aishield/utils/__init__.py
+-rw-rw-rw-   0        0        0      816 2022-10-25 15:02:47.000000 aishield-0.1.5/aishield/utils/exceptions.py
+-rw-rw-rw-   0        0        0      559 2022-11-29 05:18:14.000000 aishield-0.1.5/aishield/utils/logger.py
+-rw-rw-rw-   0        0        0     3318 2023-01-13 09:56:26.000000 aishield-0.1.5/aishield/utils/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:34.999542 aishield-0.1.5/aishield.egg-info/
+-rw-rw-rw-   0        0        0     3850 2023-07-10 11:27:34.000000 aishield-0.1.5/aishield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-07-10 11:27:34.000000 aishield-0.1.5/aishield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 11:27:34.000000 aishield-0.1.5/aishield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 11:27:34.000000 aishield-0.1.5/aishield.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-10 11:27:34.000000 aishield-0.1.5/aishield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2022-11-18 10:08:05.000000 aishield-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 11:27:35.167168 aishield-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2023-07-06 09:03:00.000000 aishield-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:27:35.162079 aishield-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-23 18:04:29.000000 aishield-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      931 2022-11-29 05:22:31.000000 aishield-0.1.5/tests/test_aishield_api.py
```

### Comparing `aishield-0.1.4/PKG-INFO` & `aishield-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishield
-Version: 0.1.4
+Version: 0.1.5
 Summary: AIShield provides the Python convenience package to allow users to seamlessly integrate AIShield Vulnerability Assessment and Defense capabilities into their AI development workflows.
 Home-page: https://www.boschaishield.com/
 Author: Contact AIShield
 Author-email: aishield.contact@bosch.com
 License: Apache License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,19 @@
    
 ## More about AIShield
 
 - Website:  https://www.boschaishield.com/
 - Email:   <AIShield.Contact@bosch.com>
 
 ## Version History
+
+### 0.1.5
+- Added vulnerability analysis for image segmentation: model extraction attack
+- Updated to be compatible with latest AIShield API version. Also, now api_key is not required to be provided explicitly for analysis. It will be generated from org_id and policies are consumed accordingly. 
+
 ### 0.1.4
 - Added vulnerability analysis for time series forecasting: model extraction attack
 
 ### 0.1.3
 - Updated to be compatible with latest AIShield API version
 - Added vulnerability analysis for tabular classification: model evasion attack
```

### Comparing `aishield-0.1.4/README.md` & `aishield-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,19 @@
    
 ## More about AIShield
 
 - Website:  https://www.boschaishield.com/
 - Email:   <AIShield.Contact@bosch.com>
 
 ## Version History
+
+### 0.1.5
+- Added vulnerability analysis for image segmentation: model extraction attack
+- Updated to be compatible with latest AIShield API version. Also, now api_key is not required to be provided explicitly for analysis. It will be generated from org_id and policies are consumed accordingly. 
+
 ### 0.1.4
 - Added vulnerability analysis for time series forecasting: model extraction attack
 
 ### 0.1.3
 - Updated to be compatible with latest AIShield API version
 - Added vulnerability analysis for tabular classification: model evasion attack
```

### Comparing `aishield-0.1.4/aishield/__init__.py` & `aishield-0.1.5/aishield/__init__.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/aishield_api.py` & `aishield-0.1.5/aishield/aishield_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     poision as ic_poison
 )
 from aishield.tabular_classification import (
     extraction as tc_extraction,
     evasion as tc_evasion
 )
 from aishield.timeseries_forecasting import extraction as tsf_extraction
+from aishield.image_segmentation import extraction as is_extraction
 from aishield.utils.util import (
     uri_validator,
     get_all_keys_by_val
 )
 from aishield.utils.util import delete_keys_from_dict
 
 
@@ -77,52 +78,56 @@
             else:
                 raise NotImplementedError('Feature coming soon')
         elif task_type == Task.TIMESERIES_FORECAST:
             if analysis_type == Attack.EXTRACTION:
                 vul_config_obj = tsf_extraction.VulnConfig(defense_generate)
             else:
                 raise NotImplementedError('Feature coming soon')
-        elif task_type == Task.NLP:
-            raise NotImplementedError('Feature coming soon')
         elif task_type == Task.IMAGE_SEGMENTATION:
+            if analysis_type == Attack.EXTRACTION:
+                vul_config_obj = is_extraction.VulnConfig(defense_generate)
+            else:
+                raise NotImplementedError('Feature coming soon')
+        elif task_type == Task.NLP:
             raise NotImplementedError('Feature coming soon')
         else:
             raise NotImplementedError('New task-pairs would be added soon')
         return vul_config_obj
 
 
 class AIShieldApi:
     """
     Instantiates for performing vulnerability analysis
     """
 
-    def __init__(self, api_url: str, api_key: str, org_id: str):
+    def __init__(self, api_url: str, org_id: str):
         """
         Initializes the AIShield API with request headers
 
         Parameters
         ----------
         api_url: api endpoint of AIShield vulnerability analysis
-        api_key: user api key
         org_id: organization key
         """
         if not api_url:
             raise ValueError('AIShield api is not provided')
-        if not api_key:
-            raise ValueError('api_key is not provided')
         if not org_id:
             raise ValueError('org_id is not provided')
         if not uri_validator(api_url):
             raise ValueError('aishield api is invalid')
 
         headers = {
             'Cache-Control': 'no-cache',
-            'x-api-key': api_key,
             'Org-Id': org_id
         }
+        # Get api_key from org_id
+        api_key = RequestProcessor(api_url, headers).get_api_key()
+        # Append the api key to the headers, which will be used for all future requests
+        headers['x-api-key'] = api_key
+
         self.request_processor = RequestProcessor(api_url, headers)
         self.job_details = JobDetails()
         self.task_type = None
         self.analysis_type = None
         self.job_payload = None
 
     def register_model(self, task_type: Optional[Task] = Task.IMAGE_CLASSIFICATION,
@@ -143,26 +148,51 @@
         self.task_type = task_type
         self.analysis_type = analysis_type
         model_registration_payload = {
             'task_type': task_type.value,
             "analysis_type": analysis_type.value
         }
         status, response_json = self.request_processor.register(payload=model_registration_payload)
-        response_json_urls = response_json[UploadURIKeys.URL_FIELD_KEY.value]
         self.job_details.model_id = response_json[UploadURIKeys.MODEL_ID_KEY.value]
-        self.job_details.data_upload_uri = response_json_urls[UploadURIKeys.DATA_UPLOAD_URI_KEY.value]
-        self.job_details.model_upload_uri = response_json_urls[UploadURIKeys.MODEL_UPLOAD_URI_KEY.value]
-        if task_type == Task.IMAGE_CLASSIFICATION:
-            self.job_details.label_upload_uri = response_json_urls[UploadURIKeys.LABEL_UPLOAD_URI_KEY.value]
+
+        data_upload_dtls = response_json[UploadURIKeys.URLS_KEY.value][
+            UploadURIKeys.DATA_UPLOAD_URI_KEY.value]
+        model_upload_dtls = response_json[UploadURIKeys.URLS_KEY.value][
+            UploadURIKeys.MODEL_UPLOAD_URI_KEY.value]
+        # data upload details
+        self.job_details.data_upload_uri = data_upload_dtls[UploadURIKeys.URL_KEY.value]
+        self.job_details.data_upload_policy = data_upload_dtls[UploadURIKeys.FIELDS_KEY.value]
+        # model upload details
+        self.job_details.model_upload_uri = model_upload_dtls[UploadURIKeys.URL_KEY.value]
+        self.job_details.model_upload_policy = model_upload_dtls[UploadURIKeys.FIELDS_KEY.value]
+
+        if task_type in [Task.IMAGE_CLASSIFICATION, Task.IMAGE_SEGMENTATION]:
+            # label upload details
+            label_upload_dtls = response_json[UploadURIKeys.URLS_KEY.value][
+                UploadURIKeys.LABEL_UPLOAD_URI_KEY.value]
+            self.job_details.label_upload_uri = label_upload_dtls[UploadURIKeys.URL_KEY.value]
+            self.job_details.label_upload_policy = label_upload_dtls[UploadURIKeys.FIELDS_KEY.value]
             if analysis_type == Attack.POISONING:
-                clean_model_upload_uris = [response_json_urls[UploadURIKeys.CLEAN_MODEL1_UPLOAD_URI_KEY.value],
-                                           response_json_urls[UploadURIKeys.CLEAN_MODEL2_UPLOAD_URI_KEY.value]]
+                # clean models upload details
+                clean_model1_upload_dtls = response_json[UploadURIKeys.URLS_KEY.value][
+                    UploadURIKeys.CLEAN_MODEL1_UPLOAD_URI_KEY.value]
+                clean_model2_upload_dtls = response_json[UploadURIKeys.URLS_KEY.value][
+                    UploadURIKeys.CLEAN_MODEL2_UPLOAD_URI_KEY.value]
+                clean_model_upload_uris = [clean_model1_upload_dtls[UploadURIKeys.URL_KEY.value],
+                                           clean_model2_upload_dtls[UploadURIKeys.URL_KEY.value]]
+                clean_model_upload_policies = [clean_model1_upload_dtls[UploadURIKeys.FIELDS_KEY.value],
+                                               clean_model2_upload_dtls[UploadURIKeys.FIELDS_KEY.value]]
                 self.job_details.clean_model_upload_uris = clean_model_upload_uris
+                self.job_details.clean_model_upload_policies = clean_model_upload_policies
         elif task_type in [Task.TABULAR_CLASSIFICATION, Task.TIMESERIES_FORECAST]:
-            self.job_details.minmax_upload_uri = response_json_urls[UploadURIKeys.MINMAX_UPLOAD_URI_KEY.value]
+            # minmax upload details
+            minmax_upload_dtls = response_json[UploadURIKeys.URLS_KEY.value][
+                UploadURIKeys.MINMAX_UPLOAD_URI_KEY.value]
+            self.job_details.minmax_upload_uri = minmax_upload_dtls[UploadURIKeys.URL_KEY.value]
+            self.job_details.minmax_upload_policy = minmax_upload_dtls[UploadURIKeys.FIELDS_KEY.value]
         else:
             raise NotImplementedError('New task-pairs would be added soon')
         return status, self.job_details
 
     def upload_input_artifacts(self, job_details: JobDetails, data_path: str = None, label_path: str = None,
                                minmax_path: str = None, model_path: str = None, clean_model_paths: list = None) -> list:
         """
@@ -183,54 +213,66 @@
         """
         if clean_model_paths is None:
             clean_model_paths = []
         upload_status_msg = []
         error_flag = False
         if data_path:
             data_upload_uri = job_details.data_upload_uri
-            upload_status = self.request_processor.upload_file(file_path=data_path, upload_uri=data_upload_uri)
+            data_upload_policy = job_details.data_upload_policy
+            upload_status = self.request_processor.upload_file(file_path=data_path, upload_uri=data_upload_uri,
+                                                               upload_policy=data_upload_policy)
             if upload_status == ResponseStatus.SUCCESS:
                 upload_status_msg.append('data file upload successful')
             else:
                 error_flag = True
                 upload_status_msg.append('data file upload failed')
         if label_path:
             label_upload_uri = job_details.label_upload_uri
-            upload_status = self.request_processor.upload_file(file_path=label_path, upload_uri=label_upload_uri)
+            label_upload_policy = job_details.label_upload_policy
+            upload_status = self.request_processor.upload_file(file_path=label_path, upload_uri=label_upload_uri,
+                                                               upload_policy=label_upload_policy)
             if upload_status == ResponseStatus.SUCCESS:
                 upload_status_msg.append('label file upload successful')
             else:
                 error_flag = True
                 upload_status_msg.append('label file upload failed')
 
         if minmax_path:
             minmax_upload_uri = job_details.minmax_upload_uri
-            upload_status = self.request_processor.upload_file(file_path=minmax_path, upload_uri=minmax_upload_uri)
+            minmax_upload_policy = job_details.minmax_upload_policy
+            upload_status = self.request_processor.upload_file(file_path=minmax_path, upload_uri=minmax_upload_uri,
+                                                               upload_policy=minmax_upload_policy)
             if upload_status == ResponseStatus.SUCCESS:
                 upload_status_msg.append('minmax file upload successful')
             else:
                 error_flag = True
                 upload_status_msg.append('minmax file upload failed')
 
         if model_path:
             model_upload_uri = job_details.model_upload_uri
-            upload_status = self.request_processor.upload_file(file_path=model_path, upload_uri=model_upload_uri)
+            model_upload_policy = job_details.model_upload_policy
+            upload_status = self.request_processor.upload_file(file_path=model_path, upload_uri=model_upload_uri,
+                                                               upload_policy=model_upload_policy)
             if upload_status == ResponseStatus.SUCCESS:
                 upload_status_msg.append('model file upload successful')
             else:
                 error_flag = True
                 upload_status_msg.append('model file upload failed')
 
         if clean_model_paths:
             num_clean_models_required = 2
             if len(clean_model_paths) < 2 or not all(clean_model_paths):
-                raise Exception('Model poison analysis requires atleast {} numbers of clean model'.format(num_clean_models_required))
+                raise Exception('Model poison analysis requires atleast {} numbers of clean model'.format(
+                    num_clean_models_required))
             clean_model_upload_uris = job_details.clean_model_upload_uris
+            clean_model_upload_policies = job_details.clean_model_upload_policies
             for idx in range(num_clean_models_required):
-                upload_status = self.request_processor.upload_file(file_path=clean_model_paths[idx], upload_uri=clean_model_upload_uris[idx])
+                upload_status = self.request_processor.upload_file(file_path=clean_model_paths[idx],
+                                                                   upload_uri=clean_model_upload_uris[idx],
+                                                                   upload_policy=clean_model_upload_policies[idx])
                 if upload_status == ResponseStatus.SUCCESS:
                     upload_status_msg.append('clean model file{} upload successful'.format(idx))
                 else:
                     error_flag = True
                     upload_status_msg.append('clean model file{} upload failed'.format(idx))
         if error_flag:
             raise Exception('some error occurred while uploading. Status is: {}'.format(', '.join(upload_status_msg)))
@@ -253,30 +295,31 @@
 
         if not model_id:
             raise ValueError('model_id must be provided')
         if not vuln_config:
             raise ValueError('vulnerability config must be provided')
 
         payload = {key: getattr(vuln_config, key) for key in dir(vuln_config) if not key.startswith('_')}
-        payload = delete_keys_from_dict(payload, ['task_type', 'attack', 'get_all_params'])  # delete non-relevant params for API call
+        payload = delete_keys_from_dict(payload, ['task_type', 'attack',
+                                                  'get_all_params'])  # delete non-relevant params for API call
         # validation - raise error any key in payload has None value
         keys_with_none_val = get_all_keys_by_val(payload, None)
         if keys_with_none_val:
             raise ValueError('None values found for {}.'.format(', '.join(keys_with_none_val)))
 
         task_type = vuln_config.task_type
         attack_strategy = vuln_config.attack
 
         if self.task_type != task_type or attack_strategy != self.analysis_type:
             raise Exception('Mismatch in task_type, analysis_type specified in model registration and analysis')
 
         self.job_payload = payload
         status, response_json = self.request_processor.send_for_analysis(model_id=model_id, payload=payload)
         self.job_details.job_id = response_json['job_id']
-        self.job_details.job_monitor_uri = response_json['monitor_link']
+        self.job_details.job_dashboard_uri = response_json['dashboard_link']
         return status, self.job_details
 
     def job_status(self, job_id):
         """
         Prints the status of each vulnerability analysis while the job is running.
         Once job completes, returns with status: success or failed
 
@@ -312,15 +355,15 @@
         save_folder_path = output_config.save_folder_path
 
         if file_format not in FileFormat.valid_types():
             raise ValueError('invalid file_format value {}. Must be one of {}'.format(file_format,
                                                                                       FileFormat.valid_types()))
         if report_type not in ReportType.valid_types():
             raise ValueError('invalid report_type value {}. Must be one of {}'.format(report_type,
-                                                                                ReportType.valid_types()))
+                                                                                      ReportType.valid_types()))
 
         # poisoning supports only pdf report format type
         if self.analysis_type == Attack.POISONING and not (FileFormat(output_config.file_format) == FileFormat.PDF):
             raise ValueError('invalid file_format value. poisoning analysis supports only pdf type')
 
         saved_loc = self.request_processor.get_artifacts(job_id=job_id, report_type=report_type,
                                                          file_format=file_format,
```

### Comparing `aishield-0.1.4/aishield/configs.py` & `aishield-0.1.5/aishield/configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,81 @@
 import os
+from typing import List
+
 from aishield.constants import (
     FileFormat,
     ReportType,
 )
 from aishield.utils.util import check_or_create_directory
 
 
+class UploadPolicy:
+    def __init__(self, policy=None):
+        self.policy = policy
+
+    @property
+    def policy(self):
+        return self.__policy
+
+    @policy.setter
+    def job_id(self, policy):
+        self.__policy = policy
+
+
 class JobDetails:
     """
     Instantiates to details of a vulnerability analysis job
     """
-    def __init__(self, job_id=None, job_monitor_uri=None, model_id=None, data_upload_uri=None, label_upload_uri=None,
-                 minmax_upload_uri: str = None, model_upload_uri=None, clean_model_upload_uris=[]):
+
+    def __init__(self, job_id=None, job_dashboard_uri=None, model_id=None, data_upload_uri=None, label_upload_uri=None,
+                 minmax_upload_uri: str = None, model_upload_uri=None, clean_model_upload_uris=[],
+                 data_upload_policy: dict = {}, label_upload_policy: dict = {}, minmax_upload_policy: dict = {},
+                 model_upload_policy: dict = {}, clean_model_upload_policies: List[dict] = []):
         """
         Constructor for Job Details class.
         Parameters
         ----------
         job_id: job_id of the submitted job
-        job_monitor_uri: uri for monitoring the progress of job
+        job_dashboard_uri: uri for monitoring the progress of job and downloading of output artifacts
         model_id: model id obtained after model registration
         data_upload_uri: uri returned by model registration service where data file in zip needs to be uploaded
         label_upload_uri: uri returned by model registration service where label file in zip needs to be uploaded
         minmax_upload_uri: uri returned by model registration service where minmax(for tabular data) file in zip needs to be uploaded
         model_upload_uri: uri returned by model registration service where model file in zip needs to be uploaded
         clean_model_upload_uris: uri's returned by model registration service where clean model files in zip needs to be uploaded (for model poison check)
         """
         self.job_id = job_id
-        self.job_monitor_uri = job_monitor_uri
+        self.job_dashboard_uri = job_dashboard_uri
         self.model_id = model_id
         self.data_upload_uri = data_upload_uri
         self.label_upload_uri = label_upload_uri
         self.model_upload_uri = model_upload_uri
         self.minmax_upload_uri = minmax_upload_uri  # for Tabular datatype
         self.clean_model_upload_uris = clean_model_upload_uris  # for model poison analysis
-
+        self.data_upload_policy = data_upload_policy
+        self.label_upload_policy = label_upload_policy
+        self.minmax_upload_policy = minmax_upload_policy
+        self.model_upload_policy = model_upload_policy
+        self.clean_model_upload_policies = clean_model_upload_policies
 
     @property
     def job_id(self):
         return self.__job_id
 
     @job_id.setter
     def job_id(self, job_id):
         self.__job_id = job_id
 
     @property
-    def job_monitor_uri(self):
-        return self.__job_monitor_uri
+    def job_dashboard_uri(self):
+        return self.__job_dashboard_uri
 
-    @job_monitor_uri.setter
-    def job_monitor_uri(self, job_monitor_uri):
-        self.__job_monitor_uri = job_monitor_uri
+    @job_dashboard_uri.setter
+    def job_dashboard_uri(self, job_dashboard_uri):
+        self.__job_dashboard_uri = job_dashboard_uri
 
     @property
     def data_upload_uri(self):
         return self.__data_upload_uri
 
     @data_upload_uri.setter
     def data_upload_uri(self, data_upload_uri):
```

### Comparing `aishield-0.1.4/aishield/connection.py` & `aishield-0.1.5/aishield/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,50 @@
         ----------
         api_endpoint: api endpoint of AIShield vulnerability analysis
         headers: headers for the request
         """
         self.api_endpoint = api_endpoint
         self.headers = headers
 
+    def get_api_key(self):
+        """
+            Sends HTTP Post request to api_endpoint to get api_key. This is used for managing policies.
+            Parameters
+            ----------
+
+            Returns
+            -------
+            the api_key
+            raises AIShieldException in case of errors or if the response from server does not indicate 'SUCCESS'.
+        """
+        model_registration_url = self.api_endpoint + "/get_aws_api_key"
+        try:
+            response = requests.get(url=model_registration_url, headers=self.headers)
+            response.raise_for_status()
+        except requests.RequestException as e:
+            raise AIShieldException(e)
+
+        resp_json = None
+
+        try:
+            resp_json = response.json()
+        except ValueError:
+            raise AIShieldException(
+                'Error response from server: {}{}'.format(
+                    response.text[0:150], len(response.text) > 150 and '...' or ''
+                )
+            )
+        if 'x_api_key' in resp_json:
+            response_json = resp_json['x_api_key']
+        else:
+            raise AIShieldException('x_api_key not found in response')
+
+        return response_json
+
+
     def register(self, payload):
         """
             Sends HTTP Post request to api_endpoint for model registration.
             Parameters
             ----------
             payload: task and analysis type as as JSON.
 
@@ -61,38 +97,41 @@
             status = 'success'
             response_json = resp_json['data']
         else:
             raise AIShieldException('data or urls field not found in response')
 
         return status, response_json
 
-    def upload_file(self, file_path, upload_uri):
+    def upload_file(self, file_path, upload_uri, upload_policy):
         """
         Upload file to a particular uri for vulnerability analysis.
         Parameters
         ----------
         file_path: location of file to be uploaded
         upload_uri : uri where file to be uploaded
+        upload_policy : policy control of the artifact being uploaded
 
         Returns
         -------
         the status of job with details
         raises AIShieldException in case of errors or if the response from server does not indicate 'SUCCESS'.
         """
         if not check_valid_filepath(file_path):
             raise FileNotFoundError('file at {} not found or not accessible'.format(file_path))
         try:
-            data = open(file_path, 'rb')
-            response = requests.request(method="PUT", url=upload_uri, data=data)
+            files = [
+                ('file', (os.path.basename(file_path), open(file_path, 'rb'), 'application/zip'))
+            ]
+            response = requests.request(method="POST", url=upload_uri, files=files, data=upload_policy)
             response.raise_for_status()
         except requests.RequestException as e:
             raise AIShieldException(e)
 
         status_cd = response.status_code
-        if status_cd == 200:
+        if status_cd == 204:  # No Content success
             status = ResponseStatus.SUCCESS
         else:
             status = ResponseStatus.FAILED
         return status
 
     def send_for_analysis(self, model_id, payload):
         """
```

### Comparing `aishield-0.1.4/aishield/constants.py` & `aishield-0.1.5/aishield/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 class SupportedFramework(ExtendedEnum):
     TENSORFLOW = 'tensorflow'
     SCIKIT_LEARN = 'scikit-learn'
 
 
 class UploadURIKeys(ExtendedEnum):
     MODEL_ID_KEY = 'model_id'
-    URL_FIELD_KEY = 'urls'
+    URLS_KEY = 'urls'
+    URL_KEY = 'url'
+    FIELDS_KEY = 'fields'
     DATA_UPLOAD_URI_KEY = 'data_upload_url'
     LABEL_UPLOAD_URI_KEY = 'label_upload_url'
     MODEL_UPLOAD_URI_KEY = 'model_upload_url'
     MINMAX_UPLOAD_URI_KEY = 'minmax_upload_url'
     CLEAN_MODEL1_UPLOAD_URI_KEY = 'clean_model1_upload_url'
     CLEAN_MODEL2_UPLOAD_URI_KEY = 'clean_model2_upload_url'
```

### Comparing `aishield-0.1.4/aishield/image_classification/base_ic.py` & `aishield-0.1.5/aishield/image_classification/base_ic.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/image_classification/evasion.py` & `aishield-0.1.5/aishield/image_classification/evasion.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/image_classification/extraction.py` & `aishield-0.1.5/aishield/image_classification/extraction.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/image_classification/poision.py` & `aishield-0.1.5/aishield/image_classification/poision.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/tabular_classification/base_tc.py` & `aishield-0.1.5/aishield/tabular_classification/base_tc.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/tabular_classification/evasion.py` & `aishield-0.1.5/aishield/tabular_classification/evasion.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/tabular_classification/extraction.py` & `aishield-0.1.5/aishield/tabular_classification/extraction.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/timeseries_forecasting/base_tsf.py` & `aishield-0.1.5/aishield/timeseries_forecasting/base_tsf.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/timeseries_forecasting/extraction.py` & `aishield-0.1.5/aishield/timeseries_forecasting/extraction.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/utils/exceptions.py` & `aishield-0.1.5/aishield/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/utils/logger.py` & `aishield-0.1.5/aishield/utils/logger.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield/utils/util.py` & `aishield-0.1.5/aishield/utils/util.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/aishield.egg-info/PKG-INFO` & `aishield-0.1.5/aishield.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishield
-Version: 0.1.4
+Version: 0.1.5
 Summary: AIShield provides the Python convenience package to allow users to seamlessly integrate AIShield Vulnerability Assessment and Defense capabilities into their AI development workflows.
 Home-page: https://www.boschaishield.com/
 Author: Contact AIShield
 Author-email: aishield.contact@bosch.com
 License: Apache License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,19 @@
    
 ## More about AIShield
 
 - Website:  https://www.boschaishield.com/
 - Email:   <AIShield.Contact@bosch.com>
 
 ## Version History
+
+### 0.1.5
+- Added vulnerability analysis for image segmentation: model extraction attack
+- Updated to be compatible with latest AIShield API version. Also, now api_key is not required to be provided explicitly for analysis. It will be generated from org_id and policies are consumed accordingly. 
+
 ### 0.1.4
 - Added vulnerability analysis for time series forecasting: model extraction attack
 
 ### 0.1.3
 - Updated to be compatible with latest AIShield API version
 - Added vulnerability analysis for tabular classification: model evasion attack
```

### Comparing `aishield-0.1.4/aishield.egg-info/SOURCES.txt` & `aishield-0.1.5/aishield.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 aishield.egg-info/requires.txt
 aishield.egg-info/top_level.txt
 aishield/image_classification/__init__.py
 aishield/image_classification/base_ic.py
 aishield/image_classification/evasion.py
 aishield/image_classification/extraction.py
 aishield/image_classification/poision.py
+aishield/image_segmentation/__init__.py
+aishield/image_segmentation/base_is.py
+aishield/image_segmentation/extraction.py
 aishield/tabular_classification/__init__.py
 aishield/tabular_classification/base_tc.py
 aishield/tabular_classification/evasion.py
 aishield/tabular_classification/extraction.py
 aishield/timeseries_forecasting/__init__.py
 aishield/timeseries_forecasting/base_tsf.py
 aishield/timeseries_forecasting/extraction.py
```

### Comparing `aishield-0.1.4/pyproject.toml` & `aishield-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aishield-0.1.4/setup.py` & `aishield-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="aishield",
-    version="0.1.4",
+    version="0.1.5",
     description="AIShield provides the Python convenience package to allow users to seamlessly integrate AIShield Vulnerability Assessment and Defense capabilities into their AI development workflows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.boschaishield.com/',
     author="Contact AIShield",
     author_email="aishield.contact@bosch.com",
     license="Apache License",
```

### Comparing `aishield-0.1.4/tests/test_aishield_api.py` & `aishield-0.1.5/tests/test_aishield_api.py`

 * *Files identical despite different names*

