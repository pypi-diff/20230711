# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.931.tar", last modified: Mon Jul 10 00:40:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.932.tar", last modified: Tue Jul 11 00:43:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.931.tar` & `tencentcloud-sdk-python-ess-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud_sdk_python_ess.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    59451 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24834 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   408951 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:34.000000 tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    61652 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   428631 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/__init__.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.931/setup.py` & `tencentcloud-sdk-python-ess-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.931/README.rst` & `tencentcloud-sdk-python-ess-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.931/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,63 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateFlowGroupByFiles(self, request):
+        """此接口（CreateFlowGroupByFiles）通过多文件创建合同组签署流程。<br/>
+        PDF资源Id 通过上传文件接口获取
+        此接口合同组中的子合同必须都是文件发起的合同
+
+        :param request: Request instance for CreateFlowGroupByFiles.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowGroupByFilesRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowGroupByFilesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateFlowGroupByFiles", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateFlowGroupByFilesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateFlowGroupByTemplates(self, request):
+        """此接口（CreateFlowGroupByTemplates）通过多模板创建合同组签署流程。<br/>
+        此接口合同组中的子合同必须都是模板发起的合同。 <br/>目前最大仅支持50个子合同
+
+        :param request: Request instance for CreateFlowGroupByTemplates.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowGroupByTemplatesRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowGroupByTemplatesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateFlowGroupByTemplates", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateFlowGroupByTemplatesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateFlowReminds(self, request):
         """指定需要批量催办的签署流程Id，批量催办合同，最多100个; 接口失败后返回错误信息
         注意:
         该接口不可直接调用，请联系客户经理申请使用
         仅能催办当前状态为“待签署”的签署人，且只能催办一次
         发起合同时，签署人的NotifyType需设置为sms，否则无法催办
```

### Comparing `tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.931/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,18 @@
 3：企业静默签署
 注：类型为3（企业静默签署）时，此接口会默认完成该签署方的签署。静默签署仅进行盖章操作，不能自动签名。
         :type ApproverType: int
         :param _ApproverName: 签署人的姓名
         :type ApproverName: str
         :param _ApproverMobile: 签署人的手机号，11位数字
         :type ApproverMobile: str
-        :param _SignComponents: 签署人的签署控件列表
-        :type SignComponents: list of Component
         :param _OrganizationName: 如果签署方是企业签署方，则为企业名
         :type OrganizationName: str
+        :param _SignComponents: 签署人的签署控件列表
+        :type SignComponents: list of Component
         :param _ApproverIdCardNumber: 签署人的身份证号
         :type ApproverIdCardNumber: str
         :param _ApproverIdCardType: 签署人的身份证件类型 
 ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
         :type ApproverIdCardType: str
@@ -200,16 +200,16 @@
         :type ApproverSignTypes: list of int
         :param _ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批，true 则为需要。为个人签署方时则由发起方企业审核。	
         :type ApproverNeedSignReview: bool
         """
         self._ApproverType = None
         self._ApproverName = None
         self._ApproverMobile = None
-        self._SignComponents = None
         self._OrganizationName = None
+        self._SignComponents = None
         self._ApproverIdCardNumber = None
         self._ApproverIdCardType = None
         self._NotifyType = None
         self._ApproverRole = None
         self._VerifyChannel = None
         self._PreReadTime = None
         self._UserId = None
@@ -241,30 +241,30 @@
         return self._ApproverMobile
 
     @ApproverMobile.setter
     def ApproverMobile(self, ApproverMobile):
         self._ApproverMobile = ApproverMobile
 
     @property
-    def SignComponents(self):
-        return self._SignComponents
-
-    @SignComponents.setter
-    def SignComponents(self, SignComponents):
-        self._SignComponents = SignComponents
-
-    @property
     def OrganizationName(self):
         return self._OrganizationName
 
     @OrganizationName.setter
     def OrganizationName(self, OrganizationName):
         self._OrganizationName = OrganizationName
 
     @property
