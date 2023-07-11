# Comparing `tmp/alibabacloud_aiearth-engine20220609-1.0.5.tar.gz` & `tmp/alibabacloud_aiearth-engine20220609-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiearth-engine20220609-1.0.5.tar", last modified: Thu May 25 11:51:15 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiearth-engine20220609-1.0.6.tar", last modified: Tue Jul 11 11:47:38 2023, max compression
```

## Comparing `alibabacloud_aiearth-engine20220609-1.0.5.tar` & `alibabacloud_aiearth-engine20220609-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45127 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/client.py
--rw-r--r--   0 root         (0) root         (0)    82980 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52999 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609/client.py
+-rw-r--r--   0 root         (0) root         (0)    92238 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-07-11 11:47:38.000000 alibabacloud_aiearth-engine20220609-1.0.6/setup.py
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/LICENSE` & `alibabacloud_aiearth-engine20220609-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/PKG-INFO` & `alibabacloud_aiearth-engine20220609-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiearth-engine20220609
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud AIEarth-Engine (20220609) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/README-CN.md` & `alibabacloud_aiearth-engine20220609-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/README.md` & `alibabacloud_aiearth-engine20220609-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/client.py` & `alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -229,14 +229,170 @@
     async def delete_jobs_async(
         self,
         request: aiearth__engine_20220609_models.DeleteJobsRequest,
     ) -> aiearth__engine_20220609_models.DeleteJobsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_jobs_with_options_async(request, runtime)
 
+    def delete_user_raster_datas_with_options(
+        self,
+        tmp_req: aiearth__engine_20220609_models.DeleteUserRasterDatasRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> aiearth__engine_20220609_models.DeleteUserRasterDatasResponse:
+        UtilClient.validate_model(tmp_req)
+        request = aiearth__engine_20220609_models.DeleteUserRasterDatasShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.data_ids):
+            request.data_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_ids, 'DataIds', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.data_ids_shrink):
+            body['DataIds'] = request.data_ids_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteUserRasterDatas',
+            version='2022-06-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiearth__engine_20220609_models.DeleteUserRasterDatasResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_user_raster_datas_with_options_async(
+        self,
+        tmp_req: aiearth__engine_20220609_models.DeleteUserRasterDatasRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> aiearth__engine_20220609_models.DeleteUserRasterDatasResponse:
+        UtilClient.validate_model(tmp_req)
+        request = aiearth__engine_20220609_models.DeleteUserRasterDatasShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.data_ids):
+            request.data_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_ids, 'DataIds', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.data_ids_shrink):
+            body['DataIds'] = request.data_ids_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteUserRasterDatas',
+            version='2022-06-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiearth__engine_20220609_models.DeleteUserRasterDatasResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_user_raster_datas(
+        self,
+        request: aiearth__engine_20220609_models.DeleteUserRasterDatasRequest,
+    ) -> aiearth__engine_20220609_models.DeleteUserRasterDatasResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_user_raster_datas_with_options(request, runtime)
+
+    async def delete_user_raster_datas_async(
+        self,
+        request: aiearth__engine_20220609_models.DeleteUserRasterDatasRequest,
+    ) -> aiearth__engine_20220609_models.DeleteUserRasterDatasResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_user_raster_datas_with_options_async(request, runtime)
+
+    def delete_user_vector_datas_with_options(
+        self,
+        tmp_req: aiearth__engine_20220609_models.DeleteUserVectorDatasRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> aiearth__engine_20220609_models.DeleteUserVectorDatasResponse:
+        UtilClient.validate_model(tmp_req)
+        request = aiearth__engine_20220609_models.DeleteUserVectorDatasShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.data_ids):
+            request.data_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_ids, 'DataIds', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.data_ids_shrink):
+            body['DataIds'] = request.data_ids_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteUserVectorDatas',
+            version='2022-06-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiearth__engine_20220609_models.DeleteUserVectorDatasResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_user_vector_datas_with_options_async(
+        self,
+        tmp_req: aiearth__engine_20220609_models.DeleteUserVectorDatasRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> aiearth__engine_20220609_models.DeleteUserVectorDatasResponse:
+        UtilClient.validate_model(tmp_req)
+        request = aiearth__engine_20220609_models.DeleteUserVectorDatasShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.data_ids):
+            request.data_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_ids, 'DataIds', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.data_ids_shrink):
+            body['DataIds'] = request.data_ids_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteUserVectorDatas',
+            version='2022-06-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiearth__engine_20220609_models.DeleteUserVectorDatasResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_user_vector_datas(
+        self,
+        request: aiearth__engine_20220609_models.DeleteUserVectorDatasRequest,
+    ) -> aiearth__engine_20220609_models.DeleteUserVectorDatasResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_user_vector_datas_with_options(request, runtime)
+
+    async def delete_user_vector_datas_async(
+        self,
+        request: aiearth__engine_20220609_models.DeleteUserVectorDatasRequest,
+    ) -> aiearth__engine_20220609_models.DeleteUserVectorDatasResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_user_vector_datas_with_options_async(request, runtime)
+
     def download_data_with_options(
         self,
         request: aiearth__engine_20220609_models.DownloadDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> aiearth__engine_20220609_models.DownloadDataResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -318,16 +474,26 @@
     ) -> aiearth__engine_20220609_models.GetJobsResponse:
         UtilClient.validate_model(tmp_req)
         request = aiearth__engine_20220609_models.GetJobsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.job_ids):
             request.job_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.job_ids, 'JobIds', 'json')
         body = {}
