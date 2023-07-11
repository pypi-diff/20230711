# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.931.tar", last modified: Mon Jul 10 00:40:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.932.tar", last modified: Tue Jul 11 00:43:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.931.tar` & `tencentcloud-sdk-python-essbasic-3.0.932.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/essbasic_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   375558 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52742 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/essbasic_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   380285 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53839 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1673,15 +1673,15 @@
 class ChannelCreateFlowGroupByFilesRequest(AbstractModel):
     """ChannelCreateFlowGroupByFiles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _FlowFileInfos: 每个子合同的发起所需的信息，数量限制2-100
+        :param _FlowFileInfos: 每个子合同的发起所需的信息，数量限制2-50
         :type FlowFileInfos: list of FlowFileInfo
         :param _FlowGroupName: 合同组名称，长度不超过200个字符
         :type FlowGroupName: str
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _ApproverVerifyType: 签署人校验方式
 VerifyCheck: 人脸识别（默认）
@@ -1814,14 +1814,145 @@
 
     def _deserialize(self, params):
         self._FlowGroupId = params.get("FlowGroupId")
         self._FlowIds = params.get("FlowIds")
         self._RequestId = params.get("RequestId")
 
 
+class ChannelCreateFlowGroupByTemplatesRequest(AbstractModel):
+    """ChannelCreateFlowGroupByTemplates请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 均必填。
+        :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
+        :param _FlowInfos: 每个子合同的发起所需的信息，数量限制2-50（合同组暂不支持抄送功能）
+        :type FlowInfos: list of FlowInfo
+        :param _FlowGroupName: 合同组名称，长度不超过200个字符
+        :type FlowGroupName: str
+        """
+        self._Agent = None
+        self._FlowInfos = None
+        self._FlowGroupName = None
+
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
+    @property
+    def FlowInfos(self):
+        return self._FlowInfos
+
+    @FlowInfos.setter
+    def FlowInfos(self, FlowInfos):
+        self._FlowInfos = FlowInfos
+
+    @property
+    def FlowGroupName(self):
+        return self._FlowGroupName
+
+    @FlowGroupName.setter
+    def FlowGroupName(self, FlowGroupName):
+        self._FlowGroupName = FlowGroupName
+
+
+    def _deserialize(self, params):
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
+        if params.get("FlowInfos") is not None:
+            self._FlowInfos = []
+            for item in params.get("FlowInfos"):
+                obj = FlowInfo()
+                obj._deserialize(item)
+                self._FlowInfos.append(obj)
+        self._FlowGroupName = params.get("FlowGroupName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ChannelCreateFlowGroupByTemplatesResponse(AbstractModel):
+    """ChannelCreateFlowGroupByTemplates返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FlowGroupId: 合同组ID
+        :type FlowGroupId: str
+        :param _FlowIds: 子合同ID列表
+        :type FlowIds: list of str
+        :param _TaskInfos: 复杂文档合成任务（如，包含动态表格的预览任务）的任务信息数组；
+如果文档需要异步合成，此字段会返回该异步任务的任务信息，后续可以通过ChannelGetTaskResultApi接口查询任务详情；
+        :type TaskInfos: list of TaskInfo
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._FlowGroupId = None
+        self._FlowIds = None
+        self._TaskInfos = None
+        self._RequestId = None
+
+    @property
+    def FlowGroupId(self):
+        return self._FlowGroupId
+
+    @FlowGroupId.setter
+    def FlowGroupId(self, FlowGroupId):
+        self._FlowGroupId = FlowGroupId
+
+    @property
+    def FlowIds(self):
+        return self._FlowIds
+
+    @FlowIds.setter
+    def FlowIds(self, FlowIds):
+        self._FlowIds = FlowIds
+
+    @property
+    def TaskInfos(self):
+        return self._TaskInfos
+
+    @TaskInfos.setter
+    def TaskInfos(self, TaskInfos):
+        self._TaskInfos = TaskInfos
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._FlowGroupId = params.get("FlowGroupId")
+        self._FlowIds = params.get("FlowIds")
+        if params.get("TaskInfos") is not None:
+            self._TaskInfos = []
+            for item in params.get("TaskInfos"):
+                obj = TaskInfo()
+                obj._deserialize(item)
+                self._TaskInfos.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class ChannelCreateFlowRemindsRequest(AbstractModel):
     """ChannelCreateFlowReminds请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8033,28 +8164,31 @@
         :type FlowType: str
         :param _CallbackUrl: 签署流程回调地址，长度不超过255个字符
         :type CallbackUrl: str
         :param _CustomerData: 第三方应用的业务信息，最大长度1000个字符。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
         :type CustomerData: str
         :param _Unordered: 合同签署顺序类型(无序签,顺序签)，默认为false，即有序签署
         :type Unordered: bool
+        :param _Components: 签署文件中的发起方的填写控件，需要在发起的时候进行填充
+        :type Components: list of Component
         :param _CustomShowMap: 合同显示的页卡模板，说明：只支持{合同名称}, {发起方企业}, {发起方姓名}, {签署方N企业}, {签署方N姓名}，且N不能超过签署人的数量，N从1开始
         :type CustomShowMap: str
         :param _NeedSignReview: 本企业(发起方企业)是否需要签署审批
         :type NeedSignReview: bool
         """
         self._FileIds = None
         self._FlowName = None
         self._FlowApprovers = None
         self._Deadline = None
         self._FlowDescription = None
         self._FlowType = None
         self._CallbackUrl = None
         self._CustomerData = None
         self._Unordered = None