+    def SignComponents(self):
+        return self._SignComponents
+
+    @SignComponents.setter
+    def SignComponents(self, SignComponents):
+        self._SignComponents = SignComponents
+
+    @property
     def ApproverIdCardNumber(self):
         return self._ApproverIdCardNumber
 
     @ApproverIdCardNumber.setter
     def ApproverIdCardNumber(self, ApproverIdCardNumber):
         self._ApproverIdCardNumber = ApproverIdCardNumber
 
@@ -365,21 +365,21 @@
         self._ApproverNeedSignReview = ApproverNeedSignReview
 
 
     def _deserialize(self, params):
         self._ApproverType = params.get("ApproverType")
         self._ApproverName = params.get("ApproverName")
         self._ApproverMobile = params.get("ApproverMobile")
+        self._OrganizationName = params.get("OrganizationName")
         if params.get("SignComponents") is not None:
             self._SignComponents = []
             for item in params.get("SignComponents"):
                 obj = Component()
                 obj._deserialize(item)
                 self._SignComponents.append(obj)
-        self._OrganizationName = params.get("OrganizationName")
         self._ApproverIdCardNumber = params.get("ApproverIdCardNumber")
         self._ApproverIdCardType = params.get("ApproverIdCardType")
         self._NotifyType = params.get("NotifyType")
         self._ApproverRole = params.get("ApproverRole")
         self._VerifyChannel = params.get("VerifyChannel")
         self._PreReadTime = params.get("PreReadTime")
         self._UserId = params.get("UserId")
@@ -2823,14 +2823,300 @@
     def _deserialize(self, params):
         self._ReportId = params.get("ReportId")
         self._Status = params.get("Status")
         self._ReportUrl = params.get("ReportUrl")
         self._RequestId = params.get("RequestId")
 
 