+        if not UtilClient.is_unset(request.app_name):
+            body['AppName'] = request.app_name
         if not UtilClient.is_unset(request.job_ids_shrink):
             body['JobIds'] = request.job_ids_shrink
+        if not UtilClient.is_unset(request.job_type):
+            body['JobType'] = request.job_type
+        if not UtilClient.is_unset(request.name_like):
+            body['NameLike'] = request.name_like
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetJobs',
             version='2022-06-09',
             protocol='HTTPS',
@@ -350,16 +516,26 @@
     ) -> aiearth__engine_20220609_models.GetJobsResponse:
         UtilClient.validate_model(tmp_req)
         request = aiearth__engine_20220609_models.GetJobsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.job_ids):
             request.job_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.job_ids, 'JobIds', 'json')
         body = {}
+        if not UtilClient.is_unset(request.app_name):
+            body['AppName'] = request.app_name
         if not UtilClient.is_unset(request.job_ids_shrink):
             body['JobIds'] = request.job_ids_shrink
+        if not UtilClient.is_unset(request.job_type):
+            body['JobType'] = request.job_type
+        if not UtilClient.is_unset(request.name_like):
+            body['NameLike'] = request.name_like
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetJobs',
             version='2022-06-09',
             protocol='HTTPS',
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/models.py` & `alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -571,14 +571,276 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteJobsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteUserRasterDatasRequest(TeaModel):
+    def __init__(
+        self,
+        data_ids: List[str] = None,
+    ):
+        self.data_ids = data_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_ids is not None:
+            result['DataIds'] = self.data_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataIds') is not None:
+            self.data_ids = m.get('DataIds')
+        return self
+
+
+class DeleteUserRasterDatasShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        data_ids_shrink: str = None,
+    ):
+        self.data_ids_shrink = data_ids_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_ids_shrink is not None:
+            result['DataIds'] = self.data_ids_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataIds') is not None:
+            self.data_ids_shrink = m.get('DataIds')
+        return self
+
+
+class DeleteUserRasterDatasResponseBody(TeaModel):
+    def __init__(
+        self,
+        num: int = None,
+        request_id: str = None,
+    ):
+        self.num = num
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.num is not None:
+            result['Num'] = self.num
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Num') is not None:
+            self.num = m.get('Num')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteUserRasterDatasResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteUserRasterDatasResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteUserRasterDatasResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteUserVectorDatasRequest(TeaModel):
+    def __init__(
+        self,
+        data_ids: List[str] = None,
+    ):
+        self.data_ids = data_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_ids is not None:
+            result['DataIds'] = self.data_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataIds') is not None:
+            self.data_ids = m.get('DataIds')
+        return self
+
+
+class DeleteUserVectorDatasShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        data_ids_shrink: str = None,
+    ):
+        self.data_ids_shrink = data_ids_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_ids_shrink is not None:
+            result['DataIds'] = self.data_ids_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataIds') is not None:
+            self.data_ids_shrink = m.get('DataIds')
+        return self
+
+
+class DeleteUserVectorDatasResponseBody(TeaModel):
+    def __init__(
+        self,
+        num: int = None,
+        request_id: str = None,
+    ):
+        self.num = num
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.num is not None:
+            result['Num'] = self.num
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Num') is not None:
+            self.num = m.get('Num')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteUserVectorDatasResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteUserVectorDatasResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteUserVectorDatasResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DownloadDataRequest(TeaModel):
     def __init__(
         self,
         band_no: str = None,
         compress: bool = None,
         data_id: str = None,
     ):