+        self._Components = None
         self._CustomShowMap = None
         self._NeedSignReview = None
 
     @property
     def FileIds(self):
         return self._FileIds
 
@@ -8123,14 +8257,22 @@
         return self._Unordered
 
     @Unordered.setter
     def Unordered(self, Unordered):
         self._Unordered = Unordered
 
     @property
+    def Components(self):
+        return self._Components
+
+    @Components.setter
+    def Components(self, Components):
+        self._Components = Components
+
+    @property
     def CustomShowMap(self):
         return self._CustomShowMap
 
     @CustomShowMap.setter
     def CustomShowMap(self, CustomShowMap):
         self._CustomShowMap = CustomShowMap
 
@@ -8154,14 +8296,20 @@
                 self._FlowApprovers.append(obj)
         self._Deadline = params.get("Deadline")
         self._FlowDescription = params.get("FlowDescription")
         self._FlowType = params.get("FlowType")
         self._CallbackUrl = params.get("CallbackUrl")
         self._CustomerData = params.get("CustomerData")
         self._Unordered = params.get("Unordered")
+        if params.get("Components") is not None:
+            self._Components = []
+            for item in params.get("Components"):
+                obj = Component()
+                obj._deserialize(item)
+                self._Components.append(obj)
         self._CustomShowMap = params.get("CustomShowMap")
         self._NeedSignReview = params.get("NeedSignReview")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ChannelCreateFlowGroupByTemplates(self, request):
+        """接口（ChannelCreateFlowGroupByTemplates）用于通过多模板创建合同组签署流程。
+
+        :param request: Request instance for ChannelCreateFlowGroupByTemplates.
+        :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowGroupByTemplatesRequest`
+        :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowGroupByTemplatesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ChannelCreateFlowGroupByTemplates", params, headers=headers)
+            response = json.loads(body)
+            model = models.ChannelCreateFlowGroupByTemplatesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ChannelCreateFlowReminds(self, request):
         """指定需要批量催办的签署流程Id，批量催办合同，最多100个；接口失败后返回错误信息
         注意:
         该接口不可直接调用，请联系客户经理申请使用
         仅能催办当前状态为“待签署”的签署人，且只能催办一次
 
         :param request: Request instance for ChannelCreateFlowReminds.
@@ -571,15 +594,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelDescribeRoles(self, request):
-        """查询用户角色
+        """查询角色列表，支持根据类型和状态过滤角色列表
 
         :param request: Request instance for ChannelDescribeRoles.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeRolesRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeRolesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.931'
+__version__ = '3.0.932'
```