+class CreateFlowGroupByFilesRequest(AbstractModel):
+    """CreateFlowGroupByFiles请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Operator: 调用方用户信息，userId 必填。支持填入集团子公司经办人 userId 代发合同
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _FlowGroupName: 合同（流程）组名称,最大长度200个字符
+        :type FlowGroupName: str
+        :param _FlowGroupInfos: 合同（流程）组的子合同信息，支持2-50个子合同
+        :type FlowGroupInfos: list of FlowGroupInfo
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _FlowGroupOptions: 合同（流程）组的配置项信息。包括是否通知本企业签署方，是否通知其他签署方
+        :type FlowGroupOptions: :class:`tencentcloud.ess.v20201111.models.FlowGroupOptions`
+        """
+        self._Operator = None
+        self._FlowGroupName = None
+        self._FlowGroupInfos = None
+        self._Agent = None
+        self._FlowGroupOptions = None
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def FlowGroupName(self):
+        return self._FlowGroupName
+
+    @FlowGroupName.setter
+    def FlowGroupName(self, FlowGroupName):
+        self._FlowGroupName = FlowGroupName
+
+    @property
+    def FlowGroupInfos(self):
+        return self._FlowGroupInfos
+
+    @FlowGroupInfos.setter
+    def FlowGroupInfos(self, FlowGroupInfos):
+        self._FlowGroupInfos = FlowGroupInfos
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
+    def FlowGroupOptions(self):
+        return self._FlowGroupOptions
+
+    @FlowGroupOptions.setter
+    def FlowGroupOptions(self, FlowGroupOptions):
+        self._FlowGroupOptions = FlowGroupOptions
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        self._FlowGroupName = params.get("FlowGroupName")
+        if params.get("FlowGroupInfos") is not None:
+            self._FlowGroupInfos = []
+            for item in params.get("FlowGroupInfos"):
+                obj = FlowGroupInfo()
+                obj._deserialize(item)
+                self._FlowGroupInfos.append(obj)
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
+        if params.get("FlowGroupOptions") is not None:
+            self._FlowGroupOptions = FlowGroupOptions()
+            self._FlowGroupOptions._deserialize(params.get("FlowGroupOptions"))
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
+class CreateFlowGroupByFilesResponse(AbstractModel):
+    """CreateFlowGroupByFiles返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FlowGroupId: 合同(流程)组的合同组Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FlowGroupId: str
+        :param _FlowIds: 合同(流程)组中子合同列表.
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FlowIds: list of str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._FlowGroupId = None
+        self._FlowIds = None
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
+        self._RequestId = params.get("RequestId")
+
+
+class CreateFlowGroupByTemplatesRequest(AbstractModel):
+    """CreateFlowGroupByTemplates请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Operator: 调用方用户信息，userId 必填。支持填入集团子公司经办人 userId 代发合同
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _FlowGroupName: 合同组名称,最大长度200个字符
+        :type FlowGroupName: str
+        :param _FlowGroupInfos: 合同组的子合同信息，支持2-50个子合同
+        :type FlowGroupInfos: list of FlowGroupInfo
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _FlowGroupOptions: 合同组的配置信息。包括是否通知本企业签署方，是否通知其他签署方
+        :type FlowGroupOptions: :class:`tencentcloud.ess.v20201111.models.FlowGroupOptions`
+        """
+        self._Operator = None
+        self._FlowGroupName = None
+        self._FlowGroupInfos = None
+        self._Agent = None
+        self._FlowGroupOptions = None
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def FlowGroupName(self):
+        return self._FlowGroupName
+
+    @FlowGroupName.setter
+    def FlowGroupName(self, FlowGroupName):
+        self._FlowGroupName = FlowGroupName
+
+    @property
+    def FlowGroupInfos(self):
+        return self._FlowGroupInfos
+
+    @FlowGroupInfos.setter
+    def FlowGroupInfos(self, FlowGroupInfos):
+        self._FlowGroupInfos = FlowGroupInfos
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
+    def FlowGroupOptions(self):
+        return self._FlowGroupOptions
+
+    @FlowGroupOptions.setter
+    def FlowGroupOptions(self, FlowGroupOptions):
+        self._FlowGroupOptions = FlowGroupOptions
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        self._FlowGroupName = params.get("FlowGroupName")
+        if params.get("FlowGroupInfos") is not None:
+            self._FlowGroupInfos = []
+            for item in params.get("FlowGroupInfos"):
+                obj = FlowGroupInfo()
+                obj._deserialize(item)
+                self._FlowGroupInfos.append(obj)
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
+        if params.get("FlowGroupOptions") is not None:
+            self._FlowGroupOptions = FlowGroupOptions()
+            self._FlowGroupOptions._deserialize(params.get("FlowGroupOptions"))
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
+class CreateFlowGroupByTemplatesResponse(AbstractModel):
+    """CreateFlowGroupByTemplates返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FlowGroupId: 合同(流程)组的合同组Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FlowGroupId: str
+        :param _FlowIds: 合同(流程)组中子合同列表.
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FlowIds: list of str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._FlowGroupId = None
+        self._FlowIds = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class CreateFlowRemindsRequest(AbstractModel):
     """CreateFlowReminds请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4618,27 +4904,30 @@
         :param _EndPoint: 链接类型
 HTTP：跳转电子签小程序的http_url，
 APP：第三方APP或小程序跳转电子签小程序的path。
 默认为HTTP类型
         :type EndPoint: str
         :param _FlowId: 签署流程编号 (PathType=1时必传)
         :type FlowId: str
+        :param _FlowGroupId: 合同组ID
+        :type FlowGroupId: str
         :param _PathType: 跳转页面 1: 小程序合同详情 2: 小程序合同列表页 0: 不传, 默认主页
         :type PathType: int
         :param _AutoJumpBack: 是否自动回跳 true：是， false：否。该参数只针对"APP" 类型的签署链接有效
         :type AutoJumpBack: bool
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._OrganizationName = None
         self._Name = None
         self._Mobile = None
         self._EndPoint = None
         self._FlowId = None
+        self._FlowGroupId = None
         self._PathType = None
         self._AutoJumpBack = None
         self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
@@ -4684,14 +4973,22 @@
         return self._FlowId
 
     @FlowId.setter
     def FlowId(self, FlowId):
         self._FlowId = FlowId
 
     @property
+    def FlowGroupId(self):
+        return self._FlowGroupId
+
+    @FlowGroupId.setter
+    def FlowGroupId(self, FlowGroupId):
+        self._FlowGroupId = FlowGroupId
+
+    @property
     def PathType(self):
         return self._PathType
 
     @PathType.setter
     def PathType(self, PathType):
         self._PathType = PathType
 
@@ -4717,14 +5014,15 @@
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._OrganizationName = params.get("OrganizationName")
         self._Name = params.get("Name")
         self._Mobile = params.get("Mobile")
         self._EndPoint = params.get("EndPoint")
         self._FlowId = params.get("FlowId")
+        self._FlowGroupId = params.get("FlowGroupId")
         self._PathType = params.get("PathType")
         self._AutoJumpBack = params.get("AutoJumpBack")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
@@ -6604,58 +6902,70 @@
 class DescribeFlowInfoRequest(AbstractModel):
     """DescribeFlowInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _FlowIds: 需要查询的流程ID列表，限制最大100个