@@ -708,62 +970,122 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetJobsRequest(TeaModel):
     def __init__(
         self,
+        app_name: str = None,
         job_ids: List[int] = None,
+        job_type: str = None,
+        name_like: str = None,
+        page_no: int = None,
+        page_size: int = None,
     ):
+        self.app_name = app_name
         self.job_ids = job_ids
+        self.job_type = job_type
+        self.name_like = name_like
+        self.page_no = page_no
+        self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.app_name is not None:
+            result['AppName'] = self.app_name
         if self.job_ids is not None:
             result['JobIds'] = self.job_ids
+        if self.job_type is not None:
+            result['JobType'] = self.job_type
+        if self.name_like is not None:
+            result['NameLike'] = self.name_like
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AppName') is not None:
+            self.app_name = m.get('AppName')
         if m.get('JobIds') is not None:
             self.job_ids = m.get('JobIds')
+        if m.get('JobType') is not None:
+            self.job_type = m.get('JobType')
+        if m.get('NameLike') is not None:
+            self.name_like = m.get('NameLike')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         return self
 
 
 class GetJobsShrinkRequest(TeaModel):
     def __init__(
         self,
+        app_name: str = None,
         job_ids_shrink: str = None,
+        job_type: str = None,
+        name_like: str = None,
+        page_no: int = None,
+        page_size: int = None,
     ):
+        self.app_name = app_name
         self.job_ids_shrink = job_ids_shrink
+        self.job_type = job_type
+        self.name_like = name_like
+        self.page_no = page_no
+        self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.app_name is not None:
+            result['AppName'] = self.app_name
         if self.job_ids_shrink is not None:
             result['JobIds'] = self.job_ids_shrink
+        if self.job_type is not None:
+            result['JobType'] = self.job_type
+        if self.name_like is not None:
+            result['NameLike'] = self.name_like
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AppName') is not None:
+            self.app_name = m.get('AppName')
         if m.get('JobIds') is not None:
             self.job_ids_shrink = m.get('JobIds')
+        if m.get('JobType') is not None:
+            self.job_type = m.get('JobType')
+        if m.get('NameLike') is not None:
+            self.name_like = m.get('NameLike')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         return self
 
 
 class GetJobsResponseBodyList(TeaModel):
     def __init__(
         self,
         app: str = None,
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO` & `alibabacloud_aiearth-engine20220609-1.0.6/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiearth-engine20220609
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud AIEarth-Engine (20220609) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.5/setup.py` & `alibabacloud_aiearth-engine20220609-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiearth-engine20220609.
 
-Created on 25/05/2023
+Created on 11/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiearth_engine20220609"
 NAME = "alibabacloud_aiearth-engine20220609" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIEarth-Engine (20220609) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