-        :type FlowIds: list of str
         :param _Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _FlowIds: 需要查询的流程ID列表，限制最大100个
+        :type FlowIds: list of str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _FlowGroupId: 合同组ID
+        :type FlowGroupId: str
         """
-        self._FlowIds = None
         self._Operator = None
+        self._FlowIds = None
         self._Agent = None
-
-    @property
-    def FlowIds(self):
-        return self._FlowIds
-
-    @FlowIds.setter
-    def FlowIds(self, FlowIds):
-        self._FlowIds = FlowIds
+        self._FlowGroupId = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
         self._Operator = Operator
 
     @property
+    def FlowIds(self):
+        return self._FlowIds
+
+    @FlowIds.setter
+    def FlowIds(self, FlowIds):
+        self._FlowIds = FlowIds
+
+    @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
         self._Agent = Agent
 
+    @property
+    def FlowGroupId(self):
+        return self._FlowGroupId
+
+    @FlowGroupId.setter
+    def FlowGroupId(self, FlowGroupId):
+        self._FlowGroupId = FlowGroupId
+
 
     def _deserialize(self, params):
-        self._FlowIds = params.get("FlowIds")
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
+        self._FlowIds = params.get("FlowIds")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
+        self._FlowGroupId = params.get("FlowGroupId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -6667,29 +6977,51 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FlowDetailInfos: 签署流程信息
         :type FlowDetailInfos: list of FlowDetailInfo
+        :param _FlowGroupId: 合同组ID
+        :type FlowGroupId: str
+        :param _FlowGroupName: 合同组名称
+        :type FlowGroupName: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._FlowDetailInfos = None
+        self._FlowGroupId = None
+        self._FlowGroupName = None
         self._RequestId = None
 
     @property
     def FlowDetailInfos(self):
         return self._FlowDetailInfos
 
     @FlowDetailInfos.setter
     def FlowDetailInfos(self, FlowDetailInfos):
         self._FlowDetailInfos = FlowDetailInfos
 
     @property
+    def FlowGroupId(self):
+        return self._FlowGroupId
+
+    @FlowGroupId.setter
+    def FlowGroupId(self, FlowGroupId):
+        self._FlowGroupId = FlowGroupId
+
+    @property
+    def FlowGroupName(self):
+        return self._FlowGroupName
+
+    @FlowGroupName.setter
+    def FlowGroupName(self, FlowGroupName):
+        self._FlowGroupName = FlowGroupName
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -6697,14 +7029,16 @@
     def _deserialize(self, params):
         if params.get("FlowDetailInfos") is not None:
             self._FlowDetailInfos = []
             for item in params.get("FlowDetailInfos"):
                 obj = FlowDetailInfo()
                 obj._deserialize(item)
                 self._FlowDetailInfos.append(obj)
+        self._FlowGroupId = params.get("FlowGroupId")
+        self._FlowGroupName = params.get("FlowGroupName")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeFlowTemplatesRequest(AbstractModel):
     """DescribeFlowTemplates请求参数结构体
 
     """
@@ -9653,14 +9987,263 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class FlowGroupInfo(AbstractModel):
+    """此结构体(FlowGroupInfo)描述的是合同组(流程组)的单个合同(流程)信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FlowName: 合同（流程）的名称
+        :type FlowName: str
+        :param _Approvers: 合同（流程）的签署方信息
+        :type Approvers: list of ApproverInfo
+        :param _FileIds: 发起合同（流程）的资源Id,此资源必须是PDF文件,来自UploadFiles,使用文件发起合同(流程)组时必传
+        :type FileIds: list of str
+        :param _TemplateId: 发起合同（流程）的模板Id,用模板发起合同（流程）组时必填
+        :type TemplateId: str
+        :param _FlowType: 合同（流程）的类型
+        :type FlowType: str
+        :param _FlowDescription: 合同（流程）的描述
+        :type FlowDescription: str
+        :param _Deadline: 合同（流程）的截止时间戳，单位秒。默认是一年
+        :type Deadline: int
+        :param _CallbackUrl: 合同（流程）的回调地址
+        :type CallbackUrl: str
+        :param _UserData: 第三方平台传递过来的信息, 限制1024字符 格式必须是base64的
+        :type UserData: str
+        :param _Unordered: 合同（流程）的签署是否是无序签, true - 无序。 false - 有序, 默认 
+        :type Unordered: bool
+        :param _Components: 合同（流程）发起方的填写控件，用户
+        :type Components: list of Component
+        :param _NeedSignReview: 本企业（发起方）是否需要签署审批，若需要审批则只允许查看不允许签署，需要您调用接口CreateFlowSignReview提交审批结果。
+        :type NeedSignReview: bool
+        :param _AutoSignScene: 本企业（发起方）自动签署，需要您在发起合同时给印章控件指定自动签的印章。
+        :type AutoSignScene: str
+        """
+        self._FlowName = None
+        self._Approvers = None
+        self._FileIds = None
+        self._TemplateId = None
+        self._FlowType = None
+        self._FlowDescription = None
+        self._Deadline = None
+        self._CallbackUrl = None
+        self._UserData = None
+        self._Unordered = None
+        self._Components = None
+        self._NeedSignReview = None
+        self._AutoSignScene = None
+
+    @property
+    def FlowName(self):
+        return self._FlowName
+
+    @FlowName.setter
+    def FlowName(self, FlowName):
+        self._FlowName = FlowName
+
+    @property
+    def Approvers(self):
+        return self._Approvers
+
+    @Approvers.setter
+    def Approvers(self, Approvers):
+        self._Approvers = Approvers
+
+    @property
+    def FileIds(self):
+        return self._FileIds
+
+    @FileIds.setter
+    def FileIds(self, FileIds):
+        self._FileIds = FileIds
+
+    @property
+    def TemplateId(self):
+        return self._TemplateId
+
+    @TemplateId.setter
+    def TemplateId(self, TemplateId):
+        self._TemplateId = TemplateId
+
+    @property
+    def FlowType(self):
+        return self._FlowType
+
+    @FlowType.setter
+    def FlowType(self, FlowType):
+        self._FlowType = FlowType
+
+    @property
+    def FlowDescription(self):
+        return self._FlowDescription
+
+    @FlowDescription.setter
+    def FlowDescription(self, FlowDescription):
+        self._FlowDescription = FlowDescription
+
+    @property
+    def Deadline(self):
+        return self._Deadline
+
+    @Deadline.setter
+    def Deadline(self, Deadline):
+        self._Deadline = Deadline
+
+    @property
+    def CallbackUrl(self):
+        return self._CallbackUrl
+
+    @CallbackUrl.setter
+    def CallbackUrl(self, CallbackUrl):
+        self._CallbackUrl = CallbackUrl
+
+    @property
+    def UserData(self):
+        return self._UserData
+
+    @UserData.setter
+    def UserData(self, UserData):
+        self._UserData = UserData
+
+    @property
+    def Unordered(self):
+        return self._Unordered
+
+    @Unordered.setter
+    def Unordered(self, Unordered):
+        self._Unordered = Unordered
+
+    @property
+    def Components(self):
+        return self._Components
+
+    @Components.setter
+    def Components(self, Components):
+        self._Components = Components
+
+    @property
+    def NeedSignReview(self):
+        return self._NeedSignReview
+
+    @NeedSignReview.setter
+    def NeedSignReview(self, NeedSignReview):
+        self._NeedSignReview = NeedSignReview
+
+    @property
+    def AutoSignScene(self):
+        return self._AutoSignScene
+
+    @AutoSignScene.setter
+    def AutoSignScene(self, AutoSignScene):
+        self._AutoSignScene = AutoSignScene
+
+
+    def _deserialize(self, params):
+        self._FlowName = params.get("FlowName")
+        if params.get("Approvers") is not None:
+            self._Approvers = []
+            for item in params.get("Approvers"):
+                obj = ApproverInfo()
+                obj._deserialize(item)
+                self._Approvers.append(obj)
+        self._FileIds = params.get("FileIds")
+        self._TemplateId = params.get("TemplateId")
+        self._FlowType = params.get("FlowType")
+        self._FlowDescription = params.get("FlowDescription")
+        self._Deadline = params.get("Deadline")
+        self._CallbackUrl = params.get("CallbackUrl")
+        self._UserData = params.get("UserData")
+        self._Unordered = params.get("Unordered")
+        if params.get("Components") is not None:
+            self._Components = []
+            for item in params.get("Components"):
+                obj = Component()
+                obj._deserialize(item)
+                self._Components.append(obj)
+        self._NeedSignReview = params.get("NeedSignReview")
+        self._AutoSignScene = params.get("AutoSignScene")
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
+class FlowGroupOptions(AbstractModel):
+    """此结构体(FlowGroupOptions)描述的是合同组的个性化配置，支持控制是否发送短信、未实名个人签署方查看合同组时是否需要实名认证（仅在合同组文件发起配置时生效）
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ApproverVerifyType: 发起合同（流程）组的合同（流程）签署人校验方式
+VerifyCheck: 人脸识别（默认）
+MobileCheck：手机号验证
+参数说明：此参数仅在合同组文件发起有效，可选人脸识别或手机号验证两种方式，若选择后者，未实名个人签署方在签署合同时，无需经过实名认证和意愿确认两次人脸识别，该能力仅适用于个人签署方。
+        :type ApproverVerifyType: str
+        :param _SelfOrganizationApproverNotifyType: 发起合同（流程）组本方企业经办人通知方式
+签署通知类型：sms--短信，none--不通知
+        :type SelfOrganizationApproverNotifyType: str
+        :param _OtherApproverNotifyType: 发起合同（流程）组他方经办人通知方式
+签署通知类型：sms--短信，none--不通知
+        :type OtherApproverNotifyType: str
+        """
+        self._ApproverVerifyType = None
+        self._SelfOrganizationApproverNotifyType = None
+        self._OtherApproverNotifyType = None
+
+    @property
+    def ApproverVerifyType(self):
+        return self._ApproverVerifyType
+
+    @ApproverVerifyType.setter
+    def ApproverVerifyType(self, ApproverVerifyType):
+        self._ApproverVerifyType = ApproverVerifyType
+
+    @property
+    def SelfOrganizationApproverNotifyType(self):
+        return self._SelfOrganizationApproverNotifyType
+
+    @SelfOrganizationApproverNotifyType.setter
+    def SelfOrganizationApproverNotifyType(self, SelfOrganizationApproverNotifyType):
+        self._SelfOrganizationApproverNotifyType = SelfOrganizationApproverNotifyType
+
+    @property
+    def OtherApproverNotifyType(self):
+        return self._OtherApproverNotifyType
+
+    @OtherApproverNotifyType.setter
+    def OtherApproverNotifyType(self, OtherApproverNotifyType):
+        self._OtherApproverNotifyType = OtherApproverNotifyType
+
+
+    def _deserialize(self, params):
+        self._ApproverVerifyType = params.get("ApproverVerifyType")
+        self._SelfOrganizationApproverNotifyType = params.get("SelfOrganizationApproverNotifyType")
+        self._OtherApproverNotifyType = params.get("OtherApproverNotifyType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class FormField(AbstractModel):
     """电子文档的控件填充信息。按照控件类型进行相应的填充。
 
     【数据表格传参说明】
```

